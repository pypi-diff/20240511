# Comparing `tmp/layrz_sdk-3.0.0.tar.gz` & `tmp/layrz_sdk-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz_sdk-3.0.0.tar", last modified: Fri Apr 26 06:22:50 2024, max compression
+gzip compressed data, was "layrz_sdk-3.0.1.tar", last modified: Sat May 11 19:57:07 2024, max compression
```

## Comparing `layrz_sdk-3.0.0.tar` & `layrz_sdk-3.0.1.tar`

### file list

```diff
@@ -1,88 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/
--rw-rw-r--   0 root         (0) root         (0)     1057 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1458 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      628 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/
--rw-rw-r--   0 root         (0) root         (0)       28 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/entities/
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/
--rw-rw-r--   0 root         (0) root         (0)      215 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      566 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/request.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/response.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/result.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/service.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.170030 layrz_sdk-3.0.0/layrz_sdk/entities/cases/
--rw-rw-r--   0 root         (0) root         (0)      135 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/case.py
--rw-rw-r--   0 root         (0) root         (0)      902 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/comment.py
--rw-rw-r--   0 root         (0) root         (0)      629 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/cases/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.174030 layrz_sdk-3.0.0/layrz_sdk/entities/charts/
--rw-rw-r--   0 root         (0) root         (0)      753 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      438 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/alignment.py
--rw-rw-r--   0 root         (0) root         (0)     3867 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/bar.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/column.py
--rw-rw-r--   0 root         (0) root         (0)      514 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/configuration.py
--rw-rw-r--   0 root         (0) root         (0)      447 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/data_type.py
--rw-rw-r--   0 root         (0) root         (0)      558 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      995 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/html.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/line.py
--rw-rw-r--   0 root         (0) root         (0)     4230 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/map.py
--rw-rw-r--   0 root         (0) root         (0)      811 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/number.py
--rw-rw-r--   0 root         (0) root         (0)     2972 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/pie.py
--rw-rw-r--   0 root         (0) root         (0)     3155 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/radar.py
--rw-rw-r--   0 root         (0) root         (0)     3011 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/radial_bar.py
--rw-rw-r--   0 root         (0) root         (0)     4871 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/scatter.py
--rw-rw-r--   0 root         (0) root         (0)     1509 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/serie.py
--rw-rw-r--   0 root         (0) root         (0)      463 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/serie_type.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/table.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/charts/timeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/
--rw-rw-r--   0 root         (0) root         (0)      126 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1040 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/checkpoint.py
--rw-rw-r--   0 root         (0) root         (0)      653 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/geofence.py
--rw-rw-r--   0 root         (0) root         (0)     1236 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/waypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/events/
--rw-rw-r--   0 root         (0) root         (0)       49 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/events/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/formatting/
--rw-rw-r--   0 root         (0) root         (0)       66 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/formatting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      467 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/formatting/text_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/general/
--rw-rw-r--   0 root         (0) root         (0)      218 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1786 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/asset.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/asset_operation_mode.py
--rw-rw-r--   0 root         (0) root         (0)      606 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/custom_field.py
--rw-rw-r--   0 root         (0) root         (0)      973 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/device.py
--rw-rw-r--   0 root         (0) root         (0)      615 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/sensor.py
--rw-rw-r--   0 root         (0) root         (0)      527 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/general/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.178030 layrz_sdk-3.0.0/layrz_sdk/entities/repcom/
--rw-rw-r--   0 root         (0) root         (0)       61 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/repcom/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1461 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/repcom/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/entities/reports/
--rw-rw-r--   0 root         (0) root         (0)      249 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1961 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/col.py
--rw-rw-r--   0 root         (0) root         (0)      442 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/format.py
--rw-rw-r--   0 root         (0) root         (0)     1408 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/header.py
--rw-rw-r--   0 root         (0) root         (0)     1574 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/page.py
--rw-rw-r--   0 root         (0) root         (0)     6444 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/report.py
--rw-rw-r--   0 root         (0) root         (0)      881 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/reports/row.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/
--rw-rw-r--   0 root         (0) root         (0)       87 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      789 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/message.py
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/helpers/
--rw-rw-r--   0 root         (0) root         (0)       72 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/helpers/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk/lcl/
--rw-rw-r--   0 root         (0) root         (0)       67 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/lcl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20608 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/layrz_sdk/lcl/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2505 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-26 06:22:50.000000 layrz_sdk-3.0.0/layrz_sdk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     7589 2024-04-26 06:20:42.000000 layrz_sdk-3.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 06:22:50.182030 layrz_sdk-3.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/
+-rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.351812 layrz_sdk-3.0.1/layrz_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.351812 layrz_sdk-3.0.1/layrz_sdk/entities/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.355812 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/
+-rw-rw-r--   0 root         (0) root         (0)      215 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      566 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/request.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/response.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/result.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/service.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.355812 layrz_sdk-3.0.1/layrz_sdk/entities/cases/
+-rw-rw-r--   0 root         (0) root         (0)      135 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/case.py
+-rw-rw-r--   0 root         (0) root         (0)      902 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/comment.py
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/charts/
+-rw-rw-r--   0 root         (0) root         (0)      753 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/alignment.py
+-rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/column.py
+-rw-rw-r--   0 root         (0) root         (0)      514 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)      447 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/data_type.py
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/html.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/line.py
+-rw-rw-r--   0 root         (0) root         (0)     4230 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/map.py
+-rw-rw-r--   0 root         (0) root         (0)      811 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/number.py
+-rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/pie.py
+-rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/radar.py
+-rw-rw-r--   0 root         (0) root         (0)     3011 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/radial_bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4871 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/scatter.py
+-rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/serie.py
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/serie_type.py
+-rw-rw-r--   0 root         (0) root         (0)     1344 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/table.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/timeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/
+-rw-rw-r--   0 root         (0) root         (0)      126 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/checkpoint.py
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/geofence.py
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/waypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/events/
+-rw-rw-r--   0 root         (0) root         (0)       49 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/events/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/formatting/
+-rw-rw-r--   0 root         (0) root         (0)       66 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/formatting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      467 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/formatting/text_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/general/
+-rw-rw-r--   0 root         (0) root         (0)      218 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/asset.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/asset_operation_mode.py
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/custom_field.py
+-rw-rw-r--   0 root         (0) root         (0)      973 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/device.py
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/sensor.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/repcom/
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/repcom/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/repcom/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/entities/reports/
+-rw-rw-r--   0 root         (0) root         (0)      249 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/col.py
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/format.py
+-rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/header.py
+-rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/page.py
+-rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/report.py
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/row.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      789 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/message.py
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/helpers/
+-rw-rw-r--   0 root         (0) root         (0)       72 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/helpers/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/lcl/
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/lcl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22683 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/lcl/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/tests/test_lcl.py
```

### Comparing `layrz_sdk-3.0.0/LICENSE` & `layrz_sdk-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/PKG-INFO` & `layrz_sdk-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.0
+Version: 3.0.1
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.0/README.md` & `layrz_sdk-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/__init__.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/request.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/request.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/response.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/response.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/result.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/result.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/service.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/service.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/broadcasts/status.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/status.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/cases/case.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/cases/case.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/cases/comment.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/cases/comment.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/cases/trigger.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/cases/trigger.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/__init__.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/bar.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/bar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/column.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/column.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/configuration.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/configuration.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/exceptions.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/html.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/html.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/line.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/line.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/map.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/map.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/number.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/number.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/pie.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/pie.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/radar.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/radar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/radial_bar.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/radial_bar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/scatter.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/scatter.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/serie.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/serie.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/table.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/table.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/charts/timeline.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/charts/timeline.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/checkpoint.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/checkpoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/geofence.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/geofence.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/checkpoints/waypoint.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/waypoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/events/event.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/events/event.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/general/asset.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/general/asset.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/general/asset_operation_mode.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/general/asset_operation_mode.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/general/custom_field.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/general/custom_field.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/general/device.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/general/device.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/general/sensor.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/general/sensor.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/general/user.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/general/user.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/repcom/transaction.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/repcom/transaction.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/reports/col.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/reports/col.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/reports/header.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/reports/header.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/reports/page.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/reports/page.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/reports/report.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/reports/report.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/reports/row.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/reports/row.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/message.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/message.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/entities/telemetry/position.py` & `layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/position.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/helpers/color.py` & `layrz_sdk-3.0.1/layrz_sdk/helpers/color.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.0/layrz_sdk/lcl/core.py` & `layrz_sdk-3.0.1/layrz_sdk/lcl/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,14 +124,17 @@
       return json.dumps(INVALID_ARGUMENTS.format(e=err))
 
   def GET_PARAM(self, *args: list[Any]) -> Any:
     """ GET_PARAM Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None:
+      return None
+
     if len(args) > 1:
       return self._payload.get(args[0], args[1])
     return self._payload.get(args[0], None)
 
   def GET_DISTANCE_TRAVELED(self, *args: list[Any]) -> str | float:
     """ GET_DISTANCE_TRAVELED Function """
     if len(args) > 0:
@@ -142,26 +145,32 @@
     """ GET_PREVIOUS_SENSOR Function """
     if len(args) < 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None:
+      return None
+
     if len(args) > 1:
       return self._previous_sensors.get(args[0], args[1])
     return self._previous_sensors.get(args[0], None)
 
   def GET_SENSOR(self, *args: list[Any]) -> Any:
     """ GET_SENSOR Function """
     if len(args) < 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None:
+      return None
+
     if len(args) > 1:
       return self._sensors.get(args[0], args[1])
     return self._sensors.get(args[0], None)
 
   def CONSTANT(self, *args: list[Any]) -> Any:
     """ CONSTANT Function """
     if len(args) > 1:
@@ -179,15 +188,15 @@
     if len(args) != 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
     if args[0] is None or args[1] is None:
       return None
 
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES.format(arg1=type(args[0]), arg2=type(args[1]))
+      return DIFFERENT_TYPES.format(arg1=type(args[0]).__name__, arg2=type(args[1]).__name__)
     return args[0] == args[1]
 
   def OR_OPERATOR(self, *args: list[Any]) -> bool:
     """ OR_OPERATOR Function """
     result = False
 
     for val in args:
@@ -202,44 +211,47 @@
     """ AND_OPERATOR Function """
     result = False
     is_first = True
 
     for val in args:
       if val is None:
         return None
+
       if is_first:
         is_first = False
         result = val
       elif isinstance(val, bool):
         result = result and val
 
     return result
 
   def SUM(self, *args: list[Any]) -> float:
     """ SUM Function """
     result = 0
 
     for num in args:
       if num is None:
-        continue
+        return None
+
       try:
         result += float(num)
       except Exception:  # pylint: disable=broad-except
         pass
 
     return result
 
   def SUBSTRACT(self, *args: list[Any]) -> float:
     """ SUBSTRACT Function """
     result = 0
     is_first = True
 
     for num in args:
       if num is None:
-        continue
+        return None
+
       try:
         if is_first:
           result = float(num)
           is_first = False
         else:
           result -= float(num)
       except Exception:  # pylint: disable=broad-except
@@ -250,15 +262,16 @@
   def MULTIPLY(self, *args: list[Any]) -> float:
     """ MULTIPLY Function """
     result = 0
     is_first = True
 
     for num in args:
       if num is None:
-        continue
+        return None
+
       try:
         if is_first:
           is_first = False
           result = float(num)
         else:
           result *= float(num)
       except Exception:  # pylint: disable=broad-except
@@ -269,15 +282,16 @@
   def DIVIDE(self, *args: list[Any]) -> float:
     """ DIVIDE Function """
     result = 0
     is_first = True
 
     for num in args:
       if num is None:
-        continue
+        return None
+
       try:
         if is_first:
           is_first = False
           result = float(num)
         else:
           result /= float(num)
       except Exception:  # pylint: disable=broad-except
@@ -285,256 +299,330 @@
 
     return result
 
   def TO_BOOL(self, *args: list[Any]) -> str | None | bool:
     """ TO_BOOL Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
     return bool(args[0])
 
   def TO_STR(self, *args: list[Any]) -> str | None:
     """ TO_STR Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None:
       return None
+
     return str(args[0])
 
   def TO_INT(self, *args: list[Any]) -> str | None | int:
     """ TO_INT Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
     return int(args[0])
 
   def CEIL(self, *args: list[Any]) -> str | None | int:
     """ CEIL Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
+    if not isinstance(args[0], (int, float)):
+      return f'Invalid arguments - must be real number, not {type(args[0]).__name__}'
+
     import math
     return math.ceil(args[0])
 
   def FLOOR(self, *args: list[Any]) -> str | None | int:
     """ FLOOR Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
