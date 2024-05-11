# Comparing `tmp/graphysio-2024.5.7.tar.gz` & `tmp/graphysio-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphysio-2024.5.7.tar", max compression
+gzip compressed data, was "graphysio-2024.5.8.tar", max compression
```

## Comparing `graphysio-2024.5.7.tar` & `graphysio-2024.5.8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      750 2019-03-28 09:53:36.213435 graphysio-2024.5.7/LICENSE
--rw-r--r--   0        0        0      817 2022-07-06 20:01:27.455451 graphysio-2024.5.7/README.md
--rw-r--r--   0        0        0      232 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/__init__.py
--rw-r--r--   0        0        0      516 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/__main__.py
--rw-r--r--   0        0        0       34 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/algorithms/__init__.py
--rw-r--r--   0        0        0    10396 2023-11-14 20:24:04.333629 graphysio-2024.5.7/graphysio/algorithms/filters.py
--rw-r--r--   0        0        0     6667 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/algorithms/waveform.py
--rw-r--r--   0        0        0    16364 2024-05-07 15:42:35.125241 graphysio-2024.5.7/graphysio/dialogs.py
--rw-r--r--   0        0        0      531 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/legend.py
--rw-r--r--   0        0        0      211 2023-11-11 11:36:50.904021 graphysio-2024.5.7/graphysio/main.py
--rw-r--r--   0        0        0     5661 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/mainui.py
--rw-r--r--   0        0        0      437 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/plotwidgets/__init__.py
--rw-r--r--   0        0        0     9681 2024-05-07 15:33:08.814579 graphysio-2024.5.7/graphysio/plotwidgets/curves.py
--rw-r--r--   0        0        0     5461 2023-11-22 11:41:06.571840 graphysio-2024.5.7/graphysio/plotwidgets/plotwidget.py
--rw-r--r--   0        0        0     5302 2023-11-14 20:11:39.125200 graphysio-2024.5.7/graphysio/plotwidgets/poiselector.py
--rw-r--r--   0        0        0     4895 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/plotwidgets/puplot.py
--rw-r--r--   0        0        0     5236 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/plotwidgets/spectrogram.py
--rw-r--r--   0        0        0     9698 2023-11-14 20:11:19.909073 graphysio-2024.5.7/graphysio/plotwidgets/tsplot.py
--rw-r--r--   0        0        0     1265 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/readdata/__init__.py
--rw-r--r--   0        0        0      292 2020-05-22 09:22:57.526000 graphysio-2024.5.7/graphysio/readdata/baseclass.py
--rw-r--r--   0        0        0    10332 2024-05-07 15:44:26.754416 graphysio-2024.5.7/graphysio/readdata/csv.py
--rw-r--r--   0        0        0     1701 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/readdata/edf.py
--rw-r--r--   0        0        0     1069 2024-05-07 15:45:03.802800 graphysio-2024.5.7/graphysio/readdata/parquet.py
--rw-r--r--   0        0        0     1251 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/structures.py
--rw-r--r--   0        0        0      462 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/transformations/__init__.py
--rw-r--r--   0        0        0      969 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/transformations/feet_time_interval.py
--rw-r--r--   0        0        0      863 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/transformations/feet_to_curve.py
--rw-r--r--   0        0        0     1512 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/transformations/perfusion_index.py
--rw-r--r--   0        0        0     1587 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/transformations/precise_feet.py
--rw-r--r--   0        0        0     1783 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/transformations/pulse_arrival_time.py
--rw-r--r--   0        0        0      438 2021-01-05 09:14:52.954469 graphysio-2024.5.7/graphysio/ui/__init__.py
--rw-r--r--   0        0        0      181 2022-07-18 13:39:28.978612 graphysio-2024.5.7/graphysio/ui/convert_ui_to_py.sh
--rw-r--r--   0        0        0    16236 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/csvrequest.py
--rw-r--r--   0        0        0    14702 2022-07-07 21:16:27.251901 graphysio-2024.5.7/graphysio/ui/csvrequest.ui
--rw-r--r--   0        0        0     6291 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/curveproperties.py
--rw-r--r--   0        0        0     4481 2019-05-24 13:11:00.148482 graphysio-2024.5.7/graphysio/ui/curveproperties.ui
--rw-r--r--   0        0        0     2790 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/curveselect.py
--rw-r--r--   0        0        0     1650 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/curveselect.ui
--rw-r--r--   0        0        0     1822 2022-07-18 13:39:28.982612 graphysio-2024.5.7/graphysio/ui/cycledetect.py
--rw-r--r--   0        0        0     1096 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/cycledetect.ui
--rw-r--r--   0        0        0     4117 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/datetime.py
--rw-r--r--   0        0        0     4121 2019-05-24 13:18:41.917107 graphysio-2024.5.7/graphysio/ui/datetime.ui
--rw-r--r--   0        0        0     1920 2022-07-18 13:39:28.982612 graphysio-2024.5.7/graphysio/ui/filter.py
--rw-r--r--   0        0        0     1241 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/filter.ui
--rw-r--r--   0        0        0     6039 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/loopwidget.py
--rw-r--r--   0        0        0     5748 2019-03-18 12:32:13.063040 graphysio-2024.5.7/graphysio/ui/loopwidget.ui
--rw-r--r--   0        0        0     3381 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/mainwindow.py
--rw-r--r--   0        0        0     2700 2019-05-23 08:03:05.751959 graphysio-2024.5.7/graphysio/ui/mainwindow.ui
--rw-r--r--   0        0        0     7312 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/periodexport.py
--rw-r--r--   0        0        0     4987 2019-03-18 12:32:13.067040 graphysio-2024.5.7/graphysio/ui/periodexport.ui
--rw-r--r--   0        0        0     3525 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/ui/poiwidget.py
--rw-r--r--   0        0        0     2999 2020-05-28 13:00:26.648398 graphysio-2024.5.7/graphysio/ui/poiwidget.ui
--rw-r--r--   0        0        0     2864 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/ui/setuppuloop.py
--rw-r--r--   0        0        0     1862 2019-03-18 12:32:13.067040 graphysio-2024.5.7/graphysio/ui/setuppuloop.ui
--rw-r--r--   0        0        0     2278 2023-11-14 20:09:24.028274 graphysio-2024.5.7/graphysio/utils.py
--rw-r--r--   0        0        0      342 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/__init__.py
--rwxr-xr-x   0        0        0      470 2023-11-22 11:42:18.564423 graphysio-2024.5.7/graphysio/writedata/csv.py
--rw-r--r--   0        0        0     2096 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/edf.py
--rwxr-xr-x   0        0        0     6357 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/exporter.py
--rw-r--r--   0        0        0      476 2024-05-07 15:45:25.551024 graphysio-2024.5.7/graphysio/writedata/matlab.py
--rwxr-xr-x   0        0        0      624 2023-11-22 11:42:18.560423 graphysio-2024.5.7/graphysio/writedata/parquet.py
--rw-r--r--   0        0        0      923 2024-05-07 15:46:34.255726 graphysio-2024.5.7/pyproject.toml
--rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 graphysio-2024.5.7/PKG-INFO
+-rw-r--r--   0        0        0      750 2019-03-28 09:53:36.213435 graphysio-2024.5.8/LICENSE
+-rw-r--r--   0        0        0      817 2022-07-06 20:01:27.455451 graphysio-2024.5.8/README.md
+-rw-r--r--   0        0        0      232 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/__init__.py
+-rw-r--r--   0        0        0      516 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/__main__.py
+-rw-r--r--   0        0        0       34 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/algorithms/__init__.py
+-rw-r--r--   0        0        0    10396 2023-11-14 20:24:04.333629 graphysio-2024.5.8/graphysio/algorithms/filters.py
+-rw-r--r--   0        0        0     6667 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/algorithms/waveform.py
+-rw-r--r--   0        0        0    16364 2024-05-07 15:42:35.125241 graphysio-2024.5.8/graphysio/dialogs.py
+-rw-r--r--   0        0        0      531 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/legend.py
+-rw-r--r--   0        0        0      211 2023-11-11 11:36:50.904021 graphysio-2024.5.8/graphysio/main.py
+-rw-r--r--   0        0        0     5661 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/mainui.py
+-rw-r--r--   0        0        0      437 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/plotwidgets/__init__.py
+-rw-r--r--   0        0        0     9681 2024-05-07 20:50:35.462309 graphysio-2024.5.8/graphysio/plotwidgets/curves.py
+-rw-r--r--   0        0        0     5461 2023-11-22 11:41:06.571840 graphysio-2024.5.8/graphysio/plotwidgets/plotwidget.py
+-rw-r--r--   0        0        0     5302 2023-11-14 20:11:39.125200 graphysio-2024.5.8/graphysio/plotwidgets/poiselector.py
+-rw-r--r--   0        0        0     4895 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/plotwidgets/puplot.py
+-rw-r--r--   0        0        0     5236 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/plotwidgets/spectrogram.py
+-rw-r--r--   0        0        0     9698 2023-11-14 20:11:19.909073 graphysio-2024.5.8/graphysio/plotwidgets/tsplot.py
+-rw-r--r--   0        0        0     1265 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/readdata/__init__.py
+-rw-r--r--   0        0        0      292 2020-05-22 09:22:57.526000 graphysio-2024.5.8/graphysio/readdata/baseclass.py
+-rw-r--r--   0        0        0    10369 2024-05-07 20:38:38.032372 graphysio-2024.5.8/graphysio/readdata/csv.py
+-rw-r--r--   0        0        0     1701 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/readdata/edf.py
+-rw-r--r--   0        0        0     1228 2024-05-08 14:12:52.455999 graphysio-2024.5.8/graphysio/readdata/parquet.py
+-rw-r--r--   0        0        0     1251 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/structures.py
+-rw-r--r--   0        0        0      462 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/transformations/__init__.py
+-rw-r--r--   0        0        0      969 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/transformations/feet_time_interval.py
+-rw-r--r--   0        0        0      863 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/transformations/feet_to_curve.py
+-rw-r--r--   0        0        0     1512 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/transformations/perfusion_index.py
+-rw-r--r--   0        0        0     1587 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/transformations/precise_feet.py
+-rw-r--r--   0        0        0     1783 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/transformations/pulse_arrival_time.py
+-rw-r--r--   0        0        0      438 2021-01-05 09:14:52.954469 graphysio-2024.5.8/graphysio/ui/__init__.py
+-rw-r--r--   0        0        0      181 2022-07-18 13:39:28.978612 graphysio-2024.5.8/graphysio/ui/convert_ui_to_py.sh
+-rw-r--r--   0        0        0    16236 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/ui/csvrequest.py
+-rw-r--r--   0        0        0    14702 2022-07-07 21:16:27.251901 graphysio-2024.5.8/graphysio/ui/csvrequest.ui
+-rw-r--r--   0        0        0     6291 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/ui/curveproperties.py
+-rw-r--r--   0        0        0     4481 2019-05-24 13:11:00.148482 graphysio-2024.5.8/graphysio/ui/curveproperties.ui
+-rw-r--r--   0        0        0     2790 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/ui/curveselect.py
+-rw-r--r--   0        0        0     1650 2019-03-18 12:32:13.063040 graphysio-2024.5.8/graphysio/ui/curveselect.ui
+-rw-r--r--   0        0        0     1822 2022-07-18 13:39:28.982612 graphysio-2024.5.8/graphysio/ui/cycledetect.py
+-rw-r--r--   0        0        0     1096 2019-03-18 12:32:13.063040 graphysio-2024.5.8/graphysio/ui/cycledetect.ui
+-rw-r--r--   0        0        0     4117 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/ui/datetime.py
+-rw-r--r--   0        0        0     4121 2019-05-24 13:18:41.917107 graphysio-2024.5.8/graphysio/ui/datetime.ui
+-rw-r--r--   0        0        0     1920 2022-07-18 13:39:28.982612 graphysio-2024.5.8/graphysio/ui/filter.py
+-rw-r--r--   0        0        0     1241 2019-03-18 12:32:13.063040 graphysio-2024.5.8/graphysio/ui/filter.ui
+-rw-r--r--   0        0        0     6039 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/ui/loopwidget.py
+-rw-r--r--   0        0        0     5748 2019-03-18 12:32:13.063040 graphysio-2024.5.8/graphysio/ui/loopwidget.ui
+-rw-r--r--   0        0        0     3381 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/ui/mainwindow.py
+-rw-r--r--   0        0        0     2700 2019-05-23 08:03:05.751959 graphysio-2024.5.8/graphysio/ui/mainwindow.ui
+-rw-r--r--   0        0        0     7312 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/ui/periodexport.py
+-rw-r--r--   0        0        0     4987 2019-03-18 12:32:13.067040 graphysio-2024.5.8/graphysio/ui/periodexport.ui
+-rw-r--r--   0        0        0     3525 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/ui/poiwidget.py
+-rw-r--r--   0        0        0     2999 2020-05-28 13:00:26.648398 graphysio-2024.5.8/graphysio/ui/poiwidget.ui
+-rw-r--r--   0        0        0     2864 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/ui/setuppuloop.py
+-rw-r--r--   0        0        0     1862 2019-03-18 12:32:13.067040 graphysio-2024.5.8/graphysio/ui/setuppuloop.ui
+-rw-r--r--   0        0        0     2257 2024-05-08 14:00:52.555820 graphysio-2024.5.8/graphysio/utils.py
+-rw-r--r--   0        0        0      342 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/writedata/__init__.py
+-rwxr-xr-x   0        0        0      470 2023-11-22 11:42:18.564423 graphysio-2024.5.8/graphysio/writedata/csv.py
+-rw-r--r--   0        0        0     2096 2023-11-22 11:42:18.560423 graphysio-2024.5.8/graphysio/writedata/edf.py
+-rwxr-xr-x   0        0        0     6373 2024-05-08 14:16:16.557173 graphysio-2024.5.8/graphysio/writedata/exporter.py
+-rw-r--r--   0        0        0      469 2024-05-07 20:34:45.242456 graphysio-2024.5.8/graphysio/writedata/matlab.py
+-rwxr-xr-x   0        0        0      689 2024-05-08 14:18:15.445855 graphysio-2024.5.8/graphysio/writedata/parquet.py
+-rw-r--r--   0        0        0      923 2024-05-08 14:20:12.558527 graphysio-2024.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1777 1970-01-01 00:00:00.000000 graphysio-2024.5.8/PKG-INFO
```

### Comparing `graphysio-2024.5.7/LICENSE` & `graphysio-2024.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/README.md` & `graphysio-2024.5.8/README.md`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/__main__.py` & `graphysio-2024.5.8/graphysio/__main__.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/algorithms/filters.py` & `graphysio-2024.5.8/graphysio/algorithms/filters.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/algorithms/waveform.py` & `graphysio-2024.5.8/graphysio/algorithms/waveform.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/dialogs.py` & `graphysio-2024.5.8/graphysio/dialogs.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/legend.py` & `graphysio-2024.5.8/graphysio/legend.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/mainui.py` & `graphysio-2024.5.8/graphysio/mainui.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/plotwidgets/curves.py` & `graphysio-2024.5.8/graphysio/plotwidgets/curves.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/plotwidgets/plotwidget.py` & `graphysio-2024.5.8/graphysio/plotwidgets/plotwidget.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/plotwidgets/poiselector.py` & `graphysio-2024.5.8/graphysio/plotwidgets/poiselector.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/plotwidgets/puplot.py` & `graphysio-2024.5.8/graphysio/plotwidgets/puplot.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/plotwidgets/spectrogram.py` & `graphysio-2024.5.8/graphysio/plotwidgets/spectrogram.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/plotwidgets/tsplot.py` & `graphysio-2024.5.8/graphysio/plotwidgets/tsplot.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/readdata/__init__.py` & `graphysio-2024.5.8/graphysio/readdata/__init__.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/readdata/csv.py` & `graphysio-2024.5.8/graphysio/readdata/csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             encoding=request.encoding,
             index_col=False,
             engine="c",
         )
         pdtonum = partial(pd.to_numeric, errors="coerce")
         dtformat = request.datetime_format
         if request.generatex:
-            data.index = (1e9 * data.index / request.samplerate).astype(np.int64)
+            data.index = (1e9 * data.index / request.samplerate).astype('int')
             # Make all data numeric and remove empty rows
             datacols = data.columns.difference([request.clusterid])
             data[datacols] = data[datacols].apply(pdtonum)
             data = data.dropna(axis="rows", how="all", subset=datacols)
         else:
             timestamp = data[request.dtfield]
             data = data.drop(columns=request.dtfield)
@@ -70,17 +70,17 @@
             elif dtformat == "<infer>":
                 timestamp = pd.to_datetime(timestamp, infer_datetime_format=True)
             else:
                 timestamp = pd.to_datetime(timestamp, format=dtformat)
                 timestamp = pd.Index(timestamp)
                 if timestamp.tz is None:
                     timestamp = timestamp.tz_localize(request.timezone)
-                timestamp = timestamp.tz_convert("UTC")
+                timestamp = timestamp.tz_convert("UTC").tz_localize(None)
 
-            timestamp = timestamp.astype(np.int64)
+            timestamp = timestamp.astype('datetime64[ns]').astype('int')
             data = data.set_index([timestamp])
 
         data = data.dropna(axis="columns", how="all")
         data = data.sort_index()
 
         fp = request.filepath
         if request.clusterid:
```

