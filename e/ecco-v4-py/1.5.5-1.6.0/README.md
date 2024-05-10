# Comparing `tmp/ecco_v4_py-1.5.5.tar.gz` & `tmp/ecco_v4_py-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecco_v4_py-1.5.5.tar", last modified: Mon Feb 27 19:20:02 2023, max compression
+gzip compressed data, was "ecco_v4_py-1.6.0.tar", last modified: Fri May 10 21:59:43 2024, max compression
```

## Comparing `ecco_v4_py-1.5.5.tar` & `ecco_v4_py-1.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:20:02.838798 ecco_v4_py-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-27 19:20:02.838798 ecco_v4_py-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:20:02.826798 ecco_v4_py-1.5.5/binary_data/
--rw-r--r--   0 runner    (1001) docker     (123)   421200 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/binary_data/basins.data
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/binary_data/basins.meta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:20:02.834798 ecco_v4_py-1.5.5/ecco_v4_py/
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/calc_meridional_trsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/calc_section_trsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/calc_stf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19444 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/ecco_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/get_basin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/get_section_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/llc_array_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    43118 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/netcdf_product_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/read_bin_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/read_bin_llc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/resample_to_latlon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/scalar_calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:20:02.838798 ecco_v4_py-1.5.5/ecco_v4_py/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_ecco_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_generate_ecco_netcdf_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_get_basin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_llc_array_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_meridional_trsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_proj_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_read_mds.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_scalar_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_section_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_section_trsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_stf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_tile_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/test/test_vector_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/tile_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/tile_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    26259 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/tile_plot_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/ecco_v4_py/vector_calc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:20:02.834798 ecco_v4_py-1.5.5/ecco_v4_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-27 19:20:02.000000 ecco_v4_py-1.5.5/ecco_v4_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-27 19:20:02.000000 ecco_v4_py-1.5.5/ecco_v4_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 19:20:02.000000 ecco_v4_py-1.5.5/ecco_v4_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-27 19:20:02.000000 ecco_v4_py-1.5.5/ecco_v4_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-27 19:20:02.000000 ecco_v4_py-1.5.5/ecco_v4_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:20:02.838798 ecco_v4_py-1.5.5/meta_json/
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/meta_json/ecco_meta_common.json
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/meta_json/ecco_meta_variable.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-27 19:20:02.838798 ecco_v4_py-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-27 19:19:52.000000 ecco_v4_py-1.5.5/setup.py
+drwxrwxr-x   0 ifenty   (44257) ecco      (4200)        0 2024-05-10 21:59:43.039681 ecco_v4_py-1.6.0/
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     1050 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/LICENSE.txt
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)      113 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/MANIFEST.in
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     3236 2024-05-10 21:59:43.039681 ecco_v4_py-1.6.0/PKG-INFO
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     1776 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/README.md
+drwxrwxr-x   0 ifenty   (44257) ecco      (4200)        0 2024-05-10 21:59:43.029681 ecco_v4_py-1.6.0/binary_data/
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)   421200 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/binary_data/basins.data
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)      128 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/binary_data/basins.meta
+drwxrwxr-x   0 ifenty   (44257) ecco      (4200)        0 2024-05-10 21:59:43.031681 ecco_v4_py-1.6.0/ecco_v4_py/
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     3581 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/__init__.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    10740 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/calc_meridional_trsp.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    13500 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/calc_section_trsp.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     6789 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/calc_stf.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    19444 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/ecco_utils.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     6565 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/get_basin.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    12722 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/get_section_masks.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    33477 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/llc_array_conversion.py
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)    43163 2024-05-10 20:45:53.000000 ecco_v4_py-1.6.0/ecco_v4_py/netcdf_product_generation.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     1186 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/plot_utils.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     4504 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/read_bin_gen.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    28373 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/read_bin_llc.py
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)     9147 2024-05-10 20:45:53.000000 ecco_v4_py-1.6.0/ecco_v4_py/resample_to_latlon.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     2058 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/scalar_calc.py
+drwxrwxr-x   0 ifenty   (44257) ecco      (4200)        0 2024-05-10 21:59:43.037681 ecco_v4_py-1.6.0/ecco_v4_py/test/
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)        0 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/__init__.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     4140 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_common.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     1179 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_ecco_utils.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     3439 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_generate_ecco_netcdf_product.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     2674 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_get_basin.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    13203 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_llc_array_conversion.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     4494 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_meridional_trsp.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     1326 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_plot_utils.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     1831 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_proj_plot.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)      876 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_read_mds.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)      888 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_scalar_calc.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)      646 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_section_masks.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     4952 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_section_trsp.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     4799 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_stf.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     2550 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_tile_plot.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     3203 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/test/test_vector_calc.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    18024 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/tile_io.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    13023 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/tile_plot.py
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)    26854 2024-05-10 20:45:53.000000 ecco_v4_py-1.6.0/ecco_v4_py/tile_plot_proj.py
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     2609 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/ecco_v4_py/vector_calc.py
+drwxrwxr-x   0 ifenty   (44257) ecco      (4200)        0 2024-05-10 21:59:43.038681 ecco_v4_py-1.6.0/ecco_v4_py.egg-info/
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     3236 2024-05-10 21:59:43.000000 ecco_v4_py-1.6.0/ecco_v4_py.egg-info/PKG-INFO
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)     1420 2024-05-10 21:59:43.000000 ecco_v4_py-1.6.0/ecco_v4_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)        1 2024-05-10 21:59:43.000000 ecco_v4_py-1.6.0/ecco_v4_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)      134 2024-05-10 21:59:43.000000 ecco_v4_py-1.6.0/ecco_v4_py.egg-info/requires.txt
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)       11 2024-05-10 21:59:43.000000 ecco_v4_py-1.6.0/ecco_v4_py.egg-info/top_level.txt
+drwxrwxr-x   0 ifenty   (44257) ecco      (4200)        0 2024-05-10 21:59:43.037681 ecco_v4_py-1.6.0/meta_json/
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)     5140 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/meta_json/ecco_meta_common.json
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)    10484 2023-04-12 03:06:48.000000 ecco_v4_py-1.6.0/meta_json/ecco_meta_variable.json
+-rw-r--r--   0 ifenty   (44257) ecco      (4200)       79 2024-05-10 21:59:43.040681 ecco_v4_py-1.6.0/setup.cfg
+-rw-rw-r--   0 ifenty   (44257) ecco      (4200)     1709 2024-05-10 20:45:53.000000 ecco_v4_py-1.6.0/setup.py
```

### Comparing `ecco_v4_py-1.5.5/LICENSE.txt` & `ecco_v4_py-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/PKG-INFO` & `ecco_v4_py-1.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 Metadata-Version: 2.1
 Name: ecco_v4_py
