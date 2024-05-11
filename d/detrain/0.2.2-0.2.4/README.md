# Comparing `tmp/detrain-0.2.2.tar.gz` & `tmp/detrain-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detrain-0.2.2.tar", last modified: Sat May 11 07:57:33 2024, max compression
+gzip compressed data, was "detrain-0.2.4.tar", last modified: Sat May 11 08:21:22 2024, max compression
```

## Comparing `detrain-0.2.2.tar` & `detrain-0.2.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.679732 detrain-0.2.2/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3119 2024-05-11 07:57:33.678512 detrain-0.2.2/PKG-INFO
--rwxrwxrwx   0 levi      (1000) levi      (1000)       30 2024-05-06 03:34:32.000000 detrain-0.2.2/README.md
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2818 2024-05-08 14:12:37.000000 detrain-0.2.2/README.rst
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.389914 detrain-0.2.2/detrain/
--rwxrwxrwx   0 levi      (1000) levi      (1000)       27 2024-04-27 16:33:50.000000 detrain-0.2.2/detrain/__init__.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.681295 detrain-0.2.2/detrain/fsdp_tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 16:10:13.000000 detrain-0.2.2/detrain/fsdp_tp/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1516 2024-05-02 14:20:18.000000 detrain-0.2.2/detrain/fsdp_tp/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      621 2024-04-19 14:15:33.000000 detrain-0.2.2/detrain/fsdp_tp/log_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      775 2024-05-01 09:17:35.000000 detrain-0.2.2/detrain/fsdp_tp/mesh_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      481 2024-05-01 13:12:47.000000 detrain-0.2.2/detrain/fsdp_tp/model_2d.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      223 2024-05-01 07:57:12.000000 detrain-0.2.2/detrain/fsdp_tp/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      604 2024-05-02 14:13:20.000000 detrain-0.2.2/detrain/fsdp_tp/train_eval.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.912232 detrain-0.2.2/detrain/ppl/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 10:05:01.000000 detrain-0.2.2/detrain/ppl/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1026 2024-05-11 07:49:01.000000 detrain-0.2.2/detrain/ppl/args_util.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2561 2024-05-02 13:47:16.000000 detrain-0.2.2/detrain/ppl/dataset_util.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1659 2024-04-28 10:35:08.000000 detrain-0.2.2/detrain/ppl/dis_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      924 2024-04-27 10:26:45.000000 detrain-0.2.2/detrain/ppl/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      687 2024-05-06 13:50:36.000000 detrain-0.2.2/detrain/ppl/master_node.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      989 2024-04-27 10:22:26.000000 detrain-0.2.2/detrain/ppl/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1665 2024-05-06 14:21:52.000000 detrain-0.2.2/detrain/ppl/worker.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.167726 detrain-0.2.2/detrain/tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-29 08:57:33.000000 detrain-0.2.2/detrain/tp/__init__.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1502 2024-05-02 10:18:50.000000 detrain-0.2.2/detrain/tp/evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      740 2024-05-02 10:25:59.000000 detrain-0.2.2/detrain/tp/model_utils.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1453 2024-05-02 13:18:06.000000 detrain-0.2.2/detrain/tp/sequence_evaluation.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      718 2024-05-02 13:11:12.000000 detrain-0.2.2/detrain/tp/sequence_train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      584 2024-05-02 13:05:05.000000 detrain-0.2.2/detrain/tp/sequence_train_eval.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      715 2024-05-02 10:12:36.000000 detrain-0.2.2/detrain/tp/train.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      633 2024-05-02 08:52:58.000000 detrain-0.2.2/detrain/tp/train_eval.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.661949 detrain-0.2.2/detrain.egg-info/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     3119 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/PKG-INFO
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1203 2024-05-11 07:57:32.000000 detrain-0.2.2/detrain.egg-info/SOURCES.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        1 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/dependency_links.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        6 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/requires.txt
--rwxrwxrwx   0 levi      (1000) levi      (1000)        8 2024-05-11 07:57:31.000000 detrain-0.2.2/detrain.egg-info/top_level.txt
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.304439 detrain-0.2.2/examples/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.231366 detrain-0.2.2/examples/fsdp_tp/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-01 10:21:53.000000 detrain-0.2.2/examples/fsdp_tp/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1755 2024-05-02 14:10:06.000000 detrain-0.2.2/examples/fsdp_tp/main.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.298404 detrain-0.2.2/examples/ppl/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.334011 detrain-0.2.2/examples/ppl/nn/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      465 2024-04-28 10:05:35.000000 detrain-0.2.2/examples/ppl/nn/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1756 2024-05-11 04:27:07.000000 detrain-0.2.2/examples/ppl/nn/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1324 2024-05-06 14:20:43.000000 detrain-0.2.2/examples/ppl/nn/shards_model.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.450172 detrain-0.2.2/examples/ppl/restnet/
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1945 2024-04-27 15:25:16.000000 detrain-0.2.2/examples/ppl/restnet/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1492 2024-04-28 08:27:27.000000 detrain-0.2.2/examples/ppl/restnet/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     2158 2024-04-27 15:06:01.000000 detrain-0.2.2/examples/ppl/restnet/shards_model.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:32.307451 detrain-0.2.2/examples/tp/
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.599054 detrain-0.2.2/examples/tp/nn/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-02 13:04:02.000000 detrain-0.2.2/examples/tp/nn/base_model.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1892 2024-05-05 09:39:53.000000 detrain-0.2.2/examples/tp/nn/main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      606 2024-04-29 15:44:14.000000 detrain-0.2.2/examples/tp/nn/rdz.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)     1834 2024-05-02 13:57:48.000000 detrain-0.2.2/examples/tp/nn/sequence_main.py
--rwxrwxrwx   0 levi      (1000) levi      (1000)      677 2024-05-11 07:57:17.000000 detrain-0.2.2/pyproject.toml
--rwxrwxrwx   0 levi      (1000) levi      (1000)       38 2024-05-11 07:57:33.679732 detrain-0.2.2/setup.cfg
--rwxrwxrwx   0 levi      (1000) levi      (1000)      243 2024-05-11 07:57:22.000000 detrain-0.2.2/setup.py
-drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 07:57:33.630319 detrain-0.2.2/tests/
--rwxrwxrwx   0 levi      (1000) levi      (1000)      512 2024-05-08 10:13:37.000000 detrain-0.2.2/tests/test_dataset.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.697985 detrain-0.2.4/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3485 2024-05-11 08:21:22.683593 detrain-0.2.4/PKG-INFO
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       30 2024-05-06 03:34:32.000000 detrain-0.2.4/README.md
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3198 2024-05-11 08:15:14.000000 detrain-0.2.4/README.rst
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.113057 detrain-0.2.4/detrain/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       27 2024-04-27 16:33:50.000000 detrain-0.2.4/detrain/__init__.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.423014 detrain-0.2.4/detrain/fsdp_tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 16:10:13.000000 detrain-0.2.4/detrain/fsdp_tp/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1516 2024-05-02 14:20:18.000000 detrain-0.2.4/detrain/fsdp_tp/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      621 2024-04-19 14:15:33.000000 detrain-0.2.4/detrain/fsdp_tp/log_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      775 2024-05-01 09:17:35.000000 detrain-0.2.4/detrain/fsdp_tp/mesh_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      481 2024-05-01 13:12:47.000000 detrain-0.2.4/detrain/fsdp_tp/model_2d.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      223 2024-05-01 07:57:12.000000 detrain-0.2.4/detrain/fsdp_tp/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      604 2024-05-02 14:13:20.000000 detrain-0.2.4/detrain/fsdp_tp/train_eval.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.660915 detrain-0.2.4/detrain/ppl/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-27 10:05:01.000000 detrain-0.2.4/detrain/ppl/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1026 2024-05-11 07:49:01.000000 detrain-0.2.4/detrain/ppl/args_util.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2561 2024-05-02 13:47:16.000000 detrain-0.2.4/detrain/ppl/dataset_util.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1659 2024-04-28 10:35:08.000000 detrain-0.2.4/detrain/ppl/dis_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      924 2024-04-27 10:26:45.000000 detrain-0.2.4/detrain/ppl/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      687 2024-05-06 13:50:36.000000 detrain-0.2.4/detrain/ppl/master_node.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      989 2024-04-27 10:22:26.000000 detrain-0.2.4/detrain/ppl/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1665 2024-05-06 14:21:52.000000 detrain-0.2.4/detrain/ppl/worker.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.988346 detrain-0.2.4/detrain/tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-04-29 08:57:33.000000 detrain-0.2.4/detrain/tp/__init__.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1502 2024-05-02 10:18:50.000000 detrain-0.2.4/detrain/tp/evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      740 2024-05-02 10:25:59.000000 detrain-0.2.4/detrain/tp/model_utils.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1453 2024-05-02 13:18:06.000000 detrain-0.2.4/detrain/tp/sequence_evaluation.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      718 2024-05-02 13:11:12.000000 detrain-0.2.4/detrain/tp/sequence_train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      584 2024-05-02 13:05:05.000000 detrain-0.2.4/detrain/tp/sequence_train_eval.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      715 2024-05-02 10:12:36.000000 detrain-0.2.4/detrain/tp/train.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      633 2024-05-02 08:52:58.000000 detrain-0.2.4/detrain/tp/train_eval.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.667995 detrain-0.2.4/detrain.egg-info/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     3485 2024-05-11 08:21:20.000000 detrain-0.2.4/detrain.egg-info/PKG-INFO
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1203 2024-05-11 08:21:20.000000 detrain-0.2.4/detrain.egg-info/SOURCES.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        1 2024-05-11 08:21:20.000000 detrain-0.2.4/detrain.egg-info/dependency_links.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        6 2024-05-11 08:21:20.000000 detrain-0.2.4/detrain.egg-info/requires.txt
+-rwxrwxrwx   0 levi      (1000) levi      (1000)        8 2024-05-11 08:21:20.000000 detrain-0.2.4/detrain.egg-info/top_level.txt
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.025924 detrain-0.2.4/examples/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.067448 detrain-0.2.4/examples/fsdp_tp/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-01 10:21:53.000000 detrain-0.2.4/examples/fsdp_tp/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1755 2024-05-02 14:10:06.000000 detrain-0.2.4/examples/fsdp_tp/main.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.019091 detrain-0.2.4/examples/ppl/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.239884 detrain-0.2.4/examples/ppl/nn/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      465 2024-04-28 10:05:35.000000 detrain-0.2.4/examples/ppl/nn/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1756 2024-05-11 04:27:07.000000 detrain-0.2.4/examples/ppl/nn/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1324 2024-05-06 14:20:43.000000 detrain-0.2.4/examples/ppl/nn/shards_model.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.384237 detrain-0.2.4/examples/ppl/restnet/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1945 2024-04-27 15:25:16.000000 detrain-0.2.4/examples/ppl/restnet/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1492 2024-04-28 08:27:27.000000 detrain-0.2.4/examples/ppl/restnet/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     2158 2024-04-27 15:06:01.000000 detrain-0.2.4/examples/ppl/restnet/shards_model.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:21.028936 detrain-0.2.4/examples/tp/
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.590867 detrain-0.2.4/examples/tp/nn/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      582 2024-05-02 13:04:02.000000 detrain-0.2.4/examples/tp/nn/base_model.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1892 2024-05-05 09:39:53.000000 detrain-0.2.4/examples/tp/nn/main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      606 2024-04-29 15:44:14.000000 detrain-0.2.4/examples/tp/nn/rdz.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)     1834 2024-05-02 13:57:48.000000 detrain-0.2.4/examples/tp/nn/sequence_main.py
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      677 2024-05-11 08:21:01.000000 detrain-0.2.4/pyproject.toml
+-rwxrwxrwx   0 levi      (1000) levi      (1000)       38 2024-05-11 08:21:22.699983 detrain-0.2.4/setup.cfg
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      243 2024-05-11 08:21:07.000000 detrain-0.2.4/setup.py
+drwxrwxrwx   0 levi      (1000) levi      (1000)        0 2024-05-11 08:21:22.627493 detrain-0.2.4/tests/
+-rwxrwxrwx   0 levi      (1000) levi      (1000)      512 2024-05-08 10:13:37.000000 detrain-0.2.4/tests/test_dataset.py
```

### Comparing `detrain-0.2.2/PKG-INFO` & `detrain-0.2.4/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,115 +1,116 @@
-Metadata-Version: 2.1
-Name: detrain
-Version: 0.2.2
-Summary: A package for distributed training & model parallelism using Torch
-Author: A2N Finance
-Author-email: Levi <levi@a2n.finance>, John <john@a2n.finance>
-License: MIT
-Keywords: torch,model parallelism,pipeline,tensor
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Requires-Dist: torch
-
-==============
-DeTrain
-==============
-
-Overview
---------
-
-DeTrain is a Python package designed to train AI models using model parallelism methods. This package focuses on pipeline and tensor parallelism.
-
-Installation
-------------
-
-You can install DeTrain using pip:
-
-.. code-block:: sh
-
-    pip install detrain
-
-Usage
------
-
-Once installed, you can use DeTrain in your Python scripts like this:
-
-.. code-block:: python
-
-    import torch.nn as nn
-    import time
-    import os
-    from detrain.ppl.args_util import get_args
-    from detrain.ppl.worker import run_worker
-    from detrain.ppl.dataset_util import get_torchvision_dataset
-    from shards_model import NNShard1, NNShard2
-    from torch.distributed.optim.optimizer import DistributedOptimizer
-    import torch.optim as optim
-    if __name__=="__main__":
-        args = get_args()
-        # Get args
-        world_size = int(os.environ["WORLD_SIZE"])
-        rank = int(os.environ["RANK"])
-        epochs = int(args.epochs)
-        batch_size = int(args.batch_size)
-        lr = float(args.lr)
-        device = "cpu"
-
-        # Check devices
-        if (args.gpu is not None):
-            device = "cuda:0"
-        
-        # Define optimizer & loss_fn
-        loss_fn = nn.CrossEntropyLoss()
-        optimizer_class = optim.SGD
-        
-        # Dataloaders
-
-        (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
-
-        
-        print(f"World_size: {world_size}, Rank: {rank}")
-        num_split = 4
-        tik = time.time()
-        run_worker(
-            rank, 
-            world_size, 
-            (
-                args.split_size, 
-                ["worker1", "worker2"],
-                [device, device], 
-                [NNShard1, NNShard2]
-            ), 
-            train_dataloader, 
-            test_dataloader, 
-            loss_fn, 
-            optimizer_class, 
-            epochs, 
-            batch_size,
-            lr
-        )
-        tok = time.time()
-        print(f"number of splits = {num_split}, execution time = {tok - tik}")
-
-For detailed examples, please visit the `DeTrain examples <https://github.com/a2nfinance/detrain-example>`_.
-
-Contributing
-------------
-
-Contributions are welcome! If you'd like to contribute to DeTrain, please follow these steps:
-
-1. Fork the repository on GitHub.
-2. Create a new branch.
-3. Make your changes and commit them with clear descriptions.
-4. Push your changes to your fork.
-5. Submit a pull request.
-
-Bug Reports and Feedback
-------------------------
-
-If you encounter any bugs or have feedback, please open an issue on the GitHub repository.
-
-License
--------
-
-DeTrain is licensed under the MIT License. See the LICENSE file for more information.
+==============
+DeTrain
+==============
+
+Overview
+--------
+
+DeTrain is a Python package designed to train AI models using model parallelism methods. This package focuses on pipeline and tensor parallelism.
+
+Installation
+------------
+
+You can install DeTrain using pip:
+
+.. code-block:: sh
+
+    pip install detrain
+
+Usage
+-----
+
+Once installed, you can use DeTrain in your Python scripts like this:
+
+.. code-block:: python
+
+    import torch.nn as nn
+    import torch
+    import time
+    import os
+    from detrain.ppl.args_util import get_args
+    from detrain.ppl.worker import run_worker
+    from detrain.ppl.dataset_util import get_torchvision_dataset
+    from shards_model import NNShard1, NNShard2
+    import torch.optim as optim
+
+    if __name__=="__main__":
+        args = get_args()
+        # Get args
+        world_size = int(os.environ["WORLD_SIZE"])
+        rank = int(os.environ["RANK"])
+        epochs = int(args.epochs)
+        batch_size = int(args.batch_size)
+        lr = float(args.lr)
+
+        for i in range(torch.cuda.device_count()):
+            print(torch.cuda.get_device_properties(i).name)
+
+        devices = []
+        workers = []
+        shards = [NNShard1, NNShard2]
+        # Check devices
+        if (args.gpu is not None):
+            arr = args.gpu.split('_')
+            for dv in range(len(arr)):
+                if dv > 0:
+                    workers.append(f"worker{dv}")
+                    if int(arr[dv]) == 1:
+                        devices.append("cuda:0")
+                    else:
+                        devices.append("cpu")
+
+        # Define optimizer & loss_fn
+        loss_fn = nn.CrossEntropyLoss()
+        optimizer_class = optim.SGD
+        
+        # Dataloaders
+
+        (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
+
+        
+        print(f"World_size: {world_size}, Rank: {rank}")
+        
+        num_split = 4
+        tik = time.time()
+        run_worker(
+            rank, 
+            world_size, 
+            (
+                args.split_size, 
+                workers,
+                devices, 
+                shards
+            ), 
+            train_dataloader, 
+            test_dataloader, 
+            loss_fn, 
+            optimizer_class, 
+            epochs, 
+            batch_size,
+            lr
+        )
+        tok = time.time()
+        print(f"number of splits = {num_split}, execution time = {tok - tik}")
+
+For detailed examples, please visit the `DeTrain examples <https://github.com/a2nfinance/detrain-example>`_.
+
+Contributing
+------------
+
+Contributions are welcome! If you'd like to contribute to DeTrain, please follow these steps:
+
+1. Fork the repository on GitHub.
+2. Create a new branch.
+3. Make your changes and commit them with clear descriptions.
+4. Push your changes to your fork.
+5. Submit a pull request.
+
+Bug Reports and Feedback
+------------------------
+
+If you encounter any bugs or have feedback, please open an issue on the GitHub repository.
+
+License
+-------
+
+DeTrain is licensed under the MIT License. See the LICENSE file for more information.
```

### Comparing `detrain-0.2.2/README.rst` & `detrain-0.2.4/examples/tp/nn/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,102 +1,71 @@
-==============
-DeTrain
-==============
-
-Overview
---------
-
-DeTrain is a Python package designed to train AI models using model parallelism methods. This package focuses on pipeline and tensor parallelism.
-
-Installation
-------------
-
-You can install DeTrain using pip:
-
-.. code-block:: sh
-
-    pip install detrain
-
-Usage
------
-
-Once installed, you can use DeTrain in your Python scripts like this:
-
-.. code-block:: python
-
-    import torch.nn as nn
-    import time
-    import os
-    from detrain.ppl.args_util import get_args
-    from detrain.ppl.worker import run_worker
-    from detrain.ppl.dataset_util import get_torchvision_dataset
-    from shards_model import NNShard1, NNShard2
-    from torch.distributed.optim.optimizer import DistributedOptimizer
-    import torch.optim as optim
-    if __name__=="__main__":
-        args = get_args()
-        # Get args
-        world_size = int(os.environ["WORLD_SIZE"])
-        rank = int(os.environ["RANK"])
-        epochs = int(args.epochs)
-        batch_size = int(args.batch_size)
-        lr = float(args.lr)
-        device = "cpu"
-
-        # Check devices
-        if (args.gpu is not None):
-            device = "cuda:0"
-        
-        # Define optimizer & loss_fn
-        loss_fn = nn.CrossEntropyLoss()
-        optimizer_class = optim.SGD
-        
-        # Dataloaders
-
-        (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
-
-        
-        print(f"World_size: {world_size}, Rank: {rank}")
-        num_split = 4
-        tik = time.time()
-        run_worker(
-            rank, 
-            world_size, 
-            (
-                args.split_size, 
-                ["worker1", "worker2"],
-                [device, device], 
-                [NNShard1, NNShard2]
-            ), 
-            train_dataloader, 
-            test_dataloader, 
-            loss_fn, 
-            optimizer_class, 
-            epochs, 
-            batch_size,
-            lr
-        )
-        tok = time.time()
-        print(f"number of splits = {num_split}, execution time = {tok - tik}")
-
-For detailed examples, please visit the `DeTrain examples <https://github.com/a2nfinance/detrain-example>`_.
-
-Contributing
-------------
-
-Contributions are welcome! If you'd like to contribute to DeTrain, please follow these steps:
-
-1. Fork the repository on GitHub.
-2. Create a new branch.
-3. Make your changes and commit them with clear descriptions.
-4. Push your changes to your fork.
-5. Submit a pull request.
-
-Bug Reports and Feedback
-------------------------
-
-If you encounter any bugs or have feedback, please open an issue on the GitHub repository.
-
-License
--------
-
-DeTrain is licensed under the MIT License. See the LICENSE file for more information.
+import torch
+import torch.nn as nn
+import time
+import os
+from detrain.ppl.args_util import get_args
+from detrain.tp.train_eval import train_eval
+from detrain.tp.model_utils import get_tp_model, save_model
+from detrain.ppl.dataset_util import get_torchvision_dataset
+import torch.optim as optim
+from base_model import NeuralNetwork
+from torch.distributed.tensor.parallel import (
+    ColwiseParallel,
+    RowwiseParallel,
+)
+from torch.distributed._tensor import Shard
+
+if __name__=="__main__":
+    args = get_args()
+    world_size = int(os.environ["WORLD_SIZE"])
+    # Get args
+    epochs = int(args.epochs)
+    batch_size = int(args.batch_size)
+    lr = float(args.lr)
+    device = "cpu"
+
+    # Check devices
+    if (args.gpu is not None):
+        device = "cuda"
+    
+    # Define optimizer & loss_fn
+    loss_fn = nn.CrossEntropyLoss(reduction="mean")
+    optimizer_class = optim.SGD
+    model = NeuralNetwork().to(device)
+
+   
+    mesh_shape = (world_size, )
+    tp_model = get_tp_model(model, {
+        "in_proj": ColwiseParallel(
+            use_local_output=False,
+        ),
+        "linear1": RowwiseParallel(
+            use_local_output=False,
+        ),
+        "out_proj": ColwiseParallel(
+
+            use_local_output=False,
+        ),
+    } , device, mesh_shape)
+
+    
+    # Create an optimizer for the parallelized module.
+    optimizer = torch.optim.SGD(tp_model.parameters(), lr=lr)
+    
+    # Dataloaders
+
+    (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
+
+    tik = time.time()
+    train_eval(
+        tp_model, 
+        train_dataloader, 
+        test_dataloader, 
+        loss_fn, 
+        optimizer, 
+        epochs, 
+        batch_size,
+        device
+    )
+    tok = time.time()
+    print(f"Execution time = {tok - tik}")
+    save_model(model, args.model_name)
```

### Comparing `detrain-0.2.2/detrain/fsdp_tp/evaluation.py` & `detrain-0.2.4/detrain/fsdp_tp/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/fsdp_tp/log_utils.py` & `detrain-0.2.4/detrain/fsdp_tp/log_utils.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/fsdp_tp/mesh_utils.py` & `detrain-0.2.4/detrain/fsdp_tp/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/fsdp_tp/train_eval.py` & `detrain-0.2.4/detrain/fsdp_tp/train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/args_util.py` & `detrain-0.2.4/detrain/ppl/args_util.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/dataset_util.py` & `detrain-0.2.4/detrain/ppl/dataset_util.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/dis_model.py` & `detrain-0.2.4/detrain/ppl/dis_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/evaluation.py` & `detrain-0.2.4/detrain/ppl/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/master_node.py` & `detrain-0.2.4/detrain/ppl/master_node.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/train.py` & `detrain-0.2.4/detrain/ppl/train.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/ppl/worker.py` & `detrain-0.2.4/detrain/ppl/worker.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/evaluation.py` & `detrain-0.2.4/detrain/tp/evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/model_utils.py` & `detrain-0.2.4/detrain/tp/model_utils.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/sequence_evaluation.py` & `detrain-0.2.4/detrain/tp/sequence_evaluation.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/sequence_train.py` & `detrain-0.2.4/detrain/tp/sequence_train.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/sequence_train_eval.py` & `detrain-0.2.4/detrain/tp/sequence_train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/train.py` & `detrain-0.2.4/detrain/tp/train.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain/tp/train_eval.py` & `detrain-0.2.4/detrain/tp/train_eval.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/detrain.egg-info/PKG-INFO` & `detrain-0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detrain
-Version: 0.2.2
+Version: 0.2.4
 Summary: A package for distributed training & model parallelism using Torch
 Author: A2N Finance
 Author-email: Levi <levi@a2n.finance>, John <john@a2n.finance>
 License: MIT
 Keywords: torch,model parallelism,pipeline,tensor
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -33,56 +33,70 @@
 -----
 
 Once installed, you can use DeTrain in your Python scripts like this:
 
 .. code-block:: python
 
     import torch.nn as nn
+    import torch
     import time
     import os
     from detrain.ppl.args_util import get_args
     from detrain.ppl.worker import run_worker
     from detrain.ppl.dataset_util import get_torchvision_dataset
     from shards_model import NNShard1, NNShard2
-    from torch.distributed.optim.optimizer import DistributedOptimizer
     import torch.optim as optim
+
     if __name__=="__main__":
         args = get_args()
         # Get args
         world_size = int(os.environ["WORLD_SIZE"])
         rank = int(os.environ["RANK"])
         epochs = int(args.epochs)
         batch_size = int(args.batch_size)
         lr = float(args.lr)
-        device = "cpu"
 
+        for i in range(torch.cuda.device_count()):
+            print(torch.cuda.get_device_properties(i).name)
+
+        devices = []
+        workers = []
+        shards = [NNShard1, NNShard2]
         # Check devices
         if (args.gpu is not None):
-            device = "cuda:0"
-        
+            arr = args.gpu.split('_')
+            for dv in range(len(arr)):
+                if dv > 0:
+                    workers.append(f"worker{dv}")
+                    if int(arr[dv]) == 1:
+                        devices.append("cuda:0")
+                    else:
+                        devices.append("cpu")
+
         # Define optimizer & loss_fn
         loss_fn = nn.CrossEntropyLoss()
         optimizer_class = optim.SGD
         
         # Dataloaders
 
         (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
 
         
         print(f"World_size: {world_size}, Rank: {rank}")
+        
         num_split = 4
         tik = time.time()
         run_worker(
             rank, 
             world_size, 
             (
                 args.split_size, 
-                ["worker1", "worker2"],
-                [device, device], 
-                [NNShard1, NNShard2]
+                workers,
+                devices, 
+                shards
             ), 
             train_dataloader, 
             test_dataloader, 
             loss_fn, 
             optimizer_class, 
             epochs, 
             batch_size,
```

### Comparing `detrain-0.2.2/detrain.egg-info/SOURCES.txt` & `detrain-0.2.4/detrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/fsdp_tp/base_model.py` & `detrain-0.2.4/examples/fsdp_tp/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/fsdp_tp/main.py` & `detrain-0.2.4/examples/fsdp_tp/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/ppl/nn/main.py` & `detrain-0.2.4/examples/ppl/nn/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/ppl/nn/shards_model.py` & `detrain-0.2.4/examples/ppl/nn/shards_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/ppl/restnet/base_model.py` & `detrain-0.2.4/examples/ppl/restnet/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/ppl/restnet/main.py` & `detrain-0.2.4/examples/ppl/restnet/main.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/ppl/restnet/shards_model.py` & `detrain-0.2.4/examples/ppl/restnet/shards_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/tp/nn/base_model.py` & `detrain-0.2.4/examples/tp/nn/base_model.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/examples/tp/nn/main.py` & `detrain-0.2.4/examples/tp/nn/sequence_main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import torch.nn as nn
 import time
 import os
 from detrain.ppl.args_util import get_args
-from detrain.tp.train_eval import train_eval
-from detrain.tp.model_utils import get_tp_model, save_model
+from detrain.tp.sequence_train_eval import sequence_train_eval
+from detrain.tp.model_utils import get_tp_model
 from detrain.ppl.dataset_util import get_torchvision_dataset
 import torch.optim as optim
 from base_model import NeuralNetwork
 from torch.distributed.tensor.parallel import (
     ColwiseParallel,
     RowwiseParallel,
 )
@@ -24,48 +24,45 @@
     device = "cpu"
 
     # Check devices
     if (args.gpu is not None):
         device = "cuda"
     
     # Define optimizer & loss_fn
-    loss_fn = nn.CrossEntropyLoss(reduction="mean")
+    loss_fn = nn.CrossEntropyLoss()
     optimizer_class = optim.SGD
     model = NeuralNetwork().to(device)
 
-   
+
     mesh_shape = (world_size, )
-    tp_model = get_tp_model(model, {
+    sp_model = get_tp_model(model, {
         "in_proj": ColwiseParallel(
-            use_local_output=False,
+            input_layouts=Shard(0),
         ),
         "linear1": RowwiseParallel(
-            use_local_output=False,
+            
         ),
         "out_proj": ColwiseParallel(
-
-            use_local_output=False,
+            output_layouts=Shard(0),
         ),
     } , device, mesh_shape)
 
-    
     # Create an optimizer for the parallelized module.
-    optimizer = torch.optim.SGD(tp_model.parameters(), lr=lr)
+    optimizer = torch.optim.AdamW(sp_model.parameters(), lr=lr, foreach=True)
     
     # Dataloaders
 
     (train_dataloader, test_dataloader) = get_torchvision_dataset("MNIST", batch_size)
 
     tik = time.time()
-    train_eval(
-        tp_model, 
+    sequence_train_eval(
+        sp_model, 
         train_dataloader, 
         test_dataloader, 
         loss_fn, 
         optimizer, 
         epochs, 
         batch_size,
         device
     )
     tok = time.time()
-    print(f"Execution time = {tok - tik}")
-    save_model(model, args.model_name)
+    print(f"Execution time = {tok - tik}")
```

### Comparing `detrain-0.2.2/examples/tp/nn/rdz.py` & `detrain-0.2.4/examples/tp/nn/rdz.py`

 * *Files identical despite different names*

### Comparing `detrain-0.2.2/pyproject.toml` & `detrain-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "detrain"
-version = "0.2.2"
+version = "0.2.4"
 authors = [
     {name = "Levi", email = "levi@a2n.finance"},
     {name = "John", email = "john@a2n.finance"},
 ]
 readme= "README.rst"
 description = "A package for distributed training & model parallelism using Torch"
 requires-python = ">=3.8"
```

### Comparing `detrain-0.2.2/tests/test_dataset.py` & `detrain-0.2.4/tests/test_dataset.py`

 * *Files identical despite different names*

