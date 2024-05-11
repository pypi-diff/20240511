# Comparing `tmp/luma-ml-0.7.3.tar.gz` & `tmp/luma-ml-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.7.3.tar", last modified: Tue May  7 20:10:10 2024, max compression
+gzip compressed data, was "luma-ml-0.7.4.tar", last modified: Sat May 11 18:57:26 2024, max compression
```

## Comparing `luma-ml-0.7.3.tar` & `luma-ml-0.7.4.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.377522 luma-ml-0.7.3/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.3/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-07 20:10:10.377108 luma-ml-0.7.3/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-07 20:08:48.000000 luma-ml-0.7.3/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.344821 luma-ml-0.7.3/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    10486 2024-05-07 19:27:37.000000 luma-ml-0.7.3/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.3/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.347799 luma-ml-0.7.3/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.3/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.3/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.3/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.3/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.3/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.3/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.351938 luma-ml-0.7.3/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.3/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.3/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.3/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.3/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.3/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.3/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.353338 luma-ml-0.7.3/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-04-28 07:19:53.000000 luma-ml-0.7.3/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.3/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10856 2024-05-04 18:13:20.000000 luma-ml-0.7.3/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.356246 luma-ml-0.7.3/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.3/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.3/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.3/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.3/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.3/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.357343 luma-ml-0.7.3/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.3/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-28 23:46:05.000000 luma-ml-0.7.3/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    15102 2024-05-06 13:39:46.000000 luma-ml-0.7.3/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.359164 luma-ml-0.7.3/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.3/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.3/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.3/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.3/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.359480 luma-ml-0.7.3/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.3/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.361291 luma-ml-0.7.3/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.3/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.3/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.3/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-05-06 08:57:35.000000 luma-ml-0.7.3/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.363952 luma-ml-0.7.3/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.364697 luma-ml-0.7.3/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    11922 2024-05-07 20:02:13.000000 luma-ml-0.7.3/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9322 2024-05-07 19:26:47.000000 luma-ml-0.7.3/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9429 2024-05-07 19:46:22.000000 luma-ml-0.7.3/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5281 2024-05-07 20:08:02.000000 luma-ml-0.7.3/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1673 2024-04-24 13:56:17.000000 luma-ml-0.7.3/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25499 2024-05-07 20:08:04.000000 luma-ml-0.7.3/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-04 07:19:22.000000 luma-ml-0.7.3/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16051 2024-05-07 20:00:11.000000 luma-ml-0.7.3/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-04-28 05:47:13.000000 luma-ml-0.7.3/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.3/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.364905 luma-ml-0.7.3/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.3/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.366483 luma-ml-0.7.3/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.3/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.3/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.3/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.3/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.369223 luma-ml-0.7.3/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.3/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.3/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.3/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.373034 luma-ml-0.7.3/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.3/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.3/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.3/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.3/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.3/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.3/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.3/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.373688 luma-ml-0.7.3/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.3/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.3/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.374941 luma-ml-0.7.3/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1758 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-07 20:10:10.000000 luma-ml-0.7.3/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-07 20:10:10.377601 luma-ml-0.7.3/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-07 20:09:55.000000 luma-ml-0.7.3/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-07 20:10:10.376270 luma-ml-0.7.3/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.7.3/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.3/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1403 2024-05-07 20:09:50.000000 luma-ml-0.7.3/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.080325 luma-ml-0.7.4/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.7.4/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-11 18:57:26.079932 luma-ml-0.7.4/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4946 2024-05-11 18:56:23.000000 luma-ml-0.7.4/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.045927 luma-ml-0.7.4/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10652 2024-05-11 10:39:04.000000 luma-ml-0.7.4/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.7.4/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.048955 luma-ml-0.7.4/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12302 2024-04-27 19:24:30.000000 luma-ml-0.7.4/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7629 2024-04-21 11:35:40.000000 luma-ml-0.7.4/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-04-21 11:35:39.000000 luma-ml-0.7.4/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8953 2024-04-21 11:35:43.000000 luma-ml-0.7.4/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8887 2024-04-21 11:35:41.000000 luma-ml-0.7.4/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9536 2024-04-21 11:35:42.000000 luma-ml-0.7.4/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.052923 luma-ml-0.7.4/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17291 2024-04-21 11:35:45.000000 luma-ml-0.7.4/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17401 2024-04-21 11:35:47.000000 luma-ml-0.7.4/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7672 2024-04-21 11:35:48.000000 luma-ml-0.7.4/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17695 2024-04-21 11:35:49.000000 luma-ml-0.7.4/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8019 2024-04-21 11:35:50.000000 luma-ml-0.7.4/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11404 2024-04-21 11:35:51.000000 luma-ml-0.7.4/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.054747 luma-ml-0.7.4/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5923 2024-05-08 18:17:58.000000 luma-ml-0.7.4/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      394 2024-04-28 05:47:04.000000 luma-ml-0.7.4/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10856 2024-05-04 18:13:20.000000 luma-ml-0.7.4/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.058061 luma-ml-0.7.4/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9749 2024-04-21 11:35:52.000000 luma-ml-0.7.4/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19258 2024-04-21 11:35:53.000000 luma-ml-0.7.4/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9633 2024-04-21 11:35:54.000000 luma-ml-0.7.4/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13550 2024-04-21 11:35:55.000000 luma-ml-0.7.4/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6513 2024-04-21 11:35:56.000000 luma-ml-0.7.4/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.058895 luma-ml-0.7.4/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.7.4/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4881 2024-04-28 23:46:05.000000 luma-ml-0.7.4/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    15102 2024-05-09 18:36:55.000000 luma-ml-0.7.4/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.060220 luma-ml-0.7.4/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.7.4/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5821 2024-04-24 15:56:48.000000 luma-ml-0.7.4/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-04-24 15:55:30.000000 luma-ml-0.7.4/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-04-24 15:57:32.000000 luma-ml-0.7.4/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.060552 luma-ml-0.7.4/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.7.4/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.062524 luma-ml-0.7.4/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3269 2024-04-21 11:36:03.000000 luma-ml-0.7.4/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7681 2024-04-21 11:36:04.000000 luma-ml-0.7.4/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11846 2024-04-21 11:36:05.000000 luma-ml-0.7.4/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5221 2024-05-06 08:57:35.000000 luma-ml-0.7.4/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.065019 luma-ml-0.7.4/luma/neural/
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.066290 luma-ml-0.7.4/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12134 2024-05-08 08:37:55.000000 luma-ml-0.7.4/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9602 2024-05-08 08:37:55.000000 luma-ml-0.7.4/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10380 2024-05-11 18:52:50.000000 luma-ml-0.7.4/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14491 2024-05-11 16:08:23.000000 luma-ml-0.7.4/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.7.4/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    58664 2024-05-11 18:57:22.000000 luma-ml-0.7.4/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-04 07:19:22.000000 luma-ml-0.7.4/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16567 2024-05-11 18:54:02.000000 luma-ml-0.7.4/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.7.4/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8210 2024-04-21 11:36:12.000000 luma-ml-0.7.4/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.067296 luma-ml-0.7.4/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7219 2024-04-21 11:36:13.000000 luma-ml-0.7.4/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.069305 luma-ml-0.7.4/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.7.4/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.7.4/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3602 2024-04-21 11:36:16.000000 luma-ml-0.7.4/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2555 2024-04-21 11:36:18.000000 luma-ml-0.7.4/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.071305 luma-ml-0.7.4/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18479 2024-04-21 11:36:19.000000 luma-ml-0.7.4/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39141 2024-04-21 11:36:22.000000 luma-ml-0.7.4/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16204 2024-04-21 11:36:23.000000 luma-ml-0.7.4/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.075514 luma-ml-0.7.4/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19093 2024-04-21 11:36:25.000000 luma-ml-0.7.4/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12211 2024-04-21 11:36:26.000000 luma-ml-0.7.4/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6638 2024-04-21 11:36:27.000000 luma-ml-0.7.4/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2962 2024-04-21 11:36:28.000000 luma-ml-0.7.4/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10680 2024-04-21 11:36:29.000000 luma-ml-0.7.4/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7519 2024-04-21 11:36:30.000000 luma-ml-0.7.4/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7189 2024-04-21 11:36:31.000000 luma-ml-0.7.4/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.076191 luma-ml-0.7.4/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.7.4/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24473 2024-04-21 11:36:32.000000 luma-ml-0.7.4/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.077640 luma-ml-0.7.4/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5552 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1758 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-11 18:57:25.000000 luma-ml-0.7.4/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-11 18:57:26.080462 luma-ml-0.7.4/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-11 18:56:10.000000 luma-ml-0.7.4/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-11 18:57:26.079087 luma-ml-0.7.4/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.7.4/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-04-20 19:16:53.000000 luma-ml-0.7.4/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      253 2024-05-11 18:51:25.000000 luma-ml-0.7.4/test/__test.py
```

### Comparing `luma-ml-0.7.3/LICENSE` & `luma-ml-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/PKG-INFO` & `luma-ml-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.41k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.49k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.3</td>
+                    <td>0.7.4</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~18K</td>
+                    <td>~20K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.3 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.4 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.41k-red][GitHub code size in bytes][Code Style]
+5.49k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.3
-Lines of Code  ~18K
+Latest Version 0.7.4
+Lines of Code  ~20K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.3/README.md` & `luma-ml-0.7.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.41k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.49k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -89,19 +89,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.3</td>
+                    <td>0.7.4</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~18K</td>
+                    <td>~20K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.41k-red][GitHub code size in bytes][Code Style]
+5.49k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.3
-Lines of Code  ~18K
+Latest Version 0.7.4
+Lines of Code  ~20K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.3/luma/__import__.py` & `luma-ml-0.7.4/luma/__import__.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,20 +70,25 @@
 from luma.ensemble.boost import AdaBoostClassifier, AdaBoostRegressor
 from luma.ensemble.boost import GradientBoostingClassifier, GradientBoostingRegressor
 from luma.ensemble.stack import StackingClassifier, StackingRegressor
 
 from luma.neural.base import Layer, Loss, Initializer, NeuralModel
 from luma.neural.single import PerceptronClassifier, PerceptronRegressor
 from luma.neural.layer import (
-    Convolution,
-    Pooling,
+    Convolution1D,
+    Convolution2D,
+    Convolution3D,
+    Pooling1D,
+    Pooling2D,
+    Pooling3D,
     Dense,
     Dropout,
     Flatten,
     Activation,
+    BatchNorm2D,
     Sequential,
 )
 from luma.neural.optimizer import (
     SGDOptimizer,
     MomentumOptimizer,
     RMSPropOptimizer,
     AdamOptimizer,
@@ -91,15 +96,15 @@
     AdaDeltaOptimizer,
     AdaMaxOptimizer,
     AdamWOptimizer,
     NAdamOptimizer,
 )
 from luma.neural.loss import CrossEntropy, BinaryCrossEntropy, MSELoss
 from luma.neural.init import KaimingInit, XavierInit
