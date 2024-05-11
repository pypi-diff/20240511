# Comparing `tmp/exoml-0.1.8.tar.gz` & `tmp/exoml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoml-0.1.8.tar", last modified: Fri May  3 19:29:43 2024, max compression
+gzip compressed data, was "exoml-0.1.9.tar", last modified: Tue May  7 17:27:07 2024, max compression
```

## Comparing `exoml-0.1.8.tar` & `exoml-0.1.9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 19:29:43.872556 exoml-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 19:29:20.000000 exoml-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.856556 exoml-0.1.8/exoml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.856556 exoml-0.1.8/exoml/curve_prioritizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/curve_prioritizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/curve_prioritizer/curve_prioritizer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/curve_prioritizer/curve_prioritizer_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.856556 exoml-0.1.8/exoml/detrend/
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/detrend/DETREND.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/detrend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/detrend/detrend_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.856556 exoml-0.1.8/exoml/ete6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ete6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ete6/ete6_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.860556 exoml-0.1.8/exoml/iatson/
--rwxr-xr-x   0 runner    (1001) docker     (127)    23093 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/IATSON.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24283 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/IATSON_og.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    86662 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/IATSON_planet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/iatson_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/iatson_og_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/iatson_planet_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/iatson/watson_planet_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.860556 exoml-0.1.8/exoml/ml/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.860556 exoml-0.1.8/exoml/ml/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/calibration/calibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/calibration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.864556 exoml-0.1.8/exoml/ml/callback/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/basemodel_aware_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/batch_aware_csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/get_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/learning_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/callback/training_data_aware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.864556 exoml-0.1.8/exoml/ml/encoding/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/encoding/time_position.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.864556 exoml-0.1.8/exoml/ml/functions/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/functions/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.864556 exoml-0.1.8/exoml/ml/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/layers/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/layers/transformer_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.864556 exoml-0.1.8/exoml/ml/learning_rate/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/learning_rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/learning_rate/schedulers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.864556 exoml-0.1.8/exoml/ml/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/log/get_weights_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/log/with_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.868556 exoml-0.1.8/exoml/ml/loss/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/loss/cross_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/loss/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.868556 exoml-0.1.8/exoml/ml/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/metrics/auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/metrics/fixed_mean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/ml_data_generator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5180 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/ml_single_transits_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.868556 exoml-0.1.8/exoml/ml/model/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42083 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/model/binary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/model/categorical_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/model/imbalanced_binary_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/model/imbalanced_categorical_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.868556 exoml-0.1.8/exoml/ml/physics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/physics/transit_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/ml/thread_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/exoml/preparation/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/preparation/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18135 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/preparation/empty_targets_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/preparation/ete6parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/preparation/parser_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/preparation/q1q17dr25parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/exoml/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:20.000000 exoml-0.1.8/exoml/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/exoml/resources/q1_q17/
--rwxr-xr-x   0 runner    (1001) docker     (127)   114514 2024-05-03 19:29:29.000000 exoml-0.1.8/exoml/resources/q1_q17/apjac4399t13_mrt.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/exoml/santo/
--rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-05-03 19:29:30.000000 exoml-0.1.8/exoml/santo/SANTO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:30.000000 exoml-0.1.8/exoml/santo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-03 19:29:30.000000 exoml-0.1.8/exoml/santo/santo_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-03 19:29:30.000000 exoml-0.1.8/exoml/santo/santo_test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/exoml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:30.000000 exoml-0.1.8/exoml/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      215 2024-05-03 19:29:30.000000 exoml-0.1.8/exoml/tests/test_exoml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/exoml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 19:29:43.000000 exoml-0.1.8/exoml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-03 19:29:43.000000 exoml-0.1.8/exoml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 19:29:43.000000 exoml-0.1.8/exoml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-03 19:29:43.000000 exoml-0.1.8/exoml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-03 19:29:43.000000 exoml-0.1.8/exoml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-03 19:29:30.000000 exoml-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 19:29:30.000000 exoml-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 19:29:43.872556 exoml-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:43.872556 exoml-0.1.8/transpot/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11057 2024-05-03 19:29:30.000000 exoml-0.1.8/transpot/TRANSPOT.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 19:29:30.000000 exoml-0.1.8/transpot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-03 19:29:30.000000 exoml-0.1.8/transpot/transpot_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.406688 exoml-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-07 17:27:07.406688 exoml-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 17:26:44.000000 exoml-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.390688 exoml-0.1.9/exoml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.390688 exoml-0.1.9/exoml/curve_prioritizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/curve_prioritizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/curve_prioritizer/curve_prioritizer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/curve_prioritizer/curve_prioritizer_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.390688 exoml-0.1.9/exoml/detrend/
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/detrend/DETREND.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/detrend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/detrend/detrend_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.390688 exoml-0.1.9/exoml/ete6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ete6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14866 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ete6/ete6_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.394688 exoml-0.1.9/exoml/iatson/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23093 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/IATSON.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24283 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/IATSON_og.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    86662 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/IATSON_planet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/iatson_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/iatson_og_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46616 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/iatson_planet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29748 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/iatson/watson_planet_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.394688 exoml-0.1.9/exoml/ml/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.394688 exoml-0.1.9/exoml/ml/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/calibration/calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/calibration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/callback/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/basemodel_aware_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/batch_aware_csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/get_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/learning_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/callback/training_data_aware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/encoding/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/encoding/time_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/functions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/functions/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/layers/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/layers/transformer_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/learning_rate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/learning_rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/learning_rate/schedulers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/log/get_weights_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/log/with_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.398688 exoml-0.1.9/exoml/ml/loss/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/loss/cross_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/loss/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.402688 exoml-0.1.9/exoml/ml/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/metrics/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/metrics/fixed_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3703 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/ml_data_generator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5180 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/ml_single_transits_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.402688 exoml-0.1.9/exoml/ml/model/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42083 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/model/binary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/model/categorical_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/model/imbalanced_binary_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/model/imbalanced_categorical_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.402688 exoml-0.1.9/exoml/ml/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/physics/transit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/ml/thread_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.402688 exoml-0.1.9/exoml/preparation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/preparation/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18135 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/preparation/empty_targets_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/preparation/ete6parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31695 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/preparation/parser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27267 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/preparation/q1q17dr25parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.402688 exoml-0.1.9/exoml/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:44.000000 exoml-0.1.9/exoml/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.402688 exoml-0.1.9/exoml/resources/q1_q17/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   114514 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/resources/q1_q17/apjac4399t13_mrt.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.406688 exoml-0.1.9/exoml/santo/
+-rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/santo/SANTO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/santo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/santo/santo_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/santo/santo_test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.406688 exoml-0.1.9/exoml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      215 2024-05-07 17:26:53.000000 exoml-0.1.9/exoml/tests/test_exoml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.406688 exoml-0.1.9/exoml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-07 17:27:07.000000 exoml-0.1.9/exoml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-07 17:27:07.000000 exoml-0.1.9/exoml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:27:07.000000 exoml-0.1.9/exoml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-07 17:27:07.000000 exoml-0.1.9/exoml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 17:27:07.000000 exoml-0.1.9/exoml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-07 17:26:53.000000 exoml-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-07 17:26:53.000000 exoml-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:27:07.406688 exoml-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:27:07.406688 exoml-0.1.9/transpot/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11057 2024-05-07 17:26:53.000000 exoml-0.1.9/transpot/TRANSPOT.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:26:53.000000 exoml-0.1.9/transpot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-07 17:26:53.000000 exoml-0.1.9/transpot/transpot_generator.py
```

### Comparing `exoml-0.1.8/PKG-INFO` & `exoml-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: exoml
-Version: 0.1.8
+Version: 0.1.9
 Summary: ExoML tools for exoplanet detections
 Author-email: Martín Dévora-Pajares <mdevorapajares@protonmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras==2.15.0
