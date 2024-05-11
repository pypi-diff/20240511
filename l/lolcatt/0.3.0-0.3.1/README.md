# Comparing `tmp/lolcatt-0.3.0.tar.gz` & `tmp/lolcatt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.3.0.tar", last modified: Sun May  5 20:43:17 2024, max compression
+gzip compressed data, was "lolcatt-0.3.1.tar", last modified: Sat May 11 16:47:28 2024, max compression
```

## Comparing `lolcatt-0.3.0.tar` & `lolcatt-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,163 @@
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1074 2024-02-16 09:11:52.000000 lolcatt-0.3.0/LICENSE
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      239 2024-02-16 09:11:52.000000 lolcatt-0.3.0/MANIFEST.in
--rw-r--r--   0 lueftinger  (1000) lueftinger  (1000)     4312 2024-05-05 20:43:17.610986 lolcatt-0.3.0/PKG-INFO
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     3504 2024-02-16 09:11:52.000000 lolcatt-0.3.0/README.rst
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/docs/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      608 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/Makefile
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/docs/_static/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       84 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/_static/custom.css
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)    26168 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/_static/screenshot.png
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     4983 2024-02-16 09:15:01.000000 lolcatt-0.3.0/docs/conf.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      264 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/index.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1138 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/installation.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      346 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.casting.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      517 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1232 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.ui.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      331 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/lolcatt.utils.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      805 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/make.bat
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       58 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/modules.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       27 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/readme.rst
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       69 2024-02-16 09:11:52.000000 lolcatt-0.3.0/docs/usage.rst
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      125 2024-05-05 20:42:54.000000 lolcatt-0.3.0/lolcatt/__init__.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1378 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/app.py
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/casting/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        0 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/casting/__init__.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)    10035 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/casting/caster.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1336 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/casting/youtube_playlist_handler.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1828 2024-05-05 20:42:54.000000 lolcatt-0.3.0/lolcatt/cli.py
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/ui/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        0 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/ui/__init__.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1579 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     4860 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1265 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1640 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     3068 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     3016 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt/utils/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        0 2024-02-16 09:11:52.000000 lolcatt-0.3.0/lolcatt/utils/__init__.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     2422 2024-02-16 09:15:01.000000 lolcatt-0.3.0/lolcatt/utils/utils.py
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/lolcatt.egg-info/
--rw-r--r--   0 lueftinger  (1000) lueftinger  (1000)     4312 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      982 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        1 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       45 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        1 2024-05-05 20:28:54.000000 lolcatt-0.3.0/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       54 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)        8 2024-05-05 20:43:17.000000 lolcatt-0.3.0/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      559 2024-05-05 20:42:54.000000 lolcatt-0.3.0/pyproject.toml
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       38 2024-05-05 20:43:17.610986 lolcatt-0.3.0/setup.cfg
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)     1556 2024-05-05 20:42:54.000000 lolcatt-0.3.0/setup.py
-drwxrwxr-x   0 lueftinger  (1000) lueftinger  (1000)        0 2024-05-05 20:43:17.610986 lolcatt-0.3.0/tests/
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)       37 2024-02-16 09:11:52.000000 lolcatt-0.3.0/tests/__init__.py
--rw-rw-r--   0 lueftinger  (1000) lueftinger  (1000)      211 2024-02-16 09:11:52.000000 lolcatt-0.3.0/tests/test_lolcatt.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1074 2023-07-23 10:21:40.000000 lolcatt-0.3.1/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      239 2023-07-23 10:21:40.000000 lolcatt-0.3.1/MANIFEST.in
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     4312 2024-05-11 16:47:28.289271 lolcatt-0.3.1/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3504 2023-07-23 10:25:50.000000 lolcatt-0.3.1/README.rst
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.192604 lolcatt-0.3.1/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      608 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/Makefile
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.145938 lolcatt-0.3.1/docs/_build/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.145938 lolcatt-0.3.1/docs/_build/html/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.209271 lolcatt-0.3.1/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    14813 2023-07-23 10:39:33.000000 lolcatt-0.3.1/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       84 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      286 2023-05-12 22:36:26.000000 lolcatt-0.3.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       90 2023-05-12 22:36:26.000000 lolcatt-0.3.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4208 2023-07-23 10:39:33.000000 lolcatt-0.3.1/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       90 2023-05-12 22:36:26.000000 lolcatt-0.3.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4956 2023-07-23 10:39:33.000000 lolcatt-0.3.1/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    26168 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_build/html/_static/screenshot.png
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.212604 lolcatt-0.3.1/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       84 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    26168 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4983 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      264 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1138 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      346 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      517 2023-07-23 10:39:30.000000 lolcatt-0.3.1/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1232 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      331 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      805 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       58 2023-07-23 10:39:30.000000 lolcatt-0.3.1/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       27 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       69 2023-07-23 10:21:40.000000 lolcatt-0.3.1/docs/usage.rst
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.212604 lolcatt-0.3.1/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 00:01:30.000000 lolcatt-0.3.1/lolcatt/.githash
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)      125 2024-05-11 16:44:59.000000 lolcatt-0.3.1/lolcatt/__init__.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1378 2024-05-11 16:30:11.000000 lolcatt-0.3.1/lolcatt/app.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.215937 lolcatt-0.3.1/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.3.1/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    10035 2023-10-29 15:57:12.000000 lolcatt-0.3.1/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1336 2023-10-29 15:57:47.000000 lolcatt-0.3.1/lolcatt/casting/youtube_playlist_handler.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1827 2024-05-11 16:41:39.000000 lolcatt-0.3.1/lolcatt/cli.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.219271 lolcatt-0.3.1/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.3.1/lolcatt/ui/__init__.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1579 2024-05-11 16:30:11.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4860 2023-10-29 15:57:12.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1265 2023-07-23 10:25:25.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_device_info.py
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1640 2024-05-11 16:30:11.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3068 2023-07-23 10:25:50.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3016 2023-10-29 15:57:12.000000 lolcatt-0.3.1/lolcatt/ui/lolcatt_url_input.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.219271 lolcatt-0.3.1/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)        0 2023-07-23 10:21:40.000000 lolcatt-0.3.1/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     2422 2023-10-29 15:57:52.000000 lolcatt-0.3.1/lolcatt/utils/utils.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/lolcatt.egg-info/
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     4312 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/PKG-INFO
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     5711 2024-05-11 16:47:28.000000 lolcatt-0.3.1/lolcatt.egg-info/SOURCES.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)        1 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/dependency_links.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)       45 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/entry_points.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)        1 2024-05-09 17:01:17.000000 lolcatt-0.3.1/lolcatt.egg-info/not-zip-safe
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)       54 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/requires.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)        8 2024-05-11 16:47:27.000000 lolcatt-0.3.1/lolcatt.egg-info/top_level.txt
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)      559 2024-05-11 16:44:59.000000 lolcatt-0.3.1/pyproject.toml
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)       38 2024-05-11 16:47:28.289271 lolcatt-0.3.1/setup.cfg
+-rw-r--r--   0 atav1st   (1000) atav1st   (1001)     1556 2024-05-11 16:44:59.000000 lolcatt-0.3.1/setup.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.219271 lolcatt-0.3.1/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       37 2023-07-23 10:21:40.000000 lolcatt-0.3.1/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      211 2023-07-23 10:21:40.000000 lolcatt-0.3.1/tests/test_lolcatt.py
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.222604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html4css1/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7219 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html4css1/html4css1.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.249271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/math.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7388 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7749 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/plain.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    11895 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    12023 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/html5_polyglot/tuftig.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.249271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/pep_html/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6367 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/pep_html/pep.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.252604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      910 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3605 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.255937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      905 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3565 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.262604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1002 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      648 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4383 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      818 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      450 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      283 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/slides.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.262604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4029 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.262604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      943 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3989 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.265937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4028 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.265937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      940 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3999 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.265937 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/.githash
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.269271 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/ui_textual/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1579 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/ui_textual/lolcatt.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.272604 lolcatt-0.3.1/venv/lib/python3.10/site-packages/textual/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3515 2023-07-16 15:29:00.000000 lolcatt-0.3.1/venv/lib/python3.10/site-packages/textual/demo.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.155938 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html4css1/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7219 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html4css1/html4css1.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/math.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7388 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     7749 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/plain.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    11895 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)    12023 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/html5_polyglot/tuftig.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/pep_html/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     6367 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/pep_html/pep.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.149271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.152604 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      910 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3605 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.285937 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      905 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3565 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1002 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      261 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      648 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4383 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      818 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      450 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      283 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/default/slides.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4029 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      943 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3989 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     4028 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)      940 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3999 2023-07-16 15:28:55.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)       41 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/.githash
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.155938 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/ui/
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/ui/ui_textual/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     1579 2023-07-16 15:29:01.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/lolcatt/ui/ui_textual/lolcatt.css
+drwxr-xr-x   0 atav1st   (1000) atav1st   (1001)        0 2024-05-11 16:47:28.289271 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/textual/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1001)     3515 2023-07-16 15:29:00.000000 lolcatt-0.3.1/venv/lib64/python3.10/site-packages/textual/demo.css
```

### Comparing `lolcatt-0.3.0/LICENSE` & `lolcatt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/PKG-INFO` & `lolcatt-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.3.0
+Version: 0.3.1
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.3.0/README.rst` & `lolcatt-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/Makefile` & `lolcatt-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/_static/screenshot.png` & `lolcatt-0.3.1/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/conf.py` & `lolcatt-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/installation.rst` & `lolcatt-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/lolcatt.rst` & `lolcatt-0.3.1/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/lolcatt.ui.rst` & `lolcatt-0.3.1/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/docs/make.bat` & `lolcatt-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/app.py` & `lolcatt-0.3.1/lolcatt/app.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/casting/caster.py` & `lolcatt-0.3.1/lolcatt/casting/caster.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/casting/youtube_playlist_handler.py` & `lolcatt-0.3.1/lolcatt/casting/youtube_playlist_handler.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/cli.py` & `lolcatt-0.3.1/lolcatt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,20 +47,20 @@
     config = Path(str(config)).expanduser()
     if not config.exists():
         config.parent.mkdir(parents=True, exist_ok=True)
         write_initial_config(config)
 
     config = toml.loads(config.read_text())
 
-    if url_or_path is None and scan:
+    if len(url_or_path) == 0 and scan:
         do_scan()
         return
 
     lolcatt = LolCatt(device_name=device, config=config)
-    if url_or_path is not None:
+    if len(url_or_path) > 0:
         for up in url_or_path:
             lolcatt.caster.enqueue(up)
         lolcatt.caster.cast_next()
     lolcatt.run()
 
 
 if __name__ == '__main__':
```

### Comparing `lolcatt-0.3.0/lolcatt/ui/lolcatt.css` & `lolcatt-0.3.1/venv/lib/python3.10/site-packages/lolcatt/ui/ui_textual/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.3.1/lolcatt/ui/lolcatt_controls.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.3.1/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.3.1/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.3.1/lolcatt/ui/lolcatt_progress.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.3.1/lolcatt/ui/lolcatt_url_input.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt/utils/utils.py` & `lolcatt-0.3.1/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.3.0/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.3.1/lolcatt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.3.0
+Version: 0.3.1
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.3.0/pyproject.toml` & `lolcatt-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.3.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.3.0/setup.py` & `lolcatt-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

