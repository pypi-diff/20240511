# Comparing `tmp/nobuco-0.9.1.tar.gz` & `tmp/nobuco-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.9.1.tar", last modified: Thu Nov 30 15:43:46 2023, max compression
+gzip compressed data, was "nobuco-0.9.2.tar", last modified: Thu Nov 30 23:33:46 2023, max compression
```

## Comparing `nobuco-0.9.1.tar` & `nobuco-0.9.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.792720 nobuco-0.9.1/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.9.1/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)    31107 2023-11-30 15:43:46.792720 nobuco-0.9.1/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    30474 2023-11-18 01:40:01.000000 nobuco-0.9.1/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.784720 nobuco-0.9.1/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      705 2023-07-31 09:28:25.000000 nobuco-0.9.1/nobuco/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.784720 nobuco-0.9.1/nobuco/addons/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-09-20 16:04:48.000000 nobuco-0.9.1/nobuco/addons/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.784720 nobuco-0.9.1/nobuco/addons/torch/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-09-22 09:40:21.000000 nobuco-0.9.1/nobuco/addons/torch/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1337 2023-11-20 15:30:15.000000 nobuco-0.9.1/nobuco/addons/torch/dense_image_warp.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      769 2023-09-22 10:52:20.000000 nobuco-0.9.1/nobuco/addons/torch/depth_to_space.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      772 2023-09-22 10:47:27.000000 nobuco-0.9.1/nobuco/addons/torch/space_to_depth.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      355 2023-09-22 10:54:22.000000 nobuco-0.9.1/nobuco/addons/torch/util.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1096 2023-08-18 20:14:33.000000 nobuco-0.9.1/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    15886 2023-10-23 13:24:04.000000 nobuco-0.9.1/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.784720 nobuco-0.9.1/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2403 2023-10-04 12:08:06.000000 nobuco-0.9.1/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1994 2023-10-23 13:47:37.000000 nobuco-0.9.1/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-08-06 12:41:35.000000 nobuco-0.9.1/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-10-23 13:46:42.000000 nobuco-0.9.1/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4294 2023-10-23 10:40:09.000000 nobuco-0.9.1/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.784720 nobuco-0.9.1/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14972 2023-10-23 12:31:14.000000 nobuco-0.9.1/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1474 2023-09-29 11:56:47.000000 nobuco-0.9.1/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.788720 nobuco-0.9.1/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5047 2023-10-23 13:50:13.000000 nobuco-0.9.1/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      630 2023-08-06 11:12:41.000000 nobuco-0.9.1/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-10-23 13:23:24.000000 nobuco-0.9.1/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.788720 nobuco-0.9.1/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.792720 nobuco-0.9.1/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      227 2023-09-22 08:35:23.000000 nobuco-0.9.1/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     7612 2023-10-18 17:43:52.000000 nobuco-0.9.1/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2249 2023-10-04 12:38:40.000000 nobuco-0.9.1/nobuco/node_converters/attention.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-08-06 10:51:45.000000 nobuco-0.9.1/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1192 2023-07-26 14:20:16.000000 nobuco-0.9.1/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3491 2023-11-30 14:36:44.000000 nobuco-0.9.1/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    11449 2023-11-15 20:02:59.000000 nobuco-0.9.1/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1309 2023-07-26 14:39:38.000000 nobuco-0.9.1/nobuco/node_converters/dropout.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1053 2023-10-31 11:09:45.000000 nobuco-0.9.1/nobuco/node_converters/fft.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4500 2023-11-27 21:13:10.000000 nobuco-0.9.1/nobuco/node_converters/grid_sampling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1750 2023-11-30 15:28:41.000000 nobuco-0.9.1/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5182 2023-10-04 12:38:40.000000 nobuco-0.9.1/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11051 2023-10-23 18:52:57.000000 nobuco-0.9.1/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1818 2023-11-30 14:38:10.000000 nobuco-0.9.1/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2909 2023-10-17 11:36:57.000000 nobuco-0.9.1/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.9.1/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3894 2023-11-15 13:51:53.000000 nobuco-0.9.1/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     7156 2023-10-31 11:30:52.000000 nobuco-0.9.1/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9721 2023-10-23 13:15:01.000000 nobuco-0.9.1/nobuco/node_converters/reduce.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14671 2023-11-30 14:59:10.000000 nobuco-0.9.1/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1160 2023-11-30 14:27:52.000000 nobuco-0.9.1/nobuco/node_converters/tensor_broadcast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-10-23 12:44:40.000000 nobuco-0.9.1/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12063 2023-11-27 13:48:16.000000 nobuco-0.9.1/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11829 2023-11-30 15:36:13.000000 nobuco-0.9.1/nobuco/node_converters/tensor_manipulation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.9.1/nobuco/node_converters/tensor_shape.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1101 2023-10-17 11:37:30.000000 nobuco-0.9.1/nobuco/node_converters/torchvision.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.792720 nobuco-0.9.1/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-10-04 13:56:18.000000 nobuco-0.9.1/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10451 2023-11-27 13:20:13.000000 nobuco-0.9.1/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2778 2023-10-23 12:36:50.000000 nobuco-0.9.1/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.792720 nobuco-0.9.1/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.9.1/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 15:43:46.792720 nobuco-0.9.1/nobuco.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)    31107 2023-11-30 15:43:46.000000 nobuco-0.9.1/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     2050 2023-11-30 15:43:46.000000 nobuco-0.9.1/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-11-30 15:43:46.000000 nobuco-0.9.1/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-11-30 15:43:46.000000 nobuco-0.9.1/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-11-30 15:43:46.000000 nobuco-0.9.1/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-11-30 15:07:10.000000 nobuco-0.9.1/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-11-30 15:43:46.792720 nobuco-0.9.1/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.940110 nobuco-0.9.2/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.9.2/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)    31107 2023-11-30 23:33:46.940110 nobuco-0.9.2/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    30474 2023-11-18 01:40:01.000000 nobuco-0.9.2/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.932110 nobuco-0.9.2/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      733 2023-11-30 21:39:14.000000 nobuco-0.9.2/nobuco/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.932110 nobuco-0.9.2/nobuco/addons/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-09-20 16:04:48.000000 nobuco-0.9.2/nobuco/addons/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.936110 nobuco-0.9.2/nobuco/addons/torch/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-09-22 09:40:21.000000 nobuco-0.9.2/nobuco/addons/torch/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1337 2023-11-20 15:30:15.000000 nobuco-0.9.2/nobuco/addons/torch/dense_image_warp.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      769 2023-09-22 10:52:20.000000 nobuco-0.9.2/nobuco/addons/torch/depth_to_space.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      772 2023-09-22 10:47:27.000000 nobuco-0.9.2/nobuco/addons/torch/space_to_depth.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      355 2023-09-22 10:54:22.000000 nobuco-0.9.2/nobuco/addons/torch/util.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1096 2023-08-18 20:14:33.000000 nobuco-0.9.2/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    15886 2023-11-30 23:31:33.000000 nobuco-0.9.2/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.936110 nobuco-0.9.2/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2403 2023-10-04 12:08:06.000000 nobuco-0.9.2/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1994 2023-10-23 13:47:37.000000 nobuco-0.9.2/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-08-06 12:41:35.000000 nobuco-0.9.2/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-10-23 13:46:42.000000 nobuco-0.9.2/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4423 2023-11-30 21:26:35.000000 nobuco-0.9.2/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.936110 nobuco-0.9.2/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14972 2023-10-23 12:31:14.000000 nobuco-0.9.2/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1474 2023-09-29 11:56:47.000000 nobuco-0.9.2/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.936110 nobuco-0.9.2/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5047 2023-10-23 13:50:13.000000 nobuco-0.9.2/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      630 2023-08-06 11:12:41.000000 nobuco-0.9.2/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1113 2023-10-23 13:23:24.000000 nobuco-0.9.2/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.936110 nobuco-0.9.2/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.940110 nobuco-0.9.2/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      227 2023-09-22 08:35:23.000000 nobuco-0.9.2/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     7612 2023-10-18 17:43:52.000000 nobuco-0.9.2/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2249 2023-10-04 12:38:40.000000 nobuco-0.9.2/nobuco/node_converters/attention.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1169 2023-08-06 10:51:45.000000 nobuco-0.9.2/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1192 2023-07-26 14:20:16.000000 nobuco-0.9.2/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3491 2023-11-30 14:36:44.000000 nobuco-0.9.2/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    11449 2023-11-15 20:02:59.000000 nobuco-0.9.2/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1309 2023-07-26 14:39:38.000000 nobuco-0.9.2/nobuco/node_converters/dropout.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1053 2023-10-31 11:09:45.000000 nobuco-0.9.2/nobuco/node_converters/fft.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4500 2023-11-27 21:13:10.000000 nobuco-0.9.2/nobuco/node_converters/grid_sampling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1750 2023-11-30 15:28:41.000000 nobuco-0.9.2/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5182 2023-10-04 12:38:40.000000 nobuco-0.9.2/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11051 2023-10-23 18:52:57.000000 nobuco-0.9.2/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1818 2023-11-30 14:38:10.000000 nobuco-0.9.2/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2909 2023-10-17 11:36:57.000000 nobuco-0.9.2/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-07-01 10:07:17.000000 nobuco-0.9.2/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3894 2023-11-15 13:51:53.000000 nobuco-0.9.2/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     7156 2023-10-31 11:30:52.000000 nobuco-0.9.2/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9721 2023-10-23 13:15:01.000000 nobuco-0.9.2/nobuco/node_converters/reduce.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14671 2023-11-30 15:56:38.000000 nobuco-0.9.2/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1160 2023-11-30 14:27:52.000000 nobuco-0.9.2/nobuco/node_converters/tensor_broadcast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-10-23 12:44:40.000000 nobuco-0.9.2/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12063 2023-11-27 13:48:16.000000 nobuco-0.9.2/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11182 2023-11-30 18:42:37.000000 nobuco-0.9.2/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-07-01 10:07:17.000000 nobuco-0.9.2/nobuco/node_converters/tensor_shape.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2738 2023-11-30 23:07:48.000000 nobuco-0.9.2/nobuco/node_converters/torchvision.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.940110 nobuco-0.9.2/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-10-04 13:56:18.000000 nobuco-0.9.2/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10507 2023-11-30 22:31:57.000000 nobuco-0.9.2/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2778 2023-10-23 12:36:50.000000 nobuco-0.9.2/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.940110 nobuco-0.9.2/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.9.2/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-11-30 23:33:46.940110 nobuco-0.9.2/nobuco.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)    31107 2023-11-30 23:33:46.000000 nobuco-0.9.2/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2050 2023-11-30 23:33:46.000000 nobuco-0.9.2/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-11-30 23:33:46.000000 nobuco-0.9.2/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-11-30 23:33:46.000000 nobuco-0.9.2/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-11-30 23:33:46.000000 nobuco-0.9.2/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      735 2023-11-30 23:32:37.000000 nobuco-0.9.2/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-11-30 23:33:46.940110 nobuco-0.9.2/setup.cfg
```

### Comparing `nobuco-0.9.1/LICENSE` & `nobuco-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/PKG-INFO` & `nobuco-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.9.1/README.md` & `nobuco-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/__init__.py` & `nobuco-0.9.2/nobuco/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 from nobuco.funcs import force_tensorflow_order, force_pytorch_order, shape
 from nobuco.locate.locate import locate_converter
 from nobuco.trace.trace import traceable
 
 from nobuco.converters.node_converter import converter, unregister_converter
 from nobuco.convert import pytorch_to_keras