+    if not isinstance(args[0], (int, float)):
+      return f'Invalid arguments - must be real number, not {type(args[0]).__name__}'
+
     import math
     return math.floor(args[0])
 
   def ROUND(self, *args: list[Any]) -> str | None | int:
     """ ROUND Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
+    if not isinstance(args[0], (int, float)):
+      return f'Invalid arguments - must be real number, not {type(args[0]).__name__}'
+
     return round(args[0])
 
   def SQRT(self, *args: list[Any]) -> str | None | float:
     """ SQRT Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
     import math
     return math.sqrt(args[0])
 
   def CONCAT(self, *args: list[Any]) -> str | None:
     """ CONCAT Function """
     for val in args:
       if val is None:
         return None
+
     return ''.join([str(val) for val in args])
 
   def RANDOM(self, *args: list[Any]) -> float | str:
     """ RANDOM Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None or args[1] is None:
+      return None
+
     import random
     return random.random() * (float(args[1]) - float(args[0])) + float(args[0])
 
   def RANDOM_INT(self, *args: list[Any]) -> int | str:
     """ RANDOM_INT Function """
     if len(args) != 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None or args[1] is None:
+      return None
+
     import random
     return random.randint(int(args[0]), int(args[1]))
 
   def GREATER_THAN_OR_EQUALS_TO(self, *args: list[Any]) -> str | None | bool:
     """ GREATER_THAN_OR_EQUALS_TO Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None or args[1] is None:
       return None
 
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES.format(arg1=type(args[0]), arg2=type(args[1]))
+      return DIFFERENT_TYPES.format(arg1=type(args[0]).__name__, arg2=type(args[1]).__name__)
     return args[0] >= args[1]
 
   def GREATER_THAN(self, *args: list[Any]) -> str | None | bool:
     """ GREATER_THAN Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None or args[1] is None:
       return None
 
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES.format(arg1=type(args[0]), arg2=type(args[1]))
+      return DIFFERENT_TYPES.format(arg1=type(args[0]).__name__, arg2=type(args[1]).__name__)
     return args[0] > args[1]
 
   def LESS_THAN_OR_EQUALS_TO(self, *args: list[Any]) -> str | None | bool:
     """ LESS_THAN_OR_EQUALS_TO Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None or args[1] is None:
       return None
 
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES.format(arg1=type(args[0]), arg2=type(args[1]))
+      return DIFFERENT_TYPES.format(arg1=type(args[0]).__name__, arg2=type(args[1]).__name__)
     return args[0] <= args[1]
 
   def LESS_THAN(self, *args: list[Any]) -> str | None | bool:
     """ LESS_THAN Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None or args[1] is None:
       return None
 
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES.format(arg1=type(args[0]), arg2=type(args[1]))
+      return DIFFERENT_TYPES.format(arg1=type(args[0]).__name__, arg2=type(args[1]).__name__)
     return args[0] < args[1]
 
   def DIFFERENT(self, *args: list[Any]) -> str | None | bool:
     """ DIFFERENT Function """
     if len(args) > 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None or args[1] is None:
       return None
 
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES.format(arg1=type(args[0]), arg2=type(args[1]))
+      return DIFFERENT_TYPES.format(arg1=type(args[0]).__name__, arg2=type(args[1]).__name__)
     return args[0] != args[1]
 
   def HEX_TO_STR(self, *args: list[Any]) -> str | None:
     """ HEX_TO_STR Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
     if args[0] is None:
       return None
