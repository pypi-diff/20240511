# Comparing `tmp/adafruit-circuitpython-pycamera-1.3.0.tar.gz` & `tmp/adafruit_circuitpython_pycamera-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pycamera-1.3.0.tar", last modified: Mon Mar 11 20:10:36 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_pycamera-1.3.1.tar", last modified: Fri May 10 22:48:58 2024, max compression
```

## Comparing `adafruit-circuitpython-pycamera-1.3.0.tar` & `adafruit_circuitpython_pycamera-1.3.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.910779 adafruit-circuitpython-pycamera-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.894780 adafruit-circuitpython-pycamera-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.898779 adafruit-circuitpython-pycamera-1.3.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.898779 adafruit-circuitpython-pycamera-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.898779 adafruit-circuitpython-pycamera-1.3.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/LICENSES/GPL-2.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-11 20:10:36.910779 adafruit-circuitpython-pycamera-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.910779 adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-03-11 20:10:36.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-11 20:10:36.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 20:10:36.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-11 20:10:36.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 20:10:36.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.902779 adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/
--rw-r--r--   0 runner    (1001) docker     (127)    39609 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/imageprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/ironbow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/ov5640_autofocus.bin
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/ov5640_autofocus.bin.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.902779 adafruit-circuitpython-pycamera-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.902779 adafruit-circuitpython-pycamera-1.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.902779 adafruit-circuitpython-pycamera-1.3.0/docs/mock/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/mock/displayio.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.894780 adafruit-circuitpython-pycamera-1.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.902779 adafruit-circuitpython-pycamera-1.3.0/examples/basic_camera/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/basic_camera/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.902779 adafruit-circuitpython-pycamera-1.3.0/examples/camera/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/camera/boot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/camera/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.906779 adafruit-circuitpython-pycamera-1.3.0/examples/filter/
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/filter/code.py
--rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/filter/cornell_box_208x208.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/filter/cornell_box_208x208.jpg.license
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/filter/testpattern_208x208.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/filter/testpattern_208x208.jpg.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.906779 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/
--rw-r--r--   0 runner    (1001) docker     (127)    49290 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/blinka_emoji_rgb888.bmp
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/blinka_emoji_rgb888.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/code_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/code_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)   230538 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/heart_frame_rgb888.bmp
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/heart_frame_rgb888.bmp.license
--rw-r--r--   0 runner    (1001) docker     (127)   307338 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/pencil_frame_rgb888.bmp
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/overlay/pencil_frame_rgb888.bmp.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.906779 adafruit-circuitpython-pycamera-1.3.0/examples/qrio/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/qrio/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.906779 adafruit-circuitpython-pycamera-1.3.0/examples/viewer/
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/viewer/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.906779 adafruit-circuitpython-pycamera-1.3.0/examples/web_camera/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/web_camera/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.906779 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 20:10:36.910779 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/metadata.js
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/make_web_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-11 20:10:34.000000 adafruit-circuitpython-pycamera-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-11 20:10:28.000000 adafruit-circuitpython-pycamera-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 20:10:36.910779 adafruit-circuitpython-pycamera-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.873173 adafruit_circuitpython_pycamera-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.877173 adafruit_circuitpython_pycamera-1.3.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.877173 adafruit_circuitpython_pycamera-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.877173 adafruit_circuitpython_pycamera-1.3.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/LICENSES/GPL-2.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-10 22:48:58.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-10 22:48:58.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:48:58.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-10 22:48:58.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 22:48:58.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/
+-rw-r--r--   0 runner    (1001) docker     (127)    39609 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/imageprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/ironbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/ov5640_autofocus.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/ov5640_autofocus.bin.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/docs/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/mock/displayio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.877173 adafruit_circuitpython_pycamera-1.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/examples/basic_camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/basic_camera/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/examples/camera/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/camera/boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/camera/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.881173 adafruit_circuitpython_pycamera-1.3.1/examples/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/filter/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/filter/cornell_box_208x208.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/filter/cornell_box_208x208.jpg.license
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/filter/testpattern_208x208.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/filter/testpattern_208x208.jpg.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)    49290 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/blinka_emoji_rgb888.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/blinka_emoji_rgb888.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/code_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/code_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230538 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/heart_frame_rgb888.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/heart_frame_rgb888.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (127)   307338 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/pencil_frame_rgb888.bmp
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/overlay/pencil_frame_rgb888.bmp.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/examples/qrio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/qrio/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/examples/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/viewer/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/examples/web_camera/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/web_camera/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/metadata.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/make_web_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-10 22:48:56.000000 adafruit_circuitpython_pycamera-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-10 22:48:50.000000 adafruit_circuitpython_pycamera-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:48:58.885173 adafruit_circuitpython_pycamera-1.3.1/setup.cfg
```

### Comparing `adafruit-circuitpython-pycamera-1.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_pycamera-1.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/.gitignore` & `adafruit_circuitpython_pycamera-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/.pre-commit-config.yaml` & `adafruit_circuitpython_pycamera-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/.pylintrc` & `adafruit_circuitpython_pycamera-1.3.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_pycamera-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/LICENSE` & `adafruit_circuitpython_pycamera-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_pycamera-1.3.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/LICENSES/CC0-1.0.txt` & `adafruit_circuitpython_pycamera-1.3.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/LICENSES/GPL-2.0-only.txt` & `adafruit_circuitpython_pycamera-1.3.1/LICENSES/GPL-2.0-only.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/LICENSES/MIT.txt` & `adafruit_circuitpython_pycamera-1.3.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_pycamera-1.3.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/PKG-INFO` & `adafruit_circuitpython_pycamera-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pycamera
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library for the Adafruit PyCamera
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PyCamera
 Keywords: adafruit,blinka,circuitpython,micropython,pycamera,camera,esp32s3,wifi,ov5640
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pycamera-1.3.0/README.rst` & `adafruit_circuitpython_pycamera-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/PKG-INFO` & `adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pycamera
-Version: 1.3.0
+Version: 1.3.1
 Summary: Library for the Adafruit PyCamera
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PyCamera
 Keywords: adafruit,blinka,circuitpython,micropython,pycamera,camera,esp32s3,wifi,ov5640
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pycamera-1.3.0/adafruit_circuitpython_pycamera.egg-info/SOURCES.txt` & `adafruit_circuitpython_pycamera-1.3.1/adafruit_circuitpython_pycamera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/__init__.py` & `adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/imageprocessing.py` & `adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/imageprocessing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/ironbow.py` & `adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/ironbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/adafruit_pycamera/ov5640_autofocus.bin` & `adafruit_circuitpython_pycamera-1.3.1/adafruit_pycamera/ov5640_autofocus.bin`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/docs/_static/favicon.ico` & `adafruit_circuitpython_pycamera-1.3.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/docs/conf.py` & `adafruit_circuitpython_pycamera-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/docs/index.rst` & `adafruit_circuitpython_pycamera-1.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/docs/mock/displayio.py` & `adafruit_circuitpython_pycamera-1.3.1/docs/mock/displayio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/basic_camera/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/basic_camera/code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/camera/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/camera/code.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,66 @@
 # SPDX-FileCopyrightText: 2023 Jeff Epler for Adafruit Industries
 # SPDX-FileCopyrightText: 2023 Limor Fried for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
-
+import ssl
+import os
 import time
+import socketpool
+import adafruit_requests
+import rtc
+import adafruit_ntp
+import wifi
 import bitmaptools
 import displayio
 import gifio
 import ulab.numpy as np
 
 import adafruit_pycamera
 
+# Wifi details are in settings.toml file, also,
+# timezone info should be included to allow local time and DST adjustments
+# # UTC_OFFSET, if present, will override TZ and DST and no API query will be done
+# UTC_OFFSET=-25200
+# # TZ="America/Phoenix"
+
+UTC_OFFSET = os.getenv("UTC_OFFSET")
+TZ = os.getenv("TZ")
+
+print(f"Connecting to {os.getenv('CIRCUITPY_WIFI_SSID')}")
+SSID = os.getenv("CIRCUITPY_WIFI_SSID")
+PASSWORD = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+
+if SSID and PASSWORD:
+    wifi.radio.connect(
+        os.getenv("CIRCUITPY_WIFI_SSID"), os.getenv("CIRCUITPY_WIFI_PASSWORD")
+    )
+    if wifi.radio.connected:
+        print(f"Connected to {os.getenv('CIRCUITPY_WIFI_SSID')}!")
+        print("My IP address is", wifi.radio.ipv4_address)
+        pool = socketpool.SocketPool(wifi.radio)
+
+        if UTC_OFFSET is None:
+            requests = adafruit_requests.Session(pool, ssl.create_default_context())
+            response = requests.get("http://worldtimeapi.org/api/timezone/" + TZ)
+            response_as_json = response.json()
+            UTC_OFFSET = response_as_json["raw_offset"] + response_as_json["dst_offset"]
+            print(f"UTC_OFFSET: {UTC_OFFSET}")
+
+        ntp = adafruit_ntp.NTP(
+            pool, server="pool.ntp.org", tz_offset=UTC_OFFSET // 3600
+        )
+
+        print(f"ntp time: {ntp.datetime}")
+        rtc.RTC().datetime = ntp.datetime
+    else:
+        print("Wifi failed to connect. Time not set.")
+else:
+    print("Wifi config not found in settintgs.toml. Time not set.")
+
 pycam = adafruit_pycamera.PyCamera()
 # pycam.live_preview_mode()
 
 settings = (
     None,
     "resolution",
     "effect",
@@ -159,15 +205,15 @@
                     pycam.blit(_gifframe)
                     t1 = time.monotonic()
                     ft.append(1 / (t1 - t0))
                     print(end=".")
                     t0 = t1
             pycam._mode_label.text = "GIF"  # pylint: disable=protected-access
             print(f"\nfinal size {f.tell()} for {i} frames")
-            print(f"average framerate {i/(t1-t00)}fps")
+            print(f"average framerate {i / (t1 - t00)}fps")
             print(f"best {max(ft)} worst {min(ft)} std. deviation {np.std(ft)}")
             f.close()
             pycam.display.refresh()
 
         if pycam.mode_text == "JPEG":
             pycam.tone(200, 0.1)
             try:
```

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/filter/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/filter/code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/filter/cornell_box_208x208.jpg` & `adafruit_circuitpython_pycamera-1.3.1/examples/filter/cornell_box_208x208.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/filter/testpattern_208x208.jpg` & `adafruit_circuitpython_pycamera-1.3.1/examples/filter/testpattern_208x208.jpg`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/overlay/blinka_emoji_rgb888.bmp` & `adafruit_circuitpython_pycamera-1.3.1/examples/overlay/blinka_emoji_rgb888.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/overlay/code_select.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/overlay/code_select.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/overlay/code_simple.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/overlay/code_simple.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/overlay/heart_frame_rgb888.bmp` & `adafruit_circuitpython_pycamera-1.3.1/examples/overlay/heart_frame_rgb888.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/overlay/pencil_frame_rgb888.bmp` & `adafruit_circuitpython_pycamera-1.3.1/examples/overlay/pencil_frame_rgb888.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/qrio/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/qrio/code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/viewer/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/viewer/code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/web_camera/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/web_camera/code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/code.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/code.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/index.html` & `adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/index.html`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/index.js` & `adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/index.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/htdocs/metadata.js` & `adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/htdocs/metadata.js`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/examples/web_settings_explorer/make_web_metadata.py` & `adafruit_circuitpython_pycamera-1.3.1/examples/web_settings_explorer/make_web_metadata.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pycamera-1.3.0/pyproject.toml` & `adafruit_circuitpython_pycamera-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pycamera"
 description = "Library for the Adafruit PyCamera"
-version = "1.3.0"
+version = "1.3.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PyCamera"}
 keywords = [
     "adafruit",
```