-from luma.neural.block import ConvBlock, DenseBlock
+from luma.neural.block import ConvBlock2D, DenseBlock
 from luma.neural.network import SimpleMLP, SimpleCNN
 from luma.neural.network import LeNet_1, LeNet_4
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
@@ -240,22 +245,23 @@
 
     SGDOptimizer, MomentumOptimizer, RMSPropOptimizer,
     AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
     AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
     Layer, Loss, Initializer, NeuralModel
 
-    Convolution, Pooling, Dense, Dropout, Flatten, Activation,
-    Sequential
+    Convolution1D, Convolution2D, Convolution3D,
+    Pooling1D, Pooling2D, Pooling3D,
+    Dense, Dropout, Flatten, Activation, BatchNorm2D, Sequential
 
     CrossEntropy, BinaryCrossEntropy, MSELoss
 
     KaimingInit, XavierInit
 
-    ConvBlock, DenseBlock
+    ConvBlock2D, DenseBlock
 
     SimpleMLP, SimpleCNN, LeNet_1, LeNet_4
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
```

### Comparing `luma-ml-0.7.3/luma/__init__.py` & `luma-ml-0.7.4/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/classifier/discriminant.py` & `luma-ml-0.7.4/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/classifier/logistic.py` & `luma-ml-0.7.4/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/classifier/naive_bayes.py` & `luma-ml-0.7.4/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/classifier/neighbors.py` & `luma-ml-0.7.4/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/classifier/svm.py` & `luma-ml-0.7.4/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/classifier/tree.py` & `luma-ml-0.7.4/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/clustering/affinity.py` & `luma-ml-0.7.4/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/clustering/density.py` & `luma-ml-0.7.4/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/clustering/hierarchy.py` & `luma-ml-0.7.4/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/clustering/kmeans.py` & `luma-ml-0.7.4/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/clustering/mixture.py` & `luma-ml-0.7.4/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/clustering/spectral.py` & `luma-ml-0.7.4/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/core/base.py` & `luma-ml-0.7.4/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/core/super.py` & `luma-ml-0.7.4/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/ensemble/bagging.py` & `luma-ml-0.7.4/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/ensemble/boost.py` & `luma-ml-0.7.4/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/ensemble/forest.py` & `luma-ml-0.7.4/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/ensemble/stack.py` & `luma-ml-0.7.4/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/ensemble/vote.py` & `luma-ml-0.7.4/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/interface/exception.py` & `luma-ml-0.7.4/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/interface/typing.py` & `luma-ml-0.7.4/luma/interface/typing.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/interface/util.py` & `luma-ml-0.7.4/luma/interface/util.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/metric/classification.py` & `luma-ml-0.7.4/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/metric/clustering.py` & `luma-ml-0.7.4/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/metric/distance.py` & `luma-ml-0.7.4/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/metric/regression.py` & `luma-ml-0.7.4/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/migrate/port.py` & `luma-ml-0.7.4/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/model_selection/cv.py` & `luma-ml-0.7.4/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/model_selection/fold.py` & `luma-ml-0.7.4/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/model_selection/search.py` & `luma-ml-0.7.4/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/model_selection/split.py` & `luma-ml-0.7.4/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/neural/_models/_lenet.py` & `luma-ml-0.7.4/luma/neural/_models/_lenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
 from luma.interface.util import Clone, InitUtil
 from luma.metric.classification import Accuracy
 
 from luma.neural.base import Loss, NeuralModel
