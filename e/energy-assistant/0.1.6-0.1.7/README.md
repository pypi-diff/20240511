# Comparing `tmp/energy_assistant-0.1.6.tar.gz` & `tmp/energy_assistant-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energy_assistant-0.1.6.tar", last modified: Sat Mar 23 13:57:28 2024, max compression
+gzip compressed data, was "energy_assistant-0.1.7.tar", last modified: Sat May 11 19:41:58 2024, max compression
```

## Comparing `energy_assistant-0.1.6.tar` & `energy_assistant-0.1.7.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.056045 energy_assistant-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-03-23 13:57:28.056045 energy_assistant-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.044045 energy_assistant-0.1.6/energy_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    35405 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/EmhassOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.044045 energy_assistant-0.1.6/energy_assistant/api/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.044045 energy_assistant-0.1.6/energy_assistant/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/config/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/config/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.044045 energy_assistant-0.1.6/energy_assistant/api/device/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/device/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/device/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/device/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.044045 energy_assistant-0.1.6/energy_assistant/api/forecast/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/forecast/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/forecast/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/forecast/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.048045 energy_assistant-0.1.6/energy_assistant/api/history/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/history/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/history/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/history/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.048045 energy_assistant-0.1.6/energy_assistant/api/home_measurement/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/home_measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/home_measurement/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/home_measurement/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/home_measurement/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.048045 energy_assistant-0.1.6/energy_assistant/api/sessionlogs/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/sessionlogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/sessionlogs/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/sessionlogs/use_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/api/sessionlogs/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.048045 energy_assistant-0.1.6/energy_assistant/config/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/config/develop.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.040045 energy_assistant-0.1.6/energy_assistant/config/deviceregistry/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.048045 energy_assistant-0.1.6/energy_assistant/config/deviceregistry/v-zug/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/config/deviceregistry/v-zug/dishwasher adora s.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/config/deviceregistry/v-zug/dryer adora TS WP.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/config/local.env
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/config/test.env
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.052045 energy_assistant-0.1.6/energy_assistant/devices/
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/evcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/heat_pump.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/home.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/homeassistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/state_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/devices/utility_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.052045 energy_assistant-0.1.6/energy_assistant/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.052045 energy_assistant-0.1.6/energy_assistant/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/0bf7066b6d6c_first_commit.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/2558c9508fcc_extend_devices_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/2dbe1d6a4fa6_add_utility_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/81f94b4136ee_added_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/b6020d5b13fc_create_session_log_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/d43efed24fbc_drop_date_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/migrations/versions/efac279d8401_create_device_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.052045 energy_assistant-0.1.6/energy_assistant/models/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/device.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/home.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/models/sessionlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/energy_assistant/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.056045 energy_assistant-0.1.6/energy_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-03-23 13:57:28.000000 energy_assistant-0.1.6/energy_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-23 13:57:28.000000 energy_assistant-0.1.6/energy_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 13:57:28.000000 energy_assistant-0.1.6/energy_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-23 13:57:28.000000 energy_assistant-0.1.6/energy_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-23 13:57:28.000000 energy_assistant-0.1.6/energy_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-23 13:57:28.000000 energy_assistant-0.1.6/energy_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-03-23 13:57:25.000000 energy_assistant-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 13:57:28.056045 energy_assistant-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 13:57:28.056045 energy_assistant-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/tests/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/tests/test_state_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-23 13:57:23.000000 energy_assistant-0.1.6/tests/test_utility_meter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.404434 energy_assistant-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-11 19:41:58.404434 energy_assistant-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.392434 energy_assistant-0.1.7/energy_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    36074 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/EmhassOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/config/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/config/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/device/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/device/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/device/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/forecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/forecast/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/forecast/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/forecast/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/history/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/history/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/history/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/history/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/home_measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/home_measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/home_measurement/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/home_measurement/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/home_measurement/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.396433 energy_assistant-0.1.7/energy_assistant/api/sessionlogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/sessionlogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/sessionlogs/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/sessionlogs/use_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/api/sessionlogs/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.400434 energy_assistant-0.1.7/energy_assistant/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/config/develop.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.392434 energy_assistant-0.1.7/energy_assistant/config/deviceregistry/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.400434 energy_assistant-0.1.7/energy_assistant/config/deviceregistry/v-zug/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/config/deviceregistry/v-zug/dishwasher adora s.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/config/deviceregistry/v-zug/dryer adora TS WP.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/config/local.env
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/config/test.env
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.400434 energy_assistant-0.1.7/energy_assistant/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/evcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/heat_pump.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/homeassistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/state_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/devices/utility_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.400434 energy_assistant-0.1.7/energy_assistant/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.400434 energy_assistant-0.1.7/energy_assistant/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/0bf7066b6d6c_first_commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/2558c9508fcc_extend_devices_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/2dbe1d6a4fa6_add_utility_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/81f94b4136ee_added_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/b6020d5b13fc_create_session_log_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/d43efed24fbc_drop_date_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/migrations/versions/efac279d8401_create_device_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.404434 energy_assistant-0.1.7/energy_assistant/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10108 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/models/sessionlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/energy_assistant/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.404434 energy_assistant-0.1.7/energy_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-11 19:41:58.000000 energy_assistant-0.1.7/energy_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-11 19:41:58.000000 energy_assistant-0.1.7/energy_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:41:58.000000 energy_assistant-0.1.7/energy_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 19:41:58.000000 energy_assistant-0.1.7/energy_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-11 19:41:58.000000 energy_assistant-0.1.7/energy_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-11 19:41:58.000000 energy_assistant-0.1.7/energy_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-11 19:41:55.000000 energy_assistant-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 19:41:58.404434 energy_assistant-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:41:58.404434 energy_assistant-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/tests/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/tests/test_state_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-11 19:41:52.000000 energy_assistant-0.1.7/tests/test_utility_meter.py
```

### Comparing `energy_assistant-0.1.6/LICENSE` & `energy_assistant-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/PKG-INFO` & `energy_assistant-0.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energy_assistant
-Version: 0.1.6
+Version: 0.1.7
 Summary: Energy Assistant
 Author-email: The Energy Assistant Creators <pail23@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2024 Paul Frank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,44 +29,44 @@
 Keywords: energy assistant,home assistant
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: SQLAlchemy==2.0.28
+Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: requests==2.31.0
-Requires-Dist: fastapi==0.110.0
+Requires-Dist: fastapi==0.111.0
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: alembic==1.13.1
 Requires-Dist: aiosqlite==0.19.0
 Requires-Dist: python-dotenv
