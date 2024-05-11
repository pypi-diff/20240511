# Comparing `tmp/Dosepy-0.6.1.tar.gz` & `tmp/dosepy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dosepy-0.6.1.tar", last modified: Mon Apr  1 22:29:02 2024, max compression
+gzip compressed data, was "dosepy-0.6.2.tar", last modified: Sat May 11 18:45:10 2024, max compression
```

## Comparing `Dosepy-0.6.1.tar` & `dosepy-0.6.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.158345 Dosepy-0.6.1/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1413 2023-10-19 15:53:23.000000 Dosepy-0.6.1/LICENSE
--rw-rw-r--   0 luis      (1000) luis      (1000)       59 2024-03-03 18:37:22.000000 Dosepy-0.6.1/MANIFEST.in
--rw-r--r--   0 luis      (1000) luis      (1000)     3828 2024-04-01 22:29:02.158345 Dosepy-0.6.1/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)     2658 2024-03-30 15:51:07.000000 Dosepy-0.6.1/README.md
--rw-rw-r--   0 luis      (1000) luis      (1000)     1416 2024-04-01 19:19:01.000000 Dosepy-0.6.1/pyproject.toml
--rw-rw-r--   0 luis      (1000) luis      (1000)       38 2024-04-01 22:29:02.158345 Dosepy-0.6.1/setup.cfg
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.142347 Dosepy-0.6.1/src/
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.146347 Dosepy-0.6.1/src/Dosepy/
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.150346 Dosepy-0.6.1/src/Dosepy/Icon/
--rw-rw-r--   0 luis      (1000) luis      (1000)   568371 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/Icon/Icon.png
--rw-rw-r--   0 luis      (1000) luis      (1000)    14061 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/Icon/Logo_Dosepy.png
--rw-rw-r--   0 luis      (1000) luis      (1000)    13444 2023-10-19 15:53:23.000000 Dosepy-0.6.1/src/Dosepy/Icon/cut_icon.png
--rwxrwxr-x   0 luis      (1000) luis      (1000)    11084 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/Icon/folder.png
--rw-rw-r--   0 luis      (1000) luis      (1000)     5824 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/Icon/save.png
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     1474 2024-03-28 18:41:08.000000 Dosepy-0.6.1/src/Dosepy/app.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.150346 Dosepy-0.6.1/src/Dosepy/app_components/
--rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/app_components/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3048 2024-03-05 23:50:08.000000 Dosepy-0.6.1/src/Dosepy/app_components/about_window.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.150346 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/
--rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3457 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/cross_hair_cursor.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      429 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/cursor.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4773 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/dp_multi_cursor.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3153 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/draggable rectangle.py
--rw-rw-r--   0 luis      (1000) luis      (1000)      415 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/multi_cursor.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4825 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/to_do_rendering.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     5604 2024-03-01 23:24:27.000000 Dosepy-0.6.1/src/Dosepy/app_components/calibration_widget.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     2074 2024-03-05 23:43:07.000000 Dosepy-0.6.1/src/Dosepy/app_components/file_dialog.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4587 2024-03-05 23:50:38.000000 Dosepy-0.6.1/src/Dosepy/app_components/licencia_window.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.150346 Dosepy-0.6.1/src/Dosepy/app_components/styles/
--rw-rw-r--   0 luis      (1000) luis      (1000)      240 2024-02-28 23:03:41.000000 Dosepy-0.6.1/src/Dosepy/app_components/styles/styles.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3451 2024-03-02 19:52:33.000000 Dosepy-0.6.1/src/Dosepy/app_components/tiff2dose_widget.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     8674 2024-03-28 18:37:44.000000 Dosepy-0.6.1/src/Dosepy/app_controller.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     2817 2024-03-28 17:23:41.000000 Dosepy-0.6.1/src/Dosepy/app_model.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3921 2024-03-03 16:45:32.000000 Dosepy-0.6.1/src/Dosepy/calibration.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.154345 Dosepy-0.6.1/src/Dosepy/data/
--rw-rw-r--   0 luis      (1000) luis      (1000)   380625 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/data/D_FILM.csv
--rw-rw-r--   0 luis      (1000) luis      (1000)   380625 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/data/D_TPS.csv
--rw-rw-r--   0 luis      (1000) luis      (1000)     2388 2024-04-01 19:35:33.000000 Dosepy-0.6.1/src/Dosepy/i_o.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    37601 2024-04-01 02:32:32.000000 Dosepy-0.6.1/src/Dosepy/image.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.154345 Dosepy-0.6.1/src/Dosepy/old/
--rw-rw-r--   0 luis      (1000) luis      (1000)    17219 2024-03-23 13:31:52.000000 Dosepy-0.6.1/src/Dosepy/old/GUI.py
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/old/__init__.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    15468 2023-10-19 15:53:23.000000 Dosepy-0.6.1/src/Dosepy/old/dose.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.158345 Dosepy-0.6.1/src/Dosepy/old/gui_components/
--rw-rw-r--   0 luis      (1000) luis      (1000)    12983 2024-03-05 23:18:39.000000 Dosepy-0.6.1/src/Dosepy/old/gui_components/Bloque_Imagenes.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     7330 2024-03-05 23:21:07.000000 Dosepy-0.6.1/src/Dosepy/old/gui_components/Bloque_gamma.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     3042 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/old/gui_components/about_window.py
--rw-rw-r--   0 luis      (1000) luis      (1000)    15764 2024-03-29 16:11:58.000000 Dosepy-0.6.1/src/Dosepy/old/gui_components/film_to_doseGUI.py
--rw-rw-r--   0 luis      (1000) luis      (1000)     4581 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/old/gui_components/licencia_window.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.158345 Dosepy-0.6.1/src/Dosepy/scripts/
--rw-rw-r--   0 luis      (1000) luis      (1000)     1034 2024-02-22 03:59:11.000000 Dosepy-0.6.1/src/Dosepy/scripts/test_tutorial.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.158345 Dosepy-0.6.1/src/Dosepy/tools/
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 Dosepy-0.6.1/src/Dosepy/tools/__init__.py
--rwxrwxr-x   0 luis      (1000) luis      (1000)     4433 2023-10-19 15:53:23.000000 Dosepy-0.6.1/src/Dosepy/tools/film_to_dose.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.158345 Dosepy-0.6.1/src/Dosepy/tools/gui_widgets/
--rw-rw-r--   0 luis      (1000) luis      (1000)        0 2024-02-27 19:07:50.000000 Dosepy-0.6.1/src/Dosepy/tools/gui_widgets/__init__.py
--rwxrwxr-x   0 luis      (1000) luis      (1000)     4243 2024-03-30 02:27:22.000000 Dosepy-0.6.1/src/Dosepy/tools/resol.py
-drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-04-01 22:29:02.158345 Dosepy-0.6.1/src/Dosepy.egg-info/
--rw-r--r--   0 luis      (1000) luis      (1000)     3828 2024-04-01 22:29:02.000000 Dosepy-0.6.1/src/Dosepy.egg-info/PKG-INFO
--rw-rw-r--   0 luis      (1000) luis      (1000)     1769 2024-04-01 22:29:02.000000 Dosepy-0.6.1/src/Dosepy.egg-info/SOURCES.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        1 2024-04-01 22:29:02.000000 Dosepy-0.6.1/src/Dosepy.egg-info/dependency_links.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)      133 2024-04-01 22:29:02.000000 Dosepy-0.6.1/src/Dosepy.egg-info/requires.txt
--rw-rw-r--   0 luis      (1000) luis      (1000)        7 2024-04-01 22:29:02.000000 Dosepy-0.6.1/src/Dosepy.egg-info/top_level.txt
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.303166 dosepy-0.6.2/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1413 2023-10-19 15:53:23.000000 dosepy-0.6.2/LICENSE
+-rw-rw-r--   0 luis      (1000) luis      (1000)       59 2024-05-09 01:21:10.000000 dosepy-0.6.2/MANIFEST.in
+-rw-r--r--   0 luis      (1000) luis      (1000)     3828 2024-05-11 18:45:10.303166 dosepy-0.6.2/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2658 2024-05-09 01:21:10.000000 dosepy-0.6.2/README.md
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1416 2024-05-10 04:18:16.000000 dosepy-0.6.2/pyproject.toml
+-rw-rw-r--   0 luis      (1000) luis      (1000)       38 2024-05-11 18:45:10.303166 dosepy-0.6.2/setup.cfg
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.271165 dosepy-0.6.2/src/
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.275165 dosepy-0.6.2/src/Dosepy/
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.283166 dosepy-0.6.2/src/Dosepy/Icon/
+-rw-rw-r--   0 luis      (1000) luis      (1000)   568371 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/Icon/Icon.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)    14061 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/Icon/Logo_Dosepy.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)    13444 2023-10-19 15:53:23.000000 dosepy-0.6.2/src/Dosepy/Icon/cut_icon.png
+-rwxrwxr-x   0 luis      (1000) luis      (1000)    11084 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/Icon/folder.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)     5824 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/Icon/save.png
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1474 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.287165 dosepy-0.6.2/src/Dosepy/app_components/
+-rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3048 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/about_window.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.287165 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/
+-rwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3457 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/cross_hair_cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      429 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4773 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/dp_multi_cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3153 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/draggable rectangle.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)      415 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/multi_cursor.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4928 2024-05-10 04:14:58.000000 dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/to_do_rendering.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     5604 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/calibration_widget.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2075 2024-05-11 17:17:28.000000 dosepy-0.6.2/src/Dosepy/app_components/file_dialog.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4587 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/licencia_window.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.291166 dosepy-0.6.2/src/Dosepy/app_components/styles/
+-rw-rw-r--   0 luis      (1000) luis      (1000)      240 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/styles/styles.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3451 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_components/tiff2dose_widget.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     8674 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_controller.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2817 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/app_model.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3874 2024-05-11 17:22:53.000000 dosepy-0.6.2/src/Dosepy/calibration.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.291166 dosepy-0.6.2/src/Dosepy/data/
+-rw-rw-r--   0 luis      (1000) luis      (1000)   380625 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/data/D_FILM.csv
+-rw-rw-r--   0 luis      (1000) luis      (1000)   380625 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/data/D_TPS.csv
+-rw-rw-r--   0 luis      (1000) luis      (1000)     2388 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/i_o.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)    39312 2024-05-11 17:22:53.000000 dosepy-0.6.2/src/Dosepy/image.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.295166 dosepy-0.6.2/src/Dosepy/old/
+-rw-rw-r--   0 luis      (1000) luis      (1000)    17219 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/GUI.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/__init__.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)    15468 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/dose.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.299166 dosepy-0.6.2/src/Dosepy/old/gui_components/
+-rw-rw-r--   0 luis      (1000) luis      (1000)    12983 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/gui_components/Bloque_Imagenes.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     7330 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/gui_components/Bloque_gamma.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     3042 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/gui_components/about_window.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)    15764 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/gui_components/film_to_doseGUI.py
+-rw-rw-r--   0 luis      (1000) luis      (1000)     4581 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/old/gui_components/licencia_window.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.299166 dosepy-0.6.2/src/Dosepy/scripts/
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1034 2024-02-22 03:59:11.000000 dosepy-0.6.2/src/Dosepy/scripts/test_tutorial.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.299166 dosepy-0.6.2/src/Dosepy/tools/
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2022-11-02 16:13:30.000000 dosepy-0.6.2/src/Dosepy/tools/__init__.py
+-rwxrwxr-x   0 luis      (1000) luis      (1000)     4433 2023-10-19 15:53:23.000000 dosepy-0.6.2/src/Dosepy/tools/film_to_dose.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.299166 dosepy-0.6.2/src/Dosepy/tools/gui_widgets/
+-rw-rw-r--   0 luis      (1000) luis      (1000)        0 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/tools/gui_widgets/__init__.py
+-rwxrwxr-x   0 luis      (1000) luis      (1000)     4243 2024-05-09 01:21:10.000000 dosepy-0.6.2/src/Dosepy/tools/resol.py
+drwxrwxr-x   0 luis      (1000) luis      (1000)        0 2024-05-11 18:45:10.303166 dosepy-0.6.2/src/Dosepy.egg-info/
+-rw-r--r--   0 luis      (1000) luis      (1000)     3828 2024-05-11 18:45:10.000000 dosepy-0.6.2/src/Dosepy.egg-info/PKG-INFO
+-rw-rw-r--   0 luis      (1000) luis      (1000)     1769 2024-05-11 18:45:10.000000 dosepy-0.6.2/src/Dosepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        1 2024-05-11 18:45:10.000000 dosepy-0.6.2/src/Dosepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)      133 2024-05-11 18:45:10.000000 dosepy-0.6.2/src/Dosepy.egg-info/requires.txt
+-rw-rw-r--   0 luis      (1000) luis      (1000)        7 2024-05-11 18:45:10.000000 dosepy-0.6.2/src/Dosepy.egg-info/top_level.txt
```

### Comparing `Dosepy-0.6.1/LICENSE` & `dosepy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/PKG-INFO` & `dosepy-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dosepy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Film dosimetry and gamma analysis for dose distributions in radiotherapy
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://dosepy.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://pypi.org/project/Dosepy/
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/Dosepy
 Keywords: Radiotherapy,Dose distribution,gamma index,python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Dosepy-0.6.1/README.md` & `dosepy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/pyproject.toml` & `dosepy-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Dosepy"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Luis Alfonso Olivares Jimenez", email="alfonso.cucei.udg@gmail.com" },
 ]
 description = "Film dosimetry and gamma analysis for dose distributions in radiotherapy"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENCE"}
