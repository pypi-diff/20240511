# Comparing `tmp/mpl_ascii-0.5.0.tar.gz` & `tmp/mpl_ascii-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl_ascii-0.5.0.tar", last modified: Fri May 10 08:49:02 2024, max compression
+gzip compressed data, was "mpl_ascii-0.6.0.tar", last modified: Fri May 10 14:15:35 2024, max compression
```

## Comparing `mpl_ascii-0.5.0.tar` & `mpl_ascii-0.6.0.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.983471 mpl_ascii-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.987471 mpl_ascii-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.995471 mpl_ascii-0.5.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_chart.txt
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_label_5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/bar_stacked.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/barh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/barh.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/categorical_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/categorical_variables.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/cohere.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/csd_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/csd_demo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/double_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/double_plot.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/errorbars_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_best_fit_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_best_fit_line.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple_colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/hist_simple_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/line_markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/line_markers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/lines_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/lines_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/scatter_multi_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/scatter_multi_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/simple_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/examples/simple_plot.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.995471 mpl_ascii-0.5.0/mpl_ascii/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/ascii_canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/color_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/mpl_ascii/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/mpl_ascii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 08:49:01.000000 mpl_ascii-0.5.0/mpl_ascii.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:49:01.999471 mpl_ascii-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-10 08:48:55.000000 mpl_ascii-0.5.0/tests/test_overlay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.570323 mpl_ascii-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.554323 mpl_ascii-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.554323 mpl_ascii-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-10 14:15:35.570323 mpl_ascii-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.566323 mpl_ascii-0.6.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8373 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_chart.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_label_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/bar_stacked.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/barh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/barh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/box_plot_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/box_plot_basic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/categorical_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21803 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/categorical_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/cohere.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/csd_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/csd_demo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/double_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/double_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8639 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/errorbars_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/hist_best_fit_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/hist_best_fit_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/hist_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/hist_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/hist_simple_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14815 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/hist_simple_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/line_markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38794 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/line_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/lines_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/lines_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/scatter_multi_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/scatter_multi_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/simple_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/simple_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/violin_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/examples/violin_plot.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.566323 mpl_ascii-0.6.0/mpl_ascii/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/mpl_ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/mpl_ascii/ascii_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/mpl_ascii/color_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14018 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/mpl_ascii/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/mpl_ascii/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/mpl_ascii/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.570323 mpl_ascii-0.6.0/mpl_ascii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-10 14:15:35.000000 mpl_ascii-0.6.0/mpl_ascii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-10 14:15:35.000000 mpl_ascii-0.6.0/mpl_ascii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:15:35.000000 mpl_ascii-0.6.0/mpl_ascii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 14:15:35.000000 mpl_ascii-0.6.0/mpl_ascii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 14:15:35.000000 mpl_ascii-0.6.0/mpl_ascii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:15:35.570323 mpl_ascii-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:35.570323 mpl_ascii-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-10 14:15:24.000000 mpl_ascii-0.6.0/tests/test_overlay.py
```

### Comparing `mpl_ascii-0.5.0/.github/workflows/python-package.yml` & `mpl_ascii-0.6.0/.github/workflows/python-package.yml`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 jobs:
   test:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install pytest
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
@@ -42,15 +42,15 @@
     needs: test
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
 
     - name: Install packaging tools
       run: |
         python -m pip install --upgrade pip
         python -m pip install build twine
@@ -65,18 +65,18 @@
 
   download-and-test:
     needs: build-and-publish
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v3
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install --pre --index-url https://${{ secrets.GEMFURY_DOWNLOAD_PYPI_API }}:@pypi.fury.io/chriscave/ --extra-index-url https://pypi.org/simple mpl_ascii
     - name: Test package
```

### Comparing `mpl_ascii-0.5.0/.gitignore` & `mpl_ascii-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/CHANGELOG.md` & `mpl_ascii-0.6.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.6.0] 2024-05-10
+
+## Added
+
+- Add support for violin plots
+
+### Fixed
+
+- Fixed empty line markers with box plots.
+
 ## [0.5.0] 2024-05-10
 
 ### Added
 
 - Added support for python 3.7+
 
 ## [0.4.0] 2024-05-05
