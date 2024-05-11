# Comparing `tmp/detrain-0.2.1.tar.gz` & `tmp/detrain-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detrain-0.2.1.tar", last modified: Wed May  8 14:13:19 2024, max compression
+gzip compressed data, was "detrain-0.2.2.tar", last modified: Sat May 11 07:57:33 2024, max compression
```

## Comparing `detrain-0.2.1.tar` & `detrain-0.2.2.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:19.177276 detrain-0.2.1/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3119 2024-05-08 14:13:19.162279 detrain-0.2.1/PKG-INFO
--rwxrwxrwx   0 levi      (1000) levi      (1000)       30 2024-05-06 03:34:32.000000 detrain-0.2.1/README.md
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2818 2024-05-08 14:12:37.000000 detrain-0.2.1/README.rst
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.048019 detrain-0.2.1/detrain/
--rwxrwxrwx   0 levi      (1000) levi      (1000)       27 2024-04-27 16:33:50.000000 detrain-0.2.1/detrain/__init__.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.378997 detrain-0.2.1/detrain/fsdp_tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 16:10:13.000000 detrain-0.2.1/detrain/fsdp_tp/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1516 2024-05-02 14:20:18.000000 detrain-0.2.1/detrain/fsdp_tp/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      621 2024-04-19 14:15:33.000000 detrain-0.2.1/detrain/fsdp_tp/log_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      775 2024-05-01 09:17:35.000000 detrain-0.2.1/detrain/fsdp_tp/mesh_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      481 2024-05-01 13:12:47.000000 detrain-0.2.1/detrain/fsdp_tp/model_2d.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      223 2024-05-01 07:57:12.000000 detrain-0.2.1/detrain/fsdp_tp/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      604 2024-05-02 14:13:20.000000 detrain-0.2.1/detrain/fsdp_tp/train_eval.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.619624 detrain-0.2.1/detrain/ppl/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 10:05:01.000000 detrain-0.2.1/detrain/ppl/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1165 2024-05-05 09:40:11.000000 detrain-0.2.1/detrain/ppl/args_util.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2561 2024-05-02 13:47:16.000000 detrain-0.2.1/detrain/ppl/dataset_util.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1659 2024-04-28 10:35:08.000000 detrain-0.2.1/detrain/ppl/dis_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      924 2024-04-27 10:26:45.000000 detrain-0.2.1/detrain/ppl/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      687 2024-05-06 13:50:36.000000 detrain-0.2.1/detrain/ppl/master_node.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      989 2024-04-27 10:22:26.000000 detrain-0.2.1/detrain/ppl/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1665 2024-05-06 14:21:52.000000 detrain-0.2.1/detrain/ppl/worker.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.797648 detrain-0.2.1/detrain/tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-29 08:57:33.000000 detrain-0.2.1/detrain/tp/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1502 2024-05-02 10:18:50.000000 detrain-0.2.1/detrain/tp/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      740 2024-05-02 10:25:59.000000 detrain-0.2.1/detrain/tp/model_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1453 2024-05-02 13:18:06.000000 detrain-0.2.1/detrain/tp/sequence_evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      718 2024-05-02 13:11:12.000000 detrain-0.2.1/detrain/tp/sequence_train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      584 2024-05-02 13:05:05.000000 detrain-0.2.1/detrain/tp/sequence_train_eval.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      715 2024-05-02 10:12:36.000000 detrain-0.2.1/detrain/tp/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      633 2024-05-02 08:52:58.000000 detrain-0.2.1/detrain/tp/train_eval.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:19.145277 detrain-0.2.1/detrain.egg-info/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3119 2024-05-08 14:13:17.000000 detrain-0.2.1/detrain.egg-info/PKG-INFO
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1203 2024-05-08 14:13:17.000000 detrain-0.2.1/detrain.egg-info/SOURCES.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        1 2024-05-08 14:13:17.000000 detrain-0.2.1/detrain.egg-info/dependency_links.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        6 2024-05-08 14:13:17.000000 detrain-0.2.1/detrain.egg-info/requires.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        8 2024-05-08 14:13:17.000000 detrain-0.2.1/detrain.egg-info/top_level.txt
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:17.983546 detrain-0.2.1/examples/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.842462 detrain-0.2.1/examples/fsdp_tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-01 10:21:53.000000 detrain-0.2.1/examples/fsdp_tp/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1755 2024-05-02 14:10:06.000000 detrain-0.2.1/examples/fsdp_tp/main.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:17.978360 detrain-0.2.1/examples/ppl/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.916687 detrain-0.2.1/examples/ppl/nn/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      465 2024-04-28 10:05:35.000000 detrain-0.2.1/examples/ppl/nn/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1635 2024-05-06 15:41:05.000000 detrain-0.2.1/examples/ppl/nn/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1324 2024-05-06 14:20:43.000000 detrain-0.2.1/examples/ppl/nn/shards_model.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:18.993920 detrain-0.2.1/examples/ppl/restnet/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1945 2024-04-27 15:25:16.000000 detrain-0.2.1/examples/ppl/restnet/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1492 2024-04-28 08:27:27.000000 detrain-0.2.1/examples/ppl/restnet/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2158 2024-04-27 15:06:01.000000 detrain-0.2.1/examples/ppl/restnet/shards_model.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:17.986046 detrain-0.2.1/examples/tp/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:19.092301 detrain-0.2.1/examples/tp/nn/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-02 13:04:02.000000 detrain-0.2.1/examples/tp/nn/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1892 2024-05-05 09:39:53.000000 detrain-0.2.1/examples/tp/nn/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      606 2024-04-29 15:44:14.000000 detrain-0.2.1/examples/tp/nn/rdz.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1834 2024-05-02 13:57:48.000000 detrain-0.2.1/examples/tp/nn/sequence_main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      677 2024-05-08 14:12:57.000000 detrain-0.2.1/pyproject.toml
--rwxrwxrwx   0 levi      (1000) levi      (1000)       38 2024-05-08 14:13:19.178275 detrain-0.2.1/setup.cfg
--rwxrwxrwx   0 levi      (1000) levi      (1000)      243 2024-05-08 08:08:37.000000 detrain-0.2.1/setup.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-08 14:13:19.111268 detrain-0.2.1/tests/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      512 2024-05-08 10:13:37.000000 detrain-0.2.1/tests/test_dataset.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.679732 detrain-0.2.2/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3119 2024-05-11 07:57:33.678512 detrain-0.2.2/PKG-INFO
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       30 2024-05-06 03:34:32.000000 detrain-0.2.2/README.md
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2818 2024-05-08 14:12:37.000000 detrain-0.2.2/README.rst
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.389914 detrain-0.2.2/detrain/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       27 2024-04-27 16:33:50.000000 detrain-0.2.2/detrain/__init__.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.681295 detrain-0.2.2/detrain/fsdp_tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 16:10:13.000000 detrain-0.2.2/detrain/fsdp_tp/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1516 2024-05-02 14:20:18.000000 detrain-0.2.2/detrain/fsdp_tp/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      621 2024-04-19 14:15:33.000000 detrain-0.2.2/detrain/fsdp_tp/log_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      775 2024-05-01 09:17:35.000000 detrain-0.2.2/detrain/fsdp_tp/mesh_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      481 2024-05-01 13:12:47.000000 detrain-0.2.2/detrain/fsdp_tp/model_2d.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      223 2024-05-01 07:57:12.000000 detrain-0.2.2/detrain/fsdp_tp/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      604 2024-05-02 14:13:20.000000 detrain-0.2.2/detrain/fsdp_tp/train_eval.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.912232 detrain-0.2.2/detrain/ppl/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 10:05:01.000000 detrain-0.2.2/detrain/ppl/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1026 2024-05-11 07:49:01.000000 detrain-0.2.2/detrain/ppl/args_util.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2561 2024-05-02 13:47:16.000000 detrain-0.2.2/detrain/ppl/dataset_util.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1659 2024-04-28 10:35:08.000000 detrain-0.2.2/detrain/ppl/dis_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      924 2024-04-27 10:26:45.000000 detrain-0.2.2/detrain/ppl/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      687 2024-05-06 13:50:36.000000 detrain-0.2.2/detrain/ppl/master_node.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      989 2024-04-27 10:22:26.000000 detrain-0.2.2/detrain/ppl/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1665 2024-05-06 14:21:52.000000 detrain-0.2.2/detrain/ppl/worker.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.167726 detrain-0.2.2/detrain/tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-29 08:57:33.000000 detrain-0.2.2/detrain/tp/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1502 2024-05-02 10:18:50.000000 detrain-0.2.2/detrain/tp/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      740 2024-05-02 10:25:59.000000 detrain-0.2.2/detrain/tp/model_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1453 2024-05-02 13:18:06.000000 detrain-0.2.2/detrain/tp/sequence_evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      718 2024-05-02 13:11:12.000000 detrain-0.2.2/detrain/tp/sequence_train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      584 2024-05-02 13:05:05.000000 detrain-0.2.2/detrain/tp/sequence_train_eval.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      715 2024-05-02 10:12:36.000000 detrain-0.2.2/detrain/tp/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      633 2024-05-02 08:52:58.000000 detrain-0.2.2/detrain/tp/train_eval.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.661949 detrain-0.2.2/detrain.egg-info/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3119 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/PKG-INFO
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1203 2024-05-11 07:57:32.000000 detrain-0.2.2/detrain.egg-info/SOURCES.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        1 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/dependency_links.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        6 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/requires.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        8 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/top_level.txt
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.304439 detrain-0.2.2/examples/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.231366 detrain-0.2.2/examples/fsdp_tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-01 10:21:53.000000 detrain-0.2.2/examples/fsdp_tp/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1755 2024-05-02 14:10:06.000000 detrain-0.2.2/examples/fsdp_tp/main.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.298404 detrain-0.2.2/examples/ppl/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.334011 detrain-0.2.2/examples/ppl/nn/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      465 2024-04-28 10:05:35.000000 detrain-0.2.2/examples/ppl/nn/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1756 2024-05-11 04:27:07.000000 detrain-0.2.2/examples/ppl/nn/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1324 2024-05-06 14:20:43.000000 detrain-0.2.2/examples/ppl/nn/shards_model.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.450172 detrain-0.2.2/examples/ppl/restnet/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1945 2024-04-27 15:25:16.000000 detrain-0.2.2/examples/ppl/restnet/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1492 2024-04-28 08:27:27.000000 detrain-0.2.2/examples/ppl/restnet/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2158 2024-04-27 15:06:01.000000 detrain-0.2.2/examples/ppl/restnet/shards_model.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.307451 detrain-0.2.2/examples/tp/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.599054 detrain-0.2.2/examples/tp/nn/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-02 13:04:02.000000 detrain-0.2.2/examples/tp/nn/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1892 2024-05-05 09:39:53.000000 detrain-0.2.2/examples/tp/nn/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      606 2024-04-29 15:44:14.000000 detrain-0.2.2/examples/tp/nn/rdz.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1834 2024-05-02 13:57:48.000000 detrain-0.2.2/examples/tp/nn/sequence_main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      677 2024-05-11 07:57:17.000000 detrain-0.2.2/pyproject.toml
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       38 2024-05-11 07:57:33.679732 detrain-0.2.2/setup.cfg
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      243 2024-05-11 07:57:22.000000 detrain-0.2.2/setup.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.630319 detrain-0.2.2/tests/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      512 2024-05-08 10:13:37.000000 detrain-0.2.2/tests/test_dataset.py
```

### Comparing `detrain-0.2.1/PKG-INFO` & `detrain-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detrain
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for distributed training & model parallelism using Torch
 Author: A2N Finance
 Author-email: Levi <levi@a2n.finance>, John <john@a2n.finance>
 License: MIT
 Keywords: torch,model parallelism,pipeline,tensor
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `detrain-0.2.1/README.rst` & `detrain-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/fsdp_tp/evaluation.py` & `detrain-0.2.2/detrain/fsdp_tp/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/fsdp_tp/log_utils.py` & `detrain-0.2.2/detrain/fsdp_tp/log_utils.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/fsdp_tp/mesh_utils.py` & `detrain-0.2.2/detrain/fsdp_tp/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/fsdp_tp/train_eval.py` & `detrain-0.2.2/detrain/fsdp_tp/train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/ppl/args_util.py` & `detrain-0.2.2/detrain/ppl/args_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,11 @@
     parser.add_argument("--split_size", default=2, type=int, help="Number of parts of the input data")
     parser.add_argument('--log', default=None, type=int, 
                         help='Enable training logs, this action can affect to training process performance')
     ## Optimizer settings
     parser.add_argument('--lr', default=1e-3, type=float, help='learning rate')
 
     ## Cluster settings
-    parser.add_argument('--gpu', default=None, type=int)
-    # parser.add_argument('--local_rank', default=-1, type=int, 
-    #                     help='local rank for distributed training')
+    parser.add_argument('--gpu', default=None, type=str)
     parser.add_argument("--model_name", default="trained_model", type=str, help='Name of the trained model to be saved')
-
     args = parser.parse_args()
     return args
```

