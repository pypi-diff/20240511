# Comparing `tmp/d3rlpy-2.4.0.tar.gz` & `tmp/d3rlpy-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3rlpy-2.4.0.tar", last modified: Sun Feb 18 03:49:08 2024, max compression
+gzip compressed data, was "d3rlpy-2.5.0.tar", last modified: Sat May 11 08:54:03 2024, max compression
```

## Comparing `d3rlpy-2.4.0.tar` & `d3rlpy-2.5.0.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.430828 d3rlpy-2.4.0/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1068 2022-09-11 02:40:22.000000 d3rlpy-2.4.0/LICENSE
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11856 2024-02-18 03:49:08.430828 d3rlpy-2.4.0/PKG-INFO
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9074 2023-12-27 07:26:20.000000 d3rlpy-2.4.0/README.md
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.414830 d3rlpy-2.4.0/d3rlpy/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      991 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       22 2024-02-18 03:48:37.000000 d3rlpy-2.4.0/d3rlpy/_version.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.414830 d3rlpy-2.4.0/d3rlpy/algos/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       75 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/algos/__init__.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.414830 d3rlpy-2.4.0/d3rlpy/algos/qlearning/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      351 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5950 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/awac.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    33993 2024-02-18 01:41:44.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5830 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/bc.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15758 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/bcq.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10546 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/bear.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12565 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/cql.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7311 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/crr.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5757 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/ddpg.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7417 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/dqn.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4208 2023-10-21 14:06:21.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/explorers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6451 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/iql.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3942 2024-02-18 01:49:27.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/nfq.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    13946 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/plas.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4320 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/random_policy.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12846 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/sac.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6527 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/td3.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6044 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/td3_plus_bc.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.418829 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      323 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3610 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/awac_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4417 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/bc_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9488 2024-01-13 05:24:14.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/bcq_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9855 2024-01-13 05:24:14.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/bear_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9427 2024-01-09 13:24:15.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/cql_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7213 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/crr_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6609 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/ddpg_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4032 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/dqn_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3772 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/iql_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7135 2024-01-13 05:24:14.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/plas_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10038 2024-01-09 13:24:15.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/sac_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2596 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/td3_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1969 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1180 2023-12-25 12:07:40.000000 d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.418829 d3rlpy-2.4.0/d3rlpy/algos/transformer/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      109 2023-10-07 08:33:28.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2150 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/action_samplers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14718 2024-02-18 01:53:14.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9917 2023-10-21 14:26:55.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/decision_transformer.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4320 2023-12-17 09:27:07.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/inputs.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.418829 d3rlpy-2.4.0/d3rlpy/algos/transformer/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       41 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5624 2024-01-04 04:05:29.000000 d3rlpy-2.4.0/d3rlpy/algos/transformer/torch/decision_transformer_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4600 2023-11-03 10:47:32.000000 d3rlpy-2.4.0/d3rlpy/algos/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    13102 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11150 2023-11-03 07:52:07.000000 d3rlpy-2.4.0/d3rlpy/cli.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1444 2024-02-18 01:26:58.000000 d3rlpy-2.4.0/d3rlpy/constants.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      729 2023-08-26 01:54:36.000000 d3rlpy-2.4.0/d3rlpy/dataclass_utils.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.422829 d3rlpy-2.4.0/d3rlpy/dataset/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      289 2023-10-21 14:02:21.000000 d3rlpy-2.4.0/d3rlpy/dataset/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3073 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/dataset/buffers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2592 2023-10-22 03:43:13.000000 d3rlpy-2.4.0/d3rlpy/dataset/compat.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11502 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/dataset/components.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2622 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/dataset/episode_generator.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3562 2024-01-04 04:13:59.000000 d3rlpy-2.4.0/d3rlpy/dataset/io.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7837 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/dataset/mini_batch.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    27844 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/dataset/replay_buffer.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7130 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/dataset/trajectory_slicers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6545 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/dataset/transition_pickers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11292 2024-02-18 01:59:34.000000 d3rlpy-2.4.0/d3rlpy/dataset/utils.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12407 2024-02-18 02:00:49.000000 d3rlpy-2.4.0/d3rlpy/dataset/writers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    23436 2023-12-17 07:59:12.000000 d3rlpy-2.4.0/d3rlpy/datasets.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1041 2023-11-27 13:38:16.000000 d3rlpy-2.4.0/d3rlpy/distributed.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.422829 d3rlpy-2.4.0/d3rlpy/envs/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-11-03 10:43:16.000000 d3rlpy-2.4.0/d3rlpy/envs/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      124 2023-11-03 10:43:24.000000 d3rlpy-2.4.0/d3rlpy/envs/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    17117 2024-02-18 01:50:39.000000 d3rlpy-2.4.0/d3rlpy/envs/wrappers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      305 2023-07-29 08:13:46.000000 d3rlpy-2.4.0/d3rlpy/healthcheck.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1005 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/interface.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/itertools.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.422829 d3rlpy-2.4.0/d3rlpy/logging/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      163 2024-02-18 01:28:05.000000 d3rlpy-2.4.0/d3rlpy/logging/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2751 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/logging/file_adapter.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4694 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/logging/logger.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1050 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/logging/noop_adapter.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2459 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/logging/tensorboard_adapter.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2115 2024-02-18 01:49:28.000000 d3rlpy-2.4.0/d3rlpy/logging/utils.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2506 2024-02-18 01:38:18.000000 d3rlpy-2.4.0/d3rlpy/logging/wandb_adapter.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.422829 d3rlpy-2.4.0/d3rlpy/metrics/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       49 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/metrics/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    17777 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/metrics/evaluators.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3184 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/metrics/utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.422829 d3rlpy-2.4.0/d3rlpy/models/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      101 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/models/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11025 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/models/builders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8922 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/models/encoders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8805 2024-01-13 03:57:11.000000 d3rlpy-2.4.0/d3rlpy/models/optimizers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7032 2023-08-26 01:54:36.000000 d3rlpy-2.4.0/d3rlpy/models/q_functions.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.426828 d3rlpy-2.4.0/d3rlpy/models/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      210 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/models/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5545 2023-08-11 07:35:00.000000 d3rlpy-2.4.0/d3rlpy/models/torch/distributions.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9943 2024-02-17 09:13:32.000000 d3rlpy-2.4.0/d3rlpy/models/torch/encoders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5390 2024-01-13 05:24:14.000000 d3rlpy-2.4.0/d3rlpy/models/torch/imitators.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      725 2024-01-09 13:24:15.000000 d3rlpy-2.4.0/d3rlpy/models/torch/parameters.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4739 2023-12-17 09:27:07.000000 d3rlpy-2.4.0/d3rlpy/models/torch/policies.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.426828 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      168 2023-08-04 14:36:24.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2663 2023-12-17 09:27:08.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12206 2024-02-18 01:51:10.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/ensemble_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8196 2023-12-17 13:49:44.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/iqn_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4118 2024-01-18 11:48:23.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/mean_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5911 2023-12-17 09:27:08.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/qr_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2580 2023-12-16 05:48:23.000000 d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    17011 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/models/torch/transformers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      957 2023-12-17 09:27:08.000000 d3rlpy-2.4.0/d3rlpy/models/torch/v_functions.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      571 2023-12-27 04:21:43.000000 d3rlpy-2.4.0/d3rlpy/models/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1242 2023-09-02 10:42:45.000000 d3rlpy-2.4.0/d3rlpy/notebook_utils.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.426828 d3rlpy-2.4.0/d3rlpy/ope/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       19 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/ope/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9185 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/ope/fqe.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.426828 d3rlpy-2.4.0/d3rlpy/ope/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       24 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/ope/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4731 2024-01-04 04:03:57.000000 d3rlpy-2.4.0/d3rlpy/ope/torch/fqe_impl.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.426828 d3rlpy-2.4.0/d3rlpy/preprocessing/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      115 2023-07-18 06:25:45.000000 d3rlpy-2.4.0/d3rlpy/preprocessing/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6674 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/preprocessing/action_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3253 2023-11-03 10:47:32.000000 d3rlpy-2.4.0/d3rlpy/preprocessing/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    17472 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/preprocessing/observation_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15005 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/preprocessing/reward_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6744 2024-02-12 13:44:45.000000 d3rlpy-2.4.0/d3rlpy/serializable_config.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.430828 d3rlpy-2.4.0/d3rlpy/tokenizers/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-12-26 03:23:48.000000 d3rlpy-2.4.0/d3rlpy/tokenizers/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1525 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/tokenizers/tokenizers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      521 2023-12-26 04:56:49.000000 d3rlpy-2.4.0/d3rlpy/tokenizers/utils.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12587 2024-02-18 01:49:29.000000 d3rlpy-2.4.0/d3rlpy/torch_utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      778 2023-12-17 09:27:07.000000 d3rlpy-2.4.0/d3rlpy/types.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-02-18 03:49:08.414830 d3rlpy-2.4.0/d3rlpy.egg-info/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11856 2024-02-18 03:49:08.000000 d3rlpy-2.4.0/d3rlpy.egg-info/PKG-INFO
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3937 2024-02-18 03:49:08.000000 d3rlpy-2.4.0/d3rlpy.egg-info/SOURCES.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2024-02-18 03:49:08.000000 d3rlpy-2.4.0/d3rlpy.egg-info/dependency_links.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       43 2024-02-18 03:49:08.000000 d3rlpy-2.4.0/d3rlpy.egg-info/entry_points.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      105 2024-02-18 03:49:08.000000 d3rlpy-2.4.0/d3rlpy.egg-info/requires.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        7 2024-02-18 03:49:08.000000 d3rlpy-2.4.0/d3rlpy.egg-info/top_level.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2024-02-18 03:49:05.000000 d3rlpy-2.4.0/d3rlpy.egg-info/zip-safe
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       38 2024-02-18 03:49:08.430828 d3rlpy-2.4.0/setup.cfg
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1850 2023-09-02 11:17:46.000000 d3rlpy-2.4.0/setup.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1068 2024-05-05 03:41:06.000000 d3rlpy-2.5.0/LICENSE
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12222 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/PKG-INFO
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9408 2024-05-06 11:37:30.000000 d3rlpy-2.5.0/README.md
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.121286 d3rlpy-2.5.0/d3rlpy/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1143 2024-05-05 06:43:39.000000 d3rlpy-2.5.0/d3rlpy/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       22 2024-05-11 08:45:54.000000 d3rlpy-2.5.0/d3rlpy/_version.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.121286 d3rlpy-2.5.0/d3rlpy/algos/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       75 2024-02-12 13:44:45.000000 d3rlpy-2.5.0/d3rlpy/algos/__init__.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.121286 d3rlpy-2.5.0/d3rlpy/algos/qlearning/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      373 2024-03-24 06:51:23.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5950 2024-02-18 01:49:27.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/awac.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    35069 2024-05-06 05:21:48.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5830 2024-02-18 01:49:27.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/bc.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15758 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/bcq.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10546 2024-02-18 01:49:27.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/bear.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6508 2024-05-06 11:34:04.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/cal_ql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12876 2024-05-06 11:34:04.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/cql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7311 2024-02-18 01:49:27.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/crr.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5757 2024-02-18 01:49:27.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/ddpg.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7417 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/dqn.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4208 2023-10-21 14:06:21.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/explorers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6451 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/iql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3942 2024-02-18 01:49:27.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/nfq.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    13946 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/plas.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4320 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/random_policy.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12846 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/sac.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6527 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/td3.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6044 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/td3_plus_bc.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      350 2024-03-24 06:14:16.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3610 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/awac_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4417 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/bc_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9488 2024-01-13 05:24:14.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/bcq_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9855 2024-01-13 05:24:14.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/bear_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      612 2024-05-06 11:39:15.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/cal_ql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9727 2024-05-06 11:34:04.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/cql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7213 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/crr_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6609 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/ddpg_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4032 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/dqn_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3772 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/iql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7135 2024-01-13 05:24:14.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/plas_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10038 2024-01-09 13:24:15.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/sac_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2596 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/td3_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1969 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2990 2024-05-06 11:34:04.000000 d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/algos/transformer/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      109 2023-10-07 08:33:28.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2150 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/action_samplers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    19537 2024-05-05 13:24:28.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9917 2023-10-21 14:26:55.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/decision_transformer.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4320 2023-12-17 09:27:07.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/inputs.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/algos/transformer/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       41 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5624 2024-05-05 09:27:17.000000 d3rlpy-2.5.0/d3rlpy/algos/transformer/torch/decision_transformer_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4612 2024-04-05 12:08:04.000000 d3rlpy-2.5.0/d3rlpy/algos/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    13102 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11141 2024-04-28 16:19:31.000000 d3rlpy-2.5.0/d3rlpy/cli.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1444 2024-02-18 01:26:58.000000 d3rlpy-2.5.0/d3rlpy/constants.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      729 2023-08-26 01:54:36.000000 d3rlpy-2.5.0/d3rlpy/dataclass_utils.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/dataset/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      289 2023-10-21 14:02:21.000000 d3rlpy-2.5.0/d3rlpy/dataset/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3073 2024-04-05 11:32:57.000000 d3rlpy-2.5.0/d3rlpy/dataset/buffers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2592 2023-10-22 03:43:13.000000 d3rlpy-2.5.0/d3rlpy/dataset/compat.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10561 2024-04-28 05:18:27.000000 d3rlpy-2.5.0/d3rlpy/dataset/components.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2815 2024-05-06 00:12:01.000000 d3rlpy-2.5.0/d3rlpy/dataset/episode_generator.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3562 2024-01-04 04:13:59.000000 d3rlpy-2.5.0/d3rlpy/dataset/io.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7606 2024-04-21 14:31:49.000000 d3rlpy-2.5.0/d3rlpy/dataset/mini_batch.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    28070 2024-04-05 11:35:59.000000 d3rlpy-2.5.0/d3rlpy/dataset/replay_buffer.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7130 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/dataset/trajectory_slicers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6981 2024-05-11 05:27:44.000000 d3rlpy-2.5.0/d3rlpy/dataset/transition_pickers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11292 2024-02-18 01:59:34.000000 d3rlpy-2.5.0/d3rlpy/dataset/utils.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12914 2024-04-05 11:40:22.000000 d3rlpy-2.5.0/d3rlpy/dataset/writers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    23844 2024-05-06 09:04:43.000000 d3rlpy-2.5.0/d3rlpy/datasets.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1041 2023-11-27 13:38:16.000000 d3rlpy-2.5.0/d3rlpy/distributed.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/envs/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-11-03 10:43:16.000000 d3rlpy-2.5.0/d3rlpy/envs/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      124 2023-11-03 10:43:24.000000 d3rlpy-2.5.0/d3rlpy/envs/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    17117 2024-02-18 01:50:39.000000 d3rlpy-2.5.0/d3rlpy/envs/wrappers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      305 2023-07-29 08:13:46.000000 d3rlpy-2.5.0/d3rlpy/healthcheck.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1005 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/interface.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/itertools.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/logging/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      163 2024-02-18 01:28:05.000000 d3rlpy-2.5.0/d3rlpy/logging/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2751 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/logging/file_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4694 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/logging/logger.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1050 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/logging/noop_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2437 2024-04-05 12:11:51.000000 d3rlpy-2.5.0/d3rlpy/logging/tensorboard_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2115 2024-02-18 01:49:28.000000 d3rlpy-2.5.0/d3rlpy/logging/utils.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2506 2024-02-18 01:38:18.000000 d3rlpy-2.5.0/d3rlpy/logging/wandb_adapter.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/metrics/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       49 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/metrics/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    17825 2024-04-05 12:09:34.000000 d3rlpy-2.5.0/d3rlpy/metrics/evaluators.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3184 2024-05-06 06:27:12.000000 d3rlpy-2.5.0/d3rlpy/metrics/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/models/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      101 2024-02-12 13:44:45.000000 d3rlpy-2.5.0/d3rlpy/models/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11025 2024-05-06 11:12:59.000000 d3rlpy-2.5.0/d3rlpy/models/builders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8922 2024-02-18 01:49:29.000000 d3rlpy-2.5.0/d3rlpy/models/encoders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8805 2024-01-13 03:57:11.000000 d3rlpy-2.5.0/d3rlpy/models/optimizers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7032 2023-08-26 01:54:36.000000 d3rlpy-2.5.0/d3rlpy/models/q_functions.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.125286 d3rlpy-2.5.0/d3rlpy/models/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      210 2024-02-12 13:44:45.000000 d3rlpy-2.5.0/d3rlpy/models/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5545 2023-08-11 07:35:00.000000 d3rlpy-2.5.0/d3rlpy/models/torch/distributions.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9943 2024-02-17 09:13:32.000000 d3rlpy-2.5.0/d3rlpy/models/torch/encoders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5390 2024-01-13 05:24:14.000000 d3rlpy-2.5.0/d3rlpy/models/torch/imitators.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      725 2024-01-09 13:24:15.000000 d3rlpy-2.5.0/d3rlpy/models/torch/parameters.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4739 2024-05-06 09:02:22.000000 d3rlpy-2.5.0/d3rlpy/models/torch/policies.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      168 2023-08-04 14:36:24.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2663 2023-12-17 09:27:08.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12206 2024-02-18 01:51:10.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/ensemble_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8196 2023-12-17 13:49:44.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/iqn_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4118 2024-01-18 11:48:23.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/mean_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5911 2023-12-17 09:27:08.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/qr_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2580 2023-12-16 05:48:23.000000 d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    16575 2024-05-05 12:05:45.000000 d3rlpy-2.5.0/d3rlpy/models/torch/transformers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      957 2023-12-17 09:27:08.000000 d3rlpy-2.5.0/d3rlpy/models/torch/v_functions.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      571 2023-12-27 04:21:43.000000 d3rlpy-2.5.0/d3rlpy/models/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1242 2023-09-02 10:42:45.000000 d3rlpy-2.5.0/d3rlpy/notebook_utils.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/d3rlpy/ope/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       19 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/ope/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9185 2024-02-18 01:49:29.000000 d3rlpy-2.5.0/d3rlpy/ope/fqe.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/d3rlpy/ope/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       24 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/ope/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4731 2024-01-04 04:03:57.000000 d3rlpy-2.5.0/d3rlpy/ope/torch/fqe_impl.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/d3rlpy/preprocessing/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      115 2023-07-18 06:25:45.000000 d3rlpy-2.5.0/d3rlpy/preprocessing/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6674 2024-02-18 01:49:29.000000 d3rlpy-2.5.0/d3rlpy/preprocessing/action_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3253 2023-11-03 10:47:32.000000 d3rlpy-2.5.0/d3rlpy/preprocessing/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    17472 2024-02-18 01:49:29.000000 d3rlpy-2.5.0/d3rlpy/preprocessing/observation_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15685 2024-04-29 13:12:24.000000 d3rlpy-2.5.0/d3rlpy/preprocessing/reward_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6744 2024-02-12 13:44:45.000000 d3rlpy-2.5.0/d3rlpy/serializable_config.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/d3rlpy/tokenizers/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-12-26 03:23:48.000000 d3rlpy-2.5.0/d3rlpy/tokenizers/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1525 2024-02-18 01:49:29.000000 d3rlpy-2.5.0/d3rlpy/tokenizers/tokenizers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      521 2023-12-26 04:56:49.000000 d3rlpy-2.5.0/d3rlpy/tokenizers/utils.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    13511 2024-04-28 16:24:42.000000 d3rlpy-2.5.0/d3rlpy/torch_utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      778 2023-12-17 09:27:07.000000 d3rlpy-2.5.0/d3rlpy/types.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2024-05-11 08:54:03.121286 d3rlpy-2.5.0/d3rlpy.egg-info/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12222 2024-05-11 08:54:03.000000 d3rlpy-2.5.0/d3rlpy.egg-info/PKG-INFO
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4014 2024-05-11 08:54:03.000000 d3rlpy-2.5.0/d3rlpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2024-05-11 08:54:03.000000 d3rlpy-2.5.0/d3rlpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       43 2024-05-11 08:54:03.000000 d3rlpy-2.5.0/d3rlpy.egg-info/entry_points.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      113 2024-05-11 08:54:03.000000 d3rlpy-2.5.0/d3rlpy.egg-info/requires.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        7 2024-05-11 08:54:03.000000 d3rlpy-2.5.0/d3rlpy.egg-info/top_level.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2024-05-11 08:53:59.000000 d3rlpy-2.5.0/d3rlpy.egg-info/zip-safe
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       38 2024-05-11 08:54:03.129287 d3rlpy-2.5.0/setup.cfg
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1858 2024-05-05 07:37:20.000000 d3rlpy-2.5.0/setup.py
```

### Comparing `d3rlpy-2.4.0/LICENSE` & `d3rlpy-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/PKG-INFO` & `d3rlpy-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d3rlpy
-Version: 2.4.0
+Version: 2.5.0
 Summary: An offline deep reinforcement learning library
 Home-page: https://github.com/takuseno/d3rlpy
 Author: Takuma Seno
 Author-email: takuma.seno@gmail.com
 License: MIT License
 Description: <p align="center"><img align="center" width="300px" src="assets/logo.png"></p>
         