```

### Comparing `mpl_ascii-0.5.0/LICENSE` & `mpl_ascii-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/Makefile` & `mpl_ascii-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/PKG-INFO` & `mpl_ascii-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.5.0
+Version: 0.6.0
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
@@ -51,25 +51,28 @@
 import mpl_ascii
 
 mpl_ascii.AXES_WIDTH=100
 mpl_ascii.AXES_HEIGHT=40
 
 mpl.use("module://mpl_ascii")
 
-fig, ax = plt.subplots()
+import matplotlib.pyplot as plt
 
+# Example data
 fruits = ['apple', 'blueberry', 'cherry', 'orange']
-counts = [40, 100, 30, 55]
-bar_labels = ['red', 'blue', '_red', 'orange']
-bar_colors = ['tab:red', 'tab:blue', 'tab:red', 'tab:orange']
+counts = [10, 15, 7, 5]
+colors = ['red', 'blue', 'red', 'orange']  # Colors corresponding to each fruit
+
+fig, ax = plt.subplots()
 
-ax.bar(fruits, counts, label=bar_labels, color=bar_colors)
+# Plot each bar individually
+for fruit, count, color in zip(fruits, counts, colors):
+    ax.bar(fruit, count, color=color, label=color)
 
-ax.set_ylabel('fruit supply')
-ax.set_title('Fruit supply by kind and color')
+# Display the legend
 ax.legend(title='Fruit color')
 
 plt.show()
 ```
 
 ![bar chart with color](https://imgur.com/u4pRU3E.png)
```

### Comparing `mpl_ascii-0.5.0/README.md` & `mpl_ascii-0.6.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -36,25 +36,28 @@
 import mpl_ascii
 
 mpl_ascii.AXES_WIDTH=100
 mpl_ascii.AXES_HEIGHT=40
 
 mpl.use("module://mpl_ascii")
 
-fig, ax = plt.subplots()
+import matplotlib.pyplot as plt
 
+# Example data
 fruits = ['apple', 'blueberry', 'cherry', 'orange']
-counts = [40, 100, 30, 55]
-bar_labels = ['red', 'blue', '_red', 'orange']
-bar_colors = ['tab:red', 'tab:blue', 'tab:red', 'tab:orange']
+counts = [10, 15, 7, 5]
+colors = ['red', 'blue', 'red', 'orange']  # Colors corresponding to each fruit
+
+fig, ax = plt.subplots()
 
-ax.bar(fruits, counts, label=bar_labels, color=bar_colors)
+# Plot each bar individually
+for fruit, count, color in zip(fruits, counts, colors):
+    ax.bar(fruit, count, color=color, label=color)
 
-ax.set_ylabel('fruit supply')
-ax.set_title('Fruit supply by kind and color')
+# Display the legend
 ax.legend(title='Fruit color')
 
 plt.show()
 ```
 
 ![bar chart with color](https://imgur.com/u4pRU3E.png)
```

### Comparing `mpl_ascii-0.5.0/examples/bar_chart.py` & `mpl_ascii-0.6.0/examples/bar_chart.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_chart.txt` & `mpl_ascii-0.6.0/examples/bar_chart.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_color.py` & `mpl_ascii-0.6.0/examples/bar_color.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     parser.add_argument("--out", type=str)
 
     args = parser.parse_args()
     out = args.out
 
     import matplotlib.pyplot as plt
 
-    import matplotlib.pyplot as plt
-
     # Example data
     fruits = ['apple', 'blueberry', 'cherry', 'orange']
     counts = [10, 15, 7, 5]
     colors = ['red', 'blue', 'red', 'orange']  # Colors corresponding to each fruit
 
     fig, ax = plt.subplots()
