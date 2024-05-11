# Comparing `tmp/openav-1.0.0a8.tar.gz` & `tmp/openav-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openav-1.0.0a8.tar", last modified: Thu May  2 18:33:25 2024, max compression
+gzip compressed data, was "openav-1.0.0a9.tar", last modified: Fri May  3 15:15:02 2024, max compression
```

## Comparing `openav-1.0.0a8.tar` & `openav-1.0.0a9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.302820 openav-1.0.0a8/
--rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a8/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a8/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-05-02 18:33:25.303416 openav-1.0.0a8/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a8/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.242962 openav-1.0.0a8/openav/
--rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a8/openav/__garbage__.py
--rw-r--r--   0 dl         (501) staff       (20)     1077 2024-05-02 18:33:11.000000 openav-1.0.0a8/openav/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.265587 openav-1.0.0a8/openav/api/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/api/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a8/openav/api/augmentation.py
--rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a8/openav/api/download.py
--rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a8/openav/api/preprocess_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a8/openav/api/preprocess_video.py
--rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/test_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    19855 2024-05-02 17:42:44.000000 openav-1.0.0a8/openav/api/test_audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/test_video.py
--rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a8/openav/api/testing.py
--rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/train_audio.py
--rw-r--r--   0 dl         (501) staff       (20)    22373 2024-04-27 18:53:38.000000 openav-1.0.0a8/openav/api/train_audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a8/openav/api/train_video.py
--rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a8/openav/api/vad.py
--rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a8/openav/api/vad_gui.py
--rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a8/openav/api/vosk_sr.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.266863 openav-1.0.0a8/openav/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a8/openav/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.274727 openav-1.0.0a8/openav/modules/core/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/modules/core/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    31017 2024-04-26 16:59:06.000000 openav-1.0.0a8/openav/modules/core/core.py
--rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a8/openav/modules/core/exceptions.py
--rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/core/language.py
--rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/core/logging.py
--rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/core/messages.py
--rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a8/openav/modules/core/settings.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.276617 openav-1.0.0a8/openav/modules/dataset_recording/
--rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a8/openav/modules/dataset_recording/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a8/openav/modules/dataset_recording/app.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.282422 openav-1.0.0a8/openav/modules/file_manager/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a8/openav/modules/file_manager/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a8/openav/modules/file_manager/download.py
--rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a8/openav/modules/file_manager/file_manager.py
--rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/file_manager/json_manager.py
--rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a8/openav/modules/file_manager/unzip.py
--rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/file_manager/yaml_manager.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.290877 openav-1.0.0a8/openav/modules/lab/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a8/openav/modules/lab/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a8/openav/modules/lab/audio.py
--rw-r--r--   0 dl         (501) staff       (20)    35524 2024-05-02 18:05:21.000000 openav-1.0.0a8/openav/modules/lab/audiovisual.py
--rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/lab/build.py
--rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a8/openav/modules/lab/video.py
--rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a8/openav/modules/lab/video_converter.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.238180 openav-1.0.0a8/openav/modules/locales/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.237995 openav-1.0.0a8/openav/modules/locales/en/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.292937 openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.238299 openav-1.0.0a8/openav/modules/locales/ru/
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.294624 openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/
--rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
--rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.298117 openav-1.0.0a8/openav/modules/nn/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/modules/nn/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)    11245 2024-04-26 16:34:46.000000 openav-1.0.0a8/openav/modules/nn/av_dataset.py
--rw-r--r--   0 dl         (501) staff       (20)    11719 2024-05-02 18:32:54.000000 openav-1.0.0a8/openav/modules/nn/models.py
--rw-r--r--   0 dl         (501) staff       (20)     2727 2024-04-26 17:11:00.000000 openav-1.0.0a8/openav/modules/nn/utils.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.300133 openav-1.0.0a8/openav/modules/trml/
--rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a8/openav/modules/trml/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/modules/trml/shell.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.301706 openav-1.0.0a8/openav/rsrs/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a8/openav/rsrs/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.302290 openav-1.0.0a8/openav/rsrs/favicon/
--rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a8/openav/rsrs/favicon/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-02 18:33:25.245826 openav-1.0.0a8/openav.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)     4144 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1865 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)      330 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/entry_points.txt
--rw-r--r--   0 dl         (501) staff       (20)      459 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)        7 2024-05-02 18:33:25.000000 openav-1.0.0a8/openav.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a8/pyproject.toml
--rw-r--r--   0 dl         (501) staff       (20)       79 2024-05-02 18:33:25.304658 openav-1.0.0a8/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     4567 2024-05-02 18:32:33.000000 openav-1.0.0a8/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:02.003891 openav-1.0.0a9/
+-rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a9/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a9/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-05-03 15:15:02.004595 openav-1.0.0a9/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a9/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.939204 openav-1.0.0a9/openav/
+-rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a9/openav/__garbage__.py
+-rw-r--r--   0 dl         (501) staff       (20)     1077 2024-05-03 15:14:52.000000 openav-1.0.0a9/openav/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.962418 openav-1.0.0a9/openav/api/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a9/openav/api/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a9/openav/api/augmentation.py
+-rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a9/openav/api/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    21181 2024-04-27 12:48:45.000000 openav-1.0.0a9/openav/api/preprocess_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    19835 2024-04-27 12:48:33.000000 openav-1.0.0a9/openav/api/preprocess_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a9/openav/api/test_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    21205 2024-05-03 15:00:30.000000 openav-1.0.0a9/openav/api/test_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a9/openav/api/test_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a9/openav/api/testing.py
+-rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a9/openav/api/train_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    22373 2024-05-03 13:25:35.000000 openav-1.0.0a9/openav/api/train_audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a9/openav/api/train_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a9/openav/api/vad.py
+-rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a9/openav/api/vad_gui.py
+-rw-r--r--   0 dl         (501) staff       (20)    23001 2024-04-27 12:49:02.000000 openav-1.0.0a9/openav/api/vosk_sr.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.963643 openav-1.0.0a9/openav/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a9/openav/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.972468 openav-1.0.0a9/openav/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a9/openav/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    31099 2024-05-03 15:13:54.000000 openav-1.0.0a9/openav/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a9/openav/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/core/logging.py
+-rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    14550 2024-04-21 20:40:49.000000 openav-1.0.0a9/openav/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.974378 openav-1.0.0a9/openav/modules/dataset_recording/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a9/openav/modules/dataset_recording/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     4518 2024-04-26 09:47:40.000000 openav-1.0.0a9/openav/modules/dataset_recording/app.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.979831 openav-1.0.0a9/openav/modules/file_manager/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a9/openav/modules/file_manager/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a9/openav/modules/file_manager/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a9/openav/modules/file_manager/file_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/file_manager/json_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a9/openav/modules/file_manager/unzip.py
+-rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/file_manager/yaml_manager.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.990377 openav-1.0.0a9/openav/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a9/openav/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   120642 2024-04-24 09:54:17.000000 openav-1.0.0a9/openav/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    39330 2024-05-03 15:07:23.000000 openav-1.0.0a9/openav/modules/lab/audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)    24427 2024-04-24 13:03:57.000000 openav-1.0.0a9/openav/modules/lab/video.py
+-rw-r--r--   0 dl         (501) staff       (20)      202 2024-04-23 19:00:17.000000 openav-1.0.0a9/openav/modules/lab/video_converter.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.933137 openav-1.0.0a9/openav/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.932837 openav-1.0.0a9/openav/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.992781 openav-1.0.0a9/openav/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a9/openav/modules/locales/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a9/openav/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.933308 openav-1.0.0a9/openav/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.994507 openav-1.0.0a9/openav/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a9/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a9/openav/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.999007 openav-1.0.0a9/openav/modules/nn/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a9/openav/modules/nn/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    18842 2024-05-02 19:29:10.000000 openav-1.0.0a9/openav/modules/nn/av_dataset.py
+-rw-r--r--   0 dl         (501) staff       (20)    10390 2024-05-03 15:14:42.000000 openav-1.0.0a9/openav/modules/nn/models.py
+-rw-r--r--   0 dl         (501) staff       (20)     4071 2024-05-03 15:10:38.000000 openav-1.0.0a9/openav/modules/nn/utils.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:02.001352 openav-1.0.0a9/openav/modules/trml/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a9/openav/modules/trml/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/modules/trml/shell.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:02.002542 openav-1.0.0a9/openav/rsrs/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a9/openav/rsrs/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:02.003125 openav-1.0.0a9/openav/rsrs/favicon/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a9/openav/rsrs/favicon/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-05-03 15:15:01.943117 openav-1.0.0a9/openav.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-05-03 15:15:01.000000 openav-1.0.0a9/openav.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1865 2024-05-03 15:15:01.000000 openav-1.0.0a9/openav.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2024-05-03 15:15:01.000000 openav-1.0.0a9/openav.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      330 2024-05-03 15:15:01.000000 openav-1.0.0a9/openav.egg-info/entry_points.txt
+-rw-r--r--   0 dl         (501) staff       (20)      475 2024-05-03 15:15:01.000000 openav-1.0.0a9/openav.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)        7 2024-05-03 15:15:01.000000 openav-1.0.0a9/openav.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a9/pyproject.toml
+-rw-r--r--   0 dl         (501) staff       (20)       79 2024-05-03 15:15:02.008041 openav-1.0.0a9/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     4592 2024-05-03 15:13:11.000000 openav-1.0.0a9/setup.py
```

### Comparing `openav-1.0.0a8/LICENSE` & `openav-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/PKG-INFO` & `openav-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a8/README.md` & `openav-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/__garbage__.py` & `openav-1.0.0a9/openav/__garbage__.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/__init__.py` & `openav-1.0.0a9/openav/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 __title__ = "OpenAV"
 __summary__ = "OpenAV"
 __uri__ = "https://github.com/DmitryRyumin/openav"
 
 __version__ = "1.0"
