# Comparing `tmp/neon-utils-1.9.2a4.tar.gz` & `tmp/neon-utils-1.9.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-utils-1.9.2a4.tar", last modified: Tue Apr  9 19:51:46 2024, max compression
+gzip compressed data, was "neon-utils-1.9.2a5.tar", last modified: Thu Apr 18 19:48:28 2024, max compression
```

## Comparing `neon-utils-1.9.2a4.tar` & `neon-utils-1.9.2a5.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.529284 neon-utils-1.9.2a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 19:51:46.529284 neon-utils-1.9.2a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.517284 neon-utils-1.9.2a4/neon_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/authentication_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    68558 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/configuration_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.517284 neon-utils-1.9.2a4/neon_utils/default_configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/default_configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/default_configurations/default_user_conf.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/hana_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/language_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/location_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/messagebus_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/mq_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/process_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.513284 neon-utils-1.9.2a4/neon_utils/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.521284 neon-utils-1.9.2a4/neon_utils/res/snd/
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/snd/acknowledge.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   428660 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/snd/loaded.wav
--rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/snd/start_listening.wav
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.513284 neon-utils-1.9.2a4/neon_utils/res/text/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.521284 neon-utils-1.9.2a4/neon_utils/res/text/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/text/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/text/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/text/en-us/stop.voc
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/text/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.521284 neon-utils-1.9.2a4/neon_utils/res/ui/
--rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/res/ui/neon_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.521284 neon-utils-1.9.2a4/neon_utils/skills/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/common_message_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/common_play_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/common_query_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/instructor_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/kiosk_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/mycroft_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    38699 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/neon_fallback_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)    38468 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/neon_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/skills/skill_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/socket_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/validator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/neon_utils/web_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.517284 neon-utils-1.9.2a4/neon_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-09 19:51:46.000000 neon-utils-1.9.2a4/neon_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-09 19:51:46.000000 neon-utils-1.9.2a4/neon_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:51:46.000000 neon-utils-1.9.2a4/neon_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-09 19:51:46.000000 neon-utils-1.9.2a4/neon_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-09 19:51:46.000000 neon-utils-1.9.2a4/neon_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-09 19:51:46.000000 neon-utils-1.9.2a4/neon_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 19:51:46.529284 neon-utils-1.9.2a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.525284 neon-utils-1.9.2a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/authentication_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/cache_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    63829 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/configuration_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/file_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/hana_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/language_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/location_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/log_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/message_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/messagebus_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/metric_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/mq_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    57964 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/neon_skill_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/net_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/packaging_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/parse_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/search_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/signal_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.525284 neon-utils-1.9.2a4/tests/skills/
--rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/skills/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.529284 neon-utils-1.9.2a4/tests/skills/test_skill/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/skills/test_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/skills/test_skill/settingsmeta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/socket_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/user_util_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:51:46.529284 neon-utils-1.9.2a4/tests/valid_skill/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/valid_skill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/validator_util_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-09 19:51:43.000000 neon-utils-1.9.2a4/tests/web_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.125346 neon-utils-1.9.2a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 19:48:28.125346 neon-utils-1.9.2a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.113345 neon-utils-1.9.2a5/neon_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/authentication_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68558 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/configuration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.117345 neon-utils-1.9.2a5/neon_utils/default_configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/default_configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/default_configurations/default_user_conf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/hana_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/language_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/location_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8727 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/messagebus_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/mq_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/process_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.109346 neon-utils-1.9.2a5/neon_utils/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.117345 neon-utils-1.9.2a5/neon_utils/res/snd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/snd/acknowledge.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)   428660 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/snd/loaded.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    67090 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/snd/start_listening.wav
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.109346 neon-utils-1.9.2a5/neon_utils/res/text/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.117345 neon-utils-1.9.2a5/neon_utils/res/text/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/text/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/text/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/text/en-us/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/text/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.117345 neon-utils-1.9.2a5/neon_utils/res/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/res/ui/neon_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.121346 neon-utils-1.9.2a5/neon_utils/skills/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9762 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/common_message_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/common_play_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/common_query_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/instructor_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8138 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/kiosk_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/mycroft_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38699 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/neon_fallback_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38468 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/neon_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/skills/skill_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/socket_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/validator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/neon_utils/web_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.117345 neon-utils-1.9.2a5/neon_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 19:48:28.000000 neon-utils-1.9.2a5/neon_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-18 19:48:28.000000 neon-utils-1.9.2a5/neon_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:48:28.000000 neon-utils-1.9.2a5/neon_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 19:48:28.000000 neon-utils-1.9.2a5/neon_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-18 19:48:28.000000 neon-utils-1.9.2a5/neon_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 19:48:28.000000 neon-utils-1.9.2a5/neon_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:48:28.125346 neon-utils-1.9.2a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.121346 neon-utils-1.9.2a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/authentication_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/cache_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63829 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/configuration_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/file_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/hana_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/language_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/location_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/log_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/message_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/messagebus_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/metric_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/mq_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57964 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/neon_skill_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/net_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/packaging_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/parse_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/search_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/signal_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.125346 neon-utils-1.9.2a5/tests/skills/
+-rw-r--r--   0 runner    (1001) docker     (127)     5219 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/skills/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.125346 neon-utils-1.9.2a5/tests/skills/test_skill/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/skills/test_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/skills/test_skill/settingsmeta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/socket_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/user_util_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:48:28.125346 neon-utils-1.9.2a5/tests/valid_skill/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/valid_skill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/validator_util_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-18 19:48:24.000000 neon-utils-1.9.2a5/tests/web_util_tests.py
```

### Comparing `neon-utils-1.9.2a4/LICENSE.md` & `neon-utils-1.9.2a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/PKG-INFO` & `neon-utils-1.9.2a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.9.2a4
+Version: 1.9.2a5
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.9.2a4/neon_utils/__init__.py` & `neon-utils-1.9.2a5/neon_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/authentication_utils.py` & `neon-utils-1.9.2a5/neon_utils/authentication_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/cache_utils.py` & `neon-utils-1.9.2a5/neon_utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/configuration_utils.py` & `neon-utils-1.9.2a5/neon_utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/decorators.py` & `neon-utils-1.9.2a5/neon_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/default_configurations/__init__.py` & `neon-utils-1.9.2a5/neon_utils/default_configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/default_configurations/default_user_conf.yml` & `neon-utils-1.9.2a5/neon_utils/default_configurations/default_user_conf.yml`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/file_utils.py` & `neon-utils-1.9.2a5/neon_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/hana_utils.py` & `neon-utils-1.9.2a5/neon_utils/hana_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/language_utils.py` & `neon-utils-1.9.2a5/neon_utils/language_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/location_utils.py` & `neon-utils-1.9.2a5/neon_utils/location_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,15 +122,16 @@
         return None
     location = address.reverse([lat, lng], language="en-US")
     LOG.debug(f"{location}")
     LOG.debug(f"{location.raw}")
     LOG.debug(f"{location.raw.get('address')}")
     city = location.raw.get('address').get('city') or \
         location.raw.get('address').get('town') or \
-        location.raw.get('address').get('village')
+        location.raw.get('address').get('village') or \
+        location.raw.get('address').get('hamlet')
     county = location.raw.get('address').get('county')
     state = location.raw.get('address').get('state')
     country = location.raw.get('address').get('country')
     return city, county, state, country
 
 
 def get_timezone(lat, lng) -> (str, float):
```