```

### Comparing `mpl_ascii-0.5.0/examples/bar_color.txt` & `mpl_ascii-0.6.0/examples/bar_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_1.py` & `mpl_ascii-0.6.0/examples/bar_label_1.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_1.txt` & `mpl_ascii-0.6.0/examples/bar_label_1.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_2.py` & `mpl_ascii-0.6.0/examples/bar_label_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_2.txt` & `mpl_ascii-0.6.0/examples/bar_label_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_3.py` & `mpl_ascii-0.6.0/examples/bar_label_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_3.txt` & `mpl_ascii-0.6.0/examples/bar_label_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_4.py` & `mpl_ascii-0.6.0/examples/bar_label_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_4.txt` & `mpl_ascii-0.6.0/examples/bar_label_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_5.py` & `mpl_ascii-0.6.0/examples/bar_label_5.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_label_5.txt` & `mpl_ascii-0.6.0/examples/bar_label_5.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_stacked.py` & `mpl_ascii-0.6.0/examples/bar_stacked.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/bar_stacked.txt` & `mpl_ascii-0.6.0/examples/bar_stacked.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/barh.py` & `mpl_ascii-0.6.0/examples/barh.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/barh.txt` & `mpl_ascii-0.6.0/examples/barh.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/categorical_variables.py` & `mpl_ascii-0.6.0/examples/categorical_variables.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/categorical_variables.txt` & `mpl_ascii-0.6.0/examples/categorical_variables.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/cohere.py` & `mpl_ascii-0.6.0/examples/cohere.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/cohere.txt` & `mpl_ascii-0.6.0/examples/cohere.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/csd_demo.py` & `mpl_ascii-0.6.0/examples/csd_demo.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/csd_demo.txt` & `mpl_ascii-0.6.0/examples/csd_demo.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/double_plot.py` & `mpl_ascii-0.6.0/examples/double_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/double_plot.txt` & `mpl_ascii-0.6.0/examples/double_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars.txt` & `mpl_ascii-0.6.0/examples/errorbars.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars_2.py` & `mpl_ascii-0.6.0/examples/errorbars_2.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars_2.txt` & `mpl_ascii-0.6.0/examples/errorbars_2.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars_3.py` & `mpl_ascii-0.6.0/examples/errorbars_3.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars_3.txt` & `mpl_ascii-0.6.0/examples/errorbars_3.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars_4.py` & `mpl_ascii-0.6.0/examples/errorbars_4.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/errorbars_4.txt` & `mpl_ascii-0.6.0/examples/errorbars_4.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/hist_best_fit_line.py` & `mpl_ascii-0.6.0/examples/hist_best_fit_line.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/hist_best_fit_line.txt` & `mpl_ascii-0.6.0/examples/hist_best_fit_line.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/hist_simple.py` & `mpl_ascii-0.6.0/examples/hist_simple.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/hist_simple.txt` & `mpl_ascii-0.6.0/examples/hist_simple.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/hist_simple_colors.py` & `mpl_ascii-0.6.0/examples/hist_simple_colors.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/hist_simple_colors.txt` & `mpl_ascii-0.6.0/examples/hist_simple_colors.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/line_markers.py` & `mpl_ascii-0.6.0/examples/line_markers.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/line_markers.txt` & `mpl_ascii-0.6.0/examples/line_markers.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/lines_multi_color.py` & `mpl_ascii-0.6.0/examples/lines_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/lines_multi_color.txt` & `mpl_ascii-0.6.0/examples/lines_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/scatter_multi_color.py` & `mpl_ascii-0.6.0/examples/scatter_multi_color.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/scatter_multi_color.txt` & `mpl_ascii-0.6.0/examples/scatter_multi_color.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/simple_plot.py` & `mpl_ascii-0.6.0/examples/simple_plot.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/examples/simple_plot.txt` & `mpl_ascii-0.6.0/examples/simple_plot.txt`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/mpl_ascii/__init__.py` & `mpl_ascii-0.6.0/mpl_ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/mpl_ascii/ascii_canvas.py` & `mpl_ascii-0.6.0/mpl_ascii/ascii_canvas.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/mpl_ascii/color_map.py` & `mpl_ascii-0.6.0/mpl_ascii/color_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import matplotlib
-from matplotlib.collections import PathCollection
+from matplotlib.collections import LineCollection, PathCollection, PolyCollection
 from matplotlib.container import BarContainer
 from matplotlib.patches import Rectangle
 
 
 bar_chars = [
     "#",
     "%",
@@ -76,14 +76,30 @@
     gen = ascii_chars(line_chars)
     for line in lines:
         color = std_color(line.get_color())
         if color in color_to_ascii:
             continue
         color_to_ascii[color] = Char(next(gen), color)
 
+    for collection in ax.collections:
+        if isinstance(collection, PolyCollection):
+            for color in collection.get_facecolor():
+                color = std_color(tuple(color.tolist()))
+                if color in color_to_ascii:
+                    continue
+                color_to_ascii[color] = Char(next(gen), color)
+
+        if isinstance(collection, LineCollection):
+            for color in collection.get_color():
+                color = std_color(tuple(color.tolist()))
+                if color in color_to_ascii:
+                    continue
+                color_to_ascii[color] = Char(next(gen), color)
+
+
 
     gen = ascii_chars(scatter_chars)
     for collection in ax.collections:
         if not isinstance(collection, PathCollection):
             continue
         for color in collection.get_facecolor():
             color = std_color(tuple(color.tolist()))
```