-__release__ = __version__ + ".0-a8"
+__release__ = __version__ + ".0-a9"
 
 __author__ru__ = "Рюмин Дмитрий, Иванько Денис, Шилов Николай, Маркитантов Максим, Карпов Алексей"
 __author__en__ = "Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov"
 __email__ = (
     "dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, " "karpov@iias.spb.su"
 )
```

### Comparing `openav-1.0.0a8/openav/api/augmentation.py` & `openav-1.0.0a9/openav/api/augmentation.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/download.py` & `openav-1.0.0a9/openav/api/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/preprocess_audio.py` & `openav-1.0.0a9/openav/api/preprocess_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/preprocess_video.py` & `openav-1.0.0a9/openav/api/preprocess_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/test_audio.py` & `openav-1.0.0a9/openav/api/test_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/test_audiovisual.py` & `openav-1.0.0a9/openav/api/test_audiovisual.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,21 @@
 # Персональные
 import openav  # Библиотека в целом
 from openav.modules.trml.shell import Shell  # Работа с Shell
 from openav.modules.lab.build import Run  # Сборка библиотеки
 from openav import rsrs  # Ресурсы библиотеки
 
 from openav.modules.core.logging import ARG_PATH_TO_LOGS
-from openav.modules.lab.audiovisual import SUBFOLDERS_TEST, SHAPE_AUDIO, SHAPE_VIDEO, EXTH_MODELS
+from openav.modules.lab.audiovisual import (
+    SUBFOLDERS_TEST,
+    SHAPE_AUDIO,
+    SHAPE_VIDEO,
+    EXTH_MODELS,
+    FIGSIZE_CONFUSION_MATRIX,
+)
 
 
 # ######################################################################################################################
 # Сообщения
 # ######################################################################################################################
 @dataclass
 class MessagesTestAudioVisual(Run):