-Requires-Dist: tensorflow==2.15.0
 Requires-Dist: keras_nlp==0.8.1
 Requires-Dist: ellc==1.8.8
-Requires-Dist: lcbuilder==0.17.1
+Requires-Dist: lcbuilder==0.18.0
 Requires-Dist: ruamel.yaml==0.17.32
 Requires-Dist: pydot==1.4.2
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib==3.8.2
 Requires-Dist: typeguard==4.1.5
```

### Comparing `exoml-0.1.8/exoml/curve_prioritizer/curve_prioritizer_generator.py` & `exoml-0.1.9/exoml/curve_prioritizer/curve_prioritizer_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/curve_prioritizer/curve_prioritizer_model.py` & `exoml-0.1.9/exoml/curve_prioritizer/curve_prioritizer_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/detrend/DETREND.py` & `exoml-0.1.9/exoml/detrend/DETREND.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/detrend/detrend_generator.py` & `exoml-0.1.9/exoml/detrend/detrend_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ete6/ete6_generator.py` & `exoml-0.1.9/exoml/ete6/ete6_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/IATSON.py` & `exoml-0.1.9/exoml/iatson/IATSON.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/IATSON_og.py` & `exoml-0.1.9/exoml/iatson/IATSON_og.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/IATSON_planet.py` & `exoml-0.1.9/exoml/iatson/IATSON_planet.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/iatson_generator.py` & `exoml-0.1.9/exoml/iatson/iatson_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/iatson_og_generator.py` & `exoml-0.1.9/exoml/iatson/iatson_og_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/iatson_planet_generator.py` & `exoml-0.1.9/exoml/iatson/iatson_planet_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/iatson/watson_planet_generator.py` & `exoml-0.1.9/exoml/iatson/watson_planet_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/calibration/calibrator.py` & `exoml-0.1.9/exoml/ml/calibration/calibrator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/calibration/utils.py` & `exoml-0.1.9/exoml/ml/calibration/utils.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/auc.py` & `exoml-0.1.9/exoml/ml/callback/auc.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/basemodel_aware_callback.py` & `exoml-0.1.9/exoml/ml/callback/basemodel_aware_callback.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/batch_aware_csv_logger.py` & `exoml-0.1.9/exoml/ml/callback/batch_aware_csv_logger.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/checkpoint.py` & `exoml-0.1.9/exoml/ml/callback/checkpoint.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/early_stopping.py` & `exoml-0.1.9/exoml/ml/callback/early_stopping.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/learning_rate.py` & `exoml-0.1.9/exoml/ml/callback/learning_rate.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/callback/training_data_aware.py` & `exoml-0.1.9/exoml/ml/callback/training_data_aware.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/layers/dropout.py` & `exoml-0.1.9/exoml/ml/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/layers/transformer.py` & `exoml-0.1.9/exoml/ml/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/layers/transformer_classifier.py` & `exoml-0.1.9/exoml/ml/layers/transformer_classifier.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/learning_rate/schedulers.py` & `exoml-0.1.9/exoml/ml/learning_rate/schedulers.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/log/get_weights_logger.py` & `exoml-0.1.9/exoml/ml/log/get_weights_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 
 import numpy as np