### Comparing `mpl_ascii-0.5.0/mpl_ascii/draw.py` & `mpl_ascii-0.6.0/mpl_ascii/draw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import math
-from matplotlib.collections import PathCollection
+from matplotlib.collections import LineCollection, PathCollection, PolyCollection
 from matplotlib.container import BarContainer, ErrorbarContainer
 from matplotlib.lines import Line2D
 from matplotlib.patches import Rectangle
 import numpy as np
 
 from mpl_ascii.ascii_canvas import AsciiCanvas
 from mpl_ascii.color_map import Char, ax_color_map, std_color
@@ -30,56 +29,56 @@
         y_range = y_range[1], y_range[0]
 
     x_min, x_max = x_range
     y_min, y_max = y_range
 
     canvas = AsciiCanvas(np.full((axes_height, axes_width), fill_value=" "))
 
-    all_bars = []
+    errorbar_caplines = []
+    error_barlinescols = []
+    for container in ax.containers:
+        if not isinstance(container, ErrorbarContainer):
+            continue
+        _, caplines, barlinescols = tuple(container)
+        errorbar_caplines += [*caplines]
+        error_barlinescols += [*barlinescols]
+
 
     for container in ax.containers:
         if not isinstance(container, BarContainer):
             continue
         for bar in container.patches:
             if not isinstance(bar, Rectangle):
                 continue
-            all_bars.append(bar)
 
-    for bar in all_bars:
-        char = color_to_ascii[std_color(bar.get_facecolor())]
+            char = color_to_ascii[std_color(bar.get_facecolor())]
 