```

### Comparing `Dosepy-0.6.1/src/Dosepy/Icon/Icon.png` & `dosepy-0.6.2/src/Dosepy/Icon/Icon.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/Icon/Logo_Dosepy.png` & `dosepy-0.6.2/src/Dosepy/Icon/Logo_Dosepy.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/Icon/cut_icon.png` & `dosepy-0.6.2/src/Dosepy/Icon/cut_icon.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/Icon/folder.png` & `dosepy-0.6.2/src/Dosepy/Icon/folder.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/Icon/save.png` & `dosepy-0.6.2/src/Dosepy/Icon/save.png`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app.py` & `dosepy-0.6.2/src/Dosepy/app.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/about_window.py` & `dosepy-0.6.2/src/Dosepy/app_components/about_window.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/cross_hair_cursor.py` & `dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/cross_hair_cursor.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/dp_multi_cursor.py` & `dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/dp_multi_cursor.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/draggable rectangle.py` & `dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/draggable rectangle.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/blitting_examples/to_do_rendering.py` & `dosepy-0.6.2/src/Dosepy/app_components/blitting_examples/to_do_rendering.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,141 +4,155 @@
 from matplotlib.backends.backend_qtagg import \
 	NavigationToolbar2QT as NavigationToolbar
 import sys
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_qtagg import FigureCanvas
 import matplotlib.colors as colors
 import numpy as np
-import pkg_resources
+#import pkg_resources
+from importlib import resources
 
 
-class BlittedCursorCrossHair:
+class BlittedCrossHair:
 	"""
-	A cross hair cursor using blitting for faster redraw.
+	A cross hair cursor using blitting for faster redraw. It works from Canvas' events.
 	"""
 	def __init__(self, ax):
 		self.ax = ax
 		self.background = None
 		self.horizontal_line = ax.axhline(color = 'cornflowerblue', lw = 1.5, ls = '--', alpha = 0.8)
 		self.vertical_line = ax.axvline(color = 'orange', lw = 1.5, ls = '--', alpha = 0.8)
 		# text location in axes coordinates
 		#self.text = ax.text(0.65, 0.9, '', transform=ax.transAxes)
 		self._creating_background = False
-		ax.figure.canvas.mpl_connect('draw_event', self.on_draw)
+		ax.figure.canvas.mpl_connect('draw_event', self._on_draw)
 
-	def on_draw(self, event):
-		#De utilidad si hay un cambio en el tamaño de la ventana
-		self.create_new_background()
-		print(event)
+	def _on_draw(self, event):
+		# Used when draw_event occurs.
+		self._create_new_background()
+		#print(event)
 
-	def set_cross_hair_visible(self, visible):
+	def _set_cross_hair_visible(self, visible):
 		need_redraw = self.horizontal_line.get_visible() != visible
 		self.horizontal_line.set_visible(visible)
 		self.vertical_line.set_visible(visible)
 		#self.text.set_visible(visible)
 		return need_redraw
 
-	def create_new_background(self):
+	def _create_new_background(self):
 		if self._creating_background:
 			# discard calls triggered from within this function
 			return
 		self._creating_background = True
-		self.set_cross_hair_visible(False)
+		self._set_cross_hair_visible(False)
 		self.ax.figure.canvas.draw()
 		self.background = self.ax.figure.canvas.copy_from_bbox(self.ax.bbox)
-		self.set_cross_hair_visible(True)
+		self._set_cross_hair_visible(True)
 		self._creating_background = False
 
-	def on_mouse_move(self, event):
+	def on_event(self, event):
 		#if event.inaxes != self.ax:
 		#	return
 		if self.background is None:
-			self.create_new_background()
+			self._create_new_background()
 		if not event.inaxes:
-			need_redraw = self.set_cross_hair_visible(False)
+			need_redraw = self._set_cross_hair_visible(False)
 			if need_redraw:
 				self.ax.figure.canvas.restore_region(self.background)
 				self.ax.figure.canvas.blit(self.ax.bbox)
 		else:
 			if event.inaxes != self.ax:	#Descartar evento fuera de Axes que contiene la imagen
 				return
-			self.set_cross_hair_visible(True)
+			self._set_cross_hair_visible(True)
 			# update the line positions
 			x, y = event.xdata, event.ydata
 			#dose = 
 
-			self.horizontal_line.set_ydata(y)
-			self.vertical_line.set_xdata(x)
+			self.horizontal_line.set_ydata([y])
+			self.vertical_line.set_xdata([x])
 			#self.text.set_text('x=%1.0f, y=%1.0f' % (x, y))
 			
 			self.ax.figure.canvas.restore_region(self.background)
 			self.ax.draw_artist(self.horizontal_line)
 			self.ax.draw_artist(self.vertical_line)
 			#self.ax.draw_artist(self.text)
 			self.ax.figure.canvas.blit(self.ax.bbox)
 
 
 class QtImageWidget(QWidget):
 	def __init__(self):
 		super().__init__()  # Call QWidget constructor
 		self.setWindowTitle('Dose distribution')
 
-		file_name_FILM = pkg_resources.resource_filename('Dosepy', 'data/D_FILM.csv')
-		self.array_refer = np.genfromtxt(file_name_FILM, delimiter = ',')
+		#file_name_film = pkg_resources.resource_filename('Dosepy', 'data/D_FILM.csv')
+		file_name_film = str(resources.files("Dosepy") / "data" / "D_FILM.csv")
+		self.array_refer = np.genfromtxt(file_name_film, delimiter = ',')
         
 		self.main_layout = QVBoxLayout()
-		self.iniciarUI()
+		self._iniciarUI()
         
-	def iniciarUI(self):
+	def _iniciarUI(self):
+		
+		self.mpl_left = Canvas()
+		self.mpl_left.show_dist(self.array_refer)
+
+		self.main_layout.addWidget(NavigationToolbar(self.mpl_left.canvas, self))
+		self.main_layout.addWidget(self.mpl_left.canvas)
 		
-		self.Mpl_Izq = Canvas()
-		self.Mpl_Izq.show_dist(self.array_refer)
-		self.Mpl_Izq.set_colorbar(self.array_refer) 
-		self.blitted_cross_hair = BlittedCursorCrossHair(self.Mpl_Izq.ax)
-		#self.id_on_press_perfil = self.Mpl_Izq.canvas.figure.canvas.mpl_connect('motion_notify_event', self.blitted_cross_hair.on_mouse_move)
-		self.id_on_press_perfil = self.Mpl_Izq.canvas.figure.canvas.mpl_connect('button_press_event', self.blitted_cross_hair.on_mouse_move)
-		self.main_layout.addWidget(NavigationToolbar(self.Mpl_Izq.canvas, self))
-		self.main_layout.addWidget(self.Mpl_Izq.canvas)
 		self.setLayout(self.main_layout)
+
+
+		self.blitted_cross_hair = BlittedCrossHair(self.mpl_left.ax)
+		self.id_on_press_perfil = self.mpl_left.canvas.figure.canvas.mpl_connect('motion_notify_event', self.blitted_cross_hair.on_event)
+		#self.id_on_press_profile = self.mpl_left.canvas.figure.canvas.mpl_connect('button_press_event', self.blitted_cross_hair.on_event)
+
             
 class Canvas:
-	"""Widget to show a dose distribution.
+	"""
+	Canvas to hold the image.
 	"""
 
 	def __init__(self):
 		fig = Figure(
 			layout='constrained')
-		self.ax = fig.add_subplot()
+		
 		self.canvas = FigureCanvas(fig)
+		self.ax = fig.add_subplot()
+
+		self.cmap='nipy_spectral'
+
+		self.mplI = None  # matplotlib.image.AxesImage
+		self.cbar = None  # matplotlib.colorbar.Colorbar
 		
 	def show_dist(self, array):
 		''' Show the dose distribution.
 
 		Parameters
 		----------
 		array : numpy.ndarray
             The image represented as a numpy array.
 		'''
-		self.npI = array
-		self.mplI = self.ax.imshow(self.npI)
 
-	def set_colorbar(self, npI_color_ref):
+		self.mplI = self.ax.imshow(array)
+		self._setup_colorbar(array)
+
+
+	def _setup_colorbar(self, array):
 		''' 
 		Set a colorbar. 
 		
 		Parameters
 		----------
 		array : numpy.ndarray
-			An array used as a reference to define dose boundaries.
 		'''
-		color_map = 'nipy_spectral'
-		bounds = np.linspace(0, round(1.15 * np.percentile(npI_color_ref, 98)), 256)
+
+		bounds = np.linspace(0, round(1.15 * np.percentile(array, 98)), 256)
 		norm = colors.BoundaryNorm(boundaries = bounds, ncolors = 256)
 		self.mplI.set_norm(norm)
-		self.mplI.set_cmap(color_map)
+		self.mplI.set_cmap(self.cmap)
 
 		self.cbar = self.canvas.figure.colorbar(
 			self.mplI,
 			ax = self.ax,
 			orientation = 'vertical',
 			format = '%.1f',
 			shrink = 0.8,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/calibration_widget.py` & `dosepy-0.6.2/src/Dosepy/app_components/calibration_widget.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/file_dialog.py` & `dosepy-0.6.2/src/Dosepy/app_components/file_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     if dir == "home":
         dialog.setDirectory(QDir.home())
 
     elif dir == "calib":
         cali_path = Path(__file__).parent.parent / "user" / "calibration"
         dialog.setDirectory(str(cali_path))
 
-    dialog.setFileMode(QFileDialog.FileMode.ExistingFile)
+    dialog.setFileMode(QFileDialog.FileMode.ExistingFiles)
     dialog.setNameFilter(filter)
 
     if dialog.exec():
         filenames = dialog.selectedFiles()
         list_files = [str(Path(f_name)) for f_name in filenames]
         return list_files
```

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/licencia_window.py` & `dosepy-0.6.2/src/Dosepy/app_components/licencia_window.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_components/tiff2dose_widget.py` & `dosepy-0.6.2/src/Dosepy/app_components/tiff2dose_widget.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_controller.py` & `dosepy-0.6.2/src/Dosepy/app_controller.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/app_model.py` & `dosepy-0.6.2/src/Dosepy/app_model.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/calibration.py` & `dosepy-0.6.2/src/Dosepy/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         elif self.channel in ["G", "Green", "g", "green"]:
             color = "green"
         elif self.channel in ["B", "Blue", "b", "blue"]:
             color = "blue"
         elif self.channel in ["M", "Mean", "m", "mean"]:
             color = "black"
         