@@ -92,14 +92,15 @@
         | [Bootstrapping Error Accumulation Reduction (BEAR)](https://arxiv.org/abs/1906.00949) | :no_entry: | :white_check_mark: |
         | [Conservative Q-Learning (CQL)](https://arxiv.org/abs/2006.04779) | :white_check_mark: | :white_check_mark: |
         | [Advantage Weighted Actor-Critic (AWAC)](https://arxiv.org/abs/2006.09359) | :no_entry: | :white_check_mark: |
         | [Critic Reguralized Regression (CRR)](https://arxiv.org/abs/2006.15134) | :no_entry: | :white_check_mark: |
         | [Policy in Latent Action Space (PLAS)](https://arxiv.org/abs/2011.07213) | :no_entry: | :white_check_mark: |
         | [TD3+BC](https://arxiv.org/abs/2106.06860) | :no_entry: | :white_check_mark: |
         | [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169) | :no_entry: | :white_check_mark: |
+        | [Calibrated Q-Learning (Cal-QL)](https://arxiv.org/abs/2303.05479) | :no_entry: | :white_check_mark: |
         | [Decision Transformer](https://arxiv.org/abs/2106.01345) | :white_check_mark: | :white_check_mark: |
         | [Gato](https://arxiv.org/abs/2205.06175) | :construction: | :construction: |
         
         ## Supported Q functions
         - [x] standard Q function
         - [x] [Quantile Regression](https://arxiv.org/abs/1710.10044)
         - [x] [Implicit Quantile Network](https://arxiv.org/abs/1806.06923)
@@ -194,14 +195,17 @@
         Please check the [contribution guide](CONTRIBUTING.md).
         
         ## Community
         | Channel | Link |
         |:-|:-|
         | Issues | [GitHub Issues](https://github.com/takuseno/d3rlpy/issues) |
         
+        > [!IMPORTANT]
+        > Please do NOT email to any contributors including the owner of this project to ask for technical support. Such emails will be ignored without replying to your message. Use GitHub Issues to report your problems.
+        
         ## Projects using d3rlpy
         | Project | Description |
         |:-:|:-|
         | [MINERVA](https://github.com/takuseno/minerva) | An out-of-the-box GUI tool for offline RL |
         | [SCOPE-RL](https://github.com/hakuhodo-technologies/scope-rl) | An off-policy evaluation and selection library |
         
         ## Roadmap
```

### Comparing `d3rlpy-2.4.0/README.md` & `d3rlpy-2.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 | [Bootstrapping Error Accumulation Reduction (BEAR)](https://arxiv.org/abs/1906.00949) | :no_entry: | :white_check_mark: |
 | [Conservative Q-Learning (CQL)](https://arxiv.org/abs/2006.04779) | :white_check_mark: | :white_check_mark: |
 | [Advantage Weighted Actor-Critic (AWAC)](https://arxiv.org/abs/2006.09359) | :no_entry: | :white_check_mark: |
 | [Critic Reguralized Regression (CRR)](https://arxiv.org/abs/2006.15134) | :no_entry: | :white_check_mark: |
 | [Policy in Latent Action Space (PLAS)](https://arxiv.org/abs/2011.07213) | :no_entry: | :white_check_mark: |
 | [TD3+BC](https://arxiv.org/abs/2106.06860) | :no_entry: | :white_check_mark: |
 | [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169) | :no_entry: | :white_check_mark: |
+| [Calibrated Q-Learning (Cal-QL)](https://arxiv.org/abs/2303.05479) | :no_entry: | :white_check_mark: |
 | [Decision Transformer](https://arxiv.org/abs/2106.01345) | :white_check_mark: | :white_check_mark: |
 | [Gato](https://arxiv.org/abs/2205.06175) | :construction: | :construction: |
 
 ## Supported Q functions
 - [x] standard Q function
 - [x] [Quantile Regression](https://arxiv.org/abs/1710.10044)
 - [x] [Implicit Quantile Network](https://arxiv.org/abs/1806.06923)
@@ -186,14 +187,17 @@
 Please check the [contribution guide](CONTRIBUTING.md).
 
 ## Community
 | Channel | Link |
 |:-|:-|
 | Issues | [GitHub Issues](https://github.com/takuseno/d3rlpy/issues) |
 
+> [!IMPORTANT]
+> Please do NOT email to any contributors including the owner of this project to ask for technical support. Such emails will be ignored without replying to your message. Use GitHub Issues to report your problems.
+
 ## Projects using d3rlpy
 | Project | Description |
 |:-:|:-|
 | [MINERVA](https://github.com/takuseno/minerva) | An out-of-the-box GUI tool for offline RL |
 | [SCOPE-RL](https://github.com/hakuhodo-technologies/scope-rl) | An off-policy evaluation and selection library |
 
 ## Roadmap
```

### Comparing `d3rlpy-2.4.0/d3rlpy/__init__.py` & `d3rlpy-2.5.0/d3rlpy/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,37 +12,43 @@
     logging,
     metrics,
     models,
     notebook_utils,
     ope,
     preprocessing,
     tokenizers,
+    types,
 )
 from ._version import __version__
 from .base import load_learnable
-from .constants import ActionSpace, PositionEncodingType
+from .constants import ActionSpace, LoggingStrategy, PositionEncodingType
 from .healthcheck import run_healthcheck
+from .torch_utility import Modules, TorchMiniBatch
 
 __all__ = [
     "algos",
     "dataset",
     "datasets",
     "distributed",
     "envs",
     "logging",
     "metrics",
     "models",
     "notebook_utils",
     "ope",
     "preprocessing",
     "tokenizers",
+    "types",
     "__version__",
     "load_learnable",
     "ActionSpace",
+    "LoggingStrategy",
     "PositionEncodingType",
+    "Modules",
+    "TorchMiniBatch",
     "seed",
 ]
 
 
 def seed(n: int) -> None:
     """Sets random seed value.
```

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/awac.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/awac.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/base.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import (
     Callable,
     Dict,
     Generator,
     Generic,
     List,
     Optional,
+    Sequence,
     Tuple,
     TypeVar,
 )
 
 import numpy as np
 import torch
 from torch import nn
@@ -20,15 +21,15 @@
 from ...base import ImplBase, LearnableBase, LearnableConfig, save_config
 from ...constants import (
     IMPL_NOT_INITIALIZED_ERROR,
     ActionSpace,
     LoggingStrategy,
 )
 from ...dataset import (
-    ReplayBuffer,
+    ReplayBufferBase,
     TransitionMiniBatch,
     check_non_1d_array,
     create_fifo_replay_buffer,
     is_tuple_shape,
 )
 from ...logging import (
     LOG,
@@ -185,38 +186,50 @@
 
         See also
 
             * https://pytorch.org/tutorials/beginner/Intro_to_TorchScript_tutorial.html (for Python).
             * https://pytorch.org/tutorials/advanced/cpp_export.html (for C++).
             * https://onnx.ai (for ONNX)
 
+        Visit https://d3rlpy.readthedocs.io/en/stable/tutorials/after_training_policies.html#export-policies-as-torchscript for the further usage.
+
         Args:
             fname: Destination file path.
         """
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         if is_tuple_shape(self._impl.observation_shape):
-            raise NotImplementedError(
-                "save_policy method does not support tuple observation yet."
+            dummy_x = [
+                torch.rand(1, *shape, device=self._device)
+                for shape in self._impl.observation_shape
+            ]
+            num_inputs = len(self._impl.observation_shape)
+        else:
+            dummy_x = torch.rand(
+                1, *self._impl.observation_shape, device=self._device
             )
-        dummy_x = torch.rand(
-            1, *self._impl.observation_shape, device=self._device
-        )
+            num_inputs = 1
 
         # workaround until version 1.6
         self._impl.modules.freeze()
 
         # local function to select best actions
-        def _func(x: torch.Tensor) -> torch.Tensor:
+        def _func(*x: Sequence[torch.Tensor]) -> torch.Tensor:
             assert self._impl
 
+            observation: TorchObservation = x
+            if len(observation) == 1:
+                observation = observation[0]
+
             if self._config.observation_scaler:
-                x = self._config.observation_scaler.transform(x)
+                observation = self._config.observation_scaler.transform(
+                    observation
+                )
 
-            action = self._impl.predict_best_action(x)
+            action = self._impl.predict_best_action(observation)
 
             if self._config.action_scaler:
                 action = self._config.action_scaler.reverse_transform(action)
 
             return action
 
         traced_script = torch.jit.trace(_func, dummy_x, check_trace=False)
@@ -225,15 +238,15 @@
             # currently, PyTorch cannot directly export function as ONNX.
             torch.onnx.export(
                 traced_script,
                 dummy_x,
                 fname,
                 export_params=True,
                 opset_version=11,
-                input_names=["input_0"],
+                input_names=[f"input_{i}" for i in range(num_inputs)],
                 output_names=["output_0"],
             )
         elif fname.endswith(".pt"):
             traced_script.save(fname)
         else:
             raise ValueError(
                 f"invalid format type: {fname}."
@@ -355,15 +368,15 @@
             if self._config.action_scaler:
                 action = self._config.action_scaler.reverse_transform(action)
 
         return action.cpu().detach().numpy()  # type: ignore
 
     def fit(
         self,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
         n_steps: int,
         n_steps_per_epoch: int = 10000,
         experiment_name: Optional[str] = None,
         with_timestamp: bool = True,
         logging_steps: int = 500,
         logging_strategy: LoggingStrategy = LoggingStrategy.EPOCH,
         logger_adapter: LoggerAdapterFactory = FileAdapterFactory(),
@@ -424,15 +437,15 @@
                 enable_ddp=enable_ddp,
             )
         )
         return results
 
     def fitter(
         self,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
         n_steps: int,
         n_steps_per_epoch: int = 10000,
         logging_steps: int = 500,
         logging_strategy: LoggingStrategy = LoggingStrategy.EPOCH,
         experiment_name: Optional[str] = None,
         with_timestamp: bool = True,
         logger_adapter: LoggerAdapterFactory = FileAdapterFactory(),
@@ -586,19 +599,20 @@
             yield epoch, metrics
 
         logger.close()
 
     def fit_online(
         self,
         env: GymEnv,
-        buffer: Optional[ReplayBuffer] = None,
+        buffer: Optional[ReplayBufferBase] = None,
         explorer: Optional[Explorer] = None,
         n_steps: int = 1000000,
         n_steps_per_epoch: int = 10000,
         update_interval: int = 1,
+        n_updates: int = 1,
         update_start_step: int = 0,
         random_steps: int = 0,
         eval_env: Optional[GymEnv] = None,
         eval_epsilon: float = 0.0,
         save_interval: int = 1,
         experiment_name: Optional[str] = None,
         with_timestamp: bool = True,
@@ -613,14 +627,17 @@
         Args:
             env: Gym-like environment.
             buffer : Replay buffer.
             explorer: Action explorer.
             n_steps: Number of total steps to train.
             n_steps_per_epoch: Number of steps per epoch.
             update_interval: Number of steps per update.
+            n_updates: Number of gradient steps at a time. The combination of
+                ``update_interval`` and ``n_updates`` controls Update-To-Data
+                (UTD) ratio.
             update_start_step: Steps before starting updates.
             random_steps: Steps for the initial random explortion.
             eval_env: Gym-like environment. If None, evaluation is skipped.
             eval_epsilon: :math:`\\epsilon`-greedy factor during evaluation.
             save_interval: Number of epochs before saving models.
             experiment_name: Experiment name for logging. If not passed,
                 the directory name will be ``{class name}_online_{timestamp}``.
@@ -633,15 +650,15 @@
             show_progress: Flag to show progress bar for iterations.
             callback: Callable function that takes ``(algo, epoch, total_step)``
                 , which is called at the end of epochs.
         """
 
         # create default replay buffer
         if buffer is None:
-            buffer = create_fifo_replay_buffer(1000000)
+            buffer = create_fifo_replay_buffer(1000000, env=env)
 
         # check action-space
         assert_action_space_with_env(self, env)
 
         # setup logger
         if experiment_name is None:
             experiment_name = self.__class__.__name__ + "_online"
@@ -714,27 +731,28 @@
                 epoch = total_step // n_steps_per_epoch
 
                 if (
                     total_step > update_start_step
                     and buffer.transition_count > self.batch_size
                 ):
                     if total_step % update_interval == 0:
-                        # sample mini-batch
-                        with logger.measure_time("sample_batch"):
-                            batch = buffer.sample_transition_batch(
-                                self.batch_size
-                            )
-
-                        # update parameters
-                        with logger.measure_time("algorithm_update"):
-                            loss = self.update(batch)
-
-                        # record metrics
-                        for name, val in loss.items():
-                            logger.add_metric(name, val)
+                        for _ in range(n_updates):  # controls UTD ratio
+                            # sample mini-batch
+                            with logger.measure_time("sample_batch"):
+                                batch = buffer.sample_transition_batch(
+                                    self.batch_size
+                                )
+
+                            # update parameters
+                            with logger.measure_time("algorithm_update"):
+                                loss = self.update(batch)
+
+                            # record metrics
+                            for name, val in loss.items():
+                                logger.add_metric(name, val)
 
                         if (
                             logging_strategy == LoggingStrategy.STEPS
                             and total_step % logging_steps == 0
                         ):
                             logger.commit(epoch, total_step)
 
@@ -762,20 +780,20 @@
 
         # close logger
         logger.close()
 
     def collect(
         self,
         env: GymEnv,
-        buffer: Optional[ReplayBuffer] = None,
+        buffer: Optional[ReplayBufferBase] = None,
         explorer: Optional[Explorer] = None,
         deterministic: bool = False,
         n_steps: int = 1000000,
         show_progress: bool = True,
-    ) -> ReplayBuffer:
+    ) -> ReplayBufferBase:
         """Collects data via interaction with environment.
 
         If ``buffer`` is not given, ``ReplayBuffer`` will be internally created.
 
         Args:
             env: Fym-like environment.
             buffer: Replay buffer.
@@ -851,23 +869,29 @@
 
         Returns:
             Dictionary of metrics.
         """
         assert self._impl, IMPL_NOT_INITIALIZED_ERROR
         torch_batch = TorchMiniBatch.from_batch(
             batch=batch,
+            gamma=self._config.gamma,
+            compute_returns_to_go=self.need_returns_to_go,
             device=self._device,
             observation_scaler=self._config.observation_scaler,
             action_scaler=self._config.action_scaler,
             reward_scaler=self._config.reward_scaler,
         )
         loss = self._impl.update(torch_batch, self._grad_step)
         self._grad_step += 1
         return loss
 
+    @property
+    def need_returns_to_go(self) -> bool:
+        return False
+
     def copy_policy_from(
         self, algo: "QLearningAlgoBase[QLearningAlgoImplBase, LearnableConfig]"
     ) -> None:
         """Copies policy parameters from the given algorithm.
 
         .. code-block:: python
```

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/bc.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/bc.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/bcq.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/bcq.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/bear.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/bear.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/cql.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/cql.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         initial_temperature (float): Initial temperature value.
         initial_alpha (float): Initial :math:`\alpha` value.
         alpha_threshold (float): Threshold value described as :math:`\tau`.
         conservative_weight (float): Constant weight to scale conservative loss.
         n_action_samples (int): Number of sampled actions to compute
             :math:`\log{\sum_a \exp{Q(s, a)}}`.
         soft_q_backup (bool): Flag to use SAC-style backup.
+        max_q_backup (bool): Flag to sample max Q-values for target.
     """
 
     actor_learning_rate: float = 1e-4
     critic_learning_rate: float = 3e-4
     temp_learning_rate: float = 1e-4
     alpha_learning_rate: float = 1e-4
     actor_optim_factory: OptimizerFactory = make_optimizer_field()
@@ -118,27 +119,32 @@
     n_critics: int = 2
     initial_temperature: float = 1.0
     initial_alpha: float = 1.0
     alpha_threshold: float = 10.0
     conservative_weight: float = 5.0
     n_action_samples: int = 10
     soft_q_backup: bool = False
+    max_q_backup: bool = False
 
     def create(self, device: DeviceArg = False) -> "CQL":
         return CQL(self, device)
 
     @staticmethod
     def get_type() -> str:
         return "cql"
 
 
 class CQL(QLearningAlgoBase[CQLImpl, CQLConfig]):
     def inner_create_impl(
         self, observation_shape: Shape, action_size: int
     ) -> None:
+        assert not (
+            self._config.soft_q_backup and self._config.max_q_backup
+        ), "soft_q_backup and max_q_backup are mutually exclusive."
+
         policy = create_normal_policy(
             observation_shape,
             action_size,
             self._config.actor_encoder_factory,
             device=self._device,
         )
         q_funcs, q_func_fowarder = create_continuous_q_function(
@@ -205,14 +211,15 @@
             targ_q_func_forwarder=targ_q_func_forwarder,
             gamma=self._config.gamma,
             tau=self._config.tau,
             alpha_threshold=self._config.alpha_threshold,
             conservative_weight=self._config.conservative_weight,
             n_action_samples=self._config.n_action_samples,
             soft_q_backup=self._config.soft_q_backup,
+            max_q_backup=self._config.max_q_backup,
             device=self._device,
         )
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
```

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/crr.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/crr.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/ddpg.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/ddpg.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/dqn.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/dqn.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/explorers.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/explorers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/iql.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/iql.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/nfq.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/nfq.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/plas.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/plas.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/random_policy.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/random_policy.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/sac.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/sac.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/td3.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/td3.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/td3_plus_bc.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/td3_plus_bc.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/awac_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/awac_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/bc_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/bc_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/bcq_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/bcq_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/bear_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/bear_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/cql_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/cql_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import dataclasses
 import math
-from typing import Optional
+from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch.optim import Optimizer
 
 from ....models.torch import (
     ContinuousEnsembleQFunctionForwarder,
     DiscreteEnsembleQFunctionForwarder,
     Parameter,
-    build_squashed_gaussian_distribution,
     get_parameter,
 )
 from ....torch_utility import (
     TorchMiniBatch,
     expand_and_repeat_recursively,
     flatten_left_recursively,
 )
 from ....types import Shape, TorchObservation
 from .ddpg_impl import DDPGBaseCriticLoss
 from .dqn_impl import DoubleDQNImpl, DQNLoss, DQNModules
 from .sac_impl import SACImpl, SACModules
+from .utility import sample_q_values_with_policy
 
 __all__ = ["CQLImpl", "DiscreteCQLImpl", "CQLModules", "DiscreteCQLLoss"]
 
 
 @dataclasses.dataclass(frozen=True)
 class CQLModules(SACModules):
     log_alpha: Parameter
@@ -40,28 +40,30 @@
 
 class CQLImpl(SACImpl):
     _modules: CQLModules
     _alpha_threshold: float
     _conservative_weight: float
     _n_action_samples: int
     _soft_q_backup: bool
+    _max_q_backup: bool
 
     def __init__(
         self,
         observation_shape: Shape,
         action_size: int,
         modules: CQLModules,
         q_func_forwarder: ContinuousEnsembleQFunctionForwarder,
         targ_q_func_forwarder: ContinuousEnsembleQFunctionForwarder,
         gamma: float,
         tau: float,
         alpha_threshold: float,
         conservative_weight: float,
         n_action_samples: int,
         soft_q_backup: bool,
+        max_q_backup: bool,
         device: str,
     ):
         super().__init__(
             observation_shape=observation_shape,
             action_size=action_size,
             modules=modules,
             q_func_forwarder=q_func_forwarder,
@@ -70,76 +72,60 @@
             tau=tau,
             device=device,
         )
         self._alpha_threshold = alpha_threshold
         self._conservative_weight = conservative_weight
         self._n_action_samples = n_action_samples
         self._soft_q_backup = soft_q_backup
+        self._max_q_backup = max_q_backup
 
     def compute_critic_loss(
         self, batch: TorchMiniBatch, q_tpn: torch.Tensor
     ) -> CQLCriticLoss:
         loss = super().compute_critic_loss(batch, q_tpn)
         conservative_loss = self._compute_conservative_loss(
-            batch.observations, batch.actions, batch.next_observations
+            obs_t=batch.observations,
+            act_t=batch.actions,
+            obs_tp1=batch.next_observations,
+            returns_to_go=batch.returns_to_go,
         )
         if self._modules.alpha_optim:
             self.update_alpha(conservative_loss)
         return CQLCriticLoss(
-            critic_loss=loss.critic_loss + conservative_loss,
-            conservative_loss=conservative_loss,
+            critic_loss=loss.critic_loss + conservative_loss.sum(),
+            conservative_loss=conservative_loss.sum(),
             alpha=get_parameter(self._modules.log_alpha).exp(),
         )
 
     def update_alpha(self, conservative_loss: torch.Tensor) -> None:
         assert self._modules.alpha_optim
         self._modules.alpha_optim.zero_grad()
         # the original implementation does scale the loss value
-        loss = -conservative_loss
+        loss = -conservative_loss.mean()
         loss.backward(retain_graph=True)
         self._modules.alpha_optim.step()
 
     def _compute_policy_is_values(
-        self, policy_obs: TorchObservation, value_obs: TorchObservation
-    ) -> torch.Tensor:
-        with torch.no_grad():
-            dist = build_squashed_gaussian_distribution(
-                self._modules.policy(policy_obs)
-            )
-            policy_actions, n_log_probs = dist.sample_n_with_log_prob(
-                self._n_action_samples
-            )
-
-        # (batch, observation) -> (batch, n, observation)
-        repeated_obs = expand_and_repeat_recursively(
-            value_obs, self._n_action_samples
-        )
-        # (batch, n, observation) -> (batch * n, observation)
-        flat_obs = flatten_left_recursively(repeated_obs, dim=1)
-        # (batch, n, action) -> (batch * n, action)
-        flat_policy_acts = policy_actions.reshape(-1, self.action_size)
-
-        # estimate action-values for policy actions
-        policy_values = self._q_func_forwarder.compute_expected_q(
-            flat_obs, flat_policy_acts, "none"
-        )
-        batch_size = (
-            policy_obs.shape[0]
-            if isinstance(policy_obs, torch.Tensor)
-            else policy_obs[0].shape[0]
-        )
-        policy_values = policy_values.view(
-            -1, batch_size, self._n_action_samples
-        )
-        log_probs = n_log_probs.view(1, -1, self._n_action_samples)
-
-        # importance sampling
-        return policy_values - log_probs
-
-    def _compute_random_is_values(self, obs: TorchObservation) -> torch.Tensor:
+        self,
+        policy_obs: TorchObservation,
+        value_obs: TorchObservation,
+        returns_to_go: torch.Tensor,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        return sample_q_values_with_policy(
+            policy=self._modules.policy,
+            q_func_forwarder=self._q_func_forwarder,
+            policy_observations=policy_obs,
+            value_observations=value_obs,
+            n_action_samples=self._n_action_samples,
+            detach_policy_output=True,
+        )
+
+    def _compute_random_is_values(
+        self, obs: TorchObservation
+    ) -> Tuple[torch.Tensor, float]:
         # (batch, observation) -> (batch, n, observation)
         repeated_obs = expand_and_repeat_recursively(
             obs, self._n_action_samples
         )
         # (batch, n, observation) -> (batch * n, observation)
         flat_obs = flatten_left_recursively(repeated_obs, dim=1)
 
@@ -156,58 +142,86 @@
         )
         random_values = random_values.view(
             -1, batch_size, self._n_action_samples
         )
         random_log_probs = math.log(0.5**self._action_size)
 
         # importance sampling
-        return random_values - random_log_probs
+        return random_values, random_log_probs
 
     def _compute_conservative_loss(
         self,
         obs_t: TorchObservation,
         act_t: torch.Tensor,
         obs_tp1: TorchObservation,
+        returns_to_go: torch.Tensor,
     ) -> torch.Tensor:
-        policy_values_t = self._compute_policy_is_values(obs_t, obs_t)
-        policy_values_tp1 = self._compute_policy_is_values(obs_tp1, obs_t)
-        random_values = self._compute_random_is_values(obs_t)
+        policy_values_t, log_probs_t = self._compute_policy_is_values(
+            policy_obs=obs_t,
+            value_obs=obs_t,
+            returns_to_go=returns_to_go,
+        )
+        policy_values_tp1, log_probs_tp1 = self._compute_policy_is_values(
+            policy_obs=obs_tp1,
+            value_obs=obs_t,
+            returns_to_go=returns_to_go,
+        )
+        random_values, random_log_probs = self._compute_random_is_values(obs_t)
 
         # compute logsumexp
         # (n critics, batch, 3 * n samples) -> (n critics, batch, 1)
         target_values = torch.cat(
-            [policy_values_t, policy_values_tp1, random_values], dim=2
+            [
+                policy_values_t - log_probs_t,
+                policy_values_tp1 - log_probs_tp1,
+                random_values - random_log_probs,
+            ],
+            dim=2,
         )
         logsumexp = torch.logsumexp(target_values, dim=2, keepdim=True)
 
         # estimate action-values for data actions
         data_values = self._q_func_forwarder.compute_expected_q(
             obs_t, act_t, "none"
         )
 
-        loss = logsumexp.mean(dim=0).mean() - data_values.mean(dim=0).mean()
-        scaled_loss = self._conservative_weight * loss
+        loss = (logsumexp - data_values).mean(dim=[1, 2])
 
         # clip for stability
         log_alpha = get_parameter(self._modules.log_alpha)
         clipped_alpha = log_alpha.exp().clamp(0, 1e6)[0][0]
 
-        return clipped_alpha * (scaled_loss - self._alpha_threshold)
+        return (
+            clipped_alpha
+            * self._conservative_weight
+            * (loss - self._alpha_threshold)
+        )
 
     def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
         if self._soft_q_backup:
             target_value = super().compute_target(batch)
         else:
-            target_value = self._compute_deterministic_target(batch)
+            with torch.no_grad():
+                target_value = self._compute_deterministic_target(batch)
         return target_value
 
     def _compute_deterministic_target(
         self, batch: TorchMiniBatch
     ) -> torch.Tensor:
-        with torch.no_grad():
+        if self._max_q_backup:
+            q_values, _ = sample_q_values_with_policy(
+                policy=self._modules.policy,
+                q_func_forwarder=self._targ_q_func_forwarder,
+                policy_observations=batch.next_observations,
+                value_observations=batch.next_observations,
+                n_action_samples=self._n_action_samples,
+                detach_policy_output=True,
+            )
+            return q_values.min(dim=0).values.max(dim=1, keepdims=True).values
+        else:
             action = self._modules.policy(batch.next_observations).squashed_mu
             return self._targ_q_func_forwarder.compute_target(
                 batch.next_observations,
                 action,
                 reduction="min",
             )
```

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/crr_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/crr_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/ddpg_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/ddpg_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/dqn_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/dqn_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/iql_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/iql_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/plas_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/plas_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/sac_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/sac_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/td3_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/td3_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/transformer/action_samplers.py` & `d3rlpy-2.5.0/d3rlpy/algos/transformer/action_samplers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/transformer/base.py` & `d3rlpy-2.5.0/d3rlpy/algos/transformer/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 import dataclasses
 from abc import abstractmethod
 from collections import defaultdict, deque
-from typing import Callable, Deque, Dict, Generic, Optional, TypeVar, Union
+from typing import (
+    Callable,
+    Deque,
+    Dict,
+    Generic,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
 
 import numpy as np
 import torch
 from tqdm.auto import tqdm
 from typing_extensions import Self
 
 from ...base import ImplBase, LearnableBase, LearnableConfig, save_config
 from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ...dataset import ReplayBuffer, TrajectoryMiniBatch
+from ...dataset import ReplayBuffer, TrajectoryMiniBatch, is_tuple_shape
 from ...logging import (
     LOG,
     D3RLPyLogger,
     FileAdapterFactory,
     LoggerAdapterFactory,
 )
 from ...metrics import evaluate_transformer_with_environment
 from ...torch_utility import TorchTrajectoryMiniBatch, eval_api, train_api
-from ...types import GymEnv, NDArray, Observation
+from ...types import GymEnv, NDArray, Observation, TorchObservation
 from ..utility import (
     assert_action_space_with_dataset,
     build_scalers_with_trajectory_slicer,
 )
 from .action_samplers import (
     IdentityTransformerActionSampler,
     SoftmaxTransformerActionSampler,
@@ -198,14 +207,149 @@
         return pad_action
 
 
 class TransformerAlgoBase(
     Generic[TTransformerImpl, TTransformerConfig],
     LearnableBase[TTransformerImpl, TTransformerConfig],
 ):
+    def save_policy(self, fname: str) -> None:
+        """Save the greedy-policy computational graph as TorchScript or ONNX.
+
+        The format will be automatically detected by the file name.
+
+        .. code-block:: python
+
+            # save as TorchScript
+            algo.save_policy('policy.pt')
+
+            # save as ONNX
+            algo.save_policy('policy.onnx')
+
+        The artifacts saved with this method will work without d3rlpy.
+        This method is especially useful to deploy the learned policy to
+        production environments or embedding systems.
+
+        See also
+
+            * https://pytorch.org/tutorials/beginner/Intro_to_TorchScript_tutorial.html (for Python).
+            * https://pytorch.org/tutorials/advanced/cpp_export.html (for C++).
+            * https://onnx.ai (for ONNX)
+
+        Visit https://d3rlpy.readthedocs.io/en/stable/tutorials/after_training_policies.html#export-policies-as-torchscript for the further usage.
+
+        Args:
+            fname: Destination file path.
+        """
+        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
+
+        context_size = self._config.context_size
+        dummy_x = []
+        if is_tuple_shape(self._impl.observation_shape):
+            dummy_x.extend(
+                [
+                    torch.rand(context_size, *shape, device=self._device)
+                    for shape in self._impl.observation_shape
+                ]
+            )
+            num_observations = len(self._impl.observation_shape)
+        else:
+            dummy_x.append(
+                torch.rand(
+                    context_size,
+                    *self._impl.observation_shape,
+                    device=self._device,
+                )
+            )
+            num_observations = 1
+        # action
+        if self.get_action_type() == ActionSpace.CONTINUOUS:
+            dummy_x.append(
+                torch.rand(
+                    context_size, self._impl.action_size, device=self._device
+                )
+            )
+        else:
+            dummy_x.append(torch.rand(context_size, 1, device=self._device))
+        # return_to_go
+        dummy_x.append(torch.rand(context_size, 1, device=self._device))
+        # timesteps
+        dummy_x.append(torch.arange(context_size, device=self._device))
+
+        # workaround until version 1.6
+        self._impl.modules.freeze()
+
+        # local function to select best actions
+        def _func(*x: Sequence[torch.Tensor]) -> torch.Tensor:
+            assert self._impl
+
+            # add batch dimension
+            x = [v.view(1, *v.shape) for v in x]  # type: ignore
+
+            observations: TorchObservation = x[:-3]
+            actions = x[-3]
+            returns_to_go = x[-2]
+            timesteps = x[-1]
+
+            if len(observations) == 1:
+                observations = observations[0]
+
+            if self._config.observation_scaler:
+                observations = self._config.observation_scaler.transform(
+                    observations
+                )
+            if self._config.action_scaler:
+                actions = self._config.action_scaler.transform(actions)
+
+            inpt = TorchTransformerInput(
+                observations=observations,
+                actions=actions,
+                rewards=torch.zeros_like(returns_to_go),
+                returns_to_go=returns_to_go,
+                timesteps=timesteps,
+                masks=torch.zeros_like(returns_to_go),
+                length=self._config.context_size,
+            )
+
+            action = self._impl.predict(inpt)
+
+            if self._config.action_scaler:
+                action = self._config.action_scaler.reverse_transform(action)
+
+            if self.get_action_type() == ActionSpace.DISCRETE:
+                action = action.argmax()
+
+            return action
+
+        traced_script = torch.jit.trace(_func, dummy_x, check_trace=False)
+
+        if fname.endswith(".onnx"):
+            # currently, PyTorch cannot directly export function as ONNX.
+            torch.onnx.export(
+                traced_script,
+                dummy_x,
+                fname,
+                export_params=True,
+                opset_version=11,
+                input_names=[
+                    f"observation_{i}" for i in range(num_observations)
+                ]
+                + ["action", "return_to_go", "timestep"],
+                output_names=["output_0"],
+            )
+        elif fname.endswith(".pt"):
+            traced_script.save(fname)
+        else:
+            raise ValueError(
+                f"invalid format type: {fname}."
+                " .pt and .onnx extensions are currently supported."
+            )
+
+        # workaround until version 1.6
+        self._impl.modules.unfreeze()
+
     def predict(self, inpt: TransformerInput) -> NDArray:
         """Returns action.
 
         This is for internal use. For evaluation, use
         ``StatefulTransformerWrapper`` instead.
 
         Args:
```

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/transformer/decision_transformer.py` & `d3rlpy-2.5.0/d3rlpy/algos/transformer/decision_transformer.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/transformer/inputs.py` & `d3rlpy-2.5.0/d3rlpy/algos/transformer/inputs.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/transformer/torch/decision_transformer_impl.py` & `d3rlpy-2.5.0/d3rlpy/algos/transformer/torch/decision_transformer_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/algos/utility.py` & `d3rlpy-2.5.0/d3rlpy/algos/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ..base import LearnableBase
 from ..constants import (
     CONTINUOUS_ACTION_SPACE_MISMATCH_ERROR,
     DISCRETE_ACTION_SPACE_MISMATCH_ERROR,
     ActionSpace,
 )
-from ..dataset import DatasetInfo, ReplayBuffer
+from ..dataset import DatasetInfo, ReplayBufferBase
 from ..logging import LOG
 from ..types import GymEnv
 
 __all__ = ["assert_action_space_with_dataset", "assert_action_space_with_env"]
 
 
 def assert_action_space_with_dataset(
@@ -45,15 +45,15 @@
         ), DISCRETE_ACTION_SPACE_MISMATCH_ERROR
     else:
         action_space = type(env.action_space)
         raise ValueError(f"The action-space is not supported: {action_space}")
 
 
 def build_scalers_with_transition_picker(
-    algo: LearnableBase[Any, Any], dataset: ReplayBuffer
+    algo: LearnableBase[Any, Any], dataset: ReplayBufferBase
 ) -> None:
     # initialize observation scaler
     if algo.observation_scaler and not algo.observation_scaler.built:
         LOG.debug(
             "Fitting observation scaler...",
             observation_scaler=algo.observation_scaler.get_type(),
         )
@@ -79,15 +79,15 @@
         )
         algo.reward_scaler.fit_with_transition_picker(
             dataset.episodes, dataset.transition_picker
         )
 
 
 def build_scalers_with_trajectory_slicer(
-    algo: LearnableBase[Any, Any], dataset: ReplayBuffer
+    algo: LearnableBase[Any, Any], dataset: ReplayBufferBase
 ) -> None:
     # initialize observation scaler
     if algo.observation_scaler and not algo.observation_scaler.built:
         LOG.debug(
             "Fitting observation scaler...",
             observation_scaler=algo.observation_scaler.get_type(),
         )
```

### Comparing `d3rlpy-2.4.0/d3rlpy/base.py` & `d3rlpy-2.5.0/d3rlpy/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/cli.py` & `d3rlpy-2.5.0/d3rlpy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,14 +364,14 @@
 def install(name: str) -> None:
     if name == "atari":
         _install_module(["gym[atari,accept-rom-license]"], upgrade=True)
     elif name == "d4rl_atari":
         install("atari")
         _install_module(["git+https://github.com/takuseno/d4rl-atari"])
     elif name == "d4rl":
-        _install_module(["git+https://github.com/Farama-Foundation/D4RL"])
+        _install_module(["git+https://github.com/takuseno/D4RL"])
         _install_module(["gym"], upgrade=True)
         _uninstall_module(["pybullet"])
     elif name == "minari":
         _install_module(["minari==0.4.2", "gymnasium_robotics"], upgrade=True)
     else:
         raise ValueError(f"Unsupported command: {name}")
```

### Comparing `d3rlpy-2.4.0/d3rlpy/constants.py` & `d3rlpy-2.5.0/d3rlpy/constants.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataclass_utils.py` & `d3rlpy-2.5.0/d3rlpy/dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/buffers.py` & `d3rlpy-2.5.0/d3rlpy/dataset/buffers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/compat.py` & `d3rlpy-2.5.0/d3rlpy/dataset/compat.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/components.py` & `d3rlpy-2.5.0/d3rlpy/dataset/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,18 @@
     Float32NDArray,
     Int32NDArray,
     NDArray,
     Observation,
     ObservationSequence,
 )
 from .utils import (
-    create_zero_observation,
     get_dtype_from_observation,
     get_dtype_from_observation_sequence,
     get_shape_from_observation,
     get_shape_from_observation_sequence,
-    retrieve_observation,
 )
 
 __all__ = [
     "Signature",
     "Transition",
     "PartialTrajectory",
     "EpisodeBase",
@@ -62,26 +60,27 @@
 
     Args:
         observation: Observation.
         action: Action
         reward: Reward. This could be a multi-step discounted return.
         next_observation: Observation at next timestep. This could be
             observation at multi-step ahead.
-        return_to_go: Remaining return till the end of an episode.
         terminal: Flag of environment termination.
         interval: Timesteps between ``observation`` and ``next_observation``.
+        rewards_to_go: Remaining rewards till the end of an episode, which is
+            used to compute returns_to_go.
     """
 
     observation: Observation  # (...)
     action: NDArray  # (...)
     reward: Float32NDArray  # (1,)
     next_observation: Observation  # (...)
-    return_to_go: Float32NDArray  # (1,)
     terminal: float
     interval: int
+    rewards_to_go: Float32NDArray  # (L, 1)
 
     @property
     def observation_signature(self) -> Signature:
         r"""Returns observation sigunature.
 
         Returns:
             Observation signature.
@@ -184,42 +183,14 @@
         """Returns number of transitions.
 
         Returns:
             Number of transitions.
         """
         return self.length if bool(self.terminals[-1]) else self.length - 1
 
-    def get_as_transition(self, index: int) -> Transition:
-        """Returns Transition at the specified index.
-
-        Args:
-            index: Index of transition.
-
-        Returns:
-            Transition.
-        """
-        assert index < self.get_transition_count()
-        observation = retrieve_observation(self.observations, index)
-        terminal = float(self.terminals[index])
-        if terminal and index == self.length - 1:
-            next_observation = create_zero_observation(observation)
-        else:
-            next_observation = retrieve_observation(
-                self.observations, index + 1
-            )
-        return Transition(
-            observation=observation,
-            action=self.actions[index],
-            reward=self.rewards[index],
-            next_observation=next_observation,
-            return_to_go=self.returns_to_go[index],
-            terminal=terminal,
-            interval=1,
-        )
-
     def __len__(self) -> int:
         return self.length
 
 
 class EpisodeBase(Protocol):
     r"""Episode interface.
```

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/episode_generator.py` & `d3rlpy-2.5.0/d3rlpy/dataset/episode_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,18 @@
 
         if timeouts is None:
             timeouts = np.zeros_like(terminals)
 
         assert (
             np.sum(np.logical_and(terminals, timeouts)) == 0
         ), "terminals and timeouts never become True at the same time"
+        assert (np.sum(terminals) + np.sum(timeouts)) > 0, (
+            "No episode termination was found. Either terminals"
+            " or timeouts must include non-zero values."
+        )
 
         self._observations = observations
         self._actions = actions
         self._rewards = rewards
         self._terminals = terminals
         self._timeouts = timeouts
```

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/io.py` & `d3rlpy-2.5.0/d3rlpy/dataset/io.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/mini_batch.py` & `d3rlpy-2.5.0/d3rlpy/dataset/mini_batch.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,37 +25,36 @@
         actions: Batched actions.
         rewards: Batched rewards.
         next_observations: Batched next observations.
         returns_to_go: Batched returns-to-go.
         terminals: Batched environment terminal flags.
         intervals: Batched timesteps between observations and next
             observations.
+        transitions: List of transitions.
     """
 
     observations: Union[Float32NDArray, Sequence[Float32NDArray]]  # (B, ...)
     actions: Float32NDArray  # (B, ...)
     rewards: Float32NDArray  # (B, 1)
     next_observations: Union[
         Float32NDArray, Sequence[Float32NDArray]
     ]  # (B, ...)
-    returns_to_go: Float32NDArray  # (B, 1)
     terminals: Float32NDArray  # (B, 1)
     intervals: Float32NDArray  # (B, 1)
+    transitions: Sequence[Transition]
 
     def __post_init__(self) -> None:
         assert check_non_1d_array(self.observations)
         assert check_dtype(self.observations, np.float32)
         assert check_non_1d_array(self.actions)
         assert check_dtype(self.actions, np.float32)
         assert check_non_1d_array(self.rewards)
         assert check_dtype(self.rewards, np.float32)
         assert check_non_1d_array(self.next_observations)
         assert check_dtype(self.next_observations, np.float32)
-        assert check_non_1d_array(self.returns_to_go)
-        assert check_dtype(self.returns_to_go, np.float32)
         assert check_non_1d_array(self.terminals)
         assert check_dtype(self.terminals, np.float32)
         assert check_non_1d_array(self.intervals)
         assert check_dtype(self.intervals, np.float32)
 
     @classmethod
     def from_transitions(
@@ -77,33 +76,30 @@
         )
         rewards = np.stack(
             [transition.reward for transition in transitions], axis=0
         )
         next_observations = stack_observations(
             [transition.next_observation for transition in transitions]
         )
-        returns_to_go = np.stack(
-            [transition.return_to_go for transition in transitions], axis=0
-        )
         terminals = np.reshape(
             np.array([transition.terminal for transition in transitions]),
             [-1, 1],
         )
         intervals = np.reshape(
             np.array([transition.interval for transition in transitions]),
             [-1, 1],
         )
         return TransitionMiniBatch(
             observations=cast_recursively(observations, np.float32),
             actions=cast_recursively(actions, np.float32),
             rewards=cast_recursively(rewards, np.float32),
             next_observations=cast_recursively(next_observations, np.float32),
-            returns_to_go=cast_recursively(returns_to_go, np.float32),
             terminals=cast_recursively(terminals, np.float32),
             intervals=cast_recursively(intervals, np.float32),
+            transitions=transitions,
         )
 
     @property
     def observation_shape(self) -> Shape:
         r"""Returns observation shape.
 
         Returns:
```

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/replay_buffer.py` & `d3rlpy-2.5.0/d3rlpy/dataset/replay_buffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,14 +324,16 @@
         action_size (Optional[int]): Size of action-space. For continuous
             action-space, this represents dimension of action vectors. For
             discrete action-space, this represents the number of discrete
             actions.
         cache_size (int): Size of cache to record active episode history used
             for online training. ``cache_size`` needs to be greater than the
             maximum possible episode length.
+        write_at_termination (bool): Flag to write experiences to the buffer at the
+            end of an episode all at once.
     """
 
     _buffer: BufferProtocol
     _transition_picker: TransitionPickerProtocol
     _trajectory_slicer: TrajectorySlicerProtocol
     _writer: ExperienceWriter
     _episodes: List[EpisodeBase]
@@ -347,14 +349,15 @@
         env: Optional[GymEnv] = None,
         observation_signature: Optional[Signature] = None,
         action_signature: Optional[Signature] = None,
         reward_signature: Optional[Signature] = None,
         action_space: Optional[ActionSpace] = None,
         action_size: Optional[int] = None,
         cache_size: int = 10000,
+        write_at_termination: bool = False,
     ):
         transition_picker = transition_picker or BasicTransitionPicker()
         trajectory_slicer = trajectory_slicer or BasicTrajectorySlicer()
         writer_preprocessor = writer_preprocessor or BasicWriterPreprocess()
 
         if not (
             observation_signature and action_signature and reward_signature
@@ -430,14 +433,15 @@
         self._writer = ExperienceWriter(
             buffer,
             writer_preprocessor,
             observation_signature=observation_signature,
             action_signature=action_signature,
             reward_signature=reward_signature,
             cache_size=cache_size,
+            write_at_termination=write_at_termination,
         )
         self._transition_picker = transition_picker
         self._trajectory_slicer = trajectory_slicer
         self._dataset_info = DatasetInfo(
             observation_signature=observation_signature,
             action_signature=action_signature,
             reward_signature=reward_signature,
```

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/trajectory_slicers.py` & `d3rlpy-2.5.0/d3rlpy/dataset/trajectory_slicers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/transition_pickers.py` & `d3rlpy-2.5.0/d3rlpy/dataset/transition_pickers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import dataclasses
+
 import numpy as np
 from typing_extensions import Protocol
 
+from ..types import Float32NDArray
 from .components import EpisodeBase, Transition
 from .utils import (
     create_zero_observation,
     retrieve_observation,
     stack_recent_observations,
 )
 
 __all__ = [
     "TransitionPickerProtocol",
     "BasicTransitionPicker",
+    "SparseRewardTransitionPicker",
     "FrameStackTransitionPicker",
     "MultiStepTransitionPicker",
 ]
 
 
 def _validate_index(episode: EpisodeBase, index: int) -> None:
     assert index < episode.transition_count
@@ -36,52 +40,73 @@
         raise NotImplementedError
 
 
 class BasicTransitionPicker(TransitionPickerProtocol):
     r"""Standard transition picker.
 
     This class implements a basic transition picking.
-
-    Args:
-        gamma (float): Discount factor to compute return-to-go.
     """
 
-    _gamma: float
-
-    def __init__(self, gamma: float = 0.99):
-        self._gamma = gamma
-
     def __call__(self, episode: EpisodeBase, index: int) -> Transition:
         _validate_index(episode, index)
 
         observation = retrieve_observation(episode.observations, index)
         is_terminal = episode.terminated and index == episode.size() - 1
         if is_terminal:
             next_observation = create_zero_observation(observation)
         else:
             next_observation = retrieve_observation(
                 episode.observations, index + 1
             )
 
-        # compute return-to-go
-        length = episode.size() - index
-        cum_gammas = np.expand_dims(self._gamma ** np.arange(length), axis=1)
-        return_to_go = np.sum(cum_gammas * episode.rewards[index:], axis=0)
-
         return Transition(
             observation=observation,
             action=episode.actions[index],
             reward=episode.rewards[index],
             next_observation=next_observation,
-            return_to_go=return_to_go,
             terminal=float(is_terminal),
             interval=1,
+            rewards_to_go=episode.rewards[index:],
         )
 
 
+class SparseRewardTransitionPicker(TransitionPickerProtocol):
+    r"""Sparse reward transition picker.
+
+    This class extends BasicTransitionPicker to handle special returns_to_go
+    calculation mainly used in AntMaze environments.
+
+    For the failure trajectories, this class sets the constant return value to
+    avoid inconsistent horizon due to time out.
+
+    Args:
+        failure_return (int): Return value for failure trajectories.
+        step_reward (float): Immediate step reward value in sparse reward
+            setting.
+    """
+
+    def __init__(self, failure_return: float, step_reward: float = 0.0):
+        self._failure_return = failure_return
+        self._step_reward = step_reward
+        self._transition_picker = BasicTransitionPicker()
+
+    def __call__(self, episode: EpisodeBase, index: int) -> Transition:
+        transition = self._transition_picker(episode, index)
+        if np.all(transition.rewards_to_go == self._step_reward):
+            extended_rewards_to_go: Float32NDArray = np.array(
+                [[self._failure_return]],
+                dtype=np.float32,
+            )
+            transition = dataclasses.replace(
+                transition,
+                rewards_to_go=extended_rewards_to_go,
+            )
+        return transition
+
+
 class FrameStackTransitionPicker(TransitionPickerProtocol):
     r"""Frame-stacking transition picker.
 
     This class implements the frame-stacking logic. The observations are
     stacked with the last ``n_frames-1`` frames. When ``index`` specifies
     timestep below ``n_frames``, those frames are padded by zeros.
 
@@ -97,24 +122,21 @@
         frame_stacking_picker = FrameStackTransitionPicker(n_frames=4)
         transition = frame_stacking_picker(episode, 10)
 
         transition.observation.shape == (4, 84, 84)
 
     Args:
         n_frames (int): Number of frames to stack.
-        gamma (float): Discount factor to compute return-to-go.
     """
 
     _n_frames: int
-    _gamma: float
 
-    def __init__(self, n_frames: int, gamma: float = 0.99):
+    def __init__(self, n_frames: int):
         assert n_frames > 0
         self._n_frames = n_frames
-        self._gamma = gamma
 
     def __call__(self, episode: EpisodeBase, index: int) -> Transition:
         _validate_index(episode, index)
 
         observation = stack_recent_observations(
             episode.observations, index, self._n_frames
         )
@@ -122,27 +144,22 @@
         if is_terminal:
             next_observation = create_zero_observation(observation)
         else:
             next_observation = stack_recent_observations(
                 episode.observations, index + 1, self._n_frames
             )
 
-        # compute return-to-go
-        length = episode.size() - index
-        cum_gammas = np.expand_dims(self._gamma ** np.arange(length), axis=1)
-        return_to_go = np.sum(cum_gammas * episode.rewards[index:], axis=0)
-
         return Transition(
             observation=observation,
             action=episode.actions[index],
             reward=episode.rewards[index],
             next_observation=next_observation,
-            return_to_go=return_to_go,
             terminal=float(is_terminal),
             interval=1,
+            rewards_to_go=episode.rewards[index:],
         )
 
 
 class MultiStepTransitionPicker(TransitionPickerProtocol):
     r"""Multi-step transition picker.
 
     This class implements transition picking for the multi-step TD error.
@@ -179,26 +196,21 @@
         else:
             is_terminal = False
             next_index = min(index + self._n_steps, episode.size() - 1)
             next_observation = retrieve_observation(
                 episode.observations, next_index
             )
 
-        # compute return-to-go
-        length = episode.size() - index
-        cum_gammas = np.expand_dims(self._gamma ** np.arange(length), axis=1)
-        return_to_go = np.sum(cum_gammas * episode.rewards[index:], axis=0)
-
         # compute multi-step return
         interval = next_index - index
         cum_gammas = np.expand_dims(self._gamma ** np.arange(interval), axis=1)
         ret = np.sum(episode.rewards[index:next_index] * cum_gammas, axis=0)
 
         return Transition(
             observation=observation,
             action=episode.actions[index],
             reward=ret,
             next_observation=next_observation,
-            return_to_go=return_to_go,
             terminal=float(is_terminal),
             interval=interval,
+            rewards_to_go=episode.rewards[index:],
         )
```

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/utils.py` & `d3rlpy-2.5.0/d3rlpy/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/dataset/writers.py` & `d3rlpy-2.5.0/d3rlpy/dataset/writers.py`

 * *Files 6% similar despite different names*

```diff
@@ -246,37 +246,42 @@
         buffer: Buffer.
         preprocessor: Writer preprocess.
         observation_signature: Signature of unprocessed observation.
         action_signature: Signature of unprocessed action.
         reward_signature: Signature of unprocessed reward.
         cache_size: Size of data in active episode. This needs to be larger
             than the maximum length of episodes.
+        write_at_termination: Flag to write experiences to the buffer at the
+            end of an episode all at once.
     """
 
     _preprocessor: WriterPreprocessProtocol
     _buffer: BufferProtocol
     _cache_size: int
+    _write_at_termination: bool
     _observation_signature: Signature
     _action_signature: Signature
     _reward_signature: Signature
     _active_episode: _ActiveEpisode
     _step: int
 
     def __init__(
         self,
         buffer: BufferProtocol,
         preprocessor: WriterPreprocessProtocol,
         observation_signature: Signature,
         action_signature: Signature,
         reward_signature: Signature,
         cache_size: int = 10000,
+        write_at_termination: bool = False,
     ):
         self._buffer = buffer
         self._preprocessor = preprocessor
         self._cache_size = cache_size
+        self._write_at_termination = write_at_termination
 
         # preprocessed signatures
         if len(observation_signature.dtype) == 1:
             processed_observation = preprocessor.process_observation(
                 observation_signature.sample()[0]
             )
             assert isinstance(processed_observation, np.ndarray)
@@ -354,29 +359,36 @@
 
         Args:
             observation: Observation.
             action: Action.
             reward: Reward.
         """
         self._active_episode.append(observation, action, reward)
-        if self._active_episode.transition_count > 0:
+        if (
+            not self._write_at_termination
+            and self._active_episode.transition_count > 0
+        ):
             self._buffer.append(
                 episode=self._active_episode,
                 index=self._active_episode.transition_count - 1,
             )
 
     def clip_episode(self, terminated: bool) -> None:
         r"""Clips the current episode.
 
         Args:
             terminated: Flag to represent environment termination.
         """
         if self._active_episode.transition_count == 0:
             return
 
+        if self._write_at_termination:
+            for i in range(self._active_episode.transition_count):
+                self._buffer.append(episode=self._active_episode, index=i)
+
         # shrink heap memory
         self._active_episode.shrink(terminated)
 
         # append terminal state if necessary
         if terminated:
             self._buffer.append(
                 self._active_episode,
```

### Comparing `d3rlpy-2.4.0/d3rlpy/datasets.py` & `d3rlpy-2.5.0/d3rlpy/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,15 @@
 
 
 def get_d4rl(
     env_name: str,
     transition_picker: Optional[TransitionPickerProtocol] = None,
     trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
     render_mode: Optional[str] = None,
+    max_episode_steps: int = 1000,
 ) -> Tuple[ReplayBuffer, gym.Env[NDArray, NDArray]]:
     """Returns d4rl dataset and envrironment.
 
     The dataset is provided through d4rl.
 
     .. code-block:: python
 
@@ -406,20 +407,25 @@
         * https://github.com/rail-berkeley/d4rl
 
     Args:
         env_name: environment id of d4rl dataset.
         transition_picker: TransitionPickerProtocol object.
         trajectory_slicer: TrajectorySlicerProtocol object.
         render_mode: Mode of rendering (``human``, ``rgb_array``).
+        max_episode_steps: Maximum episode environmental steps.
 
     Returns:
         tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     try:
-        import d4rl  # type: ignore
+        import d4rl
+        from d4rl.locomotion.wrappers import NormalizedBoxEnv
+        from d4rl.utils.wrappers import (
+            NormalizedBoxEnv as NormalizedBoxEnvFromUtils,
+        )
 
         env = gym.make(env_name)
         raw_dataset: Dict[str, NDArray] = env.get_dataset()  # type: ignore
 
         observations = raw_dataset["observations"]
         actions = raw_dataset["actions"]
         rewards = raw_dataset["rewards"]
@@ -432,19 +438,25 @@
             rewards=rewards,
             terminals=terminals,
             timeouts=timeouts,
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
         )
 
-        # wrapped by NormalizedBoxEnv that is incompatible with newer Gym
-        unwrapped_env: gym.Env[Any, Any] = env.env.env.env.wrapped_env  # type: ignore
+        # remove incompatible wrappers
+        normalized_env = env.env.env.env  # type: ignore
+        assert isinstance(
+            normalized_env, (NormalizedBoxEnv, NormalizedBoxEnvFromUtils)
+        )
+        unwrapped_env: gym.Env[Any, Any] = normalized_env.wrapped_env
         unwrapped_env.render_mode = render_mode  # overwrite
 
-        return dataset, TimeLimit(unwrapped_env, max_episode_steps=1000)
+        return dataset, TimeLimit(
+            normalized_env, max_episode_steps=max_episode_steps
+        )
     except ImportError as e:
         raise ImportError(
             "d4rl is not installed.\n" "$ d3rlpy install d4rl"
         ) from e
 
 
 class _MinariEnvType(enum.Enum):
```

### Comparing `d3rlpy-2.4.0/d3rlpy/distributed.py` & `d3rlpy-2.5.0/d3rlpy/distributed.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/envs/wrappers.py` & `d3rlpy-2.5.0/d3rlpy/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/interface.py` & `d3rlpy-2.5.0/d3rlpy/interface.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/logging/file_adapter.py` & `d3rlpy-2.5.0/d3rlpy/logging/file_adapter.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/logging/logger.py` & `d3rlpy-2.5.0/d3rlpy/logging/logger.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/logging/noop_adapter.py` & `d3rlpy-2.5.0/d3rlpy/logging/noop_adapter.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/logging/tensorboard_adapter.py` & `d3rlpy-2.5.0/d3rlpy/logging/tensorboard_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         try:
             from tensorboardX import SummaryWriter
         except ImportError as e:
             raise ImportError("Please install tensorboardX") from e
 
         self._experiment_name = experiment_name
         logdir = os.path.join(root_dir, "runs", experiment_name)
-        print(logdir)
         self._writer = SummaryWriter(logdir=logdir)
         self._metrics = {}
 
     def write_params(self, params: Dict[str, Any]) -> None:
         # remove non-scaler values for HParams
         self._params = {k: v for k, v in params.items() if np.isscalar(v)}
```

### Comparing `d3rlpy-2.4.0/d3rlpy/logging/utils.py` & `d3rlpy-2.5.0/d3rlpy/logging/utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/logging/wandb_adapter.py` & `d3rlpy-2.5.0/d3rlpy/logging/wandb_adapter.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/metrics/evaluators.py` & `d3rlpy-2.5.0/d3rlpy/metrics/evaluators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterator, Optional, Sequence
 
 import numpy as np
 from typing_extensions import Protocol
 
 from ..dataset import (
     EpisodeBase,
-    ReplayBuffer,
+    ReplayBufferBase,
     TransitionMiniBatch,
     TransitionPickerProtocol,
 )
 from ..interface import QLearningAlgoProtocol
 from ..types import GymEnv
 from .utility import evaluate_qlearning_with_environment
 
@@ -32,15 +32,15 @@
 WINDOW_SIZE = 1024
 
 
 class EvaluatorProtocol(Protocol):
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         """Computes metrics.
 
         Args:
             algo: Q-learning algorithm.
             dataset: ReplayBuffer.
 
@@ -90,15 +90,15 @@
 
     def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_errors = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
@@ -151,15 +151,15 @@
 
     def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_sums = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
@@ -209,15 +209,15 @@
 
     def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_values = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
@@ -252,15 +252,15 @@
 
     def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_values = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
@@ -307,15 +307,15 @@
     ):
         self._return_threshold = return_threshold
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         success_values = []
         all_values = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             is_success = episode.compute_return() >= self._return_threshold
             for batch in make_batches(
@@ -349,15 +349,15 @@
 
     def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_diffs = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
@@ -389,15 +389,15 @@
 
     def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_matches = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
@@ -436,15 +436,15 @@
     ):
         self._base_algo = base_algo
         self._episodes = episodes
 
     def __call__(
         self,
         algo: QLearningAlgoProtocol,
-        dataset: ReplayBuffer,
+        dataset: ReplayBufferBase,
     ) -> float:
         total_diffs = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             # TODO: handle different n_frames
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
@@ -484,15 +484,15 @@
         base_algo: QLearningAlgoProtocol,
         episodes: Optional[Sequence[EpisodeBase]] = None,
     ):
         self._base_algo = base_algo
         self._episodes = episodes
 
     def __call__(
-        self, algo: QLearningAlgoProtocol, dataset: ReplayBuffer
+        self, algo: QLearningAlgoProtocol, dataset: ReplayBufferBase
     ) -> float:
         total_matches = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             # TODO: handle different n_frames
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
@@ -535,15 +535,15 @@
         epsilon: float = 0.0,
     ):
         self._env = env
         self._n_trials = n_trials
         self._epsilon = epsilon
 
     def __call__(
-        self, algo: QLearningAlgoProtocol, dataset: ReplayBuffer
+        self, algo: QLearningAlgoProtocol, dataset: ReplayBufferBase
     ) -> float:
         return evaluate_qlearning_with_environment(
             algo=algo,
             env=self._env,
             n_trials=self._n_trials,
             epsilon=self._epsilon,
         )
```

### Comparing `d3rlpy-2.4.0/d3rlpy/metrics/utility.py` & `d3rlpy-2.5.0/d3rlpy/metrics/utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/builders.py` & `d3rlpy-2.5.0/d3rlpy/models/builders.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/encoders.py` & `d3rlpy-2.5.0/d3rlpy/models/encoders.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/optimizers.py` & `d3rlpy-2.5.0/d3rlpy/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/q_functions.py` & `d3rlpy-2.5.0/d3rlpy/models/q_functions.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/distributions.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/distributions.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/encoders.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/encoders.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/imitators.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/imitators.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/parameters.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/policies.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/policies.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/base.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/ensemble_q_function.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/ensemble_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/iqn_q_function.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/iqn_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/mean_q_function.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/mean_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/qr_q_function.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/qr_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/q_functions/utility.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/q_functions/utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/transformers.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,37 +173,25 @@
         return self._embed(t)
 
 
 class GlobalPositionEncoding(PositionEncoding):
     def __init__(self, embed_dim: int, max_timestep: int, context_size: int):
         super().__init__()
         self._embed_dim = embed_dim
-        self._global_position_embedding = Parameter(
-            torch.zeros(1, max_timestep, embed_dim, dtype=torch.float32)
-        )
+        self._global_position_embedding = nn.Embedding(max_timestep, embed_dim)
         self._block_position_embedding = Parameter(
             torch.zeros(1, 3 * context_size, embed_dim, dtype=torch.float32)
         )
 
     def forward(self, t: torch.Tensor) -> torch.Tensor:
         assert t.dim() == 2, "Expects (B, T)"
-        batch_size, context_size = t.shape
+        _, context_size = t.shape
 
-        # (B, 1, 1) -> (B, 1, N)
-        last_t = torch.repeat_interleave(
-            t[:, -1].view(-1, 1, 1), self._embed_dim, dim=-1
-        )
-        # (1, Tmax, N) -> (B, Tmax, N)
-        batched_global_embedding = torch.repeat_interleave(
-            get_parameter(self._global_position_embedding),
-            batch_size,
-            dim=0,
-        )
-        # (B, Tmax, N) -> (B, 1, N)
-        global_embedding = torch.gather(batched_global_embedding, 1, last_t)
+        # (B, 1) -> (B, 1, N)
+        global_embedding = self._global_position_embedding(t[:, -1:])
 
         # (1, 3 * Cmax, N) -> (1, T, N)
         block_embedding = get_parameter(self._block_position_embedding)[
             :, :context_size, :
         ]
 
         # (B, 1, N) + (1, T, N) -> (B, T, N)
```

### Comparing `d3rlpy-2.4.0/d3rlpy/models/torch/v_functions.py` & `d3rlpy-2.5.0/d3rlpy/models/torch/v_functions.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/models/utility.py` & `d3rlpy-2.5.0/d3rlpy/models/utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/notebook_utils.py` & `d3rlpy-2.5.0/d3rlpy/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/ope/fqe.py` & `d3rlpy-2.5.0/d3rlpy/ope/fqe.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/ope/torch/fqe_impl.py` & `d3rlpy-2.5.0/d3rlpy/ope/torch/fqe_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/preprocessing/action_scalers.py` & `d3rlpy-2.5.0/d3rlpy/preprocessing/action_scalers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/preprocessing/base.py` & `d3rlpy-2.5.0/d3rlpy/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/preprocessing/observation_scalers.py` & `d3rlpy-2.5.0/d3rlpy/preprocessing/observation_scalers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/preprocessing/reward_scalers.py` & `d3rlpy-2.5.0/d3rlpy/preprocessing/reward_scalers.py`

 * *Files 3% similar despite different names*

```diff
@@ -448,17 +448,21 @@
 
     References:
         * `Kostrikov et al., Offline Reinforcement Learning with Implicit
           Q-Learning. <https://arxiv.org/abs/2110.06169>`_
 
     Args:
         shift (float): Constant shift value
+        multiplier (float): Constant multiplication value.
+        multiply_first (bool): Flag to multiply rewards and then shift.
     """
 
     shift: float
+    multiplier: float = 1.0
+    multiply_first: bool = False
 
     def fit_with_transition_picker(
         self,
         episodes: Sequence[EpisodeBase],
         transition_picker: TransitionPickerProtocol,
     ) -> None:
         pass
@@ -467,24 +471,36 @@
         self,
         episodes: Sequence[EpisodeBase],
         trajectory_slicer: TrajectorySlicerProtocol,
     ) -> None:
         pass
 
     def transform(self, x: torch.Tensor) -> torch.Tensor:
-        return self.shift + x
+        if self.multiply_first:
+            return x * self.multiplier + self.shift
+        else:
+            return (self.shift + x) * self.multiplier
 
     def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
-        return x - self.shift
+        if self.multiply_first:
+            return (x - self.shift) / self.multiplier
+        else:
+            return x / self.multiplier - self.shift
 
     def transform_numpy(self, x: NDArray) -> NDArray:
-        return self.shift + x
+        if self.multiply_first:
+            return x * self.multiplier + self.shift
+        else:
+            return (self.shift + x) * self.multiplier
 
     def reverse_transform_numpy(self, x: NDArray) -> NDArray:
-        return x - self.shift
+        if self.multiply_first:
+            return (x - self.shift) / self.multiplier
+        else:
+            return x / self.multiplier - self.shift
 
     @staticmethod
     def get_type() -> str:
         return "shift"
 
     @property
     def built(self) -> bool:
```

### Comparing `d3rlpy-2.4.0/d3rlpy/serializable_config.py` & `d3rlpy-2.5.0/d3rlpy/serializable_config.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/tokenizers/tokenizers.py` & `d3rlpy-2.5.0/d3rlpy/tokenizers/tokenizers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/tokenizers/utils.py` & `d3rlpy-2.5.0/d3rlpy/tokenizers/utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy/torch_utility.py` & `d3rlpy-2.5.0/d3rlpy/torch_utility.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.optim import Optimizer
 from typing_extensions import Self
 
 from .dataclass_utils import asdict_without_copy
 from .dataset import TrajectoryMiniBatch, TransitionMiniBatch
 from .preprocessing import ActionScaler, ObservationScaler, RewardScaler
-from .types import NDArray, TorchObservation
+from .types import Float32NDArray, NDArray, TorchObservation
 
 __all__ = [
     "soft_sync",
     "hard_sync",
     "sync_optimizer_state",
     "map_location",
     "TorchMiniBatch",
@@ -152,14 +152,31 @@
         reshaped_x = x.view(x.shape[0], 1, *x.shape[1:])
         # (batch_sie, 1, M) -> (batch_size, N, M)
         return reshaped_x.expand(x.shape[0], n, *x.shape[1:])
     else:
         return [expand_and_repeat_recursively(_x, n) for _x in x]
 
 
+def _compute_return_to_go(
+    gamma: float,
+    rewards_to_go: Float32NDArray,
+    reward_scaler: Optional[RewardScaler],
+) -> Float32NDArray:
+    rewards = (
+        reward_scaler.transform_numpy(rewards_to_go)
+        if reward_scaler
+        else rewards_to_go
+    )
+    cum_gammas: Float32NDArray = np.array(
+        np.expand_dims(gamma ** np.arange(rewards.shape[0]), axis=1),
+        dtype=np.float32,
+    )
+    return np.sum(cum_gammas * rewards, axis=0)  # type: ignore
+
+
 @dataclasses.dataclass(frozen=True)
 class TorchMiniBatch:
     observations: TorchObservation
     actions: torch.Tensor
     rewards: torch.Tensor
     next_observations: TorchObservation
     returns_to_go: torch.Tensor
@@ -168,40 +185,56 @@
     device: str
     numpy_batch: Optional[TransitionMiniBatch] = None
 
     @classmethod
     def from_batch(
         cls,
         batch: TransitionMiniBatch,
+        gamma: float,
+        compute_returns_to_go: bool,
         device: str,
         observation_scaler: Optional[ObservationScaler] = None,
         action_scaler: Optional[ActionScaler] = None,
         reward_scaler: Optional[RewardScaler] = None,
     ) -> "TorchMiniBatch":
         # convert numpy array to torch tensor
         observations = convert_to_torch_recursively(batch.observations, device)
         actions = convert_to_torch(batch.actions, device)
         rewards = convert_to_torch(batch.rewards, device)
         next_observations = convert_to_torch_recursively(
             batch.next_observations, device
         )
-        returns_to_go = convert_to_torch(batch.returns_to_go, device)
         terminals = convert_to_torch(batch.terminals, device)
         intervals = convert_to_torch(batch.intervals, device)
 
+        if compute_returns_to_go:
+            returns_to_go = convert_to_torch(
+                np.array(
+                    [
+                        _compute_return_to_go(
+                            gamma=gamma,
+                            rewards_to_go=transition.rewards_to_go,
+                            reward_scaler=reward_scaler,
+                        )
+                        for transition in batch.transitions
+                    ]
+                ),
+                device,
+            )
+        else:
+            returns_to_go = torch.zeros_like(rewards)
+
         # apply scaler
         if observation_scaler:
             observations = observation_scaler.transform(observations)
             next_observations = observation_scaler.transform(next_observations)
         if action_scaler:
             actions = action_scaler.transform(actions)
         if reward_scaler:
             rewards = reward_scaler.transform(rewards)
-            # NOTE: some operations might be incompatible with returns
-            returns_to_go = reward_scaler.transform(returns_to_go)
 
         return TorchMiniBatch(
             observations=observations,
             actions=actions,
             rewards=rewards,
             next_observations=next_observations,
             returns_to_go=returns_to_go,
```

### Comparing `d3rlpy-2.4.0/d3rlpy/types.py` & `d3rlpy-2.5.0/d3rlpy/types.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.4.0/d3rlpy.egg-info/PKG-INFO` & `d3rlpy-2.5.0/d3rlpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d3rlpy
-Version: 2.4.0
+Version: 2.5.0
 Summary: An offline deep reinforcement learning library
 Home-page: https://github.com/takuseno/d3rlpy
 Author: Takuma Seno
 Author-email: takuma.seno@gmail.com
 License: MIT License
 Description: <p align="center"><img align="center" width="300px" src="assets/logo.png"></p>
         
@@ -92,14 +92,15 @@
         | [Bootstrapping Error Accumulation Reduction (BEAR)](https://arxiv.org/abs/1906.00949) | :no_entry: | :white_check_mark: |
         | [Conservative Q-Learning (CQL)](https://arxiv.org/abs/2006.04779) | :white_check_mark: | :white_check_mark: |
         | [Advantage Weighted Actor-Critic (AWAC)](https://arxiv.org/abs/2006.09359) | :no_entry: | :white_check_mark: |
         | [Critic Reguralized Regression (CRR)](https://arxiv.org/abs/2006.15134) | :no_entry: | :white_check_mark: |
         | [Policy in Latent Action Space (PLAS)](https://arxiv.org/abs/2011.07213) | :no_entry: | :white_check_mark: |
         | [TD3+BC](https://arxiv.org/abs/2106.06860) | :no_entry: | :white_check_mark: |
         | [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169) | :no_entry: | :white_check_mark: |
+        | [Calibrated Q-Learning (Cal-QL)](https://arxiv.org/abs/2303.05479) | :no_entry: | :white_check_mark: |
         | [Decision Transformer](https://arxiv.org/abs/2106.01345) | :white_check_mark: | :white_check_mark: |
         | [Gato](https://arxiv.org/abs/2205.06175) | :construction: | :construction: |
         
         ## Supported Q functions
         - [x] standard Q function
         - [x] [Quantile Regression](https://arxiv.org/abs/1710.10044)
         - [x] [Implicit Quantile Network](https://arxiv.org/abs/1806.06923)
@@ -194,14 +195,17 @@
         Please check the [contribution guide](CONTRIBUTING.md).
         
         ## Community
         | Channel | Link |
         |:-|:-|
         | Issues | [GitHub Issues](https://github.com/takuseno/d3rlpy/issues) |
         
+        > [!IMPORTANT]
+        > Please do NOT email to any contributors including the owner of this project to ask for technical support. Such emails will be ignored without replying to your message. Use GitHub Issues to report your problems.
+        
         ## Projects using d3rlpy
         | Project | Description |
         |:-:|:-|
         | [MINERVA](https://github.com/takuseno/minerva) | An out-of-the-box GUI tool for offline RL |
         | [SCOPE-RL](https://github.com/hakuhodo-technologies/scope-rl) | An off-policy evaluation and selection library |
         
         ## Roadmap
```

### Comparing `d3rlpy-2.4.0/d3rlpy.egg-info/SOURCES.txt` & `d3rlpy-2.5.0/d3rlpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 d3rlpy/algos/utility.py
 d3rlpy/algos/qlearning/__init__.py
 d3rlpy/algos/qlearning/awac.py
 d3rlpy/algos/qlearning/base.py
 d3rlpy/algos/qlearning/bc.py
 d3rlpy/algos/qlearning/bcq.py
 d3rlpy/algos/qlearning/bear.py
+d3rlpy/algos/qlearning/cal_ql.py
 d3rlpy/algos/qlearning/cql.py
 d3rlpy/algos/qlearning/crr.py
 d3rlpy/algos/qlearning/ddpg.py
 d3rlpy/algos/qlearning/dqn.py
 d3rlpy/algos/qlearning/explorers.py
 d3rlpy/algos/qlearning/iql.py
 d3rlpy/algos/qlearning/nfq.py
@@ -44,14 +45,15 @@
 d3rlpy/algos/qlearning/td3.py
 d3rlpy/algos/qlearning/td3_plus_bc.py
 d3rlpy/algos/qlearning/torch/__init__.py
 d3rlpy/algos/qlearning/torch/awac_impl.py
 d3rlpy/algos/qlearning/torch/bc_impl.py
 d3rlpy/algos/qlearning/torch/bcq_impl.py
 d3rlpy/algos/qlearning/torch/bear_impl.py
+d3rlpy/algos/qlearning/torch/cal_ql_impl.py
 d3rlpy/algos/qlearning/torch/cql_impl.py
 d3rlpy/algos/qlearning/torch/crr_impl.py
 d3rlpy/algos/qlearning/torch/ddpg_impl.py
 d3rlpy/algos/qlearning/torch/dqn_impl.py
 d3rlpy/algos/qlearning/torch/iql_impl.py
 d3rlpy/algos/qlearning/torch/plas_impl.py
 d3rlpy/algos/qlearning/torch/sac_impl.py
```

### Comparing `d3rlpy-2.4.0/setup.py` & `d3rlpy-2.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             "Programming Language :: Python :: Implementation :: CPython",
             "Operating System :: POSIX :: Linux",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: MacOS :: MacOS X",
         ],
         install_requires=[
             "torch>=2.0.0",
-            "tqdm",
+            "tqdm>=4.66.3",
             "h5py",
             "gym>=0.26.0",
             "click",
             "typing-extensions",
             "structlog",
             "colorama",
             "dataclasses-json",
```