@@ -71,15 +77,15 @@
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
         super().__post_init__()  # Выполнение конструктора из суперкласса
 
-        self._all_layer_in_yaml = 14  # Общее количество настроек в конфигурационном файле
+        self._all_layer_in_yaml = 17  # Общее количество настроек в конфигурационном файле
 
         #  Регистратор логирования с указанным именем
         self._logger_run_train_audiovisual: logging.Logger = logging.getLogger(__class__.__name__)
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (защищенные)
     # ------------------------------------------------------------------------------------------------------------------
@@ -162,23 +168,25 @@
 
         curr_valid_layer = 0  # Валидное количество разделов
 
         # Проход по всем разделам конфигурационного файла
         for key, val in config.items():
             # 1. Скрытие метаданных
             # 2. Скрытие версий установленных библиотек
-            if key == "hide_metadata" or key == "hide_libs_vers":
+            # 3. Сохранение матрицы спутывания
+            if key == "hide_metadata" or key == "hide_libs_vers" or key == "save_confusion_matrix":
                 # Проверка значения
                 if type(val) is not bool:
                     continue
 
                 curr_valid_layer += 1
 
-            # Путь к директории набора данных
-            if key == "path_to_dataset":
+            # 1. Путь к директории набора данных
+            # 2. Путь к директории для сохранения матрицы спутывания
+            if key == "path_to_dataset" or key == "path_to_save_confusion_matrix":
                 # Проверка значения
                 if type(val) is not str or not val:
                     continue
 
                 curr_valid_layer += 1
 
             # Подкаталоги с данными