### Comparing `neon-utils-1.9.2a4/neon_utils/log_utils.py` & `neon-utils-1.9.2a5/neon_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/logger.py` & `neon-utils-1.9.2a5/neon_utils/logger.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/message_utils.py` & `neon-utils-1.9.2a5/neon_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/messagebus_utils.py` & `neon-utils-1.9.2a5/neon_utils/messagebus_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/metrics_utils.py` & `neon-utils-1.9.2a5/neon_utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/mq_utils.py` & `neon-utils-1.9.2a5/neon_utils/mq_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/net_utils.py` & `neon-utils-1.9.2a5/neon_utils/net_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/packaging_utils.py` & `neon-utils-1.9.2a5/neon_utils/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/parse_utils.py` & `neon-utils-1.9.2a5/neon_utils/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/process_utils.py` & `neon-utils-1.9.2a5/neon_utils/process_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/res/snd/acknowledge.mp3` & `neon-utils-1.9.2a5/neon_utils/res/snd/acknowledge.mp3`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/res/snd/loaded.wav` & `neon-utils-1.9.2a5/neon_utils/res/snd/loaded.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/res/snd/start_listening.wav` & `neon-utils-1.9.2a5/neon_utils/res/snd/start_listening.wav`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/res/ui/neon_logo.png` & `neon-utils-1.9.2a5/neon_utils/res/ui/neon_logo.png`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/search_utils.py` & `neon-utils-1.9.2a5/neon_utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/signal_utils.py` & `neon-utils-1.9.2a5/neon_utils/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/__init__.py` & `neon-utils-1.9.2a5/neon_utils/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/common_message_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/common_message_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/common_play_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/common_play_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/common_query_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/common_query_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/instructor_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/instructor_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/kiosk_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/kiosk_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/mycroft_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/mycroft_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/neon_fallback_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/neon_fallback_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/neon_skill.py` & `neon-utils-1.9.2a5/neon_utils/skills/neon_skill.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/skills/skill_gui.py` & `neon-utils-1.9.2a5/neon_utils/skills/skill_gui.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/socket_utils.py` & `neon-utils-1.9.2a5/neon_utils/socket_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/user_utils.py` & `neon-utils-1.9.2a5/neon_utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/validator_utils.py` & `neon-utils-1.9.2a5/neon_utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils/web_utils.py` & `neon-utils-1.9.2a5/neon_utils/web_utils.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils.egg-info/PKG-INFO` & `neon-utils-1.9.2a5/neon_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-utils
-Version: 1.9.2a4
+Version: 1.9.2a5
 Summary: Utilities for NeonAI
 Home-page: https://github.com/neongeckocom/neon-skill-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-utils-1.9.2a4/neon_utils.egg-info/SOURCES.txt` & `neon-utils-1.9.2a5/neon_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/neon_utils.egg-info/requires.txt` & `neon-utils-1.9.2a5/neon_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/setup.py` & `neon-utils-1.9.2a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/__init__.py` & `neon-utils-1.9.2a5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/authentication_util_tests.py` & `neon-utils-1.9.2a5/tests/authentication_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/cache_util_tests.py` & `neon-utils-1.9.2a5/tests/cache_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/configuration_util_tests.py` & `neon-utils-1.9.2a5/tests/configuration_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/file_util_tests.py` & `neon-utils-1.9.2a5/tests/file_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/hana_util_tests.py` & `neon-utils-1.9.2a5/tests/hana_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/language_util_tests.py` & `neon-utils-1.9.2a5/tests/language_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/location_util_tests.py` & `neon-utils-1.9.2a5/tests/location_util_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,18 @@
         lat = 47.6038321
         lng = -122.3300624
         location = get_location(lat, lng)
         self.assertEqual(len(location), 4)
         self.assertEqual(location, ("Seattle", "King County", "Washington",
                                     "United States"))
 