### Comparing `detrain-0.2.1/detrain/ppl/dataset_util.py` & `detrain-0.2.2/detrain/ppl/dataset_util.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/ppl/dis_model.py` & `detrain-0.2.2/detrain/ppl/dis_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/ppl/evaluation.py` & `detrain-0.2.2/detrain/ppl/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/ppl/master_node.py` & `detrain-0.2.2/detrain/ppl/master_node.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/ppl/train.py` & `detrain-0.2.2/detrain/ppl/train.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/ppl/worker.py` & `detrain-0.2.2/detrain/ppl/worker.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/evaluation.py` & `detrain-0.2.2/detrain/tp/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/model_utils.py` & `detrain-0.2.2/detrain/tp/model_utils.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/sequence_evaluation.py` & `detrain-0.2.2/detrain/tp/sequence_evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/sequence_train.py` & `detrain-0.2.2/detrain/tp/sequence_train.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/sequence_train_eval.py` & `detrain-0.2.2/detrain/tp/sequence_train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/train.py` & `detrain-0.2.2/detrain/tp/train.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain/tp/train_eval.py` & `detrain-0.2.2/detrain/tp/train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/detrain.egg-info/PKG-INFO` & `detrain-0.2.2/detrain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detrain
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for distributed training & model parallelism using Torch
 Author: A2N Finance
 Author-email: Levi <levi@a2n.finance>, John <john@a2n.finance>
 License: MIT
 Keywords: torch,model parallelism,pipeline,tensor
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `detrain-0.2.1/detrain.egg-info/SOURCES.txt` & `detrain-0.2.2/detrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/fsdp_tp/base_model.py` & `detrain-0.2.2/examples/fsdp_tp/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/fsdp_tp/main.py` & `detrain-0.2.2/examples/fsdp_tp/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/ppl/nn/main.py` & `detrain-0.2.2/examples/ppl/nn/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import torch.nn as nn
+import torch
 import time
 import os
 from detrain.ppl.args_util import get_args
 from detrain.ppl.worker import run_worker
 from detrain.ppl.dataset_util import get_torchvision_dataset
 from shards_model import NNShard1, NNShard2
 from torch.distributed.optim.optimizer import DistributedOptimizer
@@ -20,16 +21,20 @@
     epochs = int(args.epochs)
     batch_size = int(args.batch_size)
     lr = float(args.lr)
     device = "cpu"
 
     # Check devices
     if (args.gpu is not None):
-        device = "cuda:0"
+        device = "cuda"
+
+    for i in range(torch.cuda.device_count()):
+        print(torch.cuda.get_device_properties(i).name)
     
+
     # Define optimizer & loss_fn
     loss_fn = nn.CrossEntropyLoss()
     optimizer_class = optim.SGD
     
     # Dataloaders
 
     (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
```