@@ -289,14 +297,33 @@
                 file_path = Path(val)
 
                 if not file_path.is_file() or file_path.suffix.replace(".", "") != EXTH_MODELS:
                     continue
 
                 curr_valid_layer += 1
 
+            # Настройки для формирования изображения матрицы спутывания
+            if key == "figsize_confusion_matrix":
+                curr_valid_layer_2 = 0
+
+                # Проверка значения
+                if type(val) is not dict or len(val) == 0 or not all(k in val for k in FIGSIZE_CONFUSION_MATRIX):
+                    continue
+
+                # Проход по всем подкаталогам
+                for _, v in val.items():
+                    # Проверка значения
+                    if type(v) is not int or (v < 0):
+                        continue
+
+                    curr_valid_layer_2 += 1
+
+                if curr_valid_layer_2 == 5:
+                    curr_valid_layer += 1
+
         # Сравнение общего количества ожидаемых настроек и валидных настроек в конфигурационном файле
         if self._all_layer_in_yaml != curr_valid_layer:
             try:
                 raise TypeError
             except TypeError:
                 self.message_error(self._invalid_file, space=self._space, out=out)
                 return False
@@ -417,14 +444,17 @@
             max_segment=self._args["max_segment"],
             hidden_units=self._args["hidden_units"],
             hidden_features=self._args["hidden_features"],
             input_dim=self._args["input_dim"],
             shape_audio=self._args["shape_audio"],
             shape_video=self._args["shape_video"],
             path_to_model=self._args["path_to_model"],
+            save_confusion_matrix=self._args["save_confusion_matrix"],
+            path_to_save_confusion_matrix=self._args["path_to_save_confusion_matrix"],
+            figsize_confusion_matrix=self._args["figsize_confusion_matrix"],
             out=out,
         )
 
         return True
 
 
 def main():
```

### Comparing `openav-1.0.0a8/openav/api/test_video.py` & `openav-1.0.0a9/openav/api/test_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/testing.py` & `openav-1.0.0a9/openav/api/testing.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/train_audio.py` & `openav-1.0.0a9/openav/api/train_audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/train_audiovisual.py` & `openav-1.0.0a9/openav/api/train_audiovisual.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/train_video.py` & `openav-1.0.0a9/openav/api/train_video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/vad.py` & `openav-1.0.0a9/openav/api/vad.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/vad_gui.py` & `openav-1.0.0a9/openav/api/vad_gui.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/api/vosk_sr.py` & `openav-1.0.0a9/openav/api/vosk_sr.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/core/core.py` & `openav-1.0.0a9/openav/modules/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import librosa.display
 import matplotlib as mpl
 import mediapipe as mp
 import cv2
 import einops
 import tqdm
 import sklearn
+import seaborn as sns
 
 from datetime import datetime  # Работа со временем
 from prettytable import PrettyTable  # Отображение таблиц в терминале
 import pkg_resources  # Работа с ресурсами внутри пакетов
 
 from IPython import get_ipython
 