-Version: 1.5.5
+Version: 1.6.0
 Summary: Estimating the Circulation and Climate of the Ocean (ECCO) Version 4 Python Package
 Home-page: https://github.com/ECCO-GROUP/ECCOv4-py
 Author: Ian Fenty, Ou Wang, Tim Smith, and others
 Author-email: ian.fenty@jpl.nasa.gov, ecco-group@mit.edu
 License: MIT
 Keywords: ecco,climate,mitgcm,estimate,circulation,climate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: future
+Requires-Dist: numpy
+Requires-Dist: Bottleneck
+Requires-Dist: Cartopy
+Requires-Dist: cmocean
+Requires-Dist: dask[complete]
+Requires-Dist: matplotlib
+Requires-Dist: netCDF4
+Requires-Dist: pyresample
+Requires-Dist: python-dateutil
+Requires-Dist: xarray
+Requires-Dist: xmitgcm
+Requires-Dist: xgcm>=0.5.0
 
 ## Synopsis
 
 ecco_v4_py is a Python package that includes tools for loading and manipulating the ECCO v4 ocean and sea-ice state estimate (http://ecco-group.org)
 
 Extensive documentation is provided on our readthedocs page: 
 http://ecco-v4-python-tutorial.readthedocs.io/index.html#
```

### Comparing `ecco_v4_py-1.5.5/README.md` & `ecco_v4_py-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/binary_data/basins.data` & `ecco_v4_py-1.6.0/binary_data/basins.data`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/__init__.py` & `ecco_v4_py-1.6.0/ecco_v4_py/__init__.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/calc_meridional_trsp.py` & `ecco_v4_py-1.6.0/ecco_v4_py/calc_meridional_trsp.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/calc_section_trsp.py` & `ecco_v4_py-1.6.0/ecco_v4_py/calc_section_trsp.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/calc_stf.py` & `ecco_v4_py-1.6.0/ecco_v4_py/calc_stf.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/ecco_utils.py` & `ecco_v4_py-1.6.0/ecco_v4_py/ecco_utils.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/get_basin.py` & `ecco_v4_py-1.6.0/ecco_v4_py/get_basin.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/get_section_masks.py` & `ecco_v4_py-1.6.0/ecco_v4_py/get_section_masks.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/llc_array_conversion.py` & `ecco_v4_py-1.6.0/ecco_v4_py/llc_array_conversion.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/netcdf_product_generation.py` & `ecco_v4_py-1.6.0/ecco_v4_py/netcdf_product_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -591,25 +591,26 @@
             tmp.to_netcdf(str(new_fname), encoding=encoding)
 
     return grid
 
 
 
 #%%
-def get_time_steps_from_mds_files(mds_var_dir, mds_file):
+def get_time_steps_from_mds_files(mds_var_dir, mds_file, less_output=True):
 
     if isinstance(mds_var_dir, str):
         mds_var_dir = Path(mds_var_dir)
 
     tmp_files = np.sort(list(mds_var_dir.glob(mds_file + '*meta')))
 
     time_steps = []
 
     print ('get time steps')
-    print (tmp_files)
+    if not less_output:
+        print(tmp_files)
     for i in range(len(tmp_files)):
         time_steps.append(int(tmp_files[i].stem[-10:]))
 
     return time_steps
 #%%
```

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/plot_utils.py` & `ecco_v4_py-1.6.0/ecco_v4_py/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/read_bin_gen.py` & `ecco_v4_py-1.6.0/ecco_v4_py/read_bin_gen.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/read_bin_llc.py` & `ecco_v4_py-1.6.0/ecco_v4_py/read_bin_llc.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/scalar_calc.py` & `ecco_v4_py-1.6.0/ecco_v4_py/scalar_calc.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_common.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_common.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_ecco_utils.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_ecco_utils.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_generate_ecco_netcdf_product.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_generate_ecco_netcdf_product.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_get_basin.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_get_basin.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_llc_array_conversion.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_llc_array_conversion.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_meridional_trsp.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_meridional_trsp.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_plot_utils.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_proj_plot.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_proj_plot.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_read_mds.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_read_mds.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_scalar_calc.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_scalar_calc.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_section_masks.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_section_masks.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_section_trsp.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_section_trsp.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_stf.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_stf.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_tile_plot.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_tile_plot.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/test/test_vector_calc.py` & `ecco_v4_py-1.6.0/ecco_v4_py/test/test_vector_calc.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/tile_io.py` & `ecco_v4_py-1.6.0/ecco_v4_py/tile_io.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/tile_plot.py` & `ecco_v4_py-1.6.0/ecco_v4_py/tile_plot.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/tile_plot_proj.py` & `ecco_v4_py-1.6.0/ecco_v4_py/tile_plot_proj.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                              show_grid_lines = True,
                              show_grid_labels = False,
                              show_coastline_over_data = True,
                              show_land_over_data = True,
                              grid_linewidth = 1,
                              grid_linestyle = '--',
                              colorbar_label = None,
+                             colorbar_location = None,
                              subplot_grid=None,
                              less_output=True,
                              **kwargs):
     
     """Plot a field of data from an arbitrary projection with lat/lon coordinates
     on a geographic projection after resampling it to a regular lat/lon grid.
     
@@ -244,14 +245,15 @@
                          show_grid_lines = show_grid_lines,
                          show_grid_labels = show_grid_labels,
                          show_coastline_over_data = show_coastline_over_data,
                          show_land_over_data = show_land_over_data,
                          grid_linewidth = grid_linewidth,
                          grid_linestyle = grid_linestyle,
                          colorbar_label = colorbar_label,
+                         colorbar_location = colorbar_location,
                          less_output=less_output)
 
         new_grid_lon_centers_out = new_grid_lon_centers
         new_grid_lat_centers_out = new_grid_lat_centers
         data_latlon_projection_out = data_latlon_projection
 
     else: # not polar stereographic projection
@@ -329,15 +331,16 @@
                               show_land = show_land,
                               show_grid_lines = show_grid_lines,
                               show_grid_labels = show_grid_labels,
                               show_coastline_over_data = show_coastline_over_data,
                               show_land_over_data = show_land_over_data,
                               grid_linewidth = grid_linewidth,
                               grid_linestyle = grid_linestyle,
-                              colorbar_label =colorbar_label,
+                              colorbar_label = colorbar_label,
+                              colorbar_location = colorbar_location,
                               less_output=less_output)
     
 
     return f, ax, p, cbar, new_grid_lon_centers_out, new_grid_lat_centers_out,\
         data_latlon_projection_out, gl
     #%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
 
@@ -358,14 +361,15 @@
                  show_land_over_data = True,
                  grid_linewidth = 1,
                  grid_linestyle = '--',
                  levels = 20,
                  data_zorder = 50,
                  points_color = 'k',
                  colorbar_label = None,
+                 colorbar_location = None,
                  less_output = True):
 
     # assign cmap default
     if cmap is None:
         cmap, (new_cmin,new_cmax) = assign_colormap(data, cmap)
 
     if isinstance(ax.projection, ccrs.NorthPolarStereo):
@@ -424,15 +428,16 @@
                               show_land = show_land,
                               show_grid_lines = show_grid_lines,
                               show_grid_labels = show_grid_labels,
                               show_coastline_over_data = show_coastline_over_data,
                               show_land_over_data = show_land_over_data,
                               grid_linewidth = grid_linewidth,
                               grid_linestyle = grid_linestyle,
-                              colorbar_label = colorbar_label)
+                              colorbar_label = colorbar_label,
+                              colorbar_location = colorbar_location)
         
 
     return p, gl, cbar
 
 #%%
 
 def plot_global(xx,yy, data,
@@ -448,14 +453,15 @@
                 show_grid_labels = False,
                 show_coastline_over_data = True,
                 show_land_over_data = True,
                 grid_linewidth = 1,
                 grid_linestyle = '--',
                 levels = 20,
                 colorbar_label=None,
+                colorbar_location=None,
                 data_zorder = 50,
                 points_color = 'k',
                 less_output=True):
 
     # assign cmap default
     if cmap is None:
         cmap, (new_cmin,new_cmax) = assign_colormap(data, cmap)
@@ -495,15 +501,16 @@
                               show_land = show_land,
                               show_grid_lines = show_grid_lines,
                               show_grid_labels = show_grid_labels,
                               show_coastline_over_data = show_coastline_over_data,
                               show_land_over_data = show_land_over_data,
                               grid_linewidth = grid_linewidth,
                               grid_linestyle = grid_linestyle,
-                              colorbar_label = colorbar_label)
+                              colorbar_label = colorbar_label,
+                              colorbar_location = colorbar_location)
 
     return p, gl, cbar
 
 # -----------------------------------------------------------------------------
 
 def _add_features_to_axis(ax, p, cmin, cmax,
                           cmap = 'jet',
@@ -512,15 +519,16 @@
                           show_land=True, 
                           show_grid_lines=True,
                           show_grid_labels=True,
                           show_coastline_over_data = True,
                           show_land_over_data = True,
                           grid_linewidth = 1,
                           grid_linestyle = '--',
-                          colorbar_label = None):
+                          colorbar_label = None,
+                          colorbar_location = None):
                                      
     
     if show_land:
         if show_land_over_data:
         # place land over the data
             zorder = 75
         else:
@@ -550,16 +558,19 @@
                           linestyle=grid_linestyle,
                           zorder=110)
         
     cbar = []
     if show_colorbar:
         sm = plt.cm.ScalarMappable(cmap=cmap, norm=plt.Normalize(cmin,cmax))
         sm._A = []
-        cbar = plt.colorbar(sm,ax=ax)
-        #cbar = plt.colorbar(p, ax=ax)
+        if colorbar_location:
+            cbar = plt.colorbar(sm,ax=ax, location=colorbar_location)
+        else:
+            cbar = plt.colorbar(sm,ax=ax)
+            #cbar = plt.colorbar(p, ax=ax)
         if type(colorbar_label) is str:
             cbar.set_label(colorbar_label)
         
     return gl, cbar
 # -----------------------------------------------------------------------------
```

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py/vector_calc.py` & `ecco_v4_py-1.6.0/ecco_v4_py/vector_calc.py`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py.egg-info/PKG-INFO` & `ecco_v4_py-1.6.0/ecco_v4_py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,46 @@
 Metadata-Version: 2.1
-Name: ecco-v4-py
-Version: 1.5.5
+Name: ecco_v4_py
+Version: 1.6.0
 Summary: Estimating the Circulation and Climate of the Ocean (ECCO) Version 4 Python Package
 Home-page: https://github.com/ECCO-GROUP/ECCOv4-py
 Author: Ian Fenty, Ou Wang, Tim Smith, and others
 Author-email: ian.fenty@jpl.nasa.gov, ecco-group@mit.edu
 License: MIT
 Keywords: ecco,climate,mitgcm,estimate,circulation,climate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: future
+Requires-Dist: numpy
+Requires-Dist: Bottleneck
+Requires-Dist: Cartopy
+Requires-Dist: cmocean
+Requires-Dist: dask[complete]
+Requires-Dist: matplotlib
+Requires-Dist: netCDF4
+Requires-Dist: pyresample
+Requires-Dist: python-dateutil
+Requires-Dist: xarray
+Requires-Dist: xmitgcm
+Requires-Dist: xgcm>=0.5.0
 
 ## Synopsis
 
 ecco_v4_py is a Python package that includes tools for loading and manipulating the ECCO v4 ocean and sea-ice state estimate (http://ecco-group.org)
 
 Extensive documentation is provided on our readthedocs page: 
 http://ecco-v4-python-tutorial.readthedocs.io/index.html#
```

### Comparing `ecco_v4_py-1.5.5/ecco_v4_py.egg-info/SOURCES.txt` & `ecco_v4_py-1.6.0/ecco_v4_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/meta_json/ecco_meta_common.json` & `ecco_v4_py-1.6.0/meta_json/ecco_meta_common.json`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/meta_json/ecco_meta_variable.json` & `ecco_v4_py-1.6.0/meta_json/ecco_meta_variable.json`

 * *Files identical despite different names*

### Comparing `ecco_v4_py-1.5.5/setup.py` & `ecco_v4_py-1.6.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def README():
     with open('README.md') as f:
         return f.read()
 
 setup(
   name = 'ecco_v4_py',
   packages = ['ecco_v4_py'], # this must be the same as the name above
-  version = '1.5.5',
+  version = '1.6.0',
   description = 'Estimating the Circulation and Climate of the Ocean (ECCO) Version 4 Python Package',
   author = 'Ian Fenty, Ou Wang, Tim Smith, and others',
   author_email = 'ian.fenty@jpl.nasa.gov, ecco-group@mit.edu',
   url = 'https://github.com/ECCO-GROUP/ECCOv4-py',
   keywords = ['ecco','climate','mitgcm','estimate','circulation','climate'],
   include_package_data=True,
   data_files=[('binary_data',['binary_data/basins.data', 'binary_data/basins.meta'])],
@@ -36,12 +36,18 @@
   classifiers=[
       'Development Status :: 5 - Production/Stable',
       'Intended Audience :: Science/Research',
       'License :: OSI Approved :: MIT License',
       'Natural Language :: English',
       'Programming Language :: Python',
       'Programming Language :: Python :: 3.7',
+      'Programming Language :: Python :: 3.8',
+      'Programming Language :: Python :: 3.9',
+      'Programming Language :: Python :: 3.10',
+      'Programming Language :: Python :: 3.11',
+      'Programming Language :: Python :: 3.12',
+      'Programming Language :: Python :: 3.13',
       'Topic :: Scientific/Engineering :: Physics'
   ],
   long_description=README(),
   long_description_content_type='text/markdown'
 )
```