-    byte_array = bytes.fromhex(args[0])
-    return byte_array.decode('ASCII')
+
+    hexa = args[0]
+    if hexa.startswith('0x'):
+      hexa = hexa[2:]
+
+    try:
+      byte_array = bytes.fromhex(hexa)
+      return byte_array.decode('ASCII')
+    except Exception:  # pylint: disable=broad-except
+      return 'Invalid hex string'
 
   def STR_TO_HEX(self, *args: list[Any]) -> str | None:
     """ STR_TO_HEX Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
+
     return str(args[0]).encode('ASCII').hex()
 
   def HEX_TO_INT(self, *args: list[Any]) -> str | None | int:
     """ HEX_TO_INT Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
-    return int(int(args[0], 16))
+
+    try:
+      return int(int(args[0], 16))
+    except Exception:  # pylint: disable=broad-except
+      return 'Invalid hex string'
 
   def INT_TO_HEX(self, *args: list[Any]) -> str | None:
     """ INT_TO_HEX Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
-    return hex(int(args[0]))[2:]
+
+    try:
+      return hex(int(args[0]))[2:]
+    except Exception:  # pylint: disable=broad-except
+      return 'Invalid int value'
 
   def TO_FLOAT(self, *args: list[Any]) -> str | None | float:
     """ TO_FLOAT Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