+from keras_core import Layer
 
 
 class ModelWeightsLogger:
     def log_model_weights(self, model):
         # this function runs at the end of each epoch
         #logging.info('Generating layer weights info')
         # loop over each layer and get weights and biases
@@ -28,9 +29,11 @@
                 min_w = min_w if np.min(w) > min_w else np.min(w)
                 max_w = max_w if np.max(w) < max_w else np.max(w)
                 # logging.debug('Layer max weight is ' + str(np.nanmax(w)) + ' and min weight is ' + str(np.nanmin(w)))
                 # logging.debug('Layer max bias is ' + str(np.nanmax(b)) + ' and min bias is ' + str(np.nanmin(b)))
                 if nan_weight_indexes_count > 0 or nan_bias_indexes_count > 0:
                     logging.warning('Layer ' + str(layer_i) + ' with name ' + model.layers[layer_i].name + ' has ' + str(nan_weight_indexes_count) +
                           ' nan weights and ' + str(nan_bias_indexes_count) + ' nan biases')
-        logging.info("Min weights: %s from layer %s", min_w, min_layer.name)
-        logging.info("Max weights: %s from layer %s", max_w, max_layer.name)
+        if isinstance(min_layer, Layer):
+            logging.info("Min weights: %s from layer %s", min_w, min_layer.name)
+        if isinstance(max_layer, Layer):
+            logging.info("Max weights: %s from layer %s", max_w, max_layer.name)
```

### Comparing `exoml-0.1.8/exoml/ml/log/with_logging.py` & `exoml-0.1.9/exoml/ml/log/with_logging.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/loss/cross_entropy.py` & `exoml-0.1.9/exoml/ml/loss/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/loss/unsupervised.py` & `exoml-0.1.9/exoml/ml/loss/unsupervised.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/metrics/auc.py` & `exoml-0.1.9/exoml/ml/metrics/auc.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/ml_data_generator.py` & `exoml-0.1.9/exoml/ml/ml_data_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/ml_single_transits_classifier.py` & `exoml-0.1.9/exoml/ml/ml_single_transits_classifier.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/model/base_model.py` & `exoml-0.1.9/exoml/ml/model/base_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/model/binary_model.py` & `exoml-0.1.9/exoml/ml/model/binary_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/model/categorical_model.py` & `exoml-0.1.9/exoml/ml/model/categorical_model.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/ml/physics/transit_functions.py` & `exoml-0.1.9/exoml/ml/physics/transit_functions.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/preparation/empty_targets_preparer.py` & `exoml-0.1.9/exoml/preparation/empty_targets_preparer.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/preparation/ete6parser.py` & `exoml-0.1.9/exoml/preparation/ete6parser.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/preparation/parser_utils.py` & `exoml-0.1.9/exoml/preparation/parser_utils.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/preparation/q1q17dr25parser.py` & `exoml-0.1.9/exoml/preparation/q1q17dr25parser.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/resources/q1_q17/apjac4399t13_mrt.txt` & `exoml-0.1.9/exoml/resources/q1_q17/apjac4399t13_mrt.txt`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/santo/SANTO.py` & `exoml-0.1.9/exoml/santo/SANTO.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/santo/santo_generator.py` & `exoml-0.1.9/exoml/santo/santo_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml/santo/santo_test_data_generator.py` & `exoml-0.1.9/exoml/santo/santo_test_data_generator.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/exoml.egg-info/PKG-INFO` & `exoml-0.1.9/exoml.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: exoml
-Version: 0.1.8
+Version: 0.1.9
 Summary: ExoML tools for exoplanet detections
 Author-email: Martín Dévora-Pajares <mdevorapajares@protonmail.com>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: keras==2.15.0
-Requires-Dist: tensorflow==2.15.0
 Requires-Dist: keras_nlp==0.8.1
 Requires-Dist: ellc==1.8.8
-Requires-Dist: lcbuilder==0.17.1
+Requires-Dist: lcbuilder==0.18.0
 Requires-Dist: ruamel.yaml==0.17.32
 Requires-Dist: pydot==1.4.2
 Requires-Dist: graphviz==0.20.1
 Requires-Dist: pandas==1.5.3
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: matplotlib==3.8.2
 Requires-Dist: typeguard==4.1.5
```

### Comparing `exoml-0.1.8/exoml.egg-info/SOURCES.txt` & `exoml-0.1.9/exoml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/pyproject.toml` & `exoml-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 description = "ExoML tools for exoplanet detections"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = []
 license = {text = "MIT"}
 dynamic = ["dependencies"]
-version = "0.1.8"
+version = "0.1.9"
 
 [project.optional-dependencies]
 
 [project.scripts]
 #my-script = "my_package.module:function"
 
 [tool.setuptools]
```

### Comparing `exoml-0.1.8/transpot/TRANSPOT.py` & `exoml-0.1.9/transpot/TRANSPOT.py`

 * *Files identical despite different names*

### Comparing `exoml-0.1.8/transpot/transpot_generator.py` & `exoml-0.1.9/transpot/transpot_generator.py`

 * *Files identical despite different names*