-from luma.neural.block import ConvBlock, DenseBlock
+from luma.neural.block import ConvBlock2D, DenseBlock
 from luma.neural.layer import Activation, Dense, Flatten, Sequential
 from luma.neural.loss import CrossEntropy
 
 
 __all__ = ("_LeNet_1", "_LeNet_4", "_LeNet_5")
 
 
@@ -75,37 +75,39 @@
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += ConvBlock(
+        self.model += ConvBlock2D(
             1,
             4,
             filter_size=5,
             stride=1,
             activation=Clone(self.activation).get,
             initializer=self.initializer,
             padding="valid",
             lambda_=self.lambda_,
+            do_batch_norm=False,
             pool_filter_size=2,
             pool_stride=2,
             pool_mode="avg",
             random_state=self.random_state,
         )
-        self.model += ConvBlock(
+        self.model += ConvBlock2D(
             4,
             8,
             filter_size=5,
             stride=1,
             activation=Clone(self.activation).get,
             initializer=self.initializer,
             padding="valid",
             lambda_=self.lambda_,
+            do_batch_norm=False,
             pool_filter_size=2,
             pool_stride=2,
             pool_mode="avg",
             random_state=self.random_state,
         )
 
         self.model += Flatten()
@@ -197,37 +199,39 @@
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += ConvBlock(
+        self.model += ConvBlock2D(
             1,
             4,
             filter_size=5,
             stride=1,
             activation=Clone(self.activation).get,
             initializer=self.initializer,
             padding="valid",
             lambda_=self.lambda_,
+            do_batch_norm=False,
             pool_filter_size=2,
             pool_stride=2,
             pool_mode="avg",
             random_state=self.random_state,
         )
-        self.model += ConvBlock(
+        self.model += ConvBlock2D(
             4,
             16,
             filter_size=5,
             stride=1,
             activation=Clone(self.activation).get,
             initializer=self.initializer,
             padding="valid",
             lambda_=self.lambda_,
+            do_batch_norm=False,
             pool_filter_size=2,
             pool_stride=2,
             pool_mode="avg",
             random_state=self.random_state,
         )
 
         self.model += Flatten()
@@ -327,37 +331,39 @@
                 "patience": (f"0<,+inf", int),
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
-        self.model += ConvBlock(
+        self.model += ConvBlock2D(
             1,
             6,
             filter_size=5,
             stride=1,
             activation=Clone(self.activation).get,
             initializer=self.initializer,
             padding="valid",
             lambda_=self.lambda_,
+            do_batch_norm=False,
             pool_filter_size=2,
             pool_stride=2,
             pool_mode="avg",
             random_state=self.random_state,
         )
-        self.model += ConvBlock(
+        self.model += ConvBlock2D(
             6,
             16,
             filter_size=5,
             stride=1,
             activation=Clone(self.activation).get,
             initializer=self.initializer,
             padding="valid",
             lambda_=self.lambda_,
+            do_batch_norm=False,
             pool_filter_size=2,
             pool_stride=2,
             pool_mode="avg",
             random_state=self.random_state,
         )
 
         self.model += Flatten()
```

### Comparing `luma-ml-0.7.3/luma/neural/_models/_simple.py` & `luma-ml-0.7.4/luma/neural/_models/_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Literal, Self, override
 
 from luma.core.super import Estimator, Evaluator, Optimizer, Supervised
 from luma.interface.typing import Matrix, Tensor, Vector
 from luma.interface.util import Clone, InitUtil
 
 from luma.neural.base import Loss, NeuralModel
-from luma.neural.block import ConvBlock, DenseBlock
+from luma.neural.block import ConvBlock2D, DenseBlock
 from luma.neural.layer import Activation, Dense, Dropout, Flatten, Sequential
 
 
 __all__ = ("_SimpleMLP", "_SimpleCNN")
 
 
 class _SimpleMLP(Estimator, Supervised, NeuralModel):
@@ -129,14 +129,16 @@
         *,
         activation: Activation.FuncType,
         optimizer: Optimizer,
         loss: Loss,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
+        do_batch_norm: bool = True,
+        momentum: float = 0.9,
         do_pooling: bool = True,
         pool_filter_size: int = 2,
         pool_stride: int = 2,
         pool_mode: Literal["max", "avg"] = "max",
         do_dropout: bool = True,
         dropout_rate: float = 0.5,
         batch_size: int = 100,
@@ -157,14 +159,16 @@
         self.filter_size = filter_size
         self.activation = activation
         self.optimizer = optimizer
         self.loss = loss
         self.initializer = initializer
         self.padding = padding
         self.stride = stride
+        self.do_batch_norm = do_batch_norm
+        self.momentum = momentum
         self.do_pooling = do_pooling
         self.pool_filter_size = pool_filter_size
         self.pool_stride = pool_stride
         self.pool_mode = pool_mode
         self.do_dropout = do_dropout
         self.dropout_rate = dropout_rate
         self.lambda_ = lambda_
@@ -202,14 +206,15 @@
 
         self.set_param_ranges(
             {
                 "out_channels": ("0<,+inf", int),
                 "out_features": ("0<,+inf", int),
                 "filter_size": ("0<,+inf", int),
                 "stride": ("0<,+inf", int),
+                "momentum": ("0,1", None),
                 "pool_filter_size": ("0<,+inf", int),
                 "pool_stride": ("0<,+inf", int),
                 "dropout_rate": ("0,1", None),
                 "batch_size": ("0<,+inf", int),
                 "n_epochs": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "valid_size": ("0<,<1", None),
@@ -219,23 +224,25 @@
             }
         )
         self.check_param_ranges()
         self._build_model()
 
     def _build_model(self) -> None:
         for in_, out_ in self.feature_shapes_[0]:
-            self.model += ConvBlock(
+            self.model += ConvBlock2D(
                 in_,
                 out_,
                 self.filter_size,
                 activation=Clone(self.activation).get,
                 initializer=self.initializer,
                 padding=self.padding,
                 stride=self.stride,
                 lambda_=self.lambda_,
+                do_batch_norm=self.do_batch_norm,
+                momentum=self.momentum,
                 do_pooling=self.do_pooling,
                 pool_filter_size=self.pool_filter_size,
                 pool_stride=self.pool_stride,
                 pool_mode=self.pool_mode,
                 random_state=self.random_state,
             )
```

### Comparing `luma-ml-0.7.3/luma/neural/base.py` & `luma-ml-0.7.4/luma/neural/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Self, Tuple
+from typing import Self
 import numpy as np
 
 from luma.core.base import ModelBase, NeuralBase
 from luma.core.super import Evaluator
 
 from luma.interface.exception import NotFittedError
 from luma.interface.typing import Matrix, Tensor, TensorLike
@@ -49,15 +49,14 @@
         self.biases_: TensorLike = None
 
         self.dX: TensorLike = None
         self.dW: TensorLike = None
         self.dB: TensorLike = None
 
         self.optimizer: object = None
-        self.out_shape: tuple = None
 
     @abstractmethod
     def forward(self, X: TensorLike, is_train: bool = False) -> TensorLike: ...
 
     @abstractmethod
     def backward(self, d_out: TensorLike) -> TensorLike: ...
 
@@ -72,46 +71,47 @@
 
     def init_params(self, w_shape: tuple, b_shape: tuple) -> None:
         init_type_: type = InitUtil(self.initializer).initializer_type
 
         if init_type_ is None:
             self.weights_ = 0.01 * self.rs_.randn(*w_shape)
         else:
-            if len(w_shape) == 2:
-                self.weights_ = init_type_(self.random_state).init_2d(*w_shape)
-            elif len(w_shape) == 4:
-                self.weights_ = init_type_(self.random_state).init_4d(*w_shape)
-            else:
-                NotImplemented
+            self.weights_ = init_type_(self.random_state).init_nd(*w_shape)
 
         self.biases_: TensorLike = np.zeros(b_shape)
 
     @property
-    def param_size(self) -> Tuple[int, int]:
+    def param_size(self) -> tuple[int, int]:
         w_size, b_size = 0, 0
+        w_list: list | list[TensorLike] = []
+        b_list: list | list[TensorLike] = []
+
         if self.weights_ is not None:
-            w_size += len(self.weights_.flatten())
+            w_list.extend(self.weights_)
+            for w in w_list:
+                w_size += len(w.flatten())
         if self.biases_ is not None:
-            b_size += len(self.biases_.flatten())
+            b_list.extend(self.biases_)
+            for b in b_list:
+                b_size += len(b.flatten())
 
         return w_size, b_size
 
+    @abstractmethod
+    def out_shape(self, in_shape: tuple[int]) -> tuple[int]: ...
+
     def __call__(self, X: TensorLike, is_train: bool = False) -> TensorLike:
         return self.forward(X, is_train=is_train)
 
     def __str__(self) -> str:
         return type(self).__name__
 
     def __repr__(self) -> str:
         w_size, b_size = self.param_size
-        return (
-            f"{type(self).__name__}: "
-            + f"({w_size:,} weights, {b_size:,} biases)"
-            + f" -> {w_size + b_size:,} params"
-        )
+        return f"{type(self).__name__}({w_size + b_size} params)"
 
 
 class Loss(ABC):
     """
     An internal class for loss functions used in neural networks.
 
     Loss functions, integral to the training process of machine
@@ -148,18 +148,15 @@
     def __init__(self, random_state: int) -> None:
         self.rs_ = np.random.RandomState(random_state)
 
     @classmethod
     def __class_alias__(cls) -> None: ...
 
     @abstractmethod
-    def init_2d(self) -> Matrix: ...
-
-    @abstractmethod
-    def init_4d(self) -> Tensor: ...
+    def init_nd(self) -> TensorLike: ...
 
 
 class NeuralModel(ABC, NeuralBase):
     """
     Neural networks are computational models inspired by the human brain,
     consisting of layers of interconnected nodes (neurons) that process
     information through weighted connections. These models include an input
@@ -288,9 +285,43 @@
         ):
             out = self.model(X_batch, is_train=False)
             loss = self.loss.loss(y_batch, out)
             valid_loss.append(loss)
 
         return valid_loss
 
+    @property
+    def param_size(self) -> tuple[int, int]:
+        return self.model.param_size
+
+    def summarize(self, in_shape: tuple[int]) -> None:
+        title = f"Summary of '{str(self)}'"
+        print(f"{title:^83}")
+        print("-" * 83)
+        print(
+            "{:<20} {:<20} {:<20} {:<20}".format(
+                "Name", "Layer/Block", "Output Shape", "Weights, Biases"
+            )
+        )
+        print("=" * 83)
+
+        n_layers = 0
+        w_size, b_size = self.param_size
+        for name, layer in self.model:
+            n_layers += 1
+            print(
+                f"{name:<20}",
+                f"{str(layer):<20}",
+                f"{str(layer.out_shape(in_shape)):<20}",
+                f"{str(layer.param_size):<20}",
+            )
+            in_shape = layer.out_shape(in_shape)
+        print("=" * 83)
+        print(f"Total Layers: {n_layers}")
+        print(
+            f"Total Parameters: ({w_size:,} weights, {b_size:,} biases)",
+            f"-> {w_size + b_size:,} params",
+        )
+        print("-" * 83)
+
     def __str__(self) -> str:
         return type(self).__name__
```

### Comparing `luma-ml-0.7.3/luma/neural/init.py` & `luma-ml-0.7.4/luma/neural/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from luma.interface.typing import Matrix, Tensor
+from luma.interface.typing import Vector, Matrix, Tensor, TensorLike
 
 
 __all__ = ("KaimingInit", "XavierInit")
 
 
 class Initializer:
     @classmethod
@@ -12,50 +12,44 @@
 
 
 class KaimingInit(Initializer):
     def __init__(self, random_state: int = None) -> None:
         super().__init__()
         self.rs_ = np.random.RandomState(random_state)
 
-    def init_2d(self, input_size: int, output_size: int) -> Matrix:
-        stddev = np.sqrt(2.0 / input_size)
+    def init_nd(
+        self,
+        input_size: int,
+        output_size: int,
+        *shape: int,
+    ) -> TensorLike:
+        stddev = np.sqrt(2.0 / (input_size * np.prod(Vector(shape))))
         return self.rs_.normal(
             0.0,
             stddev,
-            (input_size, output_size),
-        )
-
-    def init_4d(
-        self, input_size: int, output_size: int, height: int, width: int
-    ) -> Tensor:
-        stddev = np.sqrt(2.0 / (input_size * height * width))
-        return self.rs_.normal(
-            0.0,
-            stddev,
-            (input_size, output_size, height, width),
+            (input_size, output_size, *shape),
         )
 
 
 class XavierInit(Initializer):
     def __init__(self, random_state: int = None) -> None:
         super().__init__()
         self.rs_ = np.random.RandomState(random_state)
 
-    def init_2d(self, input_size: int, output_size: int) -> Matrix:
-        stddev = np.sqrt(2.0 / (input_size + output_size))
-        return self.rs_.normal(
-            0.0,
-            stddev,
-            (input_size, output_size),
-        )
-
-    def init_4d(
-        self, input_size: int, output_size: int, height: int, width: int
-    ) -> Tensor:
+    def init_nd(
+        self,
+        input_size: int,
+        output_size: int,
+        *shape: int,
+    ) -> TensorLike:
         stddev = np.sqrt(
-            2.0 / (input_size * height * width + output_size * height * width)
+            2.0
+            / (
+                input_size * np.prod(Vector(shape))
+                + output_size * np.prod(Vector(shape))
+            )
         )
         return self.rs_.normal(
             0.0,
             stddev,
-            (input_size, output_size, height, width),
+            (input_size, output_size, *shape),
         )
```

### Comparing `luma-ml-0.7.3/luma/neural/loss.py` & `luma-ml-0.7.4/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/neural/network.py` & `luma-ml-0.7.4/luma/neural/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,29 +121,31 @@
     These networks typically include layers such as convolutional layers,
     pooling layers, and fully connected layers that help in reducing the
     dimensions while retaining important features.
 
     Structure
     ---------
     ```py
-    ConvBlock -> ... -> Flatten -> DenseBlock -> ... -> Dense
+    ConvBlock2D -> ... -> Flatten -> DenseBlock -> ... -> Dense
     ```
     Parameters
     ----------
     `in_channels_list` : List of input channels for convolutional blocks
     `in_features_list` : List of input features for dense blocks
     `out_channels` : Output channels for the last convolutional layer
     `out_features` : Output features for the last dense layer
     `filter_size` : Size of filters for convolution layers
     `activation` : Type of activation function
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function
     `initializer` : Type of weight initializer (`None` for dense layers)
     `padding` : Padding strategy (default `same`)
     `stride` : Step size of filters during convolution
+    `do_batch_norm` : Whether to perform batch normalization (default `True`)
+    `momentum` : Momentum for batch normalization
     `do_pooling` : Whether to perform pooling
     `pool_filter_size` : Size of filters for pooling layers
     `pool_stride` : Step size of filters during pooling
     `pool_mode` : Pooling strategy (default `max`)
     `do_dropout` : Whether to perform dropout
     `dropout_rate` : Dropout rate
     `batch_size` : Size of a single mini-batch
@@ -206,14 +208,16 @@
         *,
         activation: Activation,
         optimizer: Optimizer,
         loss: Loss,
         initializer: InitUtil.InitStr = None,
         padding: Literal["same", "valid"] = "same",
         stride: int = 1,
+        do_batch_norm: bool = True,
+        momentum: float = 0.9,
         do_pooling: bool = True,
         pool_filter_size: int = 2,
         pool_stride: int = 2,
         pool_mode: Literal["max", "avg"] = "max",
         do_dropout: bool = True,
         dropout_rate: float = 0.5,
         batch_size: int = 100,
@@ -235,14 +239,16 @@
             filter_size,
             activation,
             optimizer,
             loss,
             initializer,
             padding,
             stride,
+            do_batch_norm,
+            momentum,
             do_pooling,
             pool_filter_size,
             pool_stride,
             pool_mode,
             do_dropout,
             dropout_rate,
             batch_size,
@@ -274,24 +280,28 @@
     ---------
     Input:
     ```py
     Tensor[..., 1, 28, 28]
     ```
     Convolution Layers:
     ```py
-    ConvBlock(1, 4) -> ConvBlock(4, 8)
+    ConvBlock2D(1, 4) -> ConvBlock2D(4, 8)
     ```
     Fully Connected Layers:
     ```py
     Flatten -> Dense(8 * 4 * 4, 10)
     ```
     Output:
     ```py
     Matrix[..., 10]
     ```
+    Parameter Size:
+    ```txt
+    2,180 weights, 22 biases -> 2,202 params
+    ```
     Parameters
     ----------
     `activation` : Type of activation function (Default `Tanh`)
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function (Default `CrossEntropy`)
     `initializer` : Type of weight initializer (`None` for dense layers)
     `batch_size` : Size of a single mini-batch
@@ -357,24 +367,28 @@
     ---------
     Input:
     ```py
     Tensor[..., 1, 32, 32]
     ```
     Convolution Layers:
     ```py
-    ConvBlock(1, 4) -> ConvBlock(4, 16)
+    ConvBlock2D(1, 4) -> ConvBlock2D(4, 16)
     ```
     Fully Connected Layers:
     ```py
     Flatten -> DenseBlock(16 * 5 * 5, 120) -> Dense(10)
     ```
     Output:
     ```py
     Matrix[..., 10]
     ```
+    Parameter Size:
+    ```txt
+    50,902 weights, 150 biases -> 51,052 params
+    ```
     Parameters
     ----------
     `activation` : Type of activation function (Default `Tanh`)
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function (Default `CrossEntropy`)
     `initializer` : Type of weight initializer (`None` for dense layers)
     `batch_size` : Size of a single mini-batch
@@ -441,25 +455,29 @@
     ---------
     Input:
     ```py
     Tensor[..., 1, 32, 32]
     ```
     Convolution Layers:
     ```py
-    ConvBlock(1, 6) -> ConvBlock(6, 16)
+    ConvBlock2D(1, 6) -> ConvBlock2D(6, 16)
     ```
     Fully Connected Layers:
     ```py
     Flatten ->
     DenseBlock(16 * 5 * 5, 120) -> DenseBlock(120, 84) -> Dense(84, 10)
     ```
     Output:
     ```py
     Matrix[..., 10]
     ```
+    Parameter Size:
+    ```txt
+    61,474 weights, 236 biases -> 61,710 params
+    ```
     Parameters
     ----------
     `activation` : Type of activation function (Default `Tanh`)
     `optimizer` : Type of optimizer for weight update
     `loss` : Type of loss function (Default `CrossEntropy`)
     `initializer` : Type of weight initializer (`None` for dense layers)
     `batch_size` : Size of a single mini-batch
```

### Comparing `luma-ml-0.7.3/luma/neural/optimizer.py` & `luma-ml-0.7.4/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/neural/single.py` & `luma-ml-0.7.4/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/pipe/pipeline.py` & `luma-ml-0.7.4/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/preprocessing/encoder.py` & `luma-ml-0.7.4/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/preprocessing/imputer.py` & `luma-ml-0.7.4/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/preprocessing/outlier.py` & `luma-ml-0.7.4/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/preprocessing/scaler.py` & `luma-ml-0.7.4/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/reduction/linear.py` & `luma-ml-0.7.4/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/reduction/manifold.py` & `luma-ml-0.7.4/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/reduction/selection.py` & `luma-ml-0.7.4/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/general.py` & `luma-ml-0.7.4/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/linear.py` & `luma-ml-0.7.4/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/neighbors.py` & `luma-ml-0.7.4/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/poly.py` & `luma-ml-0.7.4/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/robust.py` & `luma-ml-0.7.4/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/svm.py` & `luma-ml-0.7.4/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/regressor/tree.py` & `luma-ml-0.7.4/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/visual/eda.py` & `luma-ml-0.7.4/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma/visual/evaluation.py` & `luma-ml-0.7.4/luma/visual/evaluation.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.7.4/luma_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.7.3
+Version: 0.7.4
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-5.41k-red">
+        <img src="https://img.shields.io/badge/total downloads-5.49k-red">
         <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
@@ -108,19 +108,19 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.7.3</td>
+                    <td>0.7.4</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~18K</td>
+                    <td>~20K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.7.3 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.7.4 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
 Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-5.41k-red][GitHub code size in bytes][Code Style]
+5.49k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -33,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.7.3
-Lines of Code  ~18K
+Latest Version 0.7.4
+Lines of Code  ~20K
 Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.7.3/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.7.4/luma_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luma-ml-0.7.3/setup.py` & `luma-ml-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.7.3",
+    version="0.7.4",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
```

### Comparing `luma-ml-0.7.3/test/__act.py` & `luma-ml-0.7.4/test/__act.py`

 * *Files identical despite different names*