-from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
+from nobuco.commons import ChannelOrder, ChannelOrderingStrategy, TraceLevel
 
 
 __all__ = [
     pytorch_to_keras,
     converter,
     unregister_converter,
     traceable,
     ChannelOrder,
     ChannelOrderingStrategy,
+    TraceLevel,
     force_tensorflow_order,
     force_pytorch_order,
     shape,
     locate_converter,
     t_pytorch2keras,
     t_keras2pytorch,
 ]
```

### Comparing `nobuco-0.9.1/nobuco/addons/torch/dense_image_warp.py` & `nobuco-0.9.2/nobuco/addons/torch/dense_image_warp.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/addons/torch/depth_to_space.py` & `nobuco-0.9.2/nobuco/addons/torch/depth_to_space.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/addons/torch/space_to_depth.py` & `nobuco-0.9.2/nobuco/addons/torch/space_to_depth.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/commons.py` & `nobuco-0.9.2/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/convert.py` & `nobuco-0.9.2/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/converters/channel_ordering.py` & `nobuco-0.9.2/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/converters/node_converter.py` & `nobuco-0.9.2/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/converters/tensor.py` & `nobuco-0.9.2/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/converters/type_cast.py` & `nobuco-0.9.2/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/converters/validation.py` & `nobuco-0.9.2/nobuco/converters/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,16 +89,19 @@
             raise Exception(f"Tensor shapes of output #{i} don't match: (Pytorch) {list(t_pt.shape)} vs {list(t_tf.shape)} (Tensorflow)")
 
         if t_tf.dtype != t_pt.dtype:
             raise Exception(f"Tensor dtypes don't match: (Pytorch) {t_pt.dtype} vs {t_tf.dtype} (Tensorflow)")
 
     def calc_diff(t1, t2):
         def calc_diff_numerical(t1, t2):