-        canvas_bar = AsciiCanvas(
-                draw_bar(
-                bar.get_height(),
-                bar.get_width(),
-                axes_height,
-                axes_width,
-                x_range,
-                y_range,
-                char
+            canvas_bar = AsciiCanvas(
+                    draw_bar(
+                    bar.get_height(),
+                    bar.get_width(),
+                    axes_height,
+                    axes_width,
+                    x_range,
+                    y_range,
+                    char
+                )
             )
-        )
-        ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
-        ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
+            ascii_x_bar = round(linear_transform(bar.xy[0], x_min, x_max, 0, axes_width-1))
+            ascii_y_bar = round(linear_transform(bar.xy[1], y_min, y_max, 1, axes_height))
 
-        canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
+            canvas = canvas.update(canvas_bar, (axes_height - ascii_y_bar - canvas_bar.shape[0]+1, ascii_x_bar))
 
-    errorbar_caplines = []
-    for container in ax.containers:
-        if not isinstance(container, ErrorbarContainer):
-            continue
-        _, caplines, _ = tuple(container)
-        errorbar_caplines += [*caplines]
 
 
     lines_with_markers = []
     for line in ax.get_lines():
         if line in errorbar_caplines:
             continue
-        if line.get_marker() != "None":
+        if line.get_marker() != "None" and line.get_marker() != "":
             lines_with_markers.append(line)
 
         char = color_to_ascii[std_color(line.get_color())]
         xy_data = line.get_xydata()
         x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
         line = AsciiCanvas(
                 draw_line(
@@ -93,37 +92,36 @@
                 linestyle=line.get_linestyle()
             )
         )
 
         canvas = canvas.update(line, (0,0))
 
     for container in ax.containers:
-        if not isinstance(container, ErrorbarContainer):
-            continue
-        _, _, barlinescols = tuple(container)
+        if isinstance(container, ErrorbarContainer):
+            _, _, barlinescols = tuple(container)
 
-        for collection in barlinescols:
-            for xy in collection.get_segments():
-                x_data = [p[0] for p in xy]
-                y_data = [p[1] for p in xy]
-                char = Char("-", "white")
-
-                if len(set(x_data)) == 1:
-                    char = Char("|", "white")
-
-                errorbar = AsciiCanvas(draw_line(
-                    width=axes_width,
-                    height=axes_height,
-                    x_data=x_data,
-                    y_data=y_data,
-                    x_range=x_range,
-                    y_range=y_range,
-                    char = char
-                ))
-                canvas = canvas.update(errorbar, (0,0))
+            for collection in barlinescols:
+                for xy in collection.get_segments():
+                    x_data = [p[0] for p in xy]
+                    y_data = [p[1] for p in xy]
+                    char = Char("-", "white")
+
+                    if len(set(x_data)) == 1:
+                        char = Char("|", "white")
+
+                    errorbar = AsciiCanvas(draw_line(
+                        width=axes_width,
+                        height=axes_height,
+                        x_data=x_data,
+                        y_data=y_data,
+                        x_range=x_range,
+                        y_range=y_range,
+                        char = char
+                    ))
+                    canvas = canvas.update(errorbar, (0,0))
 
     for line in lines_with_markers:
         marker = get_ascii_marker(line.get_marker())
 
         color = color_to_ascii[std_color(line.get_color())].color
         char = Char(marker.upper(), color)
         xy_data = line.get_xydata()
@@ -139,26 +137,64 @@
                 char = char,
                 linestyle="None"
             )
         )
         canvas = canvas.update(line, (0,0))
 
     for collection in ax.collections:
-        if not isinstance(collection, PathCollection):
-            continue
-        offsets = collection.get_offsets()
+        if isinstance(collection, PolyCollection):
+            char = color_to_ascii[std_color(collection.get_facecolor())]
+            for path in collection.get_paths():
+                xy_data = path.vertices
+                x_data, y_data = [dat[0] for dat in xy_data], [dat[1] for dat in xy_data]
+                line = AsciiCanvas(
+                    draw_line(
+                    width=axes_width,
+                    height=axes_height,
+                    x_data=x_data,
+                    y_data=y_data,
+                    x_range=x_range,
+                    y_range=y_range,
+                    char = char,
+                    )
+                )
+                canvas = canvas.update(line, (0,0))
 
-        color = collection.get_facecolors()[0]
-        for point in offsets:
-            color = tuple(color)
+        if isinstance(collection, LineCollection):
+            if collection in error_barlinescols:
+                continue
+
+            for xy in collection.get_segments():
+                x_data = [p[0] for p in xy]
+                y_data = [p[1] for p in xy]
+                char = color_to_ascii[std_color(collection.get_color())]
+                line = AsciiCanvas(
+                    draw_line(
+                    width=axes_width,
+                    height=axes_height,
+                    x_data=x_data,
+                    y_data=y_data,
+                    x_range=x_range,
+                    y_range=y_range,
+                    char = char,
+                    )
+                )
+                canvas = canvas.update(line, (0,0))
+
+        if isinstance(collection, PathCollection):
+            offsets = collection.get_offsets()
+
+            color = collection.get_facecolors()[0]
+            for point in offsets:
+                color = tuple(color)
 
-            x_new = round(linear_transform(point[0], x_min, x_max, 0, axes_width-1))
-            y_new = round(linear_transform(point[1], y_min, y_max, 1, axes_height))
+                x_new = round(linear_transform(point[0], x_min, x_max, 0, axes_width-1))
+                y_new = round(linear_transform(point[1], y_min, y_max, 1, axes_height))
 