### Comparing `graphysio-2024.5.7/graphysio/readdata/edf.py` & `graphysio-2024.5.8/graphysio/readdata/edf.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/readdata/parquet.py` & `graphysio-2024.5.8/graphysio/readdata/parquet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import numpy as np
 import pandas as pd
+from pandas.api.types import is_datetime64_any_dtype
 
 from graphysio.dialogs import DlgListChoice
 from graphysio.readdata.baseclass import BaseReader
 from graphysio.structures import PlotData
 
 try:
     import pyarrow.parquet as pa
@@ -30,10 +30,13 @@
 
     def __call__(self) -> PlotData:
         filepath = self.userdata["filepath"]
         data = pd.read_parquet(filepath, columns=self.userdata["columns"])
 
         data = data.dropna(axis="columns", how="all")
         data = data.sort_index()
-        data.index = data.index.astype(np.int64)
+
+        if is_datetime64_any_dtype(data.index):
+            data.index = data.index.tz_localize(None)
+        data.index = data.index.astype('datetime64[ns]').astype('int')
 
         return PlotData(data=data, filepath=filepath)
```

### Comparing `graphysio-2024.5.7/graphysio/structures.py` & `graphysio-2024.5.8/graphysio/structures.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/transformations/feet_time_interval.py` & `graphysio-2024.5.8/graphysio/transformations/feet_time_interval.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/transformations/feet_to_curve.py` & `graphysio-2024.5.8/graphysio/transformations/feet_to_curve.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/transformations/perfusion_index.py` & `graphysio-2024.5.8/graphysio/transformations/perfusion_index.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/transformations/precise_feet.py` & `graphysio-2024.5.8/graphysio/transformations/precise_feet.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/transformations/pulse_arrival_time.py` & `graphysio-2024.5.8/graphysio/transformations/pulse_arrival_time.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/csvrequest.py` & `graphysio-2024.5.8/graphysio/ui/csvrequest.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/csvrequest.ui` & `graphysio-2024.5.8/graphysio/ui/csvrequest.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/curveproperties.py` & `graphysio-2024.5.8/graphysio/ui/curveproperties.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/curveproperties.ui` & `graphysio-2024.5.8/graphysio/ui/curveproperties.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/curveselect.py` & `graphysio-2024.5.8/graphysio/ui/curveselect.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/curveselect.ui` & `graphysio-2024.5.8/graphysio/ui/curveselect.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/cycledetect.py` & `graphysio-2024.5.8/graphysio/ui/cycledetect.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/cycledetect.ui` & `graphysio-2024.5.8/graphysio/ui/cycledetect.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/datetime.py` & `graphysio-2024.5.8/graphysio/ui/datetime.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/datetime.ui` & `graphysio-2024.5.8/graphysio/ui/datetime.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/filter.py` & `graphysio-2024.5.8/graphysio/ui/filter.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/filter.ui` & `graphysio-2024.5.8/graphysio/ui/filter.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/loopwidget.py` & `graphysio-2024.5.8/graphysio/ui/loopwidget.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/loopwidget.ui` & `graphysio-2024.5.8/graphysio/ui/loopwidget.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/mainwindow.py` & `graphysio-2024.5.8/graphysio/ui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/mainwindow.ui` & `graphysio-2024.5.8/graphysio/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/periodexport.py` & `graphysio-2024.5.8/graphysio/ui/periodexport.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/periodexport.ui` & `graphysio-2024.5.8/graphysio/ui/periodexport.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/poiwidget.py` & `graphysio-2024.5.8/graphysio/ui/poiwidget.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/poiwidget.ui` & `graphysio-2024.5.8/graphysio/ui/poiwidget.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/setuppuloop.py` & `graphysio-2024.5.8/graphysio/ui/setuppuloop.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/ui/setuppuloop.ui` & `graphysio-2024.5.8/graphysio/ui/setuppuloop.ui`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/utils.py` & `graphysio-2024.5.8/graphysio/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import imp
 import os
 import sys
 from functools import partial
 from itertools import cycle
 
 import numpy as np
 import pathvalidate
 from pyqtgraph.Qt import QtGui, QtWidgets
 
 sanitize_filename = partial(pathvalidate.sanitize_filename, platform="auto")
 sanitize_filepath = partial(pathvalidate.sanitize_filepath, platform="auto")
 
+import importlib.util
+
 
 def Colors():
     qtcolors = [
         QtGui.QColor(0, 114, 189),
         QtGui.QColor(217, 83, 25),
         QtGui.QColor(237, 177, 32),
         QtGui.QColor(126, 47, 142),
@@ -44,25 +45,23 @@
     if not isinstance(filepath, str):
         # PyQt5 API change
         filepath = filepath[0]
     if not filepath:
         # Cancel pressed
         return
 
-    folder, filename = os.path.split(filepath)
-    modulename, _ = os.path.splitext(filename)
-    f, filename, description = imp.find_module(modulename, [folder])
-
     bcbak = sys.dont_write_bytecode
     try:
         sys.dont_write_bytecode = True
-        imp.load_module("graphysio.plugin", f, filename, description)
+        spec = importlib.util.spec_from_file_location("graphysio.plugin", filepath)
+        foo = importlib.util.module_from_spec(spec)
+        sys.modules["graphysio.plugin"] = foo
+        spec.loader.exec_module(foo)
     finally:
         sys.dont_write_bytecode = bcbak
-        f.close()
 
 
 def clip(vec, vrange):
     if vrange is None:
         return vec
     xmin, xmax = vrange
     cond = (vec > xmin) & (vec < xmax)
```