+        # Test 'hamlet' location
+        location = get_location(34.46433387046654, -81.99487538579375)
+        self.assertIsInstance(location[0], str)
+
     def test_get_timezone_from_coords(self):
         from neon_utils.location_utils import get_timezone
         lat = 47.6038321
         lng = -122.3300624
         timezone, offset = get_timezone(lat, lng)
         self.assertIsInstance(timezone, str)
         self.assertEqual(timezone, "America/Los_Angeles")
```

### Comparing `neon-utils-1.9.2a4/tests/log_util_tests.py` & `neon-utils-1.9.2a5/tests/log_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/message_util_tests.py` & `neon-utils-1.9.2a5/tests/message_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/messagebus_util_tests.py` & `neon-utils-1.9.2a5/tests/messagebus_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/metric_util_tests.py` & `neon-utils-1.9.2a5/tests/metric_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/mq_util_tests.py` & `neon-utils-1.9.2a5/tests/mq_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/neon_skill_tests.py` & `neon-utils-1.9.2a5/tests/neon_skill_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/net_util_tests.py` & `neon-utils-1.9.2a5/tests/net_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/packaging_util_tests.py` & `neon-utils-1.9.2a5/tests/packaging_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/parse_util_tests.py` & `neon-utils-1.9.2a5/tests/parse_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/search_util_tests.py` & `neon-utils-1.9.2a5/tests/search_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/signal_util_tests.py` & `neon-utils-1.9.2a5/tests/signal_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/skills/__init__.py` & `neon-utils-1.9.2a5/tests/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/skills/test_skill/__init__.py` & `neon-utils-1.9.2a5/tests/skills/test_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/socket_utils_tests.py` & `neon-utils-1.9.2a5/tests/socket_utils_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/user_util_tests.py` & `neon-utils-1.9.2a5/tests/user_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/valid_skill/__init__.py` & `neon-utils-1.9.2a5/tests/valid_skill/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/validator_util_tests.py` & `neon-utils-1.9.2a5/tests/validator_util_tests.py`

 * *Files identical despite different names*

### Comparing `neon-utils-1.9.2a4/tests/web_util_tests.py` & `neon-utils-1.9.2a5/tests/web_util_tests.py`

 * *Files identical despite different names*

