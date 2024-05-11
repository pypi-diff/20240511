# Comparing `tmp/misleep-0.2.5b0.tar.gz` & `tmp/misleep-0.2.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.2.5b0.tar", last modified: Wed Apr 24 10:18:00 2024, max compression
+gzip compressed data, was "misleep-0.2.6b0.tar", last modified: Mon May  6 06:02:51 2024, max compression
```

## Comparing `misleep-0.2.5b0.tar` & `misleep-0.2.6b0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.722715 misleep-0.2.5b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.5b0/LICENSE
--rw-rw-rw-   0        0        0     3058 2024-04-24 10:18:00.722715 misleep-0.2.5b0/PKG-INFO
--rw-rw-rw-   0        0        0     1960 2024-04-17 11:42:46.000000 misleep-0.2.5b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.700998 misleep-0.2.5b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.5b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      528 2024-04-24 10:17:54.000000 misleep-0.2.5b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.706998 misleep-0.2.5b0/misleep/gui/
--rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.5b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0    14462 2024-04-24 10:15:45.000000 misleep-0.2.5b0/misleep/gui/dialog.py
--rw-rw-rw-   0        0        0    57175 2024-04-24 08:12:38.000000 misleep-0.2.5b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.709715 misleep-0.2.5b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.5b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.5b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-24 08:07:23.000000 misleep-0.2.5b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.712714 misleep-0.2.5b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.5b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    25023 2024-04-24 06:10:23.000000 misleep-0.2.5b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/gui/uis/save_data_dialog_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0     4573 2024-04-24 10:15:01.000000 misleep-0.2.5b0/misleep/gui/uis/state_spectral_dialog_ui.py
--rw-rw-rw-   0        0        0     3917 2024-04-24 06:08:06.000000 misleep-0.2.5b0/misleep/gui/uis/transfer_result_dialog_ui.py
--rw-rw-rw-   0        0        0     5126 2024-04-24 08:00:47.000000 misleep-0.2.5b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.714714 misleep-0.2.5b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.5b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     7578 2024-04-21 09:27:40.000000 misleep-0.2.5b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     5027 2024-04-17 08:38:52.000000 misleep-0.2.5b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.715715 misleep-0.2.5b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.5b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.5b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0     2158 2024-04-24 10:08:33.000000 misleep-0.2.5b0/misleep/preprocessing/signals.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.5b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.716714 misleep-0.2.5b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.5b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.5b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.718715 misleep-0.2.5b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.5b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.5b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.5b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.5b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.702998 misleep-0.2.5b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     3058 2024-04-24 10:18:00.000000 misleep-0.2.5b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1445 2024-04-24 10:18:00.000000 misleep-0.2.5b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 10:18:00.000000 misleep-0.2.5b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-24 10:18:00.000000 misleep-0.2.5b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 10:18:00.000000 misleep-0.2.5b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 10:18:00.722715 misleep-0.2.5b0/setup.cfg
--rw-rw-rw-   0        0        0     2155 2024-04-24 10:17:50.000000 misleep-0.2.5b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:18:00.721715 misleep-0.2.5b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.5b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.5b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.5b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.5b0/test/test_show.py
--rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.5b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.5b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.5b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.285442 misleep-0.2.6b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.6b0/LICENSE
+-rw-rw-rw-   0        0        0     3058 2024-05-06 06:02:51.284443 misleep-0.2.6b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1960 2024-04-17 11:42:46.000000 misleep-0.2.6b0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.262026 misleep-0.2.6b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.6b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      492 2024-05-06 06:02:20.000000 misleep-0.2.6b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.268025 misleep-0.2.6b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.6b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0    14462 2024-04-24 10:15:45.000000 misleep-0.2.6b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    57175 2024-04-25 04:22:38.000000 misleep-0.2.6b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.270025 misleep-0.2.6b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.6b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.6b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-24 08:07:23.000000 misleep-0.2.6b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.273442 misleep-0.2.6b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.6b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    25023 2024-04-24 06:10:23.000000 misleep-0.2.6b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/gui/uis/save_data_dialog_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     4573 2024-04-24 10:15:01.000000 misleep-0.2.6b0/misleep/gui/uis/state_spectral_dialog_ui.py
+-rw-rw-rw-   0        0        0     3917 2024-04-24 06:08:06.000000 misleep-0.2.6b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     5126 2024-04-24 08:00:47.000000 misleep-0.2.6b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.274442 misleep-0.2.6b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.6b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     7578 2024-04-21 09:27:40.000000 misleep-0.2.6b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     5033 2024-04-28 02:27:38.000000 misleep-0.2.6b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.277442 misleep-0.2.6b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.6b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.6b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0     2158 2024-04-24 10:08:33.000000 misleep-0.2.6b0/misleep/preprocessing/signals.py
+-rw-rw-rw-   0        0        0     4916 2024-04-25 04:19:01.000000 misleep-0.2.6b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.279442 misleep-0.2.6b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.6b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.6b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.281442 misleep-0.2.6b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.6b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.6b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.6b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.6b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.264025 misleep-0.2.6b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     3058 2024-05-06 06:02:51.000000 misleep-0.2.6b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2024-05-06 06:02:51.000000 misleep-0.2.6b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:02:51.000000 misleep-0.2.6b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-06 06:02:51.000000 misleep-0.2.6b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-06 06:02:51.000000 misleep-0.2.6b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:02:51.285442 misleep-0.2.6b0/setup.cfg
+-rw-rw-rw-   0        0        0     2155 2024-05-06 06:02:22.000000 misleep-0.2.6b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:02:51.284443 misleep-0.2.6b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.6b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.6b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.6b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.6b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.6b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.6b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.6b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.2.5b0/LICENSE` & `misleep-0.2.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/PKG-INFO` & `misleep-0.2.6b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.5b0
+Version: 0.2.6b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.2.5b0/README.md` & `misleep-0.2.6b0/README.md`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/about.py` & `misleep-0.2.6b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/dialog.py` & `misleep-0.2.6b0/misleep/gui/dialog.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/main_window.py` & `misleep-0.2.6b0/misleep/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/resources/entire_logo.png` & `misleep-0.2.6b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/resources/logo.png` & `misleep-0.2.6b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/resources/misleep.py` & `misleep-0.2.6b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/spec_window.py` & `misleep-0.2.6b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/thread.py` & `misleep-0.2.6b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/about_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/main_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/save_data_dialog_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/save_data_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/state_spectral_dialog_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/state_spectral_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/uis/transfer_result_dialog_ui.py` & `misleep-0.2.6b0/misleep/gui/uis/transfer_result_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/gui/utils.py` & `misleep-0.2.6b0/misleep/gui/utils.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/io/annotation_io.py` & `misleep-0.2.6b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/io/base.py` & `misleep-0.2.6b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/io/signal_io.py` & `misleep-0.2.6b0/misleep/io/signal_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             time = raw_data['time'][0]
             return MiData(signals=signals, channels=channels, sf=sf, time=time)
 
         # Saved by matlab
         channels = [each for item in raw_data['channels'][0] for each in item]
         sf = [float(each[0]) for item in raw_data['sf'][0] for each in item]
         signals = [raw_data[each][0] for each in channels]
-        time = raw_data['time'][0]
+        time = raw_data['time'][0][0][0]
         
         return MiData(signals=signals, channels=channels, sf=sf, time=time)
     
     except NotImplementedError:
         # The mat file is v7.3, use mat73 to load
         raw_data = list(mat73_loadmat(data_path).values())[-1]
```