### Comparing `graphysio-2024.5.7/graphysio/writedata/edf.py` & `graphysio-2024.5.8/graphysio/writedata/edf.py`

 * *Files identical despite different names*

### Comparing `graphysio-2024.5.7/graphysio/writedata/exporter.py` & `graphysio-2024.5.8/graphysio/writedata/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             return
         self.outdir = os.path.dirname(filepath)
 
         feetseries = []
         for c in self.parent.curves.values():
             for k, v in c.feetitem.indices.items():
                 feetseries.append(pd.Series(v, name=f"{c.name()}-{k}"))
-        df = pd.concat(feetseries, axis=1)
+        df = pd.concat(feetseries, axis=1).astype('Int64')
         df.to_csv(filepath, index_label="idx")
 
 
 class PuExporter:
     def __init__(self, parent, name):
         self.parent = parent
         self.name = name
```

### Comparing `graphysio-2024.5.7/pyproject.toml` & `graphysio-2024.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "graphysio"
-version = "2024.5.7"
+version = "2024.5.8"
 description = "Visualizer and analyser for biometric signals"
 authors = ["Jona Joachim <jona@joachim.cc>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/jaj42/GraPhysio"
 
 [tool.poetry.dependencies]
```

### Comparing `graphysio-2024.5.7/PKG-INFO` & `graphysio-2024.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphysio
-Version: 2024.5.7
+Version: 2024.5.8
 Summary: Visualizer and analyser for biometric signals
 Home-page: https://github.com/jaj42/GraPhysio
 License: ISC
 Author: Jona Joachim
 Author-email: jona@joachim.cc
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved
```