-Requires-Dist: uvicorn[standard]==0.27.1
+Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: apscheduler==3.10.4
-Requires-Dist: paho-mqtt==2.0.0
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: paho-mqtt==2.1.0
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: colorlog==6.8.0
-Requires-Dist: emhass==0.8.4
+Requires-Dist: emhass==0.9.0
 Requires-Dist: energy_assistant_frontend==0.0.56
 Provides-Extra: dev
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: black==24.2.0; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: codespell==2.2.6; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: ruff==0.3.2; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.5; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-env; extra == "dev"
-Requires-Dist: pre-commit==3.6.2; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 
 # Energy Assistant
 
 Energy Assistant is a free, opensource Energy Management System which works together with [Home Assistant](https://www.home-assistant.io/) and [Evcc](https://evcc.io/).
```

### Comparing `energy_assistant-0.1.6/Readme.md` & `energy_assistant-0.1.7/Readme.md`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/alembic.ini` & `energy_assistant-0.1.7/alembic.ini`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/EmhassOptimizer.py` & `energy_assistant-0.1.7/energy_assistant/EmhassOptimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Mqtt connection for energy assistant."""
 
 import copy
 import json
 import logging
 import pathlib
 import pickle
+import shutil
 import uuid
 from datetime import datetime, timezone
 from typing import Tuple
 
+import emhass  # type: ignore
 import numpy as np
 import pandas as pd
 from emhass import utils  # type: ignore
 from emhass.forecast import Forecast  # type: ignore
 from emhass.machine_learning_forecaster import MLForecaster  # type: ignore
 from emhass.optimization import Optimization  # type: ignore
 from emhass.retrieve_hass import RetrieveHass  # type: ignore
@@ -52,14 +54,29 @@
         self._location: Location = config.location
 
         home_config = config.energy_assistant_config.get("home")
         self._solar_power_id: str | None = None
         if home_config is not None:
             self._solar_power_id = home_config.get("solar_power")
         self._emhass_config: dict | None = config.emhass_config
+
+        cec_path = self._data_folder / "src/emhass/data"
+
+        if not cec_path.exists():
+            cec_path.mkdir(parents=True, exist_ok=True)
+
+        cec_src_path = pathlib.Path(emhass.__file__).parent / "data"
+        shutil.copy(str(cec_src_path / "cec_inverters.pbz2"), str(cec_path))
+        shutil.copy(str(cec_src_path / "cec_modules.pbz2"), str(cec_path))
+
+        self._emhass_path_conf = {}
+        self._emhass_path_conf["config_path"] = pathlib.Path("./energy_assistant.yaml")
+        self._emhass_path_conf["data_path"] = self._data_folder
+        self._emhass_path_conf["root_path"] = self._data_folder
+
         self._power_no_var_loads_id = (
             f"sensor.{DEFAULT_HASS_ENTITY_PREFIX}_{SENSOR_POWER_NO_VAR_LOADS}"
         )
         if self._emhass_config is not None:
             self._cost_fun = self._emhass_config.get("costfun", DEFAULT_COST_FUNC)
             self._hass_entity_prefix = self._emhass_config.get(
                 "hass_entity_prefix", DEFAULT_HASS_ENTITY_PREFIX
@@ -290,15 +307,15 @@
             self._logger,
         )  # type: ignore
         fcst = Forecast(
             self._RetrieveHass_conf,
             self._optim_conf,
             self._plant_conf,
             params,
-            str(self._data_folder),
+            self._emhass_path_conf,
             self._logger,
             get_data_from_file=False,
         )
         opt = Optimization(
             self._RetrieveHass_conf,
             self._optim_conf,
             self._plant_conf,
```

### Comparing `energy_assistant-0.1.6/energy_assistant/alembic.ini` & `energy_assistant-0.1.7/energy_assistant/alembic.ini`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/config/use_cases.py` & `energy_assistant-0.1.7/energy_assistant/api/config/use_cases.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/config/views.py` & `energy_assistant-0.1.7/energy_assistant/api/config/views.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/device/schema.py` & `energy_assistant-0.1.7/energy_assistant/api/device/schema.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/device/use_cases.py` & `energy_assistant-0.1.7/energy_assistant/api/device/use_cases.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/device/views.py` & `energy_assistant-0.1.7/energy_assistant/api/device/views.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/forecast/use_cases.py` & `energy_assistant-0.1.7/energy_assistant/api/forecast/use_cases.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/forecast/views.py` & `energy_assistant-0.1.7/energy_assistant/api/forecast/views.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/history/schema.py` & `energy_assistant-0.1.7/energy_assistant/api/history/schema.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/history/use_cases.py` & `energy_assistant-0.1.7/energy_assistant/api/history/use_cases.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/history/views.py` & `energy_assistant-0.1.7/energy_assistant/api/history/views.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/home_measurement/use_cases.py` & `energy_assistant-0.1.7/energy_assistant/api/home_measurement/use_cases.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/home_measurement/views.py` & `energy_assistant-0.1.7/energy_assistant/api/home_measurement/views.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/main.py` & `energy_assistant-0.1.7/energy_assistant/api/main.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/sessionlogs/schema.py` & `energy_assistant-0.1.7/energy_assistant/api/sessionlogs/schema.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/sessionlogs/use_cases.py` & `energy_assistant-0.1.7/energy_assistant/api/sessionlogs/use_cases.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/api/sessionlogs/views.py` & `energy_assistant-0.1.7/energy_assistant/api/sessionlogs/views.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/db.py` & `energy_assistant-0.1.7/energy_assistant/db.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/__init__.py` & `energy_assistant-0.1.7/energy_assistant/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/analysis.py` & `energy_assistant-0.1.7/energy_assistant/devices/analysis.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/config.py` & `energy_assistant-0.1.7/energy_assistant/devices/config.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/device.py` & `energy_assistant-0.1.7/energy_assistant/devices/device.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/evcc.py` & `energy_assistant-0.1.7/energy_assistant/devices/evcc.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/heat_pump.py` & `energy_assistant-0.1.7/energy_assistant/devices/heat_pump.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/home.py` & `energy_assistant-0.1.7/energy_assistant/devices/home.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/homeassistant.py` & `energy_assistant-0.1.7/energy_assistant/devices/homeassistant.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/registry.py` & `energy_assistant-0.1.7/energy_assistant/devices/registry.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/state_value.py` & `energy_assistant-0.1.7/energy_assistant/devices/state_value.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/devices/utility_meter.py` & `energy_assistant-0.1.7/energy_assistant/devices/utility_meter.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/main.py` & `energy_assistant-0.1.7/energy_assistant/main.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/alembic.ini` & `energy_assistant-0.1.7/energy_assistant/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/env.py` & `energy_assistant-0.1.7/energy_assistant/migrations/env.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/0bf7066b6d6c_first_commit.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/0bf7066b6d6c_first_commit.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/2558c9508fcc_extend_devices_fields.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/2558c9508fcc_extend_devices_fields.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/2dbe1d6a4fa6_add_utility_meter.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/2dbe1d6a4fa6_add_utility_meter.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/81f94b4136ee_added_power_mode.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/81f94b4136ee_added_power_mode.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/b6020d5b13fc_create_session_log_table.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/b6020d5b13fc_create_session_log_table.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/d43efed24fbc_drop_date_column.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/d43efed24fbc_drop_date_column.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/migrations/versions/efac279d8401_create_device_table.py` & `energy_assistant-0.1.7/energy_assistant/migrations/versions/efac279d8401_create_device_table.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/models/base.py` & `energy_assistant-0.1.7/energy_assistant/models/base.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/models/device.py` & `energy_assistant-0.1.7/energy_assistant/models/device.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/models/home.py` & `energy_assistant-0.1.7/energy_assistant/models/home.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/models/schema.py` & `energy_assistant-0.1.7/energy_assistant/models/schema.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/models/sessionlog.py` & `energy_assistant-0.1.7/energy_assistant/models/sessionlog.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/mqtt.py` & `energy_assistant-0.1.7/energy_assistant/mqtt.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/settings.py` & `energy_assistant-0.1.7/energy_assistant/settings.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/storage.py` & `energy_assistant-0.1.7/energy_assistant/storage.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant/websocket.py` & `energy_assistant-0.1.7/energy_assistant/websocket.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant.egg-info/PKG-INFO` & `energy_assistant-0.1.7/energy_assistant.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energy_assistant
-Version: 0.1.6
+Version: 0.1.7
 Summary: Energy Assistant
 Author-email: The Energy Assistant Creators <pail23@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2024 Paul Frank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -29,44 +29,44 @@
 Keywords: energy assistant,home assistant
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: SQLAlchemy==2.0.28
+Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: requests==2.31.0
-Requires-Dist: fastapi==0.110.0
+Requires-Dist: fastapi==0.111.0
 Requires-Dist: pydantic-settings==2.2.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: alembic==1.13.1
 Requires-Dist: aiosqlite==0.19.0
 Requires-Dist: python-dotenv
-Requires-Dist: uvicorn[standard]==0.27.1
+Requires-Dist: uvicorn[standard]==0.29.0
 Requires-Dist: apscheduler==3.10.4
-Requires-Dist: paho-mqtt==2.0.0
-Requires-Dist: jinja2==3.1.3
+Requires-Dist: paho-mqtt==2.1.0
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: colorlog==6.8.0
-Requires-Dist: emhass==0.8.4
+Requires-Dist: emhass==0.9.0
 Requires-Dist: energy_assistant_frontend==0.0.56
 Provides-Extra: dev
 Requires-Dist: httpx==0.27.0; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: black==24.2.0; extra == "dev"
+Requires-Dist: black==24.3.0; extra == "dev"
 Requires-Dist: codespell==2.2.6; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
-Requires-Dist: ruff==0.3.2; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
 Requires-Dist: pytest==8.1.1; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.5; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "dev"
-Requires-Dist: pytest-cov==4.1.0; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
 Requires-Dist: pytest-env; extra == "dev"
-Requires-Dist: pre-commit==3.6.2; extra == "dev"
+Requires-Dist: pre-commit==3.7.0; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 
 # Energy Assistant
 
 Energy Assistant is a free, opensource Energy Management System which works together with [Home Assistant](https://www.home-assistant.io/) and [Evcc](https://evcc.io/).
```

### Comparing `energy_assistant-0.1.6/energy_assistant.egg-info/SOURCES.txt` & `energy_assistant-0.1.7/energy_assistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/energy_assistant.egg-info/requires.txt` & `energy_assistant-0.1.7/energy_assistant.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-SQLAlchemy==2.0.28
+SQLAlchemy==2.0.30
 requests==2.31.0
-fastapi==0.110.0
+fastapi==0.111.0
 pydantic-settings==2.2.1
 pyyaml>=6.0.1
 alembic==1.13.1
 aiosqlite==0.19.0
 python-dotenv
-uvicorn[standard]==0.27.1
+uvicorn[standard]==0.29.0
 apscheduler==3.10.4
-paho-mqtt==2.0.0
-jinja2==3.1.3
+paho-mqtt==2.1.0
+jinja2==3.1.4
 colorlog==6.8.0
-emhass==0.8.4
+emhass==0.9.0
 energy_assistant_frontend==0.0.56
 
 [dev]
 httpx==0.27.0
 bumpver
 isort
 pip-tools
-black==24.2.0
+black==24.3.0
 codespell==2.2.6
 mypy==1.9.0
-ruff==0.3.2
+ruff==0.3.5
 pytest==8.1.1
-pytest-asyncio==0.23.5
+pytest-asyncio==0.23.6
 pytest-aiohttp==1.0.5
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-env
-pre-commit==3.6.2
+pre-commit==3.7.0
 types-PyYAML
 types-requests
 pandas-stubs
```

### Comparing `energy_assistant-0.1.6/pyproject.toml` & `energy_assistant-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=62.0.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "energy_assistant"
-version = "0.1.6"
+version = "0.1.7"
 description = "Energy Assistant"
 readme = "Readme.md"
 authors = [
     { name = "The Energy Assistant Creators", email = "pail23@users.noreply.github.com" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,51 +19,51 @@
     "Programming Language :: Python :: 3.11",
 ]
 keywords = [
     "energy assistant",
     "home assistant",
 ]
 dependencies = [
-    "SQLAlchemy==2.0.28",
+    "SQLAlchemy==2.0.30",
     "requests==2.31.0",
-    "fastapi==0.110.0",
+    "fastapi==0.111.0",
     "pydantic-settings==2.2.1",
     "pyyaml >= 6.0.1",
     "alembic==1.13.1",
     "aiosqlite==0.19.0",
     "python-dotenv",
-    "uvicorn[standard]==0.27.1",
+    "uvicorn[standard]==0.29.0",
     "apscheduler==3.10.4",
-    "paho-mqtt==2.0.0",
-    "jinja2==3.1.3",
+    "paho-mqtt==2.1.0",
+    "jinja2==3.1.4",
     "colorlog==6.8.0",
-    "emhass==0.8.4",
+    "emhass==0.9.0",
     "energy_assistant_frontend==0.0.56",
 ]
 requires-python = ">=3.11"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "httpx==0.27.0",
     "bumpver",
     "isort",
     "pip-tools",
-    "black==24.2.0",
+    "black==24.3.0",
     "codespell==2.2.6",
     "mypy==1.9.0",
-    "ruff==0.3.2",
+    "ruff==0.3.5",
     "pytest==8.1.1",
-    "pytest-asyncio==0.23.5",
+    "pytest-asyncio==0.23.6",
     "pytest-aiohttp==1.0.5",
-    "pytest-cov==4.1.0",
+    "pytest-cov==5.0.0",
     "pytest-env",
-    "pre-commit==3.6.2",
+    "pre-commit==3.7.0",
     "types-PyYAML",
     "types-requests",
     "pandas-stubs",
 ]
 
 [project.scripts]
 eass = "energy_assistant.main:main"
```

### Comparing `energy_assistant-0.1.6/requirements.txt` & `energy_assistant-0.1.7/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     #   watchfiles
 apscheduler==3.10.4
     # via energy_assistant (pyproject.toml)
 attrs==23.2.0
     # via aiohttp
 beautifulsoup4==4.12.2
     # via emhass
-black==24.2.0
+black==24.3.0
     # via energy_assistant (pyproject.toml)
 blinker==1.7.0
     # via flask
 blosc2==2.3.2
     # via tables
 build==1.0.3
     # via pip-tools
@@ -48,90 +48,107 @@
     # via requests
 click==8.1.7
     # via
     #   black
     #   bumpver
     #   flask
     #   pip-tools
+    #   typer
     #   uvicorn
 codespell==2.2.6
     # via energy_assistant (pyproject.toml)
 colorama==0.4.6
     # via bumpver
 colorlog==6.8.0
     # via
     #   energy_assistant (pyproject.toml)
     #   optuna
 coverage[toml]==7.4.0
     # via pytest-cov
 distlib==0.3.8
     # via virtualenv
-emhass==0.8.4
+dnspython==2.6.1
+    # via email-validator
+email-validator==2.1.1
+    # via fastapi
+emhass==0.9.0
     # via energy_assistant (pyproject.toml)
 energy-assistant-frontend==0.0.56
     # via energy_assistant (pyproject.toml)
-fastapi==0.110.0
-    # via energy_assistant (pyproject.toml)
+fastapi==0.111.0
+    # via
+    #   energy_assistant (pyproject.toml)
+    #   fastapi-cli
+fastapi-cli==0.0.3
+    # via fastapi
 filelock==3.13.1
     # via virtualenv
 flask==3.0.1
     # via emhass
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 greenlet==3.0.2
     # via sqlalchemy
 h11==0.14.0
     # via
     #   httpcore
     #   uvicorn
-h5py==3.10.0
+h5py==3.11.0
     # via
     #   emhass
     #   pvlib
 httpcore==1.0.2
     # via httpx
 httptools==0.6.1
     # via uvicorn
 httpx==0.27.0
-    # via energy_assistant (pyproject.toml)
+    # via
+    #   energy_assistant (pyproject.toml)
+    #   fastapi
 identify==2.5.33
     # via pre-commit
 idna==3.6
     # via
     #   anyio
+    #   email-validator
     #   httpx
     #   requests
     #   yarl
 iniconfig==2.0.0
     # via pytest
 isort==5.13.2
     # via energy_assistant (pyproject.toml)
 itsdangerous==2.1.2
     # via flask
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   energy_assistant (pyproject.toml)
+    #   fastapi
     #   flask
 joblib==1.3.2
     # via
     #   scikit-learn
     #   skforecast
 lexid==2021.1006
     # via bumpver
 looseversion==1.3.0
     # via bumpver
 mako==1.3.0
     # via alembic
+markdown-it-py==3.0.0
+    # via rich
 markupsafe==2.1.3
     # via
     #   jinja2
     #   mako
     #   werkzeug
+mdurl==0.1.2
+    # via markdown-it-py
 msgpack==1.0.7
     # via blosc2
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 mypy==1.9.0
@@ -158,23 +175,25 @@
     #   pvlib
     #   scikit-learn
     #   scipy
     #   skforecast
     #   tables
 optuna==3.4.0
     # via skforecast
+orjson==3.10.3
+    # via fastapi
 packaging==23.2
     # via
     #   black
     #   build
     #   optuna
     #   plotly
     #   pytest
     #   tables
-paho-mqtt==2.0.0
+paho-mqtt==2.1.0
     # via energy_assistant (pyproject.toml)
 pandas==2.0.3
     # via
     #   emhass
     #   pvlib
     #   skforecast
 pandas-stubs==2.1.4.231227
@@ -187,15 +206,15 @@
     # via
     #   black
     #   virtualenv
 plotly==5.18.0
     # via emhass
 pluggy==1.4.0
     # via pytest
-pre-commit==3.6.2
+pre-commit==3.7.0
     # via energy_assistant (pyproject.toml)
 protobuf==4.25.1
     # via emhass
 pulp==2.7.0
     # via emhass
 pvlib==0.10.2
     # via emhass
@@ -207,40 +226,44 @@
     # via
     #   fastapi
     #   pydantic-settings
 pydantic-core==2.14.5
     # via pydantic
 pydantic-settings==2.2.1
     # via energy_assistant (pyproject.toml)
+pygments==2.18.0
+    # via rich
 pyproject-hooks==1.0.0
     # via build
 pytest==8.1.1
     # via
     #   energy_assistant (pyproject.toml)
     #   pytest-aiohttp
     #   pytest-asyncio
     #   pytest-cov
     #   pytest-env
 pytest-aiohttp==1.0.5
     # via energy_assistant (pyproject.toml)
-pytest-asyncio==0.23.5
+pytest-asyncio==0.23.6
     # via
     #   energy_assistant (pyproject.toml)
     #   pytest-aiohttp
-pytest-cov==4.1.0
+pytest-cov==5.0.0
     # via energy_assistant (pyproject.toml)
 pytest-env==1.1.3
     # via energy_assistant (pyproject.toml)
 python-dateutil==2.8.2
     # via pandas
 python-dotenv==1.0.0
     # via
     #   energy_assistant (pyproject.toml)
     #   pydantic-settings
     #   uvicorn
+python-multipart==0.0.9
+    # via fastapi
 pytz==2023.3.post1
     # via
     #   apscheduler
     #   emhass
     #   pandas
     #   pvlib
 pyyaml==6.0.1
@@ -251,78 +274,90 @@
     #   pre-commit
     #   uvicorn
 requests==2.31.0
     # via
     #   emhass
     #   energy_assistant (pyproject.toml)
     #   pvlib
-ruff==0.3.2
+rich==13.7.1
+    # via typer
+ruff==0.3.5
     # via energy_assistant (pyproject.toml)
 scikit-learn==1.3.2
     # via skforecast
 scipy==1.12.0
     # via
     #   emhass
     #   pvlib
     #   scikit-learn
+shellingham==1.5.4
+    # via typer
 six==1.16.0
     # via
     #   apscheduler
     #   python-dateutil
-skforecast==0.11.0
+skforecast==0.12.0
     # via emhass
 sniffio==1.3.0
     # via
     #   anyio
     #   httpx
 soupsieve==2.5
     # via beautifulsoup4
-sqlalchemy==2.0.28
+sqlalchemy==2.0.30
     # via
     #   alembic
     #   energy_assistant (pyproject.toml)
     #   optuna
-starlette==0.36.3
+starlette==0.37.2
     # via fastapi
 tables==3.9.1
     # via emhass
 tenacity==8.2.3
     # via plotly
 threadpoolctl==3.2.0
     # via scikit-learn
 toml==0.10.2
     # via bumpver
 tqdm==4.66.1
     # via
     #   optuna
     #   skforecast
+typer==0.12.3
+    # via fastapi-cli
 types-pytz==2023.3.1.1
     # via pandas-stubs
 types-pyyaml==6.0.12.12
     # via energy_assistant (pyproject.toml)
 types-requests==2.31.0.20231231
     # via energy_assistant (pyproject.toml)
 typing-extensions==4.9.0
     # via
     #   alembic
     #   fastapi
     #   mypy
     #   pydantic
     #   pydantic-core
     #   sqlalchemy
+    #   typer
 tzdata==2023.3
     # via pandas
 tzlocal==5.2
     # via apscheduler
+ujson==5.9.0
+    # via fastapi
 urllib3==2.1.0
     # via
     #   requests
     #   types-requests
-uvicorn[standard]==0.27.1
-    # via energy_assistant (pyproject.toml)
+uvicorn[standard]==0.29.0
+    # via
+    #   energy_assistant (pyproject.toml)
+    #   fastapi
+    #   fastapi-cli
 uvloop==0.19.0
     # via uvicorn
 virtualenv==20.25.0
     # via pre-commit
 waitress==2.1.2
     # via emhass
 watchfiles==0.21.0
```

### Comparing `energy_assistant-0.1.6/tests/test_analysis.py` & `energy_assistant-0.1.7/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/tests/test_devices.py` & `energy_assistant-0.1.7/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `energy_assistant-0.1.6/tests/test_state_value.py` & `energy_assistant-0.1.7/tests/test_state_value.py`

 * *Files identical despite different names*