### Comparing `misleep-0.2.5b0/misleep/preprocessing/signals.py` & `misleep-0.2.6b0/misleep/preprocessing/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/preprocessing/spectral.py` & `misleep-0.2.6b0/misleep/preprocessing/spectral.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         raise TypeError(f"'band' should be a list of tuple(s),"
                         f"e.g. [0.5, 30], got {type(band)}")
 
     # Define STFT parameters
     nperseg = int(window * sf)
     noverlap = int(nperseg - (step * sf))
 
-    f, t, Sxx = stft(signal, sf, nperseg=nperseg, noverlap=noverlap, padded=False)
+    f, t, Sxx = stft(signal, sf, nperseg=nperseg, noverlap=noverlap, padded=False, boundary='zeros')
 
     idx_f = np.logical_and(f >= band[0], f <= band[1])
     f = f[idx_f]
     Sxx = Sxx[idx_f, :]
     Sxx = np.square(np.abs(Sxx))
 
     if norm:
```

### Comparing `misleep-0.2.5b0/misleep/utils/annotation.py` & `misleep-0.2.6b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/utils/signals.py` & `misleep-0.2.6b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/viz/hypnogram.py` & `misleep-0.2.6b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/viz/signals.py` & `misleep-0.2.6b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep/viz/spectral.py` & `misleep-0.2.6b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/misleep.egg-info/PKG-INFO` & `misleep-0.2.6b0/misleep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.5b0
+Version: 0.2.6b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
```

### Comparing `misleep-0.2.5b0/misleep.egg-info/SOURCES.txt` & `misleep-0.2.6b0/misleep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/setup.py` & `misleep-0.2.6b0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.2.5b0"
+VERSION = "0.2.6b0"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
```

### Comparing `misleep-0.2.5b0/test/test_midata.py` & `misleep-0.2.6b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/test/test_signal_io.py` & `misleep-0.2.6b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/test/test_signals_viz.py` & `misleep-0.2.6b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.5b0/test/test_spectral_viz.py` & `misleep-0.2.6b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