-            nan_mask = torch.isnan(t1) & torch.isnan(t2)
-            diff = t1[~nan_mask] - t2[~nan_mask]
+            t1_nan_mask = torch.isnan(t1)
+            t2_nan_mask = torch.isnan(t2)
+            if not torch.all(torch.eq(t1_nan_mask, t2_nan_mask)):
+                return np.nan
+            diff = t1[~t1_nan_mask] - t2[~t2_nan_mask]
             if diff.numel() == 0:
                 return 0
             else:
                 return diff.abs().max().numpy()
 
         def calc_diff_boolean(t1, t2):
             diff = t1 ^ t2
```

### Comparing `nobuco-0.9.1/nobuco/entity/keras.py` & `nobuco-0.9.2/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/entity/pytorch.py` & `nobuco-0.9.2/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/funcs.py` & `nobuco-0.9.2/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/layers/channel_order.py` & `nobuco-0.9.2/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/layers/container.py` & `nobuco-0.9.2/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/layers/stub.py` & `nobuco-0.9.2/nobuco/layers/stub.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/layers/weight.py` & `nobuco-0.9.2/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/locate/link.py` & `nobuco-0.9.2/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/locate/locate.py` & `nobuco-0.9.2/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/activation.py` & `nobuco-0.9.2/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/attention.py` & `nobuco-0.9.2/nobuco/node_converters/attention.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/boolean.py` & `nobuco-0.9.2/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/boolean_mask.py` & `nobuco-0.9.2/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/comparison.py` & `nobuco-0.9.2/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/convolution.py` & `nobuco-0.9.2/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/dropout.py` & `nobuco-0.9.2/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/fft.py` & `nobuco-0.9.2/nobuco/node_converters/fft.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/grid_sampling.py` & `nobuco-0.9.2/nobuco/node_converters/grid_sampling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/interpolation.py` & `nobuco-0.9.2/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/linear.py` & `nobuco-0.9.2/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/math.py` & `nobuco-0.9.2/nobuco/node_converters/math.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/misc.py` & `nobuco-0.9.2/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/normalization.py` & `nobuco-0.9.2/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/padding.py` & `nobuco-0.9.2/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/pooling.py` & `nobuco-0.9.2/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/recurrent.py` & `nobuco-0.9.2/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/reduce.py` & `nobuco-0.9.2/nobuco/node_converters/reduce.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/slice.py` & `nobuco-0.9.2/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/tensor_broadcast.py` & `nobuco-0.9.2/nobuco/node_converters/tensor_broadcast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/tensor_cast.py` & `nobuco-0.9.2/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/tensor_creation.py` & `nobuco-0.9.2/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.9.2/nobuco/node_converters/tensor_manipulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,43 +212,24 @@
 @converter(torch.Tensor.unbind, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_unbind(self, dim=0):
     def func(self, dim=0):
         return tf.unstack(self, axis=dim)
     return func
 
 
-# @converter(torch.Tensor.flatten, torch.flatten, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
-# def converter_t_flatten(self, start_dim=0, end_dim=-1):
-#     def func(self, start_dim=0, end_dim=-1):
-#         start_shape = self.shape[:start_dim]
-#
-#         n_dims = len(self.shape)
-#         end_dim = _dim_make_positive(end_dim, n_dims)
-#         if end_dim < n_dims-1:
-#             end_shape = self.shape[end_dim+1:]
-#         else:
-#             end_shape = []
-#
-#         return tf.reshape(self, (*start_shape, -1, *end_shape))
-#     return func
-
-
 @converter(torch.Tensor.flatten, torch.flatten, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_t_flatten(self, start_dim=0, end_dim=-1):
     n_dims = self.dim()
     start_dim_pos = _dim_make_positive(start_dim, n_dims)
     end_dim_pos = _dim_make_positive(end_dim, n_dims)
 
     def func(self, start_dim=0, end_dim=-1):
-        start_shape = tf.shape(self)[:start_dim_pos]
-        if end_dim_pos < n_dims-1:
-            end_shape = tf.shape(self)[end_dim_pos+1:]
-        else:
-            end_shape = []
-
+        shape = tf.shape(self)
+        start_shape = shape[:start_dim_pos]
+        end_shape = shape[end_dim_pos+1:]
         return tf.reshape(self, (*start_shape, -1, *end_shape))
     return func
 
 
 @converter(torch.Tensor.narrow, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_narrow(self, dimension, start, length):
     n_dims = self.dim()
@@ -266,28 +247,30 @@
         return x
     return func
 
 
 @converter(torch.squeeze, torch.Tensor.squeeze, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_squeeze(input: Tensor, dim):
     n_dims = input.dim()
+
     def func(input, dim):
         x = input
         if get_channel_order(x) == ChannelOrder.TENSORFLOW:
             perm = perm_keras2pytorch(n_dims)
             x = _permute(perm)(x)
         x = tf.squeeze(x, axis=dim)
         x = set_channel_order(x, ChannelOrder.PYTORCH)
         return x
     return func
 
 
 @converter(torch.unsqueeze, torch.Tensor.unsqueeze, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_unsqueeze(input, dim):
     n_dims = input.dim()
+
     def func(input, dim):
         x = input
         if get_channel_order(x) == ChannelOrder.TENSORFLOW:
             perm = perm_keras2pytorch(n_dims)
             x = _permute(perm)(x)
         x = tf.expand_dims(x, axis=dim)
         x = set_channel_order(x, ChannelOrder.PYTORCH)
```

### Comparing `nobuco-0.9.1/nobuco/trace/tensor_storage.py` & `nobuco-0.9.2/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/trace/trace.py` & `nobuco-0.9.2/nobuco/trace/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,16 @@
     op_tracing_classes = [
         torch,
         torch.Tensor,
         torch.linalg,
         torch.fft,
         torch.nn.functional,
         torchvision.transforms.functional,
+        torchvision.ops,
+        torchvision.ops.boxes,
     ]
 
     op_blacklist = [
         torch.Tensor.__init__,
         torch.Tensor._make_subclass,
     ]
```

### Comparing `nobuco-0.9.1/nobuco/util.py` & `nobuco-0.9.2/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/vis/console_stylizer.py` & `nobuco-0.9.2/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco/vis/html_stylizer.py` & `nobuco-0.9.2/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/nobuco.egg-info/PKG-INFO` & `nobuco-0.9.2/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pytorch to Tensorflow conversion made intuitive
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 Project-URL: Homepage, https://github.com/AlexanderLutsenko/nobuco
 Project-URL: Bug Tracker, https://github.com/AlexanderLutsenko/nobuco/issues
 Keywords: pytorch,tensorflow,keras,converter
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `nobuco-0.9.1/nobuco.egg-info/SOURCES.txt` & `nobuco-0.9.2/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.9.1/pyproject.toml` & `nobuco-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.9.1"
+version = "0.9.2"
 description = "Pytorch to Tensorflow conversion made intuitive"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