@@ -649,14 +650,15 @@
                 "Package": [
                     "PyTorch",
                     "TorchAudio",
                     "TorchVision",
                     "NumPy",
                     "Pandas",
                     "Matplotlib",
+                    "Seaborn",
                     "PyAV",
                     "FileType",
                     "IPython",
                     "Colorama",
                     "Prettytable",
                     "PyYAML",
                     "PyMediaInfo",
@@ -675,14 +677,15 @@
                     for i in [
                         torch,
                         torchaudio,
                         torchvision,
                         np,
                         pd,
                         mpl,
+                        sns,
                         av,
                         filetype,
                         IPython,
                         colorama,
                         prettytable,
                         yaml,
                         pymediainfo,
```

### Comparing `openav-1.0.0a8/openav/modules/core/exceptions.py` & `openav-1.0.0a9/openav/modules/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/core/language.py` & `openav-1.0.0a9/openav/modules/core/language.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/core/logging.py` & `openav-1.0.0a9/openav/modules/core/logging.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/core/messages.py` & `openav-1.0.0a9/openav/modules/core/messages.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/core/settings.py` & `openav-1.0.0a9/openav/modules/core/settings.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/dataset_recording/app.py` & `openav-1.0.0a9/openav/modules/dataset_recording/app.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/file_manager/download.py` & `openav-1.0.0a9/openav/modules/file_manager/download.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/file_manager/file_manager.py` & `openav-1.0.0a9/openav/modules/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/file_manager/json_manager.py` & `openav-1.0.0a9/openav/modules/file_manager/json_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/file_manager/unzip.py` & `openav-1.0.0a9/openav/modules/file_manager/unzip.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/file_manager/yaml_manager.py` & `openav-1.0.0a9/openav/modules/file_manager/yaml_manager.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/lab/audio.py` & `openav-1.0.0a9/openav/modules/lab/audio.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/lab/audiovisual.py` & `openav-1.0.0a9/openav/modules/lab/audiovisual.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,43 +17,47 @@
 ]:
     warnings.filterwarnings(
         "ignore",
         category=warn,
     )
 
 import os
+import numpy as np
 
 from dataclasses import dataclass  # Класс данных
 
 # Типы данных
 from typing import List, Dict
 
-from pathlib import Path  # Работа с путями в файловой системе
+import datetime
 import torch
+from pathlib import Path  # Работа с путями в файловой системе
 from torch.utils.data import DataLoader
 from torch.nn import CrossEntropyLoss
 from lion_pytorch import Lion
-import datetime
+from tqdm import tqdm
+from sklearn.metrics import accuracy_score
 
 # Персональные
 from openav.modules.core.exceptions import IsNestedCatalogsNotFoundError
 from openav.modules.lab.audio import Audio  # Аудиомодальность
 from openav.modules.lab.video import Video  # Видеомодальность
-from openav.modules.nn.av_dataset import AVDataset
-from openav.modules.nn.utils import fix_seeds, train_one_epoch, val_one_epoch
+from openav.modules.nn.av_dataset import AVDataset, AVTest
+from openav.modules.nn.utils import fix_seeds, train_one_epoch, val_one_epoch, save_conf_matrix
 from openav.modules.nn.models import AVModel
 
 # ######################################################################################################################
 # Константы
 # ######################################################################################################################
 
 SUBFOLDERS: List[str] = ["train", "val", "test"]
 SUBFOLDERS_TEST: List[str] = ["test"]
 SHAPE_AUDIO: List[str] = ["channels", "n_mels", "samples"]
 SHAPE_VIDEO: List[str] = ["frames", "channels", "width", "height"]
+FIGSIZE_CONFUSION_MATRIX: List[str] = ["width", "height", "font_size", "dpi", "pad_inches"]
 EXT_AV_VIDEO: List[str] = ["mov", "mp4", "webm"]  # Расширения искомых файлов
 EXT_MODELS: str = "pt"
 EXTH_MODELS: str = "pth"
 OPTIMIZERS: List[str] = ["adam", "adamw", "sgd", "lion"]
 REQUIRED_GRAD: List[str] = ["none", "a", "v", "av"]
 
 
@@ -120,17 +124,23 @@
             self._("Точность на валидационной выборке увеличилась ({} ---> {}). Сохранение модели") + self._em
         )
         self._acc_test: str = self._("Точность для тестовой выборке: {}")
         self._acc_test_up: str = self._("Точность на тестовой выборке увеличилась ({} ---> {})")
 
         self._end_train: str = self._("Процесс обучения завершен") + self._em
 
+        self._run_test: str = self._("Запуск процесса тестирования") + self._em
+
+        self._accuracy_score: str = self._("Точность на тестовой выборке: {}") + self._em
+        self._create_confusion_matrix: str = self._("Создание матрицы спутывания") + self._em
+        self._end_test: str = self._("Процесс тестирования завершен") + self._em
+
 
 # ######################################################################################################################