-            canvas = canvas.update(AsciiCanvas(np.array([[color_to_ascii[std_color(color)]]])), (axes_height-y_new, x_new))
+                canvas = canvas.update(AsciiCanvas(np.array([[color_to_ascii[std_color(color)]]])), (axes_height-y_new, x_new))
 
 
 
     # for text in ax.texts:
     #     text_canvas = AsciiCanvas(np.array([list(text.get_text())]))
     #     ascii_x = round(linear_transform(text.xy[0], x_min, x_max, 0, axes_width-1))
     #     ascii_y = round(linear_transform(text.xy[1], y_min, y_max, 1, axes_height))
```

### Comparing `mpl_ascii-0.5.0/mpl_ascii/overlay.py` & `mpl_ascii-0.6.0/mpl_ascii/overlay.py`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/mpl_ascii.egg-info/PKG-INFO` & `mpl_ascii-0.6.0/mpl_ascii.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpl_ascii
-Version: 0.5.0
+Version: 0.6.0
 Summary: A matplotlib backend that produces plots using only ASCII characters
 Author: Chris Cave
 Maintainer: Chris Cave
 License: MIT License
 Project-URL: Homepage, https://github.com/chriscave/mpl_ascii
 Keywords: matplotlib,plotting,ASCII
 Requires-Python: >=3.7
@@ -51,25 +51,28 @@
 import mpl_ascii
 
 mpl_ascii.AXES_WIDTH=100
 mpl_ascii.AXES_HEIGHT=40
 
 mpl.use("module://mpl_ascii")
 
-fig, ax = plt.subplots()
+import matplotlib.pyplot as plt
 
+# Example data
 fruits = ['apple', 'blueberry', 'cherry', 'orange']
-counts = [40, 100, 30, 55]
-bar_labels = ['red', 'blue', '_red', 'orange']
-bar_colors = ['tab:red', 'tab:blue', 'tab:red', 'tab:orange']
+counts = [10, 15, 7, 5]
+colors = ['red', 'blue', 'red', 'orange']  # Colors corresponding to each fruit
+
+fig, ax = plt.subplots()
 
-ax.bar(fruits, counts, label=bar_labels, color=bar_colors)
+# Plot each bar individually
+for fruit, count, color in zip(fruits, counts, colors):
+    ax.bar(fruit, count, color=color, label=color)
 
-ax.set_ylabel('fruit supply')
-ax.set_title('Fruit supply by kind and color')
+# Display the legend
 ax.legend(title='Fruit color')
 
 plt.show()
 ```
 
 ![bar chart with color](https://imgur.com/u4pRU3E.png)
```

### Comparing `mpl_ascii-0.5.0/mpl_ascii.egg-info/SOURCES.txt` & `mpl_ascii-0.6.0/mpl_ascii.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 examples/bar_label_4.txt
 examples/bar_label_5.py
 examples/bar_label_5.txt
 examples/bar_stacked.py
 examples/bar_stacked.txt
 examples/barh.py
 examples/barh.txt
+examples/box_plot_basic.py
+examples/box_plot_basic.txt
 examples/categorical_variables.py
 examples/categorical_variables.txt
 examples/cohere.py
 examples/cohere.txt
 examples/csd_demo.py
 examples/csd_demo.txt
 examples/double_plot.py
@@ -50,14 +52,16 @@
 examples/line_markers.txt
 examples/lines_multi_color.py
 examples/lines_multi_color.txt
 examples/scatter_multi_color.py
 examples/scatter_multi_color.txt
 examples/simple_plot.py
 examples/simple_plot.txt
+examples/violin_plot.py
+examples/violin_plot.txt
 mpl_ascii/__init__.py
 mpl_ascii/ascii_canvas.py
 mpl_ascii/color_map.py
 mpl_ascii/draw.py
 mpl_ascii/overlay.py
 mpl_ascii/tools.py
 mpl_ascii.egg-info/PKG-INFO
```

### Comparing `mpl_ascii-0.5.0/pyproject.toml` & `mpl_ascii-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpl_ascii-0.5.0/tests/test_overlay.py` & `mpl_ascii-0.6.0/tests/test_overlay.py`

 * *Files identical despite different names*