### Comparing `detrain-0.2.1/examples/ppl/nn/shards_model.py` & `detrain-0.2.2/examples/ppl/nn/shards_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/ppl/restnet/base_model.py` & `detrain-0.2.2/examples/ppl/restnet/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/ppl/restnet/main.py` & `detrain-0.2.2/examples/ppl/restnet/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/ppl/restnet/shards_model.py` & `detrain-0.2.2/examples/ppl/restnet/shards_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/tp/nn/base_model.py` & `detrain-0.2.2/examples/tp/nn/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/tp/nn/main.py` & `detrain-0.2.2/examples/tp/nn/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/tp/nn/rdz.py` & `detrain-0.2.2/examples/tp/nn/rdz.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/examples/tp/nn/sequence_main.py` & `detrain-0.2.2/examples/tp/nn/sequence_main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.1/pyproject.toml` & `detrain-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "detrain"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     {name = "Levi", email = "levi@a2n.finance"},
     {name = "John", email = "john@a2n.finance"},
 ]
 readme= "README.rst"
 description = "A package for distributed training & model parallelism using Torch"
 requires-python = ">=3.8"
```

### Comparing `detrain-0.2.1/tests/test_dataset.py` & `detrain-0.2.2/tests/test_dataset.py`

 * *Files identical despite different names*