-# Видео
+# Мультимодальное
 # ######################################################################################################################
 @dataclass
 class AV(AVMessages):
     """Класс для мультимодального объединения аудио- и видеомодальностей
 
     Args:
         path_to_logs (str): Смотреть :attr:`~openav.modules.core.logging.Logging.path_to_logs`
@@ -145,14 +155,15 @@
         super().__post_init__()  # Выполнение конструктора из суперкласса
 
         # ----------------------- Только для внутреннего использования внутри класса
 
         self.__device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
 
         self.__model_session = "created_at_%d_%m_%Y_%H-%M"
+        self.__cm_session = "confusion_matrix_%d_%m_%Y_%H-%M.png"
 
     # ------------------------------------------------------------------------------------------------------------------
     # Свойства
     # ------------------------------------------------------------------------------------------------------------------
 
     # ------------------------------------------------------------------------------------------------------------------
     # Внутренние методы (приватные)
@@ -304,14 +315,15 @@
             shape_audio = (
                 None,
                 max_segment,
                 shape_audio[SHAPE_AUDIO[0]],
                 shape_audio[SHAPE_AUDIO[1]],
                 shape_audio[SHAPE_AUDIO[2]],
             )
+            shape_video_frames = shape_video[SHAPE_VIDEO[0]]
             shape_video = (
                 None,
                 max_segment,
                 shape_video[SHAPE_VIDEO[0]],
                 shape_video[SHAPE_VIDEO[1]],
                 shape_video[SHAPE_VIDEO[3]],
                 shape_video[SHAPE_VIDEO[2]],
@@ -433,15 +445,19 @@
                         self.message_line(self._format_percentage(test_percentage)),
                     ),
                     space=self._space,
                     out=out,
                 )
 
                 train_data = AVDataset(
-                    path_files=path_train, labels=lb_train, subset="train", len_video=29, max_segment=2
+                    path_files=path_train,
+                    labels=lb_train,
+                    subset="train",
+                    len_video=shape_video_frames,
+                    max_segment=max_segment,
                 )
 
                 train_data = AVDataset(path_files=path_train, labels=lb_train, subset="train", max_segment=max_segment)
                 test_data = AVDataset(path_files=path_test, labels=lb_test, subset="test", max_segment=max_segment)
                 val_data = AVDataset(path_files=path_val, labels=lb_val, subset="val", max_segment=max_segment)
 
                 train_dataloader = DataLoader(train_data, batch_size=batch_size, shuffle=True)
@@ -507,15 +523,15 @@
 
                 # Создание директории, где хранятся модели
                 if self.create_folder(session_path, out=False) is False:
                     return False
 
                 self.message_info(self._run_train, out=out)
 
-                for e in range(1, epochs, 1):
+                for e in range(1, epochs + 1, 1):
                     self.message_info(
                         self._epoch.format(
                             self.message_line(str(e)),
                             self.message_line(str(epochs)),
                         ),
                         out=out,
                     )
@@ -593,14 +609,17 @@
         encoder_decoder: int,
         max_segment: int,
         hidden_units: int,
         hidden_features: int,
         input_dim: int,
         shape_audio: Dict[str, int],
         shape_video: Dict[str, int],
+        save_confusion_matrix: bool,
+        path_to_save_confusion_matrix: str,
+        figsize_confusion_matrix: Dict[str, int],
         path_to_model: str,
         out: bool = True,
     ) -> bool:
         """Автоматическое тестирование на аудиовизуальных данных
 
         Args:
             subfolders (Dict[str, str]): Словарь с подкаталогами с данными
@@ -609,14 +628,17 @@
             encoder_decoder (int): Количество энкодеров и декодеров
             max_segment (int): Максимальная длительность сегмента видео
             hidden_units (int): Количество скрытых нейронов
             hidden_features (int): Количество скрытых признаков
             input_dim (int): Количество входных признаков
             shape_audio (Dict[str, int]): Входная размерность аудио лог-мел спектрограммы
             shape_video (Dict[str, int]): Входная размерность видеокадров