-        ax.plot(x, y, color = color, **kwargs)
         ax.plot(
             self.x,
             self.doses,
             color = color,
             marker = '*',
             linestyle = 'None',
             **kwargs
```

### Comparing `Dosepy-0.6.1/src/Dosepy/data/D_FILM.csv` & `dosepy-0.6.2/src/Dosepy/data/D_FILM.csv`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/data/D_TPS.csv` & `dosepy-0.6.2/src/Dosepy/data/D_TPS.csv`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/i_o.py` & `dosepy-0.6.2/src/Dosepy/i_o.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/image.py` & `dosepy-0.6.2/src/Dosepy/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,14 +207,40 @@
         return self.array.shape
 
 
     def as_type(self, dtype: np.dtype) -> np.ndarray:
         return self.array.astype(dtype)
 
 
+    def crop(
+        self,
+        pixels: int = 15,
+        edges: tuple[str, ...] = ("top", "bottom", "left", "right"),
+    ) -> None:
+        """Removes pixels on all edges of the image in-place.
+
+        Parameters
+        ----------
+        pixels : int
+            Number of pixels to cut off all sides of the image.
+        edges : tuple
+            Which edges to remove from. Can be any combination of the four edges.
+        """
+        if pixels <= 0:
+            raise ValueError("Pixels to remove must be a positive number")
+        if "top" in edges:
+            self.array = self.array[pixels:, :]
+        if "bottom" in edges:
+            self.array = self.array[:-pixels, :]
+        if "left" in edges:
+            self.array = self.array[:, pixels:]
+        if "right" in edges:
+            self.array = self.array[:, :-pixels]
+
+
 class TiffImage(BaseImage):
     """An image from a tiff file.
 
     Attributes
     ----------
     sid : float
         The SID value as passed in upon construction.
@@ -283,15 +309,14 @@
             return
 
     def get_stat(
             self,
             ch='G',
             roi=(5, 5),
             show=False,
-            threshold=None
             ) -> list:
         r"""Get average and standar deviation from pixel values at a central ROI in each film.
 
         Parameter
         ---------
         ch : str
             Color channel. "R": Red, "G": Green, "B": Blue and "M": mean.
@@ -317,15 +342,15 @@
         >>> path_to_image = r"C:\QA\image.tif"
         >>> cal_image = load(path_to_image, for_calib = True)
         >>> mean, std = cal_image.get_stat(ch = 'G', roi=(5,5), show = True)
         >>> list(zip(mean, std))
         """
 
         if not self.label_image.any():
-            self.set_labeled_img(threshold = threshold)
+            self.set_labeled_img(threshold = 0.90)
 
         if show:
             fig, axes = plt.subplots(ncols=1)
             #ax = axes.ravel()
             axes = plt.subplot(1, 1, 1)
             #axes.imshow(gray_scale, cmap="gray")
             axes.imshow(self.array/np.max(self.array))
@@ -444,29 +469,36 @@
             plt.clf()
         ax.imshow(self.array/np.max(self.array), **kwargs)
         #ax.imshow(self.array[:,:,0], **kwargs)
         if show:
             plt.show()
         return ax
 
-    def to_dose(self, cal) -> ImageLike:
+    def to_dose(self, cal, clip=False) -> ImageLike:
         """Convert the tiff image to a dose distribution. The tiff file image
         has to contain an unirradiated film used as a reference for zero Gray.
 
         Parameters
         ----------
         cal : :class:`~Dosepy.calibration.Calibration`
             Instance of a Calibration class
 
+        clip : bool, default: False
+            If True, limit the maximum dose to the greatest used for calibration. Useful to avoid very high doses.
+
         Returns
         -------
         :class:`~Dosepy.image.ArrayImage`
             Dose distribution.
         """
-        mean_pixel, _ = self.get_stat(ch=cal.channel, roi=(5, 5), show=False)
+        mean_pixel, _ = self.get_stat(
+            ch=cal.channel,
+            roi=(5, 5),
+            show=False,
+            )
         mean_pixel = sorted(mean_pixel, reverse=True)
 
         if cal.channel in ["R", "Red", "r", "red"]:
             if cal.func in ["P3", "Polynomial"]:
                 x = -np.log10(self.array[:, :, 0]/mean_pixel[0])
             elif cal.func in ["RF", "Rational"]:
                 x = self.array[:, :, 0]/mean_pixel[0]
@@ -493,14 +525,18 @@
         if cal.func in ["P3", "Polynomial"]:
             dose_image = polynomial_g3(x, *cal.popt)
         elif cal.func in ["RF", "Rational"]:
             dose_image = rational_func(x, *cal.popt)
 
         dose_image[dose_image < 0] = 0  # Remove unphysical doses < 0
 
+        if clip:  # Limit the maximum dose
+            max_calib_dose = cal.doses[-1]
+            dose_image[dose_image > max_calib_dose] = max_calib_dose
+
         return load(dose_image, dpi=self.dpi)
 
     def doses_in_central_rois(self, cal, roi, show):
         """Dose in central film rois.
 
         Parameters
         ----------
@@ -537,15 +573,15 @@
         erosion_pix = int(6*self.dpmm)  # Number of pixels used for erosion.
         #print(f"Number of pixels to remove borders: {erosion_pix}")
 
         gray_scale = rgb2gray(self.array)
         if not threshold:
             thresh = threshold_otsu(gray_scale)  # Used for films identification.
         else:
-            thresh = threshold
+            thresh = threshold * np.amax(gray_scale)
         binary = erosion(gray_scale < thresh, square(erosion_pix))
         self.label_image, self.number_of_films = label(binary, return_num=True)
         
 
 class CalibImage(TiffImage):
     """A tiff image used for calibration."""
 
@@ -604,15 +640,15 @@
         >>> cal_image = load(path_to_image, for_calib = True)
         >>> cal = cal_image.get_calibration(doses = [0, 0.5, 1, 2, 4, 6, 8, 10], channel = "G")
         >>> # Plot the calibration curve
         >>> cal.plot()
         """
 
         doses = sorted(doses)
-        mean_pixel, _ = self.get_stat(ch=channel, roi=roi, threshold=threshold)
+        mean_pixel, _ = self.get_stat(ch=channel, roi=roi)
         mean_pixel = sorted(mean_pixel, reverse=True)
         mean_pixel = np.array(mean_pixel)
 
         if func in ["P3", "Polynomial"]:
             x = -np.log10(mean_pixel/mean_pixel[0])  # Optical density
 
         elif func in ["RF", "Rational"]:
@@ -669,14 +705,19 @@
         dpi = None
         if self._dpi is not None:
             dpi = self._dpi
             if self.sid is not None:
                 dpi *= self.sid / 1000
         return dpi
 
+    @property
+    def physical_shape(self):
+        """The physical size of the image in mm."""
+        return self.shape[0] / self.dpmm, self.shape[1] / self.dpmm
+
 
     def save_as_tif(self, file_name):
         """Used to save a dose distribution (in Gy) as a tif file (in cGy).
         
         Parameters
         ----------
         file_name : str
@@ -700,18 +741,19 @@
                 dose_ta=3,
                 dist_ta=3,
                 *,
                 dose_threshold=10,
                 dose_ta_Gy=False,
                 local_norm=False,
                 mask_radius=10,
-                max_as_percentile=True
+                max_as_percentile=True,
+                exclude_above=None
                 ):
         '''
-        Calculate the gamma between the current image (reference) and a comparison image.
+        Calculate gamma between the current image against a reference image.
         The images must have the same spatial resolution (dpi) to be comparable. The size of the images must also be the same.
         An array is ​​obtained. It represents the gamma indices at each position of the dose distribution,
         as well as the approval rate defined as the percentage of gamma values ​​that are less or equal to 1.
         The registration of dose distributions is assumed, i.e. the spatial coordinate of a point in the
         reference dose distribution is equal to the coordinate of the same point in the distribution to be evaluated.
 
         Parameters
@@ -759,14 +801,17 @@
             a distance greater than the dimensions of the dose distribution (for example mask_radius = 1000).
 
         max_as_percentile : bool, default: True
             If the argument is True, 99th percentile is used as an approximation of the maximum value of the
             dose distribution. This allows us to exclude artifacts or errors in specific positions.
             If the argument is False, the maximum value of the distribution is used.
 
+        exclude_above : float, default: None
+            Dose limit in Gy. Any point in the evaluated distribution greater than exclude_above, is not accounted in the pass rate. dose_ta_Gy should be set as True.
+
         Returns
         -------
 
         gamma_map : numpy.ndarray
             The calculated gamma distribution.
 
         pass_rate : float
@@ -942,25 +987,29 @@
                                 np.sqrt(
                                     (distance**2) / (dist_ta**2)
                                     + (dose_dif**2) / (dose_ta**2))
                                         )
 
                 gamma[i,j] = min(Gamma)
 
-                # For the position in question, if the dose is below than the dose threshold,
+                # For the position in question, if the dose is below than the dose threshold, or above exclude_above,
                 # then this point is not taken into account in the approval percentage.
                 if D_eval[i,j] < Dose_threshold:
                     gamma[i,j] = np.nan
 
+                if exclude_above:
+                    if D_eval[i,j] > exclude_above:
+                        gamma[i,j] = np.nan
+
         # Returns the coordinates where the gamma values ​​are less than or equal to 1
         less_than_1_coordinate = np.where(gamma <= 1)
         # Counts the number of coordinates where gamma <= 1 is True
         less_than_1 = np.shape(less_than_1_coordinate)[1]
         # Number of values that are not np.nan
-        total_points = np.shape(gamma)[0]*np.shape(gamma)[1] - np.shape(np.where(np.isnan(gamma)))[1]
+        total_points = gamma.size - np.isnan(gamma).sum(where=True)
 
         # Pass rate
         gamma_percent = float(less_than_1)/total_points*100
         return gamma, gamma_percent            
 
 
 def load_multiples(image_file_list, for_calib=False):
```

### Comparing `Dosepy-0.6.1/src/Dosepy/old/GUI.py` & `dosepy-0.6.2/src/Dosepy/old/GUI.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/old/dose.py` & `dosepy-0.6.2/src/Dosepy/old/dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/old/gui_components/Bloque_Imagenes.py` & `dosepy-0.6.2/src/Dosepy/old/gui_components/Bloque_Imagenes.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/old/gui_components/Bloque_gamma.py` & `dosepy-0.6.2/src/Dosepy/old/gui_components/Bloque_gamma.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/old/gui_components/about_window.py` & `dosepy-0.6.2/src/Dosepy/old/gui_components/about_window.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/old/gui_components/film_to_doseGUI.py` & `dosepy-0.6.2/src/Dosepy/old/gui_components/film_to_doseGUI.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/old/gui_components/licencia_window.py` & `dosepy-0.6.2/src/Dosepy/old/gui_components/licencia_window.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/scripts/test_tutorial.py` & `dosepy-0.6.2/src/Dosepy/scripts/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/tools/film_to_dose.py` & `dosepy-0.6.2/src/Dosepy/tools/film_to_dose.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy/tools/resol.py` & `dosepy-0.6.2/src/Dosepy/tools/resol.py`

 * *Files identical despite different names*

### Comparing `Dosepy-0.6.1/src/Dosepy.egg-info/PKG-INFO` & `dosepy-0.6.2/src/Dosepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dosepy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Film dosimetry and gamma analysis for dose distributions in radiotherapy
 Author-email: Luis Alfonso Olivares Jimenez <alfonso.cucei.udg@gmail.com>
 Project-URL: homepage, https://dosepy.readthedocs.io/en/latest/intro.html
 Project-URL: repository, https://pypi.org/project/Dosepy/
 Project-URL: Bug-Tracker, https://github.com/LuisOlivaresJ/Dosepy
 Keywords: Radiotherapy,Dose distribution,gamma index,python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Dosepy-0.6.1/src/Dosepy.egg-info/SOURCES.txt` & `dosepy-0.6.2/src/Dosepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