+
     if args[0] is None:
       return None
-    return float(args[0])
+
+    try:
+      return float(args[0])
+    except Exception:  # pylint: disable=broad-except
+      return f'Invalid arguments - must be real number, not {type(args[0]).__name__}'
 
   def IS_PARAMETER_PRESENT(self, *args: list[Any]) -> str | bool:
     """ IS_PARAMETER_PRESENT Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
+    if args[0] is None:
+      return None
+
     return args[0] in self._payload
 
   def IS_SENSOR_PRESENT(self, *args: list[Any]) -> str | bool:
     """ IS_SENSOR_PRESENT Function """
     if len(args) > 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
+    if args[0] is None:
+      return None
+
     return args[0] in self._sensors
 
   def INSIDE_RANGE(self, *args: list[Any]) -> str | None | bool:
     """ INSIDE_RANGE Function """
     if len(args) != 3:
       return INVALID_NUMBER_OF_PARAMS.format(expected=3, received=len(args))
 
     if args[0] is None or args[1] is None or args[2] is None:
       return None
+
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES_RANGES.format(arg1=type(args[0]), arg2=type(args[1]), arg3=type(args[2]))
+      return DIFFERENT_TYPES_RANGES.format(
+        arg1=type(args[0]).__name__,
+        arg2=type(args[1]).__name__,
+        arg3=type(args[2]).__name__,
+      )
 
     return args[1] <= args[0] <= args[2]
 
   def OUTSIDE_RANGE(self, *args: list[Any]) -> str | None | bool:
     """ OUTSIDE_RANGE Function """
     if len(args) != 3:
       return INVALID_NUMBER_OF_PARAMS.format(expected=3, received=len(args))
 
     if args[0] is None or args[1] is None or args[2] is None:
       return None
+
     if not isinstance(args[0], type(args[1])):
-      return DIFFERENT_TYPES_RANGES.format(arg1=type(args[0]), arg2=type(args[1]), arg3=type(args[2]))
+      return DIFFERENT_TYPES_RANGES.format(
+        arg1=type(args[0]).__name__,
+        arg2=type(args[1]).__name__,
+        arg3=type(args[2]).__name__,
+      )
 
     return not args[1] <= args[0] <= args[2]
 
   def GET_TIME_DIFFERENCE(self, *args: list[Any]) -> str | float:
     """ GET_TIME_DIFFERENCE Function """
     if len(args) > 0:
       return INVALID_NUMBER_OF_PARAMS.format(expected=0, received=len(args))
+
     return self._asset_constants.get('timeElapsed', 0)
 
   def IF(self, *args: list[Any]) -> Any:
     """ IF Function """
     if len(args) != 3:
       return INVALID_NUMBER_OF_PARAMS.format(expected=3, received=len(args))
 
+    if args[0] is None or args[1] is None or args[2] is None:
+      return None
+
     return args[1] if args[0] else args[2]
 
   def NOW(self, *args: list[Any]) -> float:  # pylint: disable=unused-argument
     """ NOW Function """
     import zoneinfo
     from datetime import datetime
     return datetime.now(tz=zoneinfo.ZoneInfo('UTC')).timestamp()
@@ -562,35 +650,47 @@
     return args[0] is None
 
   def NOT(self, *args: list[Any]) -> str | bool:
     """ NOT Function """
     if len(args) != 1:
       return INVALID_NUMBER_OF_PARAMS.format(expected=1, received=len(args))
 
+    if args[0] is None:
+      return None
+
     return not args[0]
 
   def CONTAINS(self, *args: list[Any]) -> str | bool:
     """ CONTAINS function """
     if len(args) != 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None or args[1] is None:
+      return None
+
     return str(args[0]) in str(args[1])
 
   def STARTS_WITH(self, *args: list[Any]) -> str | bool:
     """ STARTS_WITH function """
     if len(args) != 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None or args[1] is None:
+      return None
+
     return str(args[1]).startswith(str(args[0]))
 
   def ENDS_WITH(self, *args: list[Any]) -> str | bool:
     """ ENDS_WITH function """
     if len(args) != 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
 
+    if args[0] is None or args[1] is None:
+      return None
+
     return str(args[1]).endswith(str(args[0]))
 
   def PRIMARY_DEVICE(self, *args: list[Any]) -> str:
     """ PRIMARY_DEVICE function """
     if len(args) > 0:
       return INVALID_NUMBER_OF_PARAMS.format(expected=0, received=len(args))
 
@@ -606,36 +706,56 @@
 
     if len(args) > 3:
       return INVALID_NUMBER_OF_PARAMS.format(
         expected=3,
         received=len(args),
       )
 
-    if args[0] is None or not isinstance(args[0], str):
-      return DIFFERENT_TYPES.format(arg1='str', arg2=type(args[0]))
+    if args[0] is None:
+      return None
+
+    if not isinstance(args[0], str):
+      return DIFFERENT_TYPES.format(arg1='str', arg2=type(args[0]).__name__)
+
+    if args[1] is None:
+      return None
 
-    if args[1] is None or not isinstance(args[1], int):
-      return DIFFERENT_TYPES.format(arg1='int', arg2=type(args[1]))
+    if not isinstance(args[1], int):
+      return DIFFERENT_TYPES.format(arg1='int', arg2=type(args[1]).__name__)
 
     if len(args) == 3:
-      if args[2] is None or not isinstance(args[2], int):
-        return DIFFERENT_TYPES.format(arg1='str', arg2=type(args[2]))
+      if args[2] is None:
+        return None
+
+      if not isinstance(args[2], int):
+        return DIFFERENT_TYPES.format(arg1='str', arg2=type(args[2]).__name__)
+
       return args[0][args[1]:args[2]]
     return args[0][args[1]:]
 
   def UNIX_TO_STR(self, *args: list[Any]) -> str:
     """ Convert UNIX timestamp date (args[0]) to format (args[1]) string """
     if len(args) < 2:
       return INVALID_NUMBER_OF_PARAMS.format(expected=2, received=len(args))
+
+    if args[0] is None:
+      return None
+
+    if args[1] is None:
+      return None
+
     import zoneinfo
     from datetime import datetime
 
     tz = zoneinfo.ZoneInfo('UTC')
 
     if len(args) > 2:
+      if args[2] is None:
+        return None
+
       try:
         tz = zoneinfo.ZoneInfo(args[2])
       except zoneinfo.ZoneInfoNotFoundError:
         tz = zoneinfo.ZoneInfo('UTC')
 
     return datetime\
           .fromtimestamp(int(args[0]), tz=zoneinfo.ZoneInfo('UTC'))\
```

### Comparing `layrz_sdk-3.0.0/layrz_sdk.egg-info/PKG-INFO` & `layrz_sdk-3.0.1/layrz_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.0
+Version: 3.0.1
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.0/layrz_sdk.egg-info/SOURCES.txt` & `layrz_sdk-3.0.1/layrz_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,8 +63,9 @@
 layrz_sdk/entities/reports/row.py
 layrz_sdk/entities/telemetry/__init__.py
 layrz_sdk/entities/telemetry/message.py
 layrz_sdk/entities/telemetry/position.py
 layrz_sdk/helpers/__init__.py
 layrz_sdk/helpers/color.py
 layrz_sdk/lcl/__init__.py
-layrz_sdk/lcl/core.py
+layrz_sdk/lcl/core.py
+tests/test_lcl.py
```

### Comparing `layrz_sdk-3.0.0/pyproject.toml` & `layrz_sdk-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "layrz-sdk"
-version = "3.0.0"
+version = "3.0.1"
 description = "Layrz SDK for Python"
 authors = [
   {name = "Golden M, Inc.", email = "software@goldenm.com"}
 ]
 requires-python = ">=3.10"
 
 maintainers = [
```