+            save_confusion_matrix (bool): Сохранение матрицы спутывания
+            path_to_save_confusion_matrix (str):  Путь к директории для сохранения матрицы спутывания
+            figsize_confusion_matrix (Dict[str, int]): Настройки для формирования изображения матрицы спутывания
             path_to_model (str): Путь к нейросетевой аудиовизуальной модели
             out (bool) Отображение
 
         Returns:
             bool: **True** если автоматическое тестирование на аудиовизуальных данных произведено, в обратном случае
             **False**
         """
@@ -642,14 +664,19 @@
                 or not (0 < input_dim)
                 or type(shape_audio) is not dict
                 or len(shape_audio) == 0
                 or not all(shape in shape_audio for shape in SHAPE_AUDIO)
                 or type(shape_video) is not dict
                 or len(shape_video) == 0
                 or not all(shape in shape_video for shape in SHAPE_VIDEO)
+                or type(save_confusion_matrix) is not bool
+                or type(path_to_save_confusion_matrix) is not str
+                or not path_to_save_confusion_matrix
+                or len(figsize_confusion_matrix) == 0
+                or not all(k in figsize_confusion_matrix for k in FIGSIZE_CONFUSION_MATRIX)
                 or type(path_to_model) is not str
                 or not path_to_model
                 or type(out) is not bool
             ):
                 raise TypeError
         except TypeError:
             self.inv_args(__class__.__name__, self.test_audiovisual.__name__, out=out)
@@ -703,27 +730,29 @@
                 ),
                 out=out,
             )
 
             hierarchy_from_paths = self.__get_hierarchy_from_paths(nested_paths, depth)
 
             path_test, lb_test = [], []
+            lb_test_names = []
 
             # Проход по всем вложенным директориям
             for nested_path in hierarchy_from_paths:
                 if nested_path[0].lower() in classes:
                     # Формирование списка с видеофайлами
                     for p in Path(os.path.join(self.path_to_dataset, *reversed(nested_path))).glob("*"):
                         # Добавление текущего пути к видеофайлу в список
                         if p.suffix.lower().replace(".", "") in EXT_AV_VIDEO:
                             [index for index, cls in enumerate(classes) if cls.lower() == nested_path[0].lower()]
 
                             if nested_path[-1] == subfolders[SUBFOLDERS_TEST[0]]:
                                 path_test.append(p.resolve())
                                 lb_test.append(classes.index(nested_path[0].lower()))
+                                lb_test_names.append(nested_path[0])
                             else:
                                 pass
 
             # Директории с поднаборами данных не содержат визуальных файлов с необходимыми расширениями
             try:
                 len_path_test = len(path_test)
                 len_lb_test = len(lb_test)
@@ -747,10 +776,54 @@
                     input_dim=input_dim,
                     h_u=hidden_units,
                     h_f=hidden_features,
                     n_class=n_classes,
                     encoder_decoder=encoder_decoder,
                 ).to(self.__device)
 
-                e = model.load_state_dict(torch.load(path_to_model, map_location=torch.device(self.__device)))
+                model.load_state_dict(torch.load(path_to_model, map_location=torch.device(self.__device)))
+
+                self.message_info(self._run_test, out=out)
+
+                processor = AVTest(max_segment=max_segment)
+
+                torch.autograd.set_detect_anomaly(True)
+
+                model.eval().to(self.__device)
+
+                preds = []
+
+                for path in tqdm(path_test):
+                    _, audio_data, video_data = processor.get_metadata(name_file=str(path))
+                    with torch.no_grad():
+                        prob = model(audio_data.to(self.__device), video_data.to(self.__device)).cpu().detach().numpy()
+                    pred = np.argmax(prob)
+                    preds.append(pred)
+
+                self.message_info(
+                    self._accuracy_score.format(
+                        self.message_line(str(round(accuracy_score(lb_test, preds) * 100, 2)) + "%"),
+                    ),
+                    out=out,
+                )
+
+                if save_confusion_matrix:
+                    self.message_info(self._create_confusion_matrix, out=out)
+
+                    date_time = datetime.datetime.now()
+                    date_path = date_time.strftime(self.__cm_session)
+
+                    save_conf_matrix(
+                        y_true=lb_test,
+                        y_pred=preds,
+                        name_labels=list(set(lb_test_names)),
+                        filename=os.path.join(path_to_save_confusion_matrix, date_path),
+                        figsize_w=figsize_confusion_matrix[FIGSIZE_CONFUSION_MATRIX[0]],
+                        figsize_h=figsize_confusion_matrix[FIGSIZE_CONFUSION_MATRIX[1]],
+                        font_size=figsize_confusion_matrix[FIGSIZE_CONFUSION_MATRIX[2]],
+                        dpi=figsize_confusion_matrix[FIGSIZE_CONFUSION_MATRIX[3]],
+                        pad_inches=figsize_confusion_matrix[FIGSIZE_CONFUSION_MATRIX[4]],
+                    )
+
+                self.message_info(self._end_test, out=out)
 
-                print(e)
+                return True
```

### Comparing `openav-1.0.0a8/openav/modules/lab/build.py` & `openav-1.0.0a9/openav/modules/lab/build.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/lab/video.py` & `openav-1.0.0a9/openav/modules/lab/video.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/locales/en/LC_MESSAGES/base.mo` & `openav-1.0.0a9/openav/modules/locales/en/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/locales/ru/LC_MESSAGES/argparse.mo` & `openav-1.0.0a9/openav/modules/locales/ru/LC_MESSAGES/argparse.mo`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav/modules/nn/models.py` & `openav-1.0.0a9/openav/modules/nn/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -244,27 +244,14 @@
         for _ in range(encoder_decoder - 1):
             self.encoders.append(SecondEncoder(input_dim=input_dim))
 
         # Создание декодеров
         for _ in range(encoder_decoder):
             self.decoders.append(Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class))
 
-        # self.enc0 = InitialEncoder(input_dim=input_dim)
-        # self.enc1 = SecondEncoder(input_dim=input_dim)
-        # self.enc2 = SecondEncoder(input_dim=input_dim)
-        # self.enc3 = SecondEncoder(input_dim=input_dim)
-        # self.enc4 = SecondEncoder(input_dim=input_dim)
-        # self.enc5 = SecondEncoder(input_dim=input_dim)
-        # self.dec0 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
-        # self.dec1 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
-        # self.dec2 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
-        # self.dec3 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
-        # self.dec4 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
-        # self.dec5 = Decoder(input_dim=input_dim, h_u=h_u, n_class=n_class)
-
     def forward(self, x):
         x_w = [x]
 
         x_w.append(self.encoders[0](x))
 
         for encoder in self.encoders[1:]:
             x_w.append(encoder(x, x_w[-1]))
@@ -274,32 +261,14 @@
             y_all.append(decoder(x_w[i]))
 
         y_all = torch.stack(y_all)
         y_mean = torch.mean(y_all, dim=0)
 
         return y_mean
 
-        # x_w0 = self.enc0(x)
-        # x_w1 = self.enc1(x, x_w0)
-        # x_w2 = self.enc2(x, x_w1)
-        # x_w3 = self.enc3(x, x_w2)
-        # x_w4 = self.enc4(x, x_w3)
-        # x_w5 = self.enc4(x, x_w4)
-        # y0 = self.dec0(x_w0)
-        # y1 = self.dec1(x_w1)
-        # y2 = self.dec2(x_w2)
-        # y3 = self.dec3(x_w3)
-        # y4 = self.dec4(x_w4)
-        # y5 = self.dec4(x_w5)
-
-        # y_all = torch.stack([y0, y1, y2, y3, y4, y5])
-        # y_mean = torch.mean(y_all, dim=0)
-
-        # return y_mean
-
 
 class AVModel(nn.Module):
     def __init__(self, shape_audio, shape_video, input_dim=512, h_u=512, h_f=64, n_class=500, encoder_decoder=5):
         super(AVModel, self).__init__()
         self.feature_audio = ResNet18(channels=shape_audio[2])
         self.fc_audio = nn.Linear(shape_audio[1], h_f)
         self.feature_video = CNNLSTMPyTorch()
```

### Comparing `openav-1.0.0a8/openav/modules/trml/shell.py` & `openav-1.0.0a9/openav/modules/trml/shell.py`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/openav.egg-info/PKG-INFO` & `openav-1.0.0a9/openav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
```

### Comparing `openav-1.0.0a8/openav.egg-info/SOURCES.txt` & `openav-1.0.0a9/openav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a8/setup.py` & `openav-1.0.0a9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "matplotlib >= 3.6.3",
     "mediapipe == 0.9.3.0",
     "opencv_contrib_python >= 4.9.0.80",
     "einops >= 0.7.0",
     "lion_pytorch >= 0.1.4",
     "scikit-learn >= 1.4.2",
     "tqdm >= 4.66.2",
+    "Seaborn >= 0.13.2",
 ]
 
 CLASSIFIERS = """\
 Development Status :: 3 - Alpha
 Natural Language :: Russian
 Natural Language :: English
 Intended Audience :: Developers
```

