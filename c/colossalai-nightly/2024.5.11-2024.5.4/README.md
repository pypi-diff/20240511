# Comparing `tmp/colossalai-nightly-2024.5.11.tar.gz` & `tmp/colossalai-nightly-2024.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2024.5.11.tar", last modified: Sat May 11 00:14:56 2024, max compression
+gzip compressed data, was "colossalai-nightly-2024.5.4.tar", last modified: Sat May  4 00:14:38 2024, max compression
```

## Comparing `colossalai-nightly-2024.5.11.tar` & `colossalai-nightly-2024.5.4.tar`

### file list

```diff
@@ -1,1179 +1,1175 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.443089 colossalai-nightly-2024.5.11/
--rw-r--r--   0 runner    (1001) docker     (127)    30134 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    36766 2024-05-11 00:14:56.443089 colossalai-nightly-2024.5.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20868 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18998 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.283087 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/accelerator/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/accelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/accelerator/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/accelerator/base_accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/accelerator/cpu_accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/accelerator/cuda_accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/accelerator/npu_accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.287088 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.291087 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.291087 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.291087 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    20031 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    18503 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.295087 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.295087 colossalai-nightly-2024.5.11/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.295087 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.299088 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20347 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.303088 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24078 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    41664 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.303088 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    20206 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.303088 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.303088 colossalai-nightly-2024.5.11/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.307088 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.307088 colossalai-nightly-2024.5.11/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    63887 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/hybrid_parallel_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    19546 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/moe_hybrid_parallel_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/pp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.307088 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    43972 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/hybrid_parallel_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29632 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.307088 colossalai-nightly-2024.5.11/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.307088 colossalai-nightly-2024.5.11/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.311088 colossalai-nightly-2024.5.11/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.311088 colossalai-nightly-2024.5.11/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cluster/process_group_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/cluster/process_group_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.311088 colossalai-nightly-2024.5.11/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/context/singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.311088 colossalai-nightly-2024.5.11/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23616 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.311088 colossalai-nightly-2024.5.11/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.311088 colossalai-nightly-2024.5.11/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45231 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.315088 colossalai-nightly-2024.5.11/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.315088 colossalai-nightly-2024.5.11/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.315088 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.319088 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.319088 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.319088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.319088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.319088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.323088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.323088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.323088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.323088 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    24642 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.323088 colossalai-nightly-2024.5.11/colossalai/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.323088 colossalai-nightly-2024.5.11/colossalai/inference/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/microbatch_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19778 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)    20627 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    21828 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/kv_cache/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/kv_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/kv_cache/batch_infer_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/kv_cache/kvcache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/quant/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/cai_gptq/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/cai_gptq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/cai_gptq/cai_quant_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/cai_gptq/gptq_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/gptq_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.327088 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20063 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    35519 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/parallel_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.331088 colossalai-nightly-2024.5.11/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/interface/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/interface/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.331088 colossalai-nightly-2024.5.11/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.331088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/base_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpp_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.331088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpu_adam/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpu_adam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpu_adam/cpu_adam_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpu_adam/cpu_adam_x86.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.331088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.331088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/arm/
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.335088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/compat.h
--rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.335088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/include/
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25829 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23530 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/scaled_softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cuda_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.335088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/flash_attention_dao_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/flash_attention_npu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/flash_attention_sdpa_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.335088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/layernorm/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/layernorm/layernorm_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.335088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/moe/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/moe/moe_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.335088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/optimizer/fused_optimizer_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.339088 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/softmax/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/softmax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/softmax/scaled_masked_softmax_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/triton_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.339088 colossalai-nightly-2024.5.11/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/jit/option.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/kernel_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.339088 colossalai-nightly-2024.5.11/colossalai/kernel/triton/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/context_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/copy_kv_cache_dest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/custom_autotune.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/flash_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/fused_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18024 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/gptq_triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/int8_rotary_embedding_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/llama_act_combine_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/qkv_matmul_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/self_attention_nofusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    21773 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/smooth_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/kernel/triton/token_attention_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.339088 colossalai-nightly-2024.5.11/colossalai/lazy/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/lazy/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25011 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/lazy/lazy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/lazy/pretrained.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/amp/
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.343088 colossalai-nightly-2024.5.11/colossalai/legacy/communication/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.347088 colossalai-nightly-2024.5.11/colossalai/legacy/context/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24229 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.347088 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.347088 colossalai-nightly-2024.5.11/colossalai/legacy/context/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.347088 colossalai-nightly-2024.5.11/colossalai/legacy/engine/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.347088 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.351088 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.351088 colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    40085 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_pipeline_schedule_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/global_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.351088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/async_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/async_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.351088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/get_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13595 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/io_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/ray_dist_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/ray_init_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/req_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.351088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.351088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/modeling/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/modeling/llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/polices/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/polices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/polices/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/pipeline/microbatch_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/batch_infer_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/kvcache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23642 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)    22757 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    17826 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/llama.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    19842 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/_ops/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.355088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.359088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.359088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44898 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.359088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35857 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    49324 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.359088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39868 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    49527 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.359088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22832 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    49624 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.359088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.363088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.363088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.363088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.363088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.363088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.363088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.367088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.367088 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    27958 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.367088 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.367088 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.367088 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.367088 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59091 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.371088 colossalai-nightly-2024.5.11/colossalai/legacy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.371088 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/tensor/tensor_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.371088 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.371088 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpoint/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.375088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11099 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28757 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.379088 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.383088 colossalai-nightly-2024.5.11/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.383088 colossalai-nightly-2024.5.11/colossalai/moe/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    36076 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16261 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/load_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.383088 colossalai-nightly-2024.5.11/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.383088 colossalai-nightly-2024.5.11/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/layer/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/layer/scaled_softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/layer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.383088 colossalai-nightly-2024.5.11/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/loss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.387088 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.387088 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.387088 colossalai-nightly-2024.5.11/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/p2p.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.387088 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26918 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/interleaved_pp.py
--rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/one_f_one_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/pipeline/stage_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.391088 colossalai-nightly-2024.5.11/colossalai/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/quantization/bnb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/quantization/bnb_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.391088 colossalai-nightly-2024.5.11/colossalai/shardformer/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.391088 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38285 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/attn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15865 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17676 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/parallel_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/qkv_fused_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/layer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.395088 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62664 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/blip2.py
--rw-r--r--   0 runner    (1001) docker     (127)    49669 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.395088 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2_6b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2_6b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2_6b/configuration_chatglm.py
--rw-r--r--   0 runner    (1001) docker     (127)    54608 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2_6b/modeling_chatglm.py
--rw-r--r--   0 runner    (1001) docker     (127)    34314 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)    59838 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/gptj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/jit.py
--rw-r--r--   0 runner    (1001) docker     (127)    46388 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    31925 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    45212 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    33866 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    37484 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)    54363 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.399088 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11302 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/auto_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/base_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    27227 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15862 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/blip2.py
--rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)    22241 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/gptj.py
--rw-r--r--   0 runner    (1001) docker     (127)    18920 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    14258 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/opt.py
--rw-r--r--   0 runner    (1001) docker     (127)    14648 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)    22174 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/t5.py
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)    23410 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/policies/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.399088 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/grad_ckpt_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/shard_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/shardformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/shardformer/shard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.403088 colossalai-nightly-2024.5.11/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    21633 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/comm_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.403088 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    27564 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.403088 colossalai-nightly-2024.5.11/colossalai/tensor/moe_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/moe_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/moe_tensor/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/moe_tensor/moe_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.403088 colossalai-nightly-2024.5.11/colossalai/tensor/padded_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/padded_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/padded_tensor/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    35882 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.403088 colossalai-nightly-2024.5.11/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.407089 colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25030 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44029 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    37804 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.411089 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.411089 colossalai-nightly-2024.5.11/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.411089 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    46268 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.415089 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    36766 2024-05-11 00:14:56.000000 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48560 2024-05-11 00:14:56.000000 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 00:14:56.000000 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-11 00:14:56.000000 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-11 00:14:56.000000 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 00:14:56.000000 colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.275087 colossalai-nightly-2024.5.11/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.415089 colossalai-nightly-2024.5.11/examples/language/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/examples/language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/examples/language/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/examples/language/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/examples/language/performance_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.415089 colossalai-nightly-2024.5.11/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/base_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/cpp_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.415089 colossalai-nightly-2024.5.11/extensions/cpu_adam/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/cpu_adam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/cpu_adam/cpu_adam_arm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/cpu_adam/cpu_adam_x86.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.415089 colossalai-nightly-2024.5.11/extensions/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.415089 colossalai-nightly-2024.5.11/extensions/csrc/arm/
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/arm/cpu_adam_arm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/arm/cpu_adam_arm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.419089 colossalai-nightly-2024.5.11/extensions/csrc/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/compat.h
--rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.419089 colossalai-nightly-2024.5.11/extensions/csrc/cuda/include/
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25829 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    23530 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/cuda/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/csrc/scaled_softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/cuda_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.419089 colossalai-nightly-2024.5.11/extensions/flash_attention/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/flash_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/flash_attention/flash_attention_dao_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/flash_attention/flash_attention_npu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/flash_attention/flash_attention_sdpa_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.419089 colossalai-nightly-2024.5.11/extensions/layernorm/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/layernorm/layernorm_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.419089 colossalai-nightly-2024.5.11/extensions/moe/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/moe/moe_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/extensions/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/optimizer/fused_optimizer_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/extensions/softmax/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/softmax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/softmax/scaled_masked_softmax_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/triton_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/requirements/requirements-infer.txt
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 00:14:56.443089 colossalai-nightly-2024.5.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-11 00:14:55.000000 colossalai-nightly-2024.5.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.279087 colossalai-nightly-2024.5.11/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.423089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.427089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.427089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.427089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.427089 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/blip2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/gptj.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/whisper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.427089 colossalai-nightly-2024.5.11/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.431089 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.431089 colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.431089 colossalai-nightly-2024.5.11/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.431089 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.435089 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.435089 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.439089 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18264 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.439089 colossalai-nightly-2024.5.11/tests/test_shardformer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:56.443089 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_blip2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_bloom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_chatglm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_gptj.py
--rw-r--r--   0 runner    (1001) docker     (127)    12165 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_sam.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_whisper.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/tests/test_shardformer/test_with_torch_ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 00:14:48.000000 colossalai-nightly-2024.5.11/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.429213 colossalai-nightly-2024.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    30134 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    36765 2024-05-04 00:14:38.429213 colossalai-nightly-2024.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31195 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20868 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18677 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18998 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8482 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12708 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.281213 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/accelerator/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/accelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/accelerator/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9402 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/accelerator/base_accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/accelerator/cpu_accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/accelerator/cuda_accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/accelerator/npu_accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.285213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.289213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.289213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.289213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20031 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18503 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17919 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.293213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11328 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22439 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.293213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.293213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.297213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11414 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20347 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.301213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24078 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7361 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41664 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.301213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20206 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.301213 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.301213 colossalai-nightly-2024.5.4/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.305213 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.305213 colossalai-nightly-2024.5.4/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63839 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/hybrid_parallel_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19546 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/moe_hybrid_parallel_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/pp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15017 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.305213 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43972 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/hybrid_parallel_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29632 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.305213 colossalai-nightly-2024.5.4/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.305213 colossalai-nightly-2024.5.4/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.309213 colossalai-nightly-2024.5.4/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.309213 colossalai-nightly-2024.5.4/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cluster/process_group_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/cluster/process_group_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.309213 colossalai-nightly-2024.5.4/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/context/singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.309213 colossalai-nightly-2024.5.4/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23616 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.309213 colossalai-nightly-2024.5.4/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.309213 colossalai-nightly-2024.5.4/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45231 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.313213 colossalai-nightly-2024.5.4/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12261 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14066 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.313213 colossalai-nightly-2024.5.4/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.313213 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.317213 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.317213 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.317213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.317213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.321213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.321213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.321213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.321213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.321213 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24642 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.321213 colossalai-nightly-2024.5.4/colossalai/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/microbatch_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19778 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20627 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21828 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/kv_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/kv_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/kv_cache/batch_infer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/kv_cache/kvcache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/quant/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/cai_gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/cai_gptq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13893 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/cai_gptq/cai_quant_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/cai_gptq/gptq_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/gptq_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.325213 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20063 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35519 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/parallel_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.329213 colossalai-nightly-2024.5.4/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/interface/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/interface/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.329213 colossalai-nightly-2024.5.4/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.329213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/base_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpp_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.329213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpu_adam/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpu_adam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpu_adam/cpu_adam_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpu_adam/cpu_adam_x86.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.329213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.329213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/arm/
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.333213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.333213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25829 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23530 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/scaled_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cuda_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.333213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/flash_attention_dao_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/flash_attention_npu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/flash_attention_sdpa_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.333213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/layernorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/layernorm/layernorm_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.337213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/moe/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/moe/moe_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.337213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/optimizer/fused_optimizer_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.337213 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/softmax/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/softmax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/softmax/scaled_masked_softmax_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/triton_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.337213 colossalai-nightly-2024.5.4/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/jit/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/kernel_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.337213 colossalai-nightly-2024.5.4/colossalai/kernel/triton/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/context_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/copy_kv_cache_dest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/custom_autotune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/flash_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/fused_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18024 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/gptq_triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/int8_rotary_embedding_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/llama_act_combine_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/qkv_matmul_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/self_attention_nofusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21773 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/smooth_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/kernel/triton/token_attention_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/lazy/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25011 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/lazy/lazy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/lazy/pretrained.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/legacy/amp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/legacy/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.341213 colossalai-nightly-2024.5.4/colossalai/legacy/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.345213 colossalai-nightly-2024.5.4/colossalai/legacy/communication/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17484 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.345213 colossalai-nightly-2024.5.4/colossalai/legacy/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24229 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.345213 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.345213 colossalai-nightly-2024.5.4/colossalai/legacy/context/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.345213 colossalai-nightly-2024.5.4/colossalai/legacy/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.345213 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.349213 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.349213 colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40085 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_pipeline_schedule_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/global_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.349213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/async_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/async_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.349213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/get_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13595 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/io_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/ray_dist_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/ray_init_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/req_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.349213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/modeling/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21591 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/modeling/llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/polices/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/polices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/polices/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11605 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/pipeline/microbatch_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/batch_infer_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/kvcache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23642 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22757 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17826 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/llama.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19842 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8669 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/_ops/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.353213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.357213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6156 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.357213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44898 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.357213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35857 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49324 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.357213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39868 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49527 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.357213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22832 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49624 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.361213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.365213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.365213 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27958 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8710 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.365213 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.365213 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.365213 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.365213 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59091 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.369213 colossalai-nightly-2024.5.4/colossalai/legacy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.369213 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10505 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/tensor/tensor_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.369213 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.369213 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16242 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.369213 colossalai-nightly-2024.5.4/colossalai/legacy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.369213 colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpoint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.373213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11099 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.377213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.377213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28757 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.377213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18982 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.377213 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.377213 colossalai-nightly-2024.5.4/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.381213 colossalai-nightly-2024.5.4/colossalai/moe/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36076 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16261 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18267 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/load_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20401 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.381213 colossalai-nightly-2024.5.4/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.381213 colossalai-nightly-2024.5.4/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/layer/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/layer/scaled_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/layer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.381213 colossalai-nightly-2024.5.4/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/loss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.381213 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.381213 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.385213 colossalai-nightly-2024.5.4/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/p2p.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.385213 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20009 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26918 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/interleaved_pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/one_f_one_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/pipeline/stage_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.385213 colossalai-nightly-2024.5.4/colossalai/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13038 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/quantization/bnb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/quantization/bnb_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.385213 colossalai-nightly-2024.5.4/colossalai/shardformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.385213 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38285 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13198 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15865 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26710 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17676 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/parallel_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/qkv_fused_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/layer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.389213 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62664 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/blip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49669 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17629 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.389213 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2_6b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2_6b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2_6b/configuration_chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54608 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2_6b/modeling_chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34314 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59838 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44054 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/jit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46388 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27319 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36942 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37484 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54363 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.393213 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/auto_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/base_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27227 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15862 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/blip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17356 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16474 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22241 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18711 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14549 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22174 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23410 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/policies/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.393213 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/grad_ckpt_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/shard_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/shardformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/shardformer/shard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.393213 colossalai-nightly-2024.5.4/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21633 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/comm_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27564 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/tensor/moe_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/moe_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/moe_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/moe_tensor/moe_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/tensor/padded_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/padded_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/padded_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35882 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11626 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.397213 colossalai-nightly-2024.5.4/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.401213 colossalai-nightly-2024.5.4/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.401213 colossalai-nightly-2024.5.4/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.401213 colossalai-nightly-2024.5.4/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.401213 colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25030 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42911 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37706 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.401213 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9569 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.401213 colossalai-nightly-2024.5.4/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.405213 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43271 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.405213 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    36765 2024-05-04 00:14:38.000000 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48382 2024-05-04 00:14:38.000000 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:14:38.000000 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-04 00:14:38.000000 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-04 00:14:38.000000 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-04 00:14:38.000000 colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.277213 colossalai-nightly-2024.5.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.405213 colossalai-nightly-2024.5.4/examples/language/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/examples/language/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/examples/language/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/examples/language/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/examples/language/performance_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.405213 colossalai-nightly-2024.5.4/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/base_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/cpp_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.405213 colossalai-nightly-2024.5.4/extensions/cpu_adam/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/cpu_adam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/cpu_adam/cpu_adam_arm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/cpu_adam/cpu_adam_x86.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.405213 colossalai-nightly-2024.5.4/extensions/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.409213 colossalai-nightly-2024.5.4/extensions/csrc/arm/
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/arm/cpu_adam_arm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/arm/cpu_adam_arm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.409213 colossalai-nightly-2024.5.4/extensions/csrc/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/compat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.409213 colossalai-nightly-2024.5.4/extensions/csrc/cuda/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25829 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25627 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23530 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/cuda/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/csrc/scaled_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/cuda_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/extensions/flash_attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/flash_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/flash_attention/flash_attention_dao_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/flash_attention/flash_attention_npu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/flash_attention/flash_attention_sdpa_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/extensions/layernorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/layernorm/layernorm_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/extensions/moe/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/moe/moe_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/extensions/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/optimizer/fused_optimizer_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/extensions/softmax/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/softmax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/softmax/scaled_masked_softmax_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/triton_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/requirements/requirements-infer.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:14:38.429213 colossalai-nightly-2024.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-04 00:14:37.000000 colossalai-nightly-2024.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.277213 colossalai-nightly-2024.5.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.413213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.417213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.417213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.417213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.417213 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/blip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/gptj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.417213 colossalai-nightly-2024.5.4/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.421213 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.421213 colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.421213 colossalai-nightly-2024.5.4/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.421213 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.421213 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.421213 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.425213 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12574 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18264 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.429213 colossalai-nightly-2024.5.4/tests/test_shardformer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:38.429213 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_blip2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_chatglm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_gptj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_sam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_whisper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/tests/test_shardformer/test_with_torch_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 00:14:29.000000 colossalai-nightly-2024.5.4/version.txt
```

### Comparing `colossalai-nightly-2024.5.11/LICENSE` & `colossalai-nightly-2024.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/PKG-INFO` & `colossalai-nightly-2024.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2024.5.11
+Version: 2024.5.4
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2024.5.11 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2024.5.4 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2024.5.11/README.md` & `colossalai-nightly-2024.5.4/README.md`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/_meta_registration.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/_monkey_patch.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/flop_tensor.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/_subclasses/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/codegen.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/graph_module.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/node_util.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/node_util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/passes/graph_profile.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/passes/graph_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/passes/shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/symbolic_profile.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/bias_addition.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/custom_leaf_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/proxy.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/symbolic_trace.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/_analyzer/fx/tracer/tracer.py` & `colossalai-nightly-2024.5.4/colossalai/_analyzer/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/accelerator/api.py` & `colossalai-nightly-2024.5.4/colossalai/accelerator/api.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/accelerator/base_accelerator.py` & `colossalai-nightly-2024.5.4/colossalai/accelerator/base_accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/accelerator/cpu_accelerator.py` & `colossalai-nightly-2024.5.4/colossalai/accelerator/cpu_accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/accelerator/cuda_accelerator.py` & `colossalai-nightly-2024.5.4/colossalai/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/accelerator/npu_accelerator.py` & `colossalai-nightly-2024.5.4/colossalai/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/base.py` & `colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py` & `colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/amp/naive_amp/mixed_precision_optimizer.py` & `colossalai-nightly-2024.5.4/colossalai/amp/naive_amp/mixed_precision_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2024.5.4/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/accelerator.py` & `colossalai-nightly-2024.5.4/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/booster.py` & `colossalai-nightly-2024.5.4/colossalai/booster/booster.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp16_apex.py` & `colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp16_apex.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp16_naive.py` & `colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp16_naive.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2024.5.4/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/gemini_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/hybrid_parallel_plugin.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/hybrid_parallel_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -731,15 +731,15 @@
                 return grads_to_sync
             else:
                 return None
 
         # Get all working gradients and gradients to be synchronized.
         all_working_grads = _get_all_working_grads()
         grads_to_sync = _get_grads_to_sync(all_working_grads)
-        if self._grad_store.require_grad_sync and grads_to_sync is not None:
+        if self.require_grad_sync and grads_to_sync is not None:
             # Synchronize sequence parallelism gradients if required.
             SeqParallelUtils.allreduce_partial_data_grad(process_group=self.tp_pg, grads=grads_to_sync)
         else:
             return
 
     def backward(self, loss, retain_graph=False):
         """
@@ -755,15 +755,15 @@
 
         Returns:
             None
         """
         # Call the superclass backward method to compute gradients.
         super().backward(loss, retain_graph)
 
-        if self._grad_store.require_grad_sync and self.model.shard_config.enable_sequence_parallelism:
+        if self.require_grad_sync and self.model.shard_config.enable_sequence_parallelism:
             # If gradient synchronization is required, sync sequence parallelism gradients.
             self._sync_sp_grads()
         else:
             # If gradient synchronization is is not required, return.
             return
 
     def backward_by_grad(self, tensor, grad):
@@ -780,15 +780,15 @@
 
         Returns:
             None
         """
         # Call the superclass backward_by_grad method to compute gradients.
         super().backward_by_grad(tensor, grad)
 
-        if self._grad_store.require_grad_sync and self.model.shard_config.enable_sequence_parallelism:
+        if self.require_grad_sync and self.model.shard_config.enable_sequence_parallelism:
             # If gradient synchronization is required, sync sequence parallelism gradients.
             self._sync_sp_grads()
         else:
             # If gradient synchronization is is not required, return.
             return
 
     def _compute_grad_norm(self, gradients: List[Tensor], norm_type: int = 2) -> float:
@@ -1268,15 +1268,15 @@
         with ctx:
             outputs = self.schedule.forward_backward_step(
                 model, data_iter, criterion, optimizer, return_loss, return_outputs
             )
 
         # run with gradients accumulation
         if model.require_grad_sync == False or (
-            isinstance(optimizer, HybridParallelZeroOptimizer) and optimizer._grad_store.require_grad_sync == False
+            isinstance(optimizer, HybridParallelZeroOptimizer) and optimizer.require_grad_sync == False
         ):
             return outputs
 
         # Synchronize the grads of shared parameters of the model.
         model.sync_shared_params()
         # Synchronize sequence parallelism gradients of the model.
         model.sync_sp_grads()
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/moe_hybrid_parallel_plugin.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/moe_hybrid_parallel_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/pp_plugin_base.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/pp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/booster/plugin/torch_fsdp_plugin.py` & `colossalai-nightly-2024.5.4/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2024.5.4/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2024.5.4/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/checkpoint_io/hybrid_parallel_checkpoint_io.py` & `colossalai-nightly-2024.5.4/colossalai/checkpoint_io/hybrid_parallel_checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2024.5.4/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2024.5.4/colossalai/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2024.5.4/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2024.5.4/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2024.5.4/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cli/launcher/run.py` & `colossalai-nightly-2024.5.4/colossalai/cli/launcher/run.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2024.5.4/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2024.5.4/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2024.5.4/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/cluster/process_group_mesh.py` & `colossalai-nightly-2024.5.4/colossalai/cluster/process_group_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/context/config.py` & `colossalai-nightly-2024.5.4/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/context/singleton_meta.py` & `colossalai-nightly-2024.5.4/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2024.5.4/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2024.5.4/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/device/device_mesh.py` & `colossalai-nightly-2024.5.4/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/_compatibility.py` & `colossalai-nightly-2024.5.4/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2024.5.4/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2024.5.4/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2024.5.4/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/graph_module.py` & `colossalai-nightly-2024.5.4/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/passes/utils.py` & `colossalai-nightly-2024.5.4/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2024.5.4/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/proxy.py` & `colossalai-nightly-2024.5.4/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2024.5.4/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/engine.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/microbatch_manager.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/microbatch_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/bloom.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/chatglm2.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/modeling/llama.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/bloom.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/chatglm2.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/engine/policies/llama.py` & `colossalai-nightly-2024.5.4/colossalai/inference/engine/policies/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/kv_cache/batch_infer_state.py` & `colossalai-nightly-2024.5.4/colossalai/inference/kv_cache/batch_infer_state.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/kv_cache/kvcache_manager.py` & `colossalai-nightly-2024.5.4/colossalai/inference/kv_cache/kvcache_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/cai_gptq/cai_quant_linear.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/cai_gptq/cai_quant_linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/cai_gptq/gptq_op.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/cai_gptq/gptq_op.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/gptq/gptq_manager.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/gptq/gptq_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/base_model.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/base_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/linear.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/llama.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/inference/quant/smoothquant/models/parallel_linear.py` & `colossalai-nightly-2024.5.4/colossalai/inference/quant/smoothquant/models/parallel_linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/initialize.py` & `colossalai-nightly-2024.5.4/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/interface/model.py` & `colossalai-nightly-2024.5.4/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/interface/optimizer.py` & `colossalai-nightly-2024.5.4/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/base_extension.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpp_extension.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpp_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpu_adam/cpu_adam_arm.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpu_adam/cpu_adam_arm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cpu_adam/cpu_adam_x86.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cpu_adam/cpu_adam_x86.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.h` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/arm/cpu_adam_arm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/colossal_C_frontend.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/cpu_adam.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/cpu_adam.h` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/include/block_reduce.h` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/moe_cuda.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/moe_cuda_kernel.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_adam.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_apply.cuh` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_lamb.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.h` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/cuda/type_shim.h` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/cuda/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/csrc/scaled_softmax.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/csrc/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/cuda_extension.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/cuda_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/flash_attention_dao_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/flash_attention_dao_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/flash_attention_npu.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/flash_attention_npu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/flash_attention/flash_attention_sdpa_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/flash_attention/flash_attention_sdpa_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/layernorm/layernorm_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/layernorm/layernorm_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/moe/moe_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/moe/moe_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/optimizer/fused_optimizer_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/optimizer/fused_optimizer_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/softmax/scaled_masked_softmax_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/softmax/scaled_masked_softmax_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/triton_extension.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/triton_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/extensions/utils.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/jit/option.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/kernel_loader.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/kernel_loader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/context_attention.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/context_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/copy_kv_cache_dest.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/copy_kv_cache_dest.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/custom_autotune.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/flash_decoding.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/flash_decoding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/fused_layernorm.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/fused_layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/gptq_triton.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/gptq_triton.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/int8_rotary_embedding_kernel.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/int8_rotary_embedding_kernel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/llama_act_combine_kernel.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/llama_act_combine_kernel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/qkv_matmul_kernel.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/qkv_matmul_kernel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/self_attention_nofusion.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/self_attention_nofusion.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/smooth_attention.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/smooth_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/softmax.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/kernel/triton/token_attention_kernel.py` & `colossalai-nightly-2024.5.4/colossalai/kernel/triton/token_attention_kernel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/lazy/construction.py` & `colossalai-nightly-2024.5.4/colossalai/lazy/construction.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/lazy/lazy_init.py` & `colossalai-nightly-2024.5.4/colossalai/lazy/lazy_init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/lazy/pretrained.py` & `colossalai-nightly-2024.5.4/colossalai/lazy/pretrained.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/apex_amp/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/builder/builder.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/communication/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/communication/collective.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/communication/p2p.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/communication/p2p_v2.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/communication/ring.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/communication/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/constants.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/parallel_context.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/parallel_mode.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/random/_helper.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/context/random/seed_manager.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/_base_engine.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/gradient_handler/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_base_schedule.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/global_variables.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/async_engine.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/async_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/async_manager.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/async_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/get_tokenizer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/get_tokenizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/infer_batch.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/infer_batch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/io_struct.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/io_struct.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/ray_dist_init.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/ray_dist_init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/ray_init_config.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/ray_init_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/req_queue.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/req_queue.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/sampling_params.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/sampling_params.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/dynamic_batching/stats.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/dynamic_batching/stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/engine.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/modeling/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/modeling/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/modeling/llama.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/hybridengine/polices/llama.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/hybridengine/polices/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/manager.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/pipeline/microbatch_manager.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/pipeline/microbatch_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/batch_infer_state.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/batch_infer_state.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/engine.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/kvcache_manager.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/kvcache_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/bloom.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/chatglm2.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/modeling/llama.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/bloom.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/chatglm2.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/inference/tensor_parallel/policies/llama.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/inference/tensor_parallel/policies/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/initialize.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/_ops/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/base_layer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/utils/common.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/vanilla/layers.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_1d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_2d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_2p5d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/loss/loss_3d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/accuracy_2d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/metric/accuracy_3d.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/data_parallel.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/embedding.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/linear.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/nn/parallel/reducer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/layer_spec.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/middleware/topo.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/pipelinable.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/pipeline_process_group.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/rpc/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/pipeline/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/registry/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/registry/registry.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/tensor/compute_spec.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/tensor/dist_spec_mgr.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/tensor/distspec.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/tensor/op_wrapper.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/tensor/process_group.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/tensor/tensor_spec.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/_trainer.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_base_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_log_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/activation_checkpoint.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpoint/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/checkpointing.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/common.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/memory.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/profiler.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/colo_init_context.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/gemini_context.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/ophooks/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/stateful_tensor.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/tensor_placement_policy.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/gemini/tensor_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/init_ctx/init_context.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/commons.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/reduce_scatter.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/utils.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_model/zero_hook.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_param/sharded_param.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/legacy/zero/sharded_param/sharded_tensor.py` & `colossalai-nightly-2024.5.4/colossalai/legacy/zero/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/logging/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/logging/logger.py` & `colossalai-nightly-2024.5.4/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/checkpoint.py` & `colossalai-nightly-2024.5.4/colossalai/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/experts.py` & `colossalai-nightly-2024.5.4/colossalai/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/layers.py` & `colossalai-nightly-2024.5.4/colossalai/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/load_balance.py` & `colossalai-nightly-2024.5.4/colossalai/moe/load_balance.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/loss.py` & `colossalai-nightly-2024.5.4/colossalai/moe/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/manager.py` & `colossalai-nightly-2024.5.4/colossalai/moe/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/routers.py` & `colossalai-nightly-2024.5.4/colossalai/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/moe/utils.py` & `colossalai-nightly-2024.5.4/colossalai/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/init.py` & `colossalai-nightly-2024.5.4/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/layer/layernorm.py` & `colossalai-nightly-2024.5.4/colossalai/nn/layer/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/layer/scaled_softmax.py` & `colossalai-nightly-2024.5.4/colossalai/nn/layer/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2024.5.4/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2024.5.4/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/p2p.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/p2p.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/base.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/generate.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/generate.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/interleaved_pp.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/interleaved_pp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/schedule/one_f_one_b.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/schedule/one_f_one_b.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/pipeline/stage_manager.py` & `colossalai-nightly-2024.5.4/colossalai/pipeline/stage_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/quantization/bnb.py` & `colossalai-nightly-2024.5.4/colossalai/quantization/bnb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/quantization/bnb_config.py` & `colossalai-nightly-2024.5.4/colossalai/quantization/bnb_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/_operation.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/attn.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/dropout.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/embedding.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/linear.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/loss.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/normalization.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/parallel_module.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/parallel_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/qkv_fused_linear.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/qkv_fused_linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/layer/utils.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/layer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/bert.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/blip2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/blip2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/bloom.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2_6b/configuration_chatglm.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2_6b/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/chatglm2_6b/modeling_chatglm.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/chatglm2_6b/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/falcon.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/falcon.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/gpt2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/gptj.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/gptj.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/jit.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/jit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/llama.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/mistral.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/mistral.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 )
 from transformers.models.mistral.modeling_mistral import MistralForCausalLM, MistralModel
 from transformers.utils import logging
 
 from colossalai.pipeline.stage_manager import PipelineStageManager
 from colossalai.shardformer.shard import ShardConfig
 
-from ..layer import ColoAttention, cross_entropy_1d
+from ..layer import ColoAttention
 
 logger = logging.get_logger(__name__)
 
 
 class MistralForwards:
     @staticmethod
     def mistral_model_forward(
@@ -266,29 +266,19 @@
             loss = None
             if labels is not None:
                 # Shift so that tokens < n predict n
                 shift_logits = logits[..., :-1, :].contiguous()
                 shift_labels = labels[..., 1:].contiguous()
                 # Flatten the tokens
                 loss_fct = CrossEntropyLoss()
+                shift_logits = shift_logits.view(-1, self.config.vocab_size)
                 shift_labels = shift_labels.view(-1)
                 # Enable model parallelism
                 shift_labels = shift_labels.to(shift_logits.device)
-                if shard_config.enable_tensor_parallelism and shard_config.parallel_output:
-                    new_vocab_size = logits.shape[-1]
-                    shift_logits = shift_logits.view(-1, new_vocab_size)
-                    loss = cross_entropy_1d(
-                        shift_logits,
-                        shift_labels,
-                        process_group=shard_config.tensor_parallel_process_group,
-                        vocab_size=self.lm_head.out_features,
-                    )
-                else:
-                    shift_logits = shift_logits.view(-1, self.config.vocab_size)
-                    loss = loss_fct(shift_logits, shift_labels)
+                loss = loss_fct(shift_logits, shift_labels)
 
             if not return_dict:
                 output = (logits,) + outputs[1:]
                 return (loss,) + output if loss is not None else output
 
             return CausalLMOutputWithPast(
                 loss=loss,
@@ -615,104 +605,7 @@
         attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
 
         attn_output = self.o_proj(attn_output)
 
         return attn_output, None, past_key_value
 
     return forward
-
-
-def get_lm_forward_with_dist_cross_entropy(shard_config: ShardConfig):
-    from transformers import MistralForCausalLM
-
-    def forward(
-        self: MistralForCausalLM,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        labels: Optional[torch.LongTensor] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, CausalLMOutputWithPast]:
-        r"""
-        Args:
-            labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
-                Labels for computing the masked language modeling loss. Indices should either be in `[0, ...,
-                config.vocab_size]` or -100 (see `input_ids` docstring). Tokens with indices set to `-100` are ignored
-                (masked), the loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`.
-
-        Returns:
-
-        Example:
-
-        ```python
-        >>> from transformers import AutoTokenizer, MistralForCausalLM
-
-        >>> model = MistralForCausalLM.from_pretrained(PATH_TO_CONVERTED_WEIGHTS)
-        >>> tokenizer = AutoTokenizer.from_pretrained(PATH_TO_CONVERTED_TOKENIZER)
-
-        >>> prompt = "Hey, are you conscious? Can you talk to me?"
-        >>> inputs = tokenizer(prompt, return_tensors="pt")
-
-        >>> # Generate
-        >>> generate_ids = model.generate(inputs.input_ids, max_length=30)
-        >>> tokenizer.batch_decode(generate_ids, skip_special_tokens=True, clean_up_tokenization_spaces=False)[0]
-        "Hey, are you conscious? Can you talk to me?\nI'm not conscious, but I can talk to you."
-        ```"""
-
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        # decoder outputs consists of (dec_features, layer_state, dec_hidden, dec_attn)
-        outputs = self.model(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-            past_key_values=past_key_values,
-            inputs_embeds=inputs_embeds,
-            use_cache=use_cache,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
-        )
-
-        hidden_states = outputs[0]
-        logits = self.lm_head(hidden_states)
-        logits = logits.float()
-
-        loss = None
-        if labels is not None:
-            # Shift so that tokens < n predict n
-            shift_logits = logits[..., :-1, :].contiguous()
-            shift_labels = labels[..., 1:].contiguous()
-            shift_labels = shift_labels.view(-1)
-            # Enable model parallelism
-            shift_labels = shift_labels.to(shift_logits.device)
-            new_vocab_size = logits.shape[-1]
-            shift_logits = shift_logits.view(-1, new_vocab_size)
-            loss = cross_entropy_1d(
-                shift_logits,
-                shift_labels,
-                process_group=shard_config.tensor_parallel_process_group,
-                vocab_size=self.lm_head.out_features,
-            )
-
-        if not return_dict:
-            output = (logits,) + outputs[1:]
-            return (loss,) + output if loss is not None else output
-
-        return CausalLMOutputWithPast(
-            loss=loss,
-            logits=logits,
-            past_key_values=outputs.past_key_values,
-            hidden_states=outputs.hidden_states,
-            attentions=outputs.attentions,
-        )
-
-    return forward
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/opt.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/opt.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 )
 from transformers.utils import logging
 
 from colossalai.pipeline.stage_manager import PipelineStageManager
 from colossalai.shardformer.layer import ColoAttention
 from colossalai.shardformer.shard import ShardConfig
 
-from ..layer import cross_entropy_1d
-
 logger = logging.get_logger(__name__)
 
 
 def _get_attention_mask(
     self: OPTModel,
     shard_config: ShardConfig,
     hidden_states: torch.Tensor,
@@ -334,30 +332,16 @@
             if labels is not None:
                 # move labels to correct device to enable model parallelism
                 labels = labels.to(logits.device)
                 # Shift so that tokens < n predict n
                 shift_logits = logits[..., :-1, :].contiguous()
                 shift_labels = labels[..., 1:].contiguous()
                 # Flatten the tokens
-
-                if shard_config.enable_tensor_parallelism and shard_config.parallel_output:
-                    new_vocab_size = logits.shape[-1]
-                    shift_logits = shift_logits.view(-1, new_vocab_size)
-                    shift_labels = shift_labels.view(-1)
-                    loss = cross_entropy_1d(
-                        shift_logits,
-                        shift_labels,
-                        process_group=shard_config.tensor_parallel_process_group,
-                        vocab_size=self.lm_head.out_features,
-                    )
-                else:
-                    loss_fct = CrossEntropyLoss()
-                    shift_logits = shift_logits.view(-1, self.config.vocab_size)
-                    loss = loss_fct(shift_logits.view(-1, self.config.vocab_size), shift_labels.view(-1))
-
+                loss_fct = CrossEntropyLoss()
+                loss = loss_fct(shift_logits.view(-1, self.config.vocab_size), shift_labels.view(-1))
             if not return_dict:
                 output = (logits,) + outputs[1:]
                 return (loss,) + output if loss is not None else output
 
             return CausalLMOutputWithPast(
                 loss=loss,
                 logits=logits,
@@ -856,150 +840,7 @@
 
         if use_cache:
             outputs += (present_key_value,)
 
         return outputs
 
     return forward
-
-
-def get_lm_forward_with_dist_cross_entropy(shard_config: ShardConfig):
-    def forward(
-        self: OPTForCausalLM,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        head_mask: Optional[torch.Tensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        labels: Optional[torch.LongTensor] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, CausalLMOutputWithPast]:
-        r"""
-        Args:
-            input_ids (`torch.LongTensor` of shape `(batch_size, sequence_length)`):
-                Indices of input sequence tokens in the vocabulary. Padding will be ignored by default should you
-                provide it.
-
-                Indices can be obtained using [`AutoTokenizer`]. See [`PreTrainedTokenizer.encode`] and
-                [`PreTrainedTokenizer.__call__`] for details.
-
-                [What are input IDs?](../glossary#input-ids)
-            attention_mask (`torch.Tensor` of shape `(batch_size, sequence_length)`, *optional*):
-                Mask to avoid performing attention on padding token indices. Mask values selected in `[0, 1]`:
-
-                - 1 for tokens that are **not masked**,
-                - 0 for tokens that are **masked**.
-
-                [What are attention masks?](../glossary#attention-mask)
-            head_mask (`torch.Tensor` of shape `(num_hidden_layers, num_attention_heads)`, *optional*):
-                Mask to nullify selected heads of the attention modules. Mask values selected in `[0, 1]`:
-
-                - 1 indicates the head is **not masked**,
-                - 0 indicates the head is **masked**.
-
-            past_key_values (`tuple(tuple(torch.FloatTensor))`, *optional*, returned when `use_cache=True` is passed or when `config.use_cache=True`):
-                Tuple of `tuple(torch.FloatTensor)` of length `config.n_layers`, with each tuple having 2 tensors of
-                shape `(batch_size, num_heads, sequence_length, embed_size_per_head)`) and 2 additional tensors of
-                shape `(batch_size, num_heads, encoder_sequence_length, embed_size_per_head)`. The two additional
-                tensors are only required when the model is used as a decoder in a Sequence to Sequence model.
-
-                Contains pre-computed hidden-states (key and values in the self-attention blocks and in the
-                cross-attention blocks) that can be used (see `past_key_values` input) to speed up sequential decoding.
-
-                If `past_key_values` are used, the user can optionally input only the last `decoder_input_ids` (those
-                that don't have their past key value states given to this model) of shape `(batch_size, 1)` instead of
-                all `decoder_input_ids` of shape `(batch_size, sequence_length)`.
-            inputs_embeds (`torch.FloatTensor` of shape `(batch_size, sequence_length, hidden_size)`, *optional*):
-                Optionally, instead of passing `input_ids` you can choose to directly pass an embedded representation.
-                This is useful if you want more control over how to convert `input_ids` indices into associated vectors
-                than the model's internal embedding lookup matrix.
-            labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
-                Labels for computing the masked language modeling loss. Indices should either be in `[0, ...,
-                config.vocab_size]` or -100 (see `input_ids` docstring). Tokens with indices set to `-100` are ignored
-                (masked), the loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`.
-            use_cache (`bool`, *optional*):
-                If set to `True`, `past_key_values` key value states are returned and can be used to speed up decoding
-                (see `past_key_values`).
-            output_attentions (`bool`, *optional*):
-                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
-                returned tensors for more detail.
-            output_hidden_states (`bool`, *optional*):
-                Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
-                for more detail.
-            return_dict (`bool`, *optional*):
-                Whether or not to return a [`~utils.ModelOutput`] instead of a plain tuple.
-
-        Returns:
-
-        Example:
-
-        ```python
-        >>> from transformers import AutoTokenizer, OPTForCausalLM
-
-        >>> model = OPTForCausalLM.from_pretrained("facebook/opt-350m")
-        >>> tokenizer = AutoTokenizer.from_pretrained("facebook/opt-350m")
-
-        >>> prompt = "Hey, are you conscious? Can you talk to me?"
-        >>> inputs = tokenizer(prompt, return_tensors="pt")
-
-        >>> # Generate
-        >>> generate_ids = model.generate(inputs.input_ids, max_length=30)
-        >>> tokenizer.batch_decode(generate_ids, skip_special_tokens=True, clean_up_tokenization_spaces=False)[0]
-        "Hey, are you conscious? Can you talk to me?\nI'm not conscious. I'm just a little bit of a weirdo."
-        ```"""
-
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        # decoder outputs consists of (dec_features, layer_state, dec_hidden, dec_attn)
-        outputs = self.model.decoder(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            head_mask=head_mask,
-            past_key_values=past_key_values,
-            inputs_embeds=inputs_embeds,
-            use_cache=use_cache,
-            output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
-        )
-
-        logits = self.lm_head(outputs[0]).contiguous()
-
-        loss = None
-        if labels is not None:
-            # move labels to correct device to enable model parallelism
-            labels = labels.to(logits.device)
-            # Shift so that tokens < n predict n
-            shift_logits = logits[..., :-1, :].contiguous()
-            shift_labels = labels[..., 1:].contiguous()
-            shift_labels = shift_labels.view(-1)
-            # Enable model parallelism
-            shift_labels = shift_labels.to(shift_logits.device)
-            new_vocab_size = logits.shape[-1]
-            shift_logits = shift_logits.view(-1, new_vocab_size)
-            loss = cross_entropy_1d(
-                shift_logits,
-                shift_labels,
-                process_group=shard_config.tensor_parallel_process_group,
-                vocab_size=self.lm_head.out_features,
-            )
-
-        if not return_dict:
-            output = (logits,) + outputs[1:]
-            return (loss,) + output if loss is not None else output
-
-        return CausalLMOutputWithPast(
-            loss=loss,
-            logits=logits,
-            past_key_values=outputs.past_key_values,
-            hidden_states=outputs.hidden_states,
-            attentions=outputs.attentions,
-        )
-
-    return forward
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/qwen2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/t5.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,758 +1,785 @@
-from typing import List, Optional, Tuple, Union
+import warnings
+from typing import Dict, List, Optional, Tuple, Union
 
 import torch
-from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
+from torch.nn import CrossEntropyLoss
 from transformers.modeling_outputs import (
-    BaseModelOutputWithPast,
-    CausalLMOutputWithPast,
-    SequenceClassifierOutputWithPast,
+    BaseModelOutput,
+    BaseModelOutputWithPastAndCrossAttentions,
+    Seq2SeqLMOutput,
+    Seq2SeqModelOutput,
 )
-
-try:
-    from transformers.models.qwen2.modeling_qwen2 import (
-        Qwen2Attention,
-        Qwen2ForCausalLM,
-        Qwen2ForSequenceClassification,
-        Qwen2Model,
-        _prepare_4d_causal_attention_mask,
-        _prepare_4d_causal_attention_mask_for_sdpa,
-        apply_rotary_pos_emb,
-        repeat_kv,
-    )
-except ImportError:
-    Qwen2Model = "Qwen2Model"
-    Qwen2ForCausalLM = "Qwen2ForCausalLM"
-    Qwen2Attention = "Qwen2Attention"
-    Qwen2ForSequenceClassification = "Qwen2ForSequenceClassification"
-
+from transformers.models.t5.modeling_t5 import T5EncoderModel, T5ForConditionalGeneration, T5Model, T5Stack
 from transformers.utils import logging
 
 from colossalai.pipeline.stage_manager import PipelineStageManager
-from colossalai.shardformer.shard import ShardConfig
 
-from ..layer import ColoAttention, cross_entropy_1d
 
-
-class Qwen2PipelineForwards:
+class T5PipelineForwards:
     """
-    This class serves as a micro library for forward function substitution of Qwen2 models
-    under pipeline setting.
+    This class serves as a micro library for forward function substitution of
+    T5 models under pipeline setting.
     """
 
     @staticmethod
-    def qwen2_model_forward(
-        self: Qwen2Model,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
+    def t5_stack_forward(
+        self: T5Stack,
+        input_ids: Optional[torch.LongTensor] = None,
+        attention_mask: Optional[torch.FloatTensor] = None,
+        encoder_hidden_states: Optional[torch.Tensor] = None,
+        encoder_attention_mask: Optional[torch.FloatTensor] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
+        head_mask: Optional[torch.FloatTensor] = None,
+        cross_attn_head_mask: Optional[torch.Tensor] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        use_cache: Optional[bool] = False,
+        output_attentions: Optional[bool] = False,
+        output_hidden_states: Optional[bool] = False,
         return_dict: Optional[bool] = None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
         stage_index: Optional[List[int]] = None,
-        shard_config: ShardConfig = None,
-    ) -> Union[Tuple, BaseModelOutputWithPast]:
-        logger = logging.get_logger(__name__)
+        decoder_starting_stage: Optional[int] = None,
+    ) -> Union[Dict, Tuple, BaseModelOutputWithPastAndCrossAttentions]:
+        # This function is modified on the basis of transformers.models.t5.modeling_t5.T5Stack.forward.
+        # Please refer to original code of transformers for more details.
 
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        # retrieve input_ids and inputs_embeds
-        if stage_manager.is_first_stage():
-            if input_ids is not None and inputs_embeds is not None:
-                raise ValueError("You cannot specify both decoder_input_ids and decoder_inputs_embeds at the same time")
-            elif input_ids is not None:
-                batch_size, seq_length = input_ids.shape
-            elif inputs_embeds is not None:
-                batch_size, seq_length, _ = inputs_embeds.shape
-            else:
-                raise ValueError("You have to specify either decoder_input_ids or decoder_inputs_embeds")
-
-            device = input_ids.device if input_ids is not None else inputs_embeds.device
-            if inputs_embeds is None:
-                inputs_embeds = self.embed_tokens(input_ids)
-            hidden_states = inputs_embeds
-        else:
-            input_shape = hidden_states.shape[:-1]
-            batch_size, seq_length = input_shape
-            device = hidden_states.device
-
-        seq_length_with_past = seq_length
-        past_key_values_length = 0
+        logger = logging.get_logger(__name__)
 
-        # TODO(jianghai): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        # TODO(baizhou): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        if past_key_values:
+            logger.warning_once("Non-empty past_key_values is not supported for pipeline models at the moment.")
+            past_key_values = None
         if output_attentions:
             logger.warning_once("output_attentions=True is not supported for pipeline models at the moment.")
             output_attentions = False
         if output_hidden_states:
             logger.warning_once("output_hidden_states=True is not supported for pipeline models at the moment.")
             output_hidden_states = False
         if use_cache:
             logger.warning_once("use_cache=True is not supported for pipeline models at the moment.")
             use_cache = False
+        if use_cache is True:
+            if not in_decoder:
+                raise ValueError(f"`use_cache` can only be set to `True` if {self} is used as a decoder")
+        if self.gradient_checkpointing and self.training:
+            if use_cache:
+                logger.warning_once(
+                    "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
+                )
+                use_cache = False
 
-        # assert past_key_values is None, "past_key_values is not supported for Qwen2 models at the moment."
-
-        if past_key_values is not None:
-            past_key_values_length = past_key_values[0][0].shape[2]
-            seq_length_with_past = seq_length_with_past + past_key_values_length
-
-        if position_ids is None:
-            device = input_ids.device if input_ids is not None else inputs_embeds.device
-            position_ids = torch.arange(
-                past_key_values_length, seq_length + past_key_values_length, dtype=torch.long, device=device
-            )
-            position_ids = position_ids.unsqueeze(0).view(-1, seq_length)
-        else:
-            position_ids = position_ids.view(-1, seq_length).long()
+        stage = stage_manager.stage
+        in_decoder = self.is_decoder
+        if in_decoder != (stage >= decoder_starting_stage):
+            raise ValueError("Config in T5Stack is not aligned with pipeline setting.")
+
+        # at_first_stage: current stage is the first stage of encoder/decoder, taking input_ids/input_embeds
+        # at_last_stage: current stage is the last stage of encoder/decoder, making outputs the same form as huggingface
+        at_first_stage = (stage == 0) or (stage == decoder_starting_stage)
+        at_last_stage = (stage == decoder_starting_stage - 1) or (stage == stage_manager.num_stages - 1)
 
-        if attention_mask is not None and self._attn_implementation == "flash_attention_2" and use_cache:
-            is_padding_right = attention_mask[:, -1].sum().item() != batch_size
-            if is_padding_right:
+        # Process inputs if at the first stage of encoder/decoder.
+        if at_first_stage:
+            if input_ids is not None and inputs_embeds is not None:
+                err_msg_prefix = "decoder_" if in_decoder else ""
                 raise ValueError(
-                    "You are attempting to perform batched generation with padding_side='right'"
-                    " this may lead to unexpected behaviour for Flash Attention version of Qwen2. Make sure to "
-                    " call `tokenizer.padding_side  = 'left'` before tokenizing the input. "
+                    f"You cannot specify both {err_msg_prefix}input_ids and {err_msg_prefix}inputs_embeds at the same time"
                 )
-        # embed positions, for the first stage, hidden_states is the input embeddings,
-        # for the other stages, hidden_states is the output of the previous stage
-        if shard_config.enable_flash_attention:
-            # in this case, attention_mask is a dict rather than a tensor
-            mask_shape = (batch_size, 1, seq_length_with_past, seq_length_with_past)
-            attention_mask = ColoAttention.prepare_attn_kwargs(
-                mask_shape,
-                hidden_states.dtype,
-                hidden_states.device,
-                q_padding_mask=attention_mask,
-                is_causal=True,
-            )
+            elif input_ids is not None:
+                input_shape = input_ids.size()
+                input_ids = input_ids.view(-1, input_shape[-1])
+            elif inputs_embeds is not None:
+                input_shape = inputs_embeds.size()[:-1]
+            else:
+                err_msg_prefix = "decoder_" if in_decoder else ""
+                raise ValueError(
+                    f"You have to specify either {err_msg_prefix}input_ids or {err_msg_prefix}inputs_embeds"
+                )
+            if inputs_embeds is None:
+                if self.embed_tokens is None:
+                    raise ValueError("You have to initialize the model with valid token embeddings")
+                inputs_embeds = self.embed_tokens(input_ids)
+            batch_size, seq_length = input_shape
+            device = inputs_embeds.device
+            hidden_states = self.dropout(inputs_embeds)
         else:
-            if self._attn_implementation == "flash_attention_2":
-                # 2d mask is passed through the layers
-                attention_mask = attention_mask if (attention_mask is not None and 0 in attention_mask) else None
-            elif self._attn_implementation == "sdpa" and not output_attentions:
-                # output_attentions=True can not be supported when using SDPA, and we fall back on
-                # the manual implementation that requires a 4D causal mask in all cases.
-
-                attention_mask = _prepare_4d_causal_attention_mask_for_sdpa(
-                    attention_mask,
-                    (batch_size, seq_length),
-                    inputs_embeds,
-                    past_key_values_length,
+            if hidden_states is None:
+                raise ValueError(
+                    "hidden_states shouldn't be None for stages other than the first stage of encoder/decoder."
                 )
-            else:
-                # 4d mask is passed through the layers
+            input_shape = hidden_states.size()[:-1]
+            batch_size, seq_length = input_shape[0], input_shape[1]
+            device = hidden_states.device
 
-                attention_mask = _prepare_4d_causal_attention_mask(
-                    attention_mask,
-                    (batch_size, seq_length),
-                    hidden_states,
-                    past_key_values_length,
-                    sliding_window=self.config.sliding_window,
-                )
+        # required mask seq length can be calculated via length of past
+        mask_seq_length = past_key_values[0][0].shape[2] + seq_length if past_key_values is not None else seq_length
+
+        # initialize past_key_values with `None` if past does not exist
+        if past_key_values is None:
+            past_key_values = [None] * len(self.block)
+
+        if attention_mask is None:
+            attention_mask = torch.ones(batch_size, mask_seq_length, device=device)
+
+        # We can provide a self-attention mask of dimensions [batch_size, from_seq_length, to_seq_length]
+        # ourselves in which case we just need to make it broadcastable to all heads.
+        extended_attention_mask = self.get_extended_attention_mask(attention_mask, input_shape)
+
+        # If a 2D or 3D attention mask is provided for the cross-attention
+        # we need to make broadcastable to [batch_size, num_heads, seq_length, seq_length]
+        if self.is_decoder and encoder_hidden_states is not None:
+            encoder_batch_size, encoder_sequence_length, _ = encoder_hidden_states.size()
+            encoder_hidden_shape = (encoder_batch_size, encoder_sequence_length)
+            if encoder_attention_mask is None:
+                encoder_attention_mask = torch.ones(encoder_hidden_shape, device=inputs_embeds.device, dtype=torch.long)
+            encoder_extended_attention_mask = self.invert_attention_mask(encoder_attention_mask)
+        else:
+            encoder_extended_attention_mask = None
 
-        # decoder layers
+        # Prepare head mask if needed
+        head_mask = self.get_head_mask(head_mask, self.config.num_layers)
+        cross_attn_head_mask = self.get_head_mask(cross_attn_head_mask, self.config.num_layers)
+        present_key_value_states = () if use_cache else None
         all_hidden_states = () if output_hidden_states else None
-        all_self_attns = () if output_attentions else None
-        next_decoder_cache = None
+        all_attentions = () if output_attentions else None
+        all_cross_attentions = () if (output_attentions and self.is_decoder) else None
 
+        # Going through held blocks.
         start_idx, end_idx = stage_index[0], stage_index[1]
-        for idx, decoder_layer in enumerate(self.layers[start_idx:end_idx], start=start_idx):
-            if output_hidden_states:
-                all_hidden_states += (hidden_states,)
 
-            past_key_value = past_key_values[idx] if past_key_values is not None else None
+        for i in range(start_idx, end_idx):
+            past_key_value = past_key_values[i]
+            layer_module = self.block[i]
+            layer_head_mask = head_mask[i]
+            cross_attn_layer_head_mask = cross_attn_head_mask[i]
+            torch.cuda.set_device(hidden_states.device)
 
             if self.gradient_checkpointing and self.training:
                 layer_outputs = self._gradient_checkpointing_func(
-                    decoder_layer.__call__,
+                    layer_module.forward,
                     hidden_states,
-                    attention_mask,
-                    position_ids,
-                    past_key_values,
-                    output_attentions,
+                    extended_attention_mask,
+                    position_bias,
+                    encoder_hidden_states,
+                    encoder_extended_attention_mask,
+                    encoder_decoder_position_bias,
+                    layer_head_mask,
+                    cross_attn_layer_head_mask,
+                    None,  # past_key_value is always None with gradient checkpointing
                     use_cache,
+                    output_attentions,
                 )
             else:
-                layer_outputs = decoder_layer(
+                layer_outputs = layer_module(
                     hidden_states,
-                    attention_mask=attention_mask,
-                    position_ids=position_ids,
+                    attention_mask=extended_attention_mask,
+                    position_bias=position_bias,
+                    encoder_hidden_states=encoder_hidden_states,
+                    encoder_attention_mask=encoder_extended_attention_mask,
+                    encoder_decoder_position_bias=encoder_decoder_position_bias,
+                    layer_head_mask=layer_head_mask,
+                    cross_attn_layer_head_mask=cross_attn_layer_head_mask,
                     past_key_value=past_key_value,
-                    output_attentions=output_attentions,
                     use_cache=use_cache,
+                    output_attentions=output_attentions,
                 )
 
-            hidden_states = layer_outputs[0]
+            # layer_outputs is a tuple with:
+            # hidden-states, key-value-states, (self-attention position bias), (self-attention weights), (cross-attention position bias), (cross-attention weights)
 
+            if use_cache is False or use_cache is None:
+                layer_outputs = layer_outputs[:1] + (None,) + layer_outputs[1:]
+            hidden_states, present_key_value_state = layer_outputs[:2]
+
+            # We share the position biases between the layers - the first layer store them
+            # layer_outputs = hidden-states, key-value-states (self-attention position bias), (self-attention weights),
+            # (cross-attention position bias), (cross-attention weights)
+            position_bias = layer_outputs[2]
+
+            if in_decoder and encoder_hidden_states is not None:
+                encoder_decoder_position_bias = layer_outputs[4 if output_attentions else 3]
+            # append next layer key value states
             if use_cache:
-                next_decoder_cache += (layer_outputs[2 if output_attentions else 1],)
-
-            if output_attentions:
-                all_self_attns += (layer_outputs[1],)
+                present_key_value_states = present_key_value_states + (present_key_value_state,)
 
-        if stage_manager.is_last_stage():
-            hidden_states = self.norm(hidden_states)
-
-        # add hidden states from the last decoder layer
-        if output_hidden_states:
-            all_hidden_states += (hidden_states,)
+        # last layer
+        if at_last_stage:
+            hidden_states = self.final_layer_norm(hidden_states)
+            hidden_states = self.dropout(hidden_states)
 
-        next_cache = next_decoder_cache if use_cache else None
-
-        if stage_manager.is_last_stage():
             if not return_dict:
-                return tuple(v for v in [hidden_states, next_cache, all_hidden_states, all_self_attns] if v is not None)
-            return BaseModelOutputWithPast(
+                return tuple(
+                    v
+                    for v in [
+                        hidden_states,
+                        present_key_value_states,
+                        all_hidden_states,
+                        all_attentions,
+                        all_cross_attentions,
+                    ]
+                    if v is not None
+                )
+            return BaseModelOutputWithPastAndCrossAttentions(
                 last_hidden_state=hidden_states,
-                past_key_values=next_cache,
+                past_key_values=present_key_value_states,
                 hidden_states=all_hidden_states,
-                attentions=all_self_attns,
+                attentions=all_attentions,
+                cross_attentions=all_cross_attentions,
             )
-        # always return dict for imediate stage
-        return {"hidden_states": hidden_states}
+        else:
+            return {
+                "hidden_states": hidden_states,
+                "position_bias": position_bias,
+                "encoder_decoder_position_bias": encoder_decoder_position_bias,
+                "backward_tensor_keys": ["hidden_states"],
+            }
 
     @staticmethod
-    def qwen2_for_causal_lm_forward(
-        self: Qwen2ForCausalLM,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        labels: Optional[torch.LongTensor] = None,
+    def t5_model_forward(
+        self: T5Model,
+        input_ids: Optional[torch.LongTensor] = None,
+        attention_mask: Optional[torch.FloatTensor] = None,
+        decoder_input_ids: Optional[torch.LongTensor] = None,
+        decoder_attention_mask: Optional[torch.BoolTensor] = None,
+        head_mask: Optional[torch.FloatTensor] = None,
+        decoder_head_mask: Optional[torch.FloatTensor] = None,
+        cross_attn_head_mask: Optional[torch.Tensor] = None,
+        encoder_outputs: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        inputs_embeds: Optional[torch.Tensor] = None,
+        decoder_inputs_embeds: Optional[torch.Tensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
+        encoder_hidden_states: Optional[torch.FloatTensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
+        backward_tensor_keys: Optional[List[str]] = None,
         stage_index: Optional[List[int]] = None,
-        shard_config: ShardConfig = None,
-    ):
-        r"""
-        Args:
-            labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
-                Labels for computing the masked language modeling loss. Indices should either be in `[0, ...,
-                config.vocab_size]` or -100 (see `input_ids` docstring). Tokens with indices set to `-100` are ignored
-                (masked), the loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`.
-
-        Returns:
-
-        Example:
-
-        ```python
-        >>> from transformers import AutoTokenizer, Qwen2ForCausalLM
-
-        >>> model = Qwen2ForCausalLM.from_pretrained(PATH_TO_CONVERTED_WEIGHTS)
-        >>> tokenizer = AutoTokenizer.from_pretrained(PATH_TO_CONVERTED_TOKENIZER)
+        decoder_starting_stage: Optional[int] = None,
+    ) -> Union[Tuple[torch.FloatTensor], Seq2SeqModelOutput]:
+        # This function is modified on the basis of transformers.models.t5.modeling_t5.T5Model.forward.
+        # Please refer to original code of transformers for more details.
+
+        __HEAD_MASK_WARNING_MSG = """
+        The input argument `head_mask` was split into two arguments `head_mask` and `decoder_head_mask`. Currently,
+        `decoder_head_mask` is set to copy `head_mask`, but this feature is deprecated and will be removed in future versions.
+        If you do not want to use any `decoder_head_mask` now, please set `decoder_head_mask = torch.ones(num_layers,
+        num_heads)`.
+        """
 
-        >>> prompt = "Hey, are you consciours? Can you talk to me?"
-        >>> inputs = tokenizer(prompt, return_tensors="pt")
+        use_cache = use_cache if use_cache is not None else self.config.use_cache
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        >>> # Generate
-        >>> generate_ids = model.generate(inputs.input_ids, max_length=30)
-        >>> tokenizer.batch_decode(generate_ids, skip_special_tokens=True, clean_up_tokenization_spaces=False)[0]
-        "Hey, are you consciours? Can you talk to me?\nI'm not consciours, but I can talk to you."
-        ```"""
         logger = logging.get_logger(__name__)
 
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        # TODO(jianghai): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        # TODO(baizhou): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        if past_key_values:
+            logger.warning_once("Non-empty past_key_values is not supported for pipeline models at the moment.")
+            past_key_values = None
         if output_attentions:
             logger.warning_once("output_attentions=True is not supported for pipeline models at the moment.")
             output_attentions = False
         if output_hidden_states:
             logger.warning_once("output_hidden_states=True is not supported for pipeline models at the moment.")
             output_hidden_states = False
+        if use_cache:
+            logger.warning_once("use_cache=True is not supported for pipeline models at the moment.")
+            use_cache = False
 
-        # decoder outputs consists of (dec_features, layer_state, dec_hidden, dec_attn)
-        outputs = Qwen2PipelineForwards.qwen2_model_forward(
-            self.model,
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
+        # FutureWarning: head_mask was separated into two input args - head_mask, decoder_head_mask
+        if head_mask is not None and decoder_head_mask is None:
+            if self.config.num_layers == self.config.num_decoder_layers:
+                warnings.warn(__HEAD_MASK_WARNING_MSG, FutureWarning)
+                decoder_head_mask = head_mask
+
+        in_decoder = stage_manager.stage >= decoder_starting_stage
+        # Stage is in encoder, directly return the output of t5_stack_forward
+        if not in_decoder:
+            encoder_outputs = T5PipelineForwards.t5_stack_forward(
+                self.encoder,
+                input_ids=input_ids,
+                attention_mask=attention_mask,
+                inputs_embeds=inputs_embeds,
+                head_mask=head_mask,
+                output_attentions=output_attentions,
+                output_hidden_states=output_hidden_states,
+                return_dict=return_dict,
+                stage_manager=stage_manager,
+                hidden_states=hidden_states,
+                position_bias=position_bias,
+                encoder_decoder_position_bias=encoder_decoder_position_bias,
+                stage_index=stage_index,
+                decoder_starting_stage=decoder_starting_stage,
+            )
+            if stage_manager.stage == decoder_starting_stage - 1:
+                # last stage of encoder
+                return {"encoder_hidden_states": encoder_outputs[0]}
+            else:
+                return encoder_outputs
+
+        at_last_decoder_stage = stage_manager.is_last_stage()
+        at_first_decoder_stage = stage_manager.stage == decoder_starting_stage
+
+        if encoder_outputs is not None:
+            encoder_hidden_states = encoder_outputs[0]
+        elif encoder_hidden_states is None:
+            raise ValueError("Non-empty encoder_hidden_states should be passed in at decoder stages.")
+
+        if not at_first_decoder_stage and hidden_states is None:
+            raise ValueError("If not at the first layer of decoder, non-empty hidden_states must be provided.")
+
+        # Decode
+        decoder_outputs = T5PipelineForwards.t5_stack_forward(
+            self.decoder,
+            input_ids=decoder_input_ids,
+            attention_mask=decoder_attention_mask,
+            inputs_embeds=decoder_inputs_embeds,
             past_key_values=past_key_values,
-            inputs_embeds=inputs_embeds,
+            encoder_hidden_states=encoder_hidden_states,
+            encoder_attention_mask=attention_mask,
+            head_mask=decoder_head_mask,
+            cross_attn_head_mask=cross_attn_head_mask,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             stage_manager=stage_manager,
             hidden_states=hidden_states,
+            position_bias=position_bias,
+            encoder_decoder_position_bias=encoder_decoder_position_bias,
             stage_index=stage_index,
-            shard_config=shard_config,
+            decoder_starting_stage=decoder_starting_stage,
         )
-        past_key_values = None
-
-        if stage_manager.is_last_stage():
-            hidden_states = outputs[0]
-            logits = self.lm_head(hidden_states)
-            loss = None
-            if labels is not None:
-                # Shift so that tokens < n predict n
-                shift_logits = logits[..., :-1, :].contiguous()
-                shift_labels = labels[..., 1:].contiguous()
-                # Flatten the tokens
-                loss_fct = CrossEntropyLoss()
-                shift_labels = shift_labels.view(-1)
-                # Enable model parallelism
-                shift_labels = shift_labels.to(shift_logits.device)
-                if shard_config.enable_tensor_parallelism:
-                    new_vocab_size = logits.shape[-1]
-                    shift_logits = shift_logits.view(-1, new_vocab_size)
-                    loss = cross_entropy_1d(
-                        shift_logits, shift_labels, process_group=shard_config.tensor_parallel_process_group
-                    )
-                else:
-                    shift_logits = shift_logits.view(-1, self.config.vocab_size)
-                    loss = loss_fct(shift_logits, shift_labels)
 
-            if not return_dict:
-                output = (logits,) + outputs[1:]
-                return (loss,) + output if loss is not None else output
+        # Directly return outputs of overloaded T5Stack forward if not at last stage.
+        if not at_last_decoder_stage:
+            # encoder_hidden_states should be passed to the next stage
+            decoder_outputs["encoder_hidden_states"] = encoder_hidden_states
+            return decoder_outputs
 
-            return CausalLMOutputWithPast(
-                loss=loss,
-                logits=logits,
-                past_key_values=outputs.past_key_values,
-                hidden_states=outputs.hidden_states,
-                attentions=outputs.attentions,
-            )
+        if not return_dict:
+            return decoder_outputs + encoder_hidden_states
         else:
-            hidden_states = outputs.get("hidden_states")
-            return {"hidden_states": hidden_states}
+            return Seq2SeqModelOutput(
+                last_hidden_state=decoder_outputs.last_hidden_state,
+                past_key_values=decoder_outputs.past_key_values,
+                decoder_hidden_states=decoder_outputs.hidden_states,
+                decoder_attentions=decoder_outputs.attentions,
+                cross_attentions=decoder_outputs.cross_attentions,
+                encoder_last_hidden_state=encoder_hidden_states,
+            )
 
     @staticmethod
-    def qwen2_for_sequence_classification_forward(
-        self: Qwen2ForSequenceClassification,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
+    def t5_for_conditional_generation_forward(
+        self: T5ForConditionalGeneration,
+        input_ids: Optional[torch.LongTensor] = None,
+        attention_mask: Optional[torch.FloatTensor] = None,
+        decoder_input_ids: Optional[torch.LongTensor] = None,
+        decoder_attention_mask: Optional[torch.BoolTensor] = None,
+        head_mask: Optional[torch.FloatTensor] = None,
+        decoder_head_mask: Optional[torch.FloatTensor] = None,
+        cross_attn_head_mask: Optional[torch.Tensor] = None,
+        encoder_outputs: Optional[Tuple[Tuple[torch.Tensor]]] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
+        decoder_inputs_embeds: Optional[torch.FloatTensor] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
+        encoder_hidden_states: Optional[torch.FloatTensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
+        backward_tensor_keys: Optional[List[str]] = None,
         stage_index: Optional[List[int]] = None,
-        shard_config: ShardConfig = None,
-    ):
-        r"""
-        labels (`torch.LongTensor` of shape `(batch_size,)`, *optional*):
-            Labels for computing the sequence classification/regression loss. Indices should be in `[0, ...,
-            config.num_labels - 1]`. If `config.num_labels == 1` a regression loss is computed (Mean-Square loss), If
-            `config.num_labels > 1` a classification loss is computed (Cross-Entropy).
+        decoder_starting_stage: Optional[int] = None,
+    ) -> Union[Tuple[torch.FloatTensor], Seq2SeqLMOutput]:
+        # This function is modified on the basis of transformers.models.t5.modeling_t5.T5ForConditionalGeneration.forward.
+        # Please refer to original code of transformers for more details.
+
+        __HEAD_MASK_WARNING_MSG = """
+        The input argument `head_mask` was split into two arguments `head_mask` and `decoder_head_mask`. Currently,
+        `decoder_head_mask` is set to copy `head_mask`, but this feature is deprecated and will be removed in future versions.
+        If you do not want to use any `decoder_head_mask` now, please set `decoder_head_mask = torch.ones(num_layers,
+        num_heads)`.
         """
-        logger = logging.get_logger(__name__)
 
+        use_cache = use_cache if use_cache is not None else self.config.use_cache
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        # TODO(jianghai): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        logger = logging.get_logger(__name__)
+
+        # TODO(baizhou): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        if past_key_values:
+            logger.warning_once("Non-empty past_key_values is not supported for pipeline models at the moment.")
+            past_key_values = None
         if output_attentions:
             logger.warning_once("output_attentions=True is not supported for pipeline models at the moment.")
             output_attentions = False
         if output_hidden_states:
             logger.warning_once("output_hidden_states=True is not supported for pipeline models at the moment.")
             output_hidden_states = False
+        if use_cache:
+            logger.warning_once("use_cache=True is not supported for pipeline models at the moment.")
+            use_cache = False
 
-        transformer_outputs = Qwen2PipelineForwards.qwen2_model_forward(
-            self.model,
-            input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
+        # FutureWarning: head_mask was separated into two input args - head_mask, decoder_head_mask
+        if head_mask is not None and decoder_head_mask is None:
+            if self.config.num_layers == self.config.num_decoder_layers:
+                warnings.warn(__HEAD_MASK_WARNING_MSG, FutureWarning)
+                decoder_head_mask = head_mask
+
+        in_decoder = stage_manager.stage >= decoder_starting_stage
+
+        # Stage is in encoder, directly return the output of t5_stack_forward
+        if not in_decoder:
+            encoder_outputs = T5PipelineForwards.t5_stack_forward(
+                self.encoder,
+                input_ids=input_ids,
+                attention_mask=attention_mask,
+                inputs_embeds=inputs_embeds,
+                head_mask=head_mask,
+                output_attentions=output_attentions,
+                output_hidden_states=output_hidden_states,
+                return_dict=return_dict,
+                stage_manager=stage_manager,
+                hidden_states=hidden_states,
+                position_bias=position_bias,
+                encoder_decoder_position_bias=encoder_decoder_position_bias,
+                stage_index=stage_index,
+                decoder_starting_stage=decoder_starting_stage,
+            )
+            if stage_manager.stage == decoder_starting_stage - 1:
+                # last stage of encoder
+                return {"encoder_hidden_states": encoder_outputs[0]}
+            else:
+                return encoder_outputs
+
+        at_last_decoder_stage = stage_manager.is_last_stage()
+        at_first_decoder_stage = stage_manager.stage == decoder_starting_stage
+
+        if encoder_outputs is not None:
+            encoder_hidden_states = encoder_outputs[0]
+        elif encoder_hidden_states is None:
+            raise ValueError("Non-empty encoder_hidden_states should be passed in at decoder stages.")
+
+        if not at_first_decoder_stage and hidden_states is None:
+            raise ValueError("If not at the first layer of decoder, non-empty hidden_states must be provided.")
+
+        if labels is not None and decoder_input_ids is None and decoder_inputs_embeds is None:
+            # get decoder inputs from shifting lm labels to the right
+            decoder_input_ids = self._shift_right(labels)
+
+        # Decode
+        decoder_outputs = T5PipelineForwards.t5_stack_forward(
+            self.decoder,
+            input_ids=decoder_input_ids,
+            attention_mask=decoder_attention_mask,
+            inputs_embeds=decoder_inputs_embeds,
             past_key_values=past_key_values,
-            inputs_embeds=inputs_embeds,
+            encoder_hidden_states=encoder_hidden_states,
+            encoder_attention_mask=attention_mask,
+            head_mask=decoder_head_mask,
+            cross_attn_head_mask=cross_attn_head_mask,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             stage_manager=stage_manager,
             hidden_states=hidden_states,
+            position_bias=position_bias,
+            encoder_decoder_position_bias=encoder_decoder_position_bias,
             stage_index=stage_index,
-            shard_config=shard_config,
+            decoder_starting_stage=decoder_starting_stage,
         )
 
-        if input_ids is not None:
-            batch_size = input_ids.shape[0]
-        elif inputs_embeds is not None:
-            batch_size = inputs_embeds.shape[0]
-        else:
-            batch_size = hidden_states.shape[0]
-
-        if stage_manager.is_last_stage():
-            hidden_states = transformer_outputs[0]
-            logits = self.score(hidden_states)
-
-            if self.config.pad_token_id is None and batch_size != 1:
-                print(self.config.pad_token_id)
-                raise ValueError("Cannot handle batch sizes > 1 if no padding token is defined.")
-            if self.config.pad_token_id is None:
-                sequence_lengths = -1
-            else:
-                if input_ids is not None:
-                    sequence_lengths = (torch.ne(input_ids, self.config.pad_token_id).sum(-1) - 1).to(logits.device)
-                else:
-                    sequence_lengths = -1
+        # Directly return outputs of overloaded T5Stack forward if not at last stage.
+        if not at_last_decoder_stage:
+            # encoder_hidden_states should be passed to the next stage
+            decoder_outputs["encoder_hidden_states"] = encoder_hidden_states
+            return decoder_outputs
+
+        sequence_output = decoder_outputs[0]
+
+        if self.config.tie_word_embeddings:
+            # Rescale output before projecting on vocab
+            # See https://github.com/tensorflow/mesh/blob/fa19d69eafc9a482aff0b59ddd96b025c0cb207d/mesh_tensorflow/transformer/transformer.py#L586
+            sequence_output = sequence_output * (self.model_dim**-0.5)
 
-            pooled_logits = logits[torch.arange(batch_size, device=logits.device), sequence_lengths]
-
-            loss = None
-            if labels is not None:
-                labels = labels.to(logits.device)
-                if self.config.problem_type is None:
-                    if self.num_labels == 1:
-                        self.config.problem_type = "regression"
-                    elif self.num_labels > 1 and (labels.dtype == torch.long or labels.dtype == torch.int):
-                        self.config.problem_type = "single_label_classification"
-                    else:
-                        self.config.problem_type = "multi_label_classification"
-
-                if self.config.problem_type == "regression":
-                    loss_fct = MSELoss()
-                    if self.num_labels == 1:
-                        loss = loss_fct(pooled_logits.squeeze(), labels.squeeze())
-                    else:
-                        loss = loss_fct(pooled_logits, labels)
-                elif self.config.problem_type == "single_label_classification":
-                    loss_fct = CrossEntropyLoss()
-                    loss = loss_fct(pooled_logits.view(-1, self.num_labels), labels.view(-1))
-                elif self.config.problem_type == "multi_label_classification":
-                    loss_fct = BCEWithLogitsLoss()
-                    loss = loss_fct(pooled_logits, labels)
-            if not return_dict:
-                output = (pooled_logits,) + transformer_outputs[1:]
-                return ((loss,) + output) if loss is not None else output
-
-            return SequenceClassifierOutputWithPast(
-                loss=loss,
-                logits=pooled_logits,
-                past_key_values=transformer_outputs.past_key_values,
-                hidden_states=transformer_outputs.hidden_states,
-                attentions=transformer_outputs.attentions,
-            )
+        lm_logits = self.lm_head(sequence_output)
 
-        else:
-            hidden_states = transformer_outputs.get("hidden_states")
-            return {"hidden_states": hidden_states}
-
-
-def get_qwen2_flash_attention_forward(shard_config: ShardConfig):
-    def forward(
-        self: Qwen2Attention,
-        hidden_states: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_value: Optional[Tuple[torch.Tensor]] = None,
-        output_attentions: bool = False,
-        use_cache: bool = False,
-        **kwargs,
-    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
-        bsz, q_len, _ = hidden_states.size()
-
-        query_states = self.q_proj(hidden_states)
-        key_states = self.k_proj(hidden_states)
-        value_states = self.v_proj(hidden_states)
-
-        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        key_states = key_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
-        value_states = value_states.view(bsz, q_len, self.num_key_value_heads, self.head_dim).transpose(1, 2)
-
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            if self.layer_idx is None:
-                raise ValueError(
-                    f"The cache structure has changed since version v4.36. If you are using {self.__class__.__name__} "
-                    "for auto-regressive decoding with k/v caching, please make sure to initialize the attention class "
-                    "with a layer index."
-                )
-            kv_seq_len += past_key_value.get_usable_length(kv_seq_len, self.layer_idx)
-        # Because the input can be padded, the absolute sequence length depends on the max position id.
-        rotary_seq_len = max(kv_seq_len, position_ids[:, -1].max().item()) + 1
-        cos, sin = self.rotary_emb(value_states, seq_len=rotary_seq_len)
-
-        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
-
-        if past_key_value is not None:
-            # Activate slicing cache only if the config has a value `sliding_windows` attribute
-            cache_has_contents = past_key_value.get_seq_length(self.layer_idx) > 0
-            if (
-                getattr(self.config, "sliding_window", None) is not None
-                and kv_seq_len > self.config.sliding_window
-                and cache_has_contents
-            ):
-                slicing_tokens = 1 - self.config.sliding_window
-
-                past_key = past_key_value[self.layer_idx][0]
-                past_value = past_key_value[self.layer_idx][1]
-
-                past_key = past_key[:, :, slicing_tokens:, :].contiguous()
-                past_value = past_value[:, :, slicing_tokens:, :].contiguous()
-
-                if past_key.shape[-2] != self.config.sliding_window - 1:
-                    raise ValueError(
-                        f"past key must have a shape of (`batch_size, num_heads, self.config.sliding_window-1, head_dim`), got"
-                        f" {past_key.shape}"
-                    )
-
-                if attention_mask is not None:
-                    attention_mask = attention_mask[:, slicing_tokens:]
-                    attention_mask = torch.cat([attention_mask, torch.ones_like(attention_mask[:, -1:])], dim=-1)
-
-            cache_kwargs = {"sin": sin, "cos": cos}  # Specific to RoPE models
-            key_states, value_states = past_key_value.update(key_states, value_states, self.layer_idx, cache_kwargs)
-
-        # repeat k/v heads if n_kv_heads < n_heads
-        key_states = repeat_kv(key_states, self.num_key_value_groups)
-        value_states = repeat_kv(value_states, self.num_key_value_groups)
-
-        assert isinstance(attention_mask, dict), "Flash Attention Error: attention_mask should be a dict."
-        attn_output = ColoAttention.attention(query_states, key_states, value_states, **attention_mask)
-        attn_output = attn_output.transpose(1, 2).contiguous()
-        attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
-        attn_output = self.o_proj(attn_output)
-
-        return attn_output, None, past_key_value
-
-    return forward
+        loss = None
+        if labels is not None:
+            loss_fct = CrossEntropyLoss(ignore_index=-100)
+            # move labels to correct device to enable PP
+            labels = labels.to(lm_logits.device)
+            loss = loss_fct(lm_logits.view(-1, lm_logits.size(-1)), labels.view(-1))
 
+        if not return_dict:
+            output = (lm_logits,) + decoder_outputs[1:] + encoder_hidden_states
+            return ((loss,) + output) if loss is not None else output
 
-def get_qwen2_model_forward_for_flash_attn(shard_config: ShardConfig):
-    logger = logging.get_logger(__name__)
-    assert shard_config.enable_flash_attention, "Flash Attention is not enabled."
+        return Seq2SeqLMOutput(
+            loss=loss,
+            logits=lm_logits,
+            past_key_values=decoder_outputs.past_key_values,
+            decoder_hidden_states=decoder_outputs.hidden_states,
+            decoder_attentions=decoder_outputs.attentions,
+            cross_attentions=decoder_outputs.cross_attentions,
+            encoder_last_hidden_state=encoder_hidden_states,
+        )
 
-    def forward(
-        self,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
+    @staticmethod
+    def t5_encoder_model_forward(
+        self: T5EncoderModel,
+        input_ids: Optional[torch.LongTensor] = None,
+        attention_mask: Optional[torch.FloatTensor] = None,
+        head_mask: Optional[torch.FloatTensor] = None,
         inputs_embeds: Optional[torch.FloatTensor] = None,
-        use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, BaseModelOutputWithPast]:
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-
+        stage_manager: Optional[PipelineStageManager] = None,
+        hidden_states: Optional[torch.FloatTensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
+        backward_tensor_keys: Optional[List[str]] = None,
+        stage_index: Optional[List[int]] = None,
+        decoder_starting_stage: Optional[int] = None,
+    ) -> Union[Tuple[torch.FloatTensor], BaseModelOutput]:
+        r"""
+        This function is modified on the basis of transformers.models.t5.modeling_gpt2.T5EncoderModel.forward.
+        Please refer to original code of transformers for more details.
+        ```"""
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        # retrieve input_ids and inputs_embeds
-        if input_ids is not None and inputs_embeds is not None:
-            raise ValueError("You cannot specify both decoder_input_ids and decoder_inputs_embeds at the same time")
-        elif input_ids is not None:
-            batch_size, seq_length = input_ids.shape
-        elif inputs_embeds is not None:
-            batch_size, seq_length, _ = inputs_embeds.shape
-        else:
-            raise ValueError("You have to specify either decoder_input_ids or decoder_inputs_embeds")
+        outputs = T5PipelineForwards.t5_stack_forward(
+            self.encoder,
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            inputs_embeds=inputs_embeds,
+            head_mask=head_mask,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            return_dict=return_dict,
+            stage_manager=stage_manager,
+            hidden_states=hidden_states,
+            position_bias=position_bias,
+            encoder_decoder_position_bias=encoder_decoder_position_bias,
+            stage_index=stage_index,
+            decoder_starting_stage=decoder_starting_stage,
+        )
 
-        seq_length_with_past = seq_length
-        past_key_values_length = 0
+        return outputs
 
-        if position_ids is None:
-            device = input_ids.device if input_ids is not None else inputs_embeds.device
-            position_ids = torch.arange(
-                past_key_values_length, seq_length + past_key_values_length, dtype=torch.long, device=device
-            )
-            position_ids = position_ids.unsqueeze(0).view(-1, seq_length)
-        else:
-            position_ids = position_ids.view(-1, seq_length).long()
 
-        if inputs_embeds is None:
-            inputs_embeds = self.embed_tokens(input_ids)
+def get_t5_flash_attention_forward():
+    from transformers.models.t5.modeling_t5 import T5Attention
 
-        # embed positions
-        hidden_states = inputs_embeds
+    def forward(
+        self: T5Attention,
+        hidden_states: torch.Tensor,
+        mask: Optional[torch.Tensor] = None,
+        key_value_states: Optional[torch.Tensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        query_length: Optional[int] = None,
+        use_cache: bool = False,
+        output_attentions: bool = False,
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]:
+        """
+        Self-attention (if key_value_states is None) or attention over source sentence (provided by key_value_states).
+        """
+        # Input is (batch_size, seq_length, dim)
+        # Mask is (batch_size, key_length) (non-causal) or (batch_size, key_length, key_length)
+        # past_key_value[0] is (batch_size, n_heads, q_len - 1, dim_per_head)
+        batch_size, seq_length = hidden_states.shape[:2]
 
-        # in this case, attention_mask is a dict rather than a tensor
-        mask_shape = (batch_size, 1, seq_length_with_past, seq_length_with_past)
-        attention_mask = ColoAttention.prepare_attn_kwargs(
-            mask_shape,
-            hidden_states.dtype,
-            hidden_states.device,
-            q_padding_mask=attention_mask,
-            is_causal=True,
-        )
+        real_seq_length = seq_length
 
-        if self.gradient_checkpointing and self.training:
-            if use_cache:
-                logger.warning_once(
-                    "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
+        if past_key_value is not None:
+            if len(past_key_value) != 2:
+                raise ValueError(
+                    f"past_key_value should have 2 past states: keys and values. Got { len(past_key_value)} past states"
                 )
-                use_cache = False
+            real_seq_length += past_key_value[0].shape[2] if query_length is None else query_length
 
-        # decoder layers
-        all_hidden_states = () if output_hidden_states else None
-        all_self_attns = () if output_attentions else None
-        next_decoder_cache = None
+        key_length = real_seq_length if key_value_states is None else key_value_states.shape[1]
 
-        for decoder_layer in self.layers:
-            if output_hidden_states:
-                all_hidden_states += (hidden_states,)
+        def shape(states):
+            """projection"""
+            return states.view(batch_size, -1, self.n_heads, self.key_value_proj_dim).transpose(1, 2)
+
+        def unshape(states):
+            """reshape"""
+            return states.transpose(1, 2).contiguous().view(batch_size, -1, self.inner_dim)
+
+        def project(hidden_states, proj_layer, key_value_states, past_key_value):
+            """projects hidden states correctly to key/query states"""
+            if key_value_states is None:
+                # self-attn
+                # (batch_size, n_heads, seq_length, dim_per_head)
+                hidden_states = shape(proj_layer(hidden_states))
+            elif past_key_value is None:
+                # cross-attn
+                # (batch_size, n_heads, seq_length, dim_per_head)
+                hidden_states = shape(proj_layer(key_value_states))
+
+            if past_key_value is not None:
+                if key_value_states is None:
+                    # self-attn
+                    # (batch_size, n_heads, key_length, dim_per_head)
+                    hidden_states = torch.cat([past_key_value, hidden_states], dim=2)
+                elif past_key_value.shape[2] != key_value_states.shape[1]:
+                    # checking that the `sequence_length` of the `past_key_value` is the same as
+                    # the provided `key_value_states` to support prefix tuning
+                    # cross-attn
+                    # (batch_size, n_heads, seq_length, dim_per_head)
+                    hidden_states = shape(proj_layer(key_value_states))
+                else:
+                    # cross-attn
+                    hidden_states = past_key_value
+            return hidden_states
+
+        # get query states
+        query_states = shape(self.q(hidden_states))  # (batch_size, n_heads, seq_length, dim_per_head)
+
+        # get key/value states
+        key_states = project(
+            hidden_states, self.k, key_value_states, past_key_value[0] if past_key_value is not None else None
+        )
+        value_states = project(
+            hidden_states, self.v, key_value_states, past_key_value[1] if past_key_value is not None else None
+        )
 
-            if self.gradient_checkpointing and self.training:
-                layer_outputs = self._gradient_checkpointing_func(
-                    decoder_layer.__call__,
-                    hidden_states,
-                    attention_mask,
-                    position_ids,
-                    past_key_values,
-                    output_attentions,
-                    use_cache,
+        if position_bias is None:
+            if not self.has_relative_attention_bias:
+                position_bias = torch.zeros(
+                    (1, self.n_heads, real_seq_length, key_length), device=query_states.device, dtype=query_states.dtype
                 )
+                if self.gradient_checkpointing and self.training:
+                    position_bias.requires_grad = True
             else:
-                layer_outputs = decoder_layer(
-                    hidden_states,
-                    attention_mask=attention_mask,
-                    position_ids=position_ids,
-                    past_key_value=past_key_values,
-                    output_attentions=output_attentions,
-                    use_cache=use_cache,
-                )
-
-            hidden_states = layer_outputs[0]
-
-            if use_cache:
-                next_decoder_cache = layer_outputs[2 if output_attentions else 1]
+                position_bias = self.compute_bias(real_seq_length, key_length, device=query_states.device)
 
-            if output_attentions:
-                all_self_attns += (layer_outputs[1],)
+            # if key and values are already calculated
+            # we want only the last query position bias
+            if past_key_value is not None:
+                position_bias = position_bias[:, :, -hidden_states.size(1) :, :]
+
+            if mask is not None:
+                position_bias = position_bias + mask  # (batch_size, n_heads, seq_length, key_length)
+
+        if self.pruned_heads:
+            mask = torch.ones(position_bias.shape[1])
+            mask[list(self.pruned_heads)] = 0
+            position_bias_masked = position_bias[:, mask.bool()]
+        else:
+            position_bias_masked = position_bias
 
-        hidden_states = self.norm(hidden_states)
+        with torch.backends.cuda.sdp_kernel(enable_flash=True, enable_mem_efficient=True):
+            attn_output = torch.nn.functional.scaled_dot_product_attention(
+                query_states,
+                key_states,
+                value_states,
+                attn_mask=position_bias_masked,
+                dropout_p=self.dropout,
+                scale=1.0,
+            )
+        attn_output = unshape(attn_output)
+        attn_output = self.o(attn_output)
 
-        # add hidden states from the last decoder layer
-        if output_hidden_states:
-            all_hidden_states += (hidden_states,)
+        present_key_value_state = (key_states, value_states) if (self.is_decoder and use_cache) else None
 
-        next_cache = next_decoder_cache if use_cache else None
+        outputs = (attn_output,) + (present_key_value_state,) + (position_bias,)
 
-        if not return_dict:
-            return tuple(v for v in [hidden_states, next_cache, all_hidden_states, all_self_attns] if v is not None)
-        return BaseModelOutputWithPast(
-            last_hidden_state=hidden_states,
-            past_key_values=next_cache,
-            hidden_states=all_hidden_states,
-            attentions=all_self_attns,
-        )
+        return outputs
 
     return forward
 
 
-def get_lm_forward_with_dist_cross_entropy(shard_config: ShardConfig):
-    def forward(
-        self: Qwen2ForCausalLM,
-        input_ids: torch.LongTensor = None,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_ids: Optional[torch.LongTensor] = None,
-        past_key_values: Optional[List[torch.FloatTensor]] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        labels: Optional[torch.LongTensor] = None,
-        use_cache: Optional[bool] = None,
-        output_attentions: Optional[bool] = None,
-        output_hidden_states: Optional[bool] = None,
-        return_dict: Optional[bool] = None,
-    ) -> Union[Tuple, CausalLMOutputWithPast]:
-        r"""
-        Args:
-            labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
-                Labels for computing the masked language modeling loss. Indices should either be in `[0, ...,
-                config.vocab_size]` or -100 (see `input_ids` docstring). Tokens with indices set to `-100` are ignored
-                (masked), the loss is only computed for the tokens with labels in `[0, ..., config.vocab_size]`.
-
-        Returns:
+def get_jit_fused_T5_layer_ff_forward():
+    from transformers.models.t5.modeling_t5 import T5LayerFF
 
-        Example:
+    def forward(self: T5LayerFF, hidden_states: torch.Tensor) -> torch.Tensor:
+        forwarded_states = self.layer_norm(hidden_states)
+        forwarded_states = self.DenseReluDense(forwarded_states)
+        hidden_states = self.dropout_add(forwarded_states, hidden_states, self.dropout.p, self.dropout.training)
+        return hidden_states
 
-        ```python
-        >>> from transformers import AutoTokenizer, Qwen2ForCausalLM
-
-        >>> model = Qwen2ForCausalLM.from_pretrained(PATH_TO_CONVERTED_WEIGHTS)
-        >>> tokenizer = AutoTokenizer.from_pretrained(PATH_TO_CONVERTED_TOKENIZER)
-
-        >>> prompt = "Hey, are you conscious? Can you talk to me?"
-        >>> inputs = tokenizer(prompt, return_tensors="pt")
+    return forward
 
-        >>> # Generate
-        >>> generate_ids = model.generate(inputs.input_ids, max_length=30)
-        >>> tokenizer.batch_decode(generate_ids, skip_special_tokens=True, clean_up_tokenization_spaces=False)[0]
-        "Hey, are you conscious? Can you talk to me?\nI'm not conscious, but I can talk to you."
-        ```"""
 
-        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-        output_hidden_states = (
-            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-        )
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+def get_T5_layer_self_attention_forward():
+    from transformers.models.t5.modeling_t5 import T5LayerSelfAttention
 
-        # decoder outputs consists of (dec_features, layer_state, dec_hidden, dec_attn)
-        outputs = self.model(
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            position_ids=position_ids,
-            past_key_values=past_key_values,
-            inputs_embeds=inputs_embeds,
+    def forward(
+        self: T5LayerSelfAttention,
+        hidden_states: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        use_cache: bool = False,
+        output_attentions: bool = False,
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]:
+        normed_hidden_states = self.layer_norm(hidden_states)
+        attention_output = self.SelfAttention(
+            normed_hidden_states,
+            mask=attention_mask,
+            position_bias=position_bias,
+            layer_head_mask=layer_head_mask,
+            past_key_value=past_key_value,
             use_cache=use_cache,
             output_attentions=output_attentions,
-            output_hidden_states=output_hidden_states,
-            return_dict=return_dict,
         )
+        hidden_states = self.dropout_add(attention_output[0], hidden_states, self.dropout.p, self.dropout.training)
+        outputs = (hidden_states,) + attention_output[1:]  # add attentions if we output them
+        return outputs
 
-        hidden_states = outputs[0]
-        logits = self.lm_head(hidden_states)
-        logits = logits.float()
+    return forward
 
-        loss = None
-        if labels is not None:
-            # Shift so that tokens < n predict n
-            shift_logits = logits[..., :-1, :].contiguous()
-            shift_labels = labels[..., 1:].contiguous()
-            # Flatten the tokens
-            loss_fct = CrossEntropyLoss()
-            shift_labels = shift_labels.view(-1)
-            # Enable model parallelism
-            shift_labels = shift_labels.to(shift_logits.device)
-            if shard_config.enable_tensor_parallelism:
-                new_vocab_size = logits.shape[-1]
-                shift_logits = shift_logits.view(-1, new_vocab_size)
-                loss = cross_entropy_1d(
-                    shift_logits, shift_labels, process_group=shard_config.tensor_parallel_process_group
-                )
-            else:
-                shift_logits = shift_logits.view(-1, self.config.vocab_size)
-                loss = loss_fct(shift_logits, shift_labels)
 
-        if not return_dict:
-            output = (logits,) + outputs[1:]
-            return (loss,) + output if loss is not None else output
+def get_T5_layer_cross_attention_forward():
+    from transformers.models.t5.modeling_t5 import T5LayerCrossAttention
 
-        return CausalLMOutputWithPast(
-            loss=loss,
-            logits=logits,
-            past_key_values=outputs.past_key_values,
-            hidden_states=outputs.hidden_states,
-            attentions=outputs.attentions,
+    def forward(
+        self: T5LayerCrossAttention,
+        hidden_states: torch.Tensor,
+        key_value_states: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
+        position_bias: Optional[torch.Tensor] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        use_cache: bool = False,
+        query_length: Optional[int] = None,
+        output_attentions: bool = False,
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]:
+        normed_hidden_states = self.layer_norm(hidden_states)
+        attention_output = self.EncDecAttention(
+            normed_hidden_states,
+            mask=attention_mask,
+            key_value_states=key_value_states,
+            position_bias=position_bias,
+            layer_head_mask=layer_head_mask,
+            past_key_value=past_key_value,
+            use_cache=use_cache,
+            query_length=query_length,
+            output_attentions=output_attentions,
         )
+        layer_output = self.dropout_add(attention_output[0], hidden_states, self.dropout.p, self.dropout.training)
+        outputs = (layer_output,) + attention_output[1:]  # add attentions if we output them
+        return outputs
 
     return forward
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/sam.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/t5.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/whisper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,785 +1,1169 @@
-import warnings
-from typing import Dict, List, Optional, Tuple, Union
+import logging
+import random
+from typing import List, Optional, Tuple, Union
 
 import torch
+from torch import nn
 from torch.nn import CrossEntropyLoss
+from transformers.modeling_attn_mask_utils import (
+    _prepare_4d_causal_attention_mask,
+    _prepare_4d_causal_attention_mask_for_sdpa,
+)
 from transformers.modeling_outputs import (
     BaseModelOutput,
     BaseModelOutputWithPastAndCrossAttentions,
     Seq2SeqLMOutput,
     Seq2SeqModelOutput,
+    SequenceClassifierOutput,
+)
+from transformers.models.whisper.modeling_whisper import (
+    WhisperDecoder,
+    WhisperEncoder,
+    WhisperForAudioClassification,
+    WhisperForConditionalGeneration,
+    WhisperModel,
+    shift_tokens_right,
 )
-from transformers.models.t5.modeling_t5 import T5EncoderModel, T5ForConditionalGeneration, T5Model, T5Stack
 from transformers.utils import logging
 
 from colossalai.pipeline.stage_manager import PipelineStageManager
+from colossalai.shardformer.layer import ColoAttention
+from colossalai.shardformer.shard import ShardConfig
+
+logger = logging.get_logger(__name__)
+
+
+def _get_attention_mask(
+    self: WhisperDecoder,
+    shard_config: ShardConfig,
+    hidden_states: torch.Tensor,
+    past_key_values_length: int,
+    attention_mask: Optional[torch.FloatTensor],
+    head_mask: Optional[torch.Tensor] = None,
+    output_attentions: bool = False,
+):
+    batch_size, seq_length = hidden_states.shape[:2]
+    mask_seq_length = past_key_values_length + seq_length
+    if shard_config.enable_flash_attention:
+        attention_mask = ColoAttention.prepare_attn_kwargs(
+            (batch_size, 1, seq_length, mask_seq_length),
+            hidden_states.dtype,
+            hidden_states.device,
+            attention_mask,
+            is_causal=True,
+        )
+    else:
+        input_shape = (batch_size, seq_length)
+        if self._use_flash_attention_2:
+            # 2d mask is passed through the layers
+            attention_mask = attention_mask if (attention_mask is not None and 0 in attention_mask) else None
+        elif self._use_sdpa and head_mask is None and not output_attentions:
+            # output_attentions=True & head_mask can not be supported when using SDPA.
+            attention_mask = _prepare_4d_causal_attention_mask_for_sdpa(
+                attention_mask, input_shape, hidden_states, past_key_values_length
+            )
+        else:
+            # 4d mask is passed through the layers
+            attention_mask = _prepare_4d_causal_attention_mask(
+                attention_mask, input_shape, hidden_states, past_key_values_length
+            )
+    return attention_mask
+
+
+def get_whisper_flash_attention_forward():
+    from transformers.models.whisper.modeling_whisper import WhisperAttention
+
+    def forward(
+        self: WhisperAttention,
+        hidden_states: torch.Tensor,
+        key_value_states: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        attention_mask: Optional[dict] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        output_attentions: bool = False,
+    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[Tuple[torch.Tensor]]]:
+        """Input shape: Batch x Time x Channel"""
+        assert layer_head_mask is None, "layer_head_mask is not supported for FlashAttention"
+        # for encoder, attention_mask is None
+        if attention_mask is None:
+            attention_mask = {}
+        # if key_value_states are provided this layer is used as a cross-attention layer
+        # for the decoder
+        is_cross_attention = key_value_states is not None
+
+        bsz, tgt_len, _ = hidden_states.size()
+
+        # get query proj
+        query_states = self.q_proj(hidden_states)
+        # get key, value proj
+        # `past_key_value[0].shape[2] == key_value_states.shape[1]`
+        # is checking that the `sequence_length` of the `past_key_value` is the same as
+        # the provided `key_value_states` to support prefix tuning
+        if (
+            is_cross_attention
+            and past_key_value is not None
+            and past_key_value[0].shape[2] == key_value_states.shape[1]
+        ):
+            # reuse k,v, cross_attentions
+            key_states = past_key_value[0]
+            value_states = past_key_value[1]
+        elif is_cross_attention:
+            # cross_attentions
+            key_states = self._shape(self.k_proj(key_value_states), -1, bsz)
+            value_states = self._shape(self.v_proj(key_value_states), -1, bsz)
+        elif past_key_value is not None:
+            # reuse k, v, self_attention
+            key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
+            value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+            key_states = torch.cat([past_key_value[0], key_states], dim=2)
+            value_states = torch.cat([past_key_value[1], value_states], dim=2)
+        else:
+            # self_attention
+            key_states = self._shape(self.k_proj(hidden_states), -1, bsz)
+            value_states = self._shape(self.v_proj(hidden_states), -1, bsz)
+
+        if self.is_decoder:
+            # if cross_attention save Tuple(torch.Tensor, torch.Tensor) of all cross attention key/value_states.
+            # Further calls to cross_attention layer can then reuse all cross-attention
+            # key/value_states (first "if" case)
+            # if uni-directional self-attention (decoder) save Tuple(torch.Tensor, torch.Tensor) of
+            # all previous decoder key/value_states. Further calls to uni-directional self-attention
+            # can concat previous decoder key/value_states to current projected key/value_states (third "elif" case)
+            # if encoder bi-directional self-attention `past_key_value` is always `None`
+            past_key_value = (key_states, value_states)
+
+        query_states = self._shape(query_states, tgt_len, bsz)
+
+        dropout_p = self.dropout if self.training else 0.0
+        attn_output = ColoAttention.attention(
+            query_states,
+            key_states,
+            value_states,
+            **attention_mask,
+            dropout_p=dropout_p,
+            scale=self.scaling,
+        )
+        attn_output = attn_output.transpose(1, 2)
+
+        # Use the `embed_dim` from the config (stored in the class) rather than `hidden_state` because `attn_output` can be
+        # partitioned across GPUs when using tensor-parallelism.
+        attn_output = attn_output.reshape(bsz, tgt_len, self.embed_dim)
+
+        attn_output = self.out_proj(attn_output)
+
+        return attn_output, None, past_key_value
+
+    return forward
+
+
+def get_whisper_decoder_forward_for_flash_attention(shard_config: ShardConfig):
+    def forward(
+        self: WhisperDecoder,
+        input_ids=None,
+        attention_mask=None,
+        encoder_hidden_states=None,
+        head_mask=None,
+        cross_attn_head_mask=None,
+        past_key_values=None,
+        inputs_embeds=None,
+        use_cache=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+    ):
+        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        output_hidden_states = (
+            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+        )
+        use_cache = use_cache if use_cache is not None else self.config.use_cache
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        # retrieve input_ids and inputs_embeds
+        if input_ids is not None and inputs_embeds is not None:
+            raise ValueError("You cannot specify both decoder_input_ids and decoder_inputs_embeds at the same time")
+        elif input_ids is not None:
+            input_shape = input_ids.size()
+            input_ids = input_ids.view(-1, input_shape[-1])
+        elif inputs_embeds is not None:
+            input_shape = inputs_embeds.size()[:-1]
+        else:
+            raise ValueError("You have to specify either decoder_input_ids or decoder_inputs_embeds")
+
+        # past_key_values_length
+        past_key_values_length = past_key_values[0][0].shape[2] if past_key_values is not None else 0
+
+        if inputs_embeds is None:
+            inputs_embeds = self.embed_tokens(input_ids)
+
+        attention_mask = _get_attention_mask(self, shard_config, inputs_embeds, past_key_values_length, attention_mask)
+
+        # embed positions
+        if input_ids is not None:
+            positions = self.embed_positions(input_ids, past_key_values_length=past_key_values_length)
+        else:
+            positions = self.embed_positions(inputs_embeds, past_key_values_length=past_key_values_length)
+
+        hidden_states = inputs_embeds + positions
+        hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
+
+        if self.gradient_checkpointing and self.training:
+            if use_cache:
+                logger.warning_once(
+                    "`use_cache = True` is incompatible with gradient checkpointing. Setting `use_cache = False`..."
+                )
+                use_cache = False
+        # decoder layers
+        all_hidden_states = () if output_hidden_states else None
+        all_self_attns = () if output_attentions else None
+        all_cross_attentions = () if (output_attentions and encoder_hidden_states is not None) else None
+        next_decoder_cache = () if use_cache else None
+
+        # check if head_mask/cross_attn_head_mask has a correct number of layers specified if desired
+        for attn_mask, mask_name in zip([head_mask, cross_attn_head_mask], ["head_mask", "cross_attn_head_mask"]):
+            if attn_mask is not None:
+                assert attn_mask.size()[0] == (len(self.layers)), (
+                    f"The `{mask_name}` should be specified for {len(self.layers)} layers, but it is for"
+                    f" {head_mask.size()[0]}."
+                )
+        for idx, decoder_layer in enumerate(self.layers):
+            # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
+            if output_hidden_states:
+                all_hidden_states += (hidden_states,)
+            if self.training:
+                dropout_probability = torch.rand([])
+                if dropout_probability < self.layerdrop:
+                    continue
+
+            past_key_value = past_key_values[idx] if past_key_values is not None else None
+
+            if self.gradient_checkpointing and self.training:
+
+                def create_custom_forward(module):
+                    def custom_forward(*inputs):
+                        # None for past_key_value
+                        return module(*inputs, output_attentions, use_cache)
 
+                    return custom_forward
 
-class T5PipelineForwards:
+                layer_outputs = torch.utils.checkpoint.checkpoint(
+                    create_custom_forward(decoder_layer),
+                    hidden_states,
+                    attention_mask,
+                    encoder_hidden_states,
+                    None,  # encoder attention mask
+                    head_mask[idx] if head_mask is not None else None,
+                    (cross_attn_head_mask[idx] if cross_attn_head_mask is not None else None),
+                    None,  # past_key_value
+                )
+            else:
+                layer_outputs = decoder_layer(
+                    hidden_states,
+                    attention_mask=attention_mask,
+                    encoder_hidden_states=encoder_hidden_states,
+                    layer_head_mask=(head_mask[idx] if head_mask is not None else None),
+                    cross_attn_layer_head_mask=(
+                        cross_attn_head_mask[idx] if cross_attn_head_mask is not None else None
+                    ),
+                    past_key_value=past_key_value,
+                    output_attentions=output_attentions,
+                    use_cache=use_cache,
+                )
+            hidden_states = layer_outputs[0]
+
+            if use_cache:
+                next_decoder_cache += (layer_outputs[3 if output_attentions else 1],)
+
+            if output_attentions:
+                all_self_attns += (layer_outputs[1],)
+
+                if encoder_hidden_states is not None:
+                    all_cross_attentions += (layer_outputs[2],)
+
+        hidden_states = self.layer_norm(hidden_states)
+        # add hidden states from the last decoder layer
+        if output_hidden_states:
+            all_hidden_states += (hidden_states,)
+
+        next_cache = next_decoder_cache if use_cache else None
+        if not return_dict:
+            return tuple(
+                v
+                for v in [
+                    hidden_states,
+                    next_cache,
+                    all_hidden_states,
+                    all_self_attns,
+                    all_cross_attentions,
+                ]
+                if v is not None
+            )
+        return BaseModelOutputWithPastAndCrossAttentions(
+            last_hidden_state=hidden_states,
+            past_key_values=next_cache,
+            hidden_states=all_hidden_states,
+            attentions=all_self_attns,
+            cross_attentions=all_cross_attentions,
+        )
+
+    return forward
+
+
+def get_jit_fused_whisper_encoder_layer_forward():
+    from transformers.models.whisper.modeling_whisper import WhisperEncoderLayer
+
+    def forward(
+        self: WhisperEncoderLayer,
+        hidden_states: torch.Tensor,
+        attention_mask: torch.Tensor,
+        layer_head_mask: torch.Tensor,
+        output_attentions: bool = False,
+    ) -> torch.Tensor:
+        """
+        Args:
+            hidden_states (`torch.FloatTensor`): input to the layer of shape `(batch, seq_len, embed_dim)`
+            attention_mask (`torch.FloatTensor`): attention mask of size
+                `(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
+            layer_head_mask (`torch.FloatTensor`): mask for attention heads in a given layer of size
+                `(encoder_attention_heads,)`.
+            output_attentions (`bool`, *optional*):
+                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
+                returned tensors for more detail.
+        """
+        residual = hidden_states
+        hidden_states = self.self_attn_layer_norm(hidden_states)
+        hidden_states, attn_weights, _ = self.self_attn(
+            hidden_states=hidden_states,
+            attention_mask=attention_mask,
+            layer_head_mask=layer_head_mask,
+            output_attentions=output_attentions,
+        )
+        hidden_states = self.dropout_add(hidden_states, residual, self.dropout, self.training)
+
+        residual = hidden_states
+        hidden_states = self.final_layer_norm(hidden_states)
+        hidden_states = self.activation_fn(self.fc1(hidden_states))
+        hidden_states = nn.functional.dropout(hidden_states, p=self.activation_dropout, training=self.training)
+        hidden_states = self.fc2(hidden_states)
+        hidden_states = self.dropout_add(hidden_states, residual, self.dropout, self.training)
+
+        if hidden_states.dtype == torch.float16 and (
+            torch.isinf(hidden_states).any() or torch.isnan(hidden_states).any()
+        ):
+            clamp_value = torch.finfo(hidden_states.dtype).max - 1000
+            hidden_states = torch.clamp(hidden_states, min=-clamp_value, max=clamp_value)
+
+        outputs = (hidden_states,)
+
+        if output_attentions:
+            outputs += (attn_weights,)
+
+        return outputs
+
+    return forward
+
+
+def get_jit_fused_whisper_decoder_layer_forward():
+    from transformers.models.whisper.modeling_whisper import WhisperDecoderLayer
+
+    def forward(
+        self: WhisperDecoderLayer,
+        hidden_states: torch.Tensor,
+        attention_mask: Optional[torch.Tensor] = None,
+        encoder_hidden_states: Optional[torch.Tensor] = None,
+        encoder_attention_mask: Optional[torch.Tensor] = None,
+        layer_head_mask: Optional[torch.Tensor] = None,
+        cross_attn_layer_head_mask: Optional[torch.Tensor] = None,
+        past_key_value: Optional[Tuple[torch.Tensor]] = None,
+        output_attentions: Optional[bool] = False,
+        use_cache: Optional[bool] = True,
+    ) -> torch.Tensor:
+        """
+        Args:
+            hidden_states (`torch.FloatTensor`): input to the layer of shape `(batch, seq_len, embed_dim)`
+            attention_mask (`torch.FloatTensor`): attention mask of size
+                `(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
+            encoder_hidden_states (`torch.FloatTensor`):
+                cross attention input to the layer of shape `(batch, seq_len, embed_dim)`
+            encoder_attention_mask (`torch.FloatTensor`): encoder attention mask of size
+                `(batch, 1, tgt_len, src_len)` where padding elements are indicated by very large negative values.
+            layer_head_mask (`torch.FloatTensor`): mask for attention heads in a given layer of size
+                `(encoder_attention_heads,)`.
+            cross_attn_layer_head_mask (`torch.FloatTensor`): mask for cross-attention heads in a given layer of
+                size `(decoder_attention_heads,)`.
+            past_key_value (`Tuple(torch.FloatTensor)`): cached past key and value projection states
+            output_attentions (`bool`, *optional*):
+                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
+                returned tensors for more detail.
+        """
+        residual = hidden_states
+        hidden_states = self.self_attn_layer_norm(hidden_states)
+
+        # Self Attention
+        # decoder uni-directional self-attention cached key/values tuple is at positions 1,2
+        self_attn_past_key_value = past_key_value[:2] if past_key_value is not None else None
+        # add present self-attn cache to positions 1,2 of present_key_value tuple
+        hidden_states, self_attn_weights, present_key_value = self.self_attn(
+            hidden_states=hidden_states,
+            past_key_value=self_attn_past_key_value,
+            attention_mask=attention_mask,
+            layer_head_mask=layer_head_mask,
+            output_attentions=output_attentions,
+        )
+        hidden_states = self.dropout_add(hidden_states, residual, self.dropout, self.training)
+
+        # Cross-Attention Block
+        cross_attn_present_key_value = None
+        cross_attn_weights = None
+        if encoder_hidden_states is not None:
+            residual = hidden_states
+            hidden_states = self.encoder_attn_layer_norm(hidden_states)
+
+            # cross_attn cached key/values tuple is at positions 3,4 of present_key_value tuple
+            cross_attn_past_key_value = past_key_value[-2:] if past_key_value is not None else None
+            hidden_states, cross_attn_weights, cross_attn_present_key_value = self.encoder_attn(
+                hidden_states=hidden_states,
+                key_value_states=encoder_hidden_states,
+                attention_mask=encoder_attention_mask,
+                layer_head_mask=cross_attn_layer_head_mask,
+                past_key_value=cross_attn_past_key_value,
+                output_attentions=output_attentions,
+            )
+            hidden_states = self.dropout_add(hidden_states, residual, self.dropout, self.training)
+
+            # add cross-attn to positions 3,4 of present_key_value tuple
+            present_key_value = present_key_value + cross_attn_present_key_value
+
+        # Fully Connected
+        residual = hidden_states
+        hidden_states = self.final_layer_norm(hidden_states)
+        hidden_states = self.activation_fn(self.fc1(hidden_states))
+        hidden_states = nn.functional.dropout(hidden_states, p=self.activation_dropout, training=self.training)
+        hidden_states = self.fc2(hidden_states)
+        hidden_states = self.dropout_add(hidden_states, residual, self.dropout, self.training)
+
+        outputs = (hidden_states,)
+
+        if output_attentions:
+            outputs += (self_attn_weights, cross_attn_weights)
+
+        if use_cache:
+            outputs += (present_key_value,)
+
+        return outputs
+
+    return forward
+
+
+class WhisperPipelineForwards:
     """
-    This class serves as a micro library for forward function substitution of
-    T5 models under pipeline setting.
+    This class serves as a micro library for forward function substitution of Llama models
+    under pipeline setting.
     """
 
     @staticmethod
-    def t5_stack_forward(
-        self: T5Stack,
-        input_ids: Optional[torch.LongTensor] = None,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        encoder_hidden_states: Optional[torch.Tensor] = None,
-        encoder_attention_mask: Optional[torch.FloatTensor] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        cross_attn_head_mask: Optional[torch.Tensor] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
-        use_cache: Optional[bool] = False,
-        output_attentions: Optional[bool] = False,
-        output_hidden_states: Optional[bool] = False,
-        return_dict: Optional[bool] = None,
+    def whisper_encoder_forward(
+        self: WhisperEncoder,
+        input_features,
+        attention_mask=None,
+        head_mask=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
+        encoder_states=None,
+        all_attentions=None,
         stage_index: Optional[List[int]] = None,
         decoder_starting_stage: Optional[int] = None,
-    ) -> Union[Dict, Tuple, BaseModelOutputWithPastAndCrossAttentions]:
-        # This function is modified on the basis of transformers.models.t5.modeling_t5.T5Stack.forward.
-        # Please refer to original code of transformers for more details.
+        shard_config: Optional[ShardConfig] = None,
+    ):
+        r"""
+        Args:
+            input_features (`torch.LongTensor` of shape `(batch_size, feature_size, sequence_length)`):
+                Float values of mel features extracted from the raw speech waveform. Raw speech waveform can be
+                obtained by loading a `.flac` or `.wav` audio file into an array of type `List[float]` or a
+                `numpy.ndarray`, *e.g.* via the soundfile library (`pip install soundfile`). To prepare the array into
+                `input_features`, the [`AutoFeatureExtractor`] should be used for extracting the mel features, padding
+                and conversion into a tensor of type `torch.FloatTensor`. See [`~WhisperFeatureExtractor.__call__`]
+            attention_mask (`torch.Tensor`)`, *optional*):
+                Whisper does not support masking of the `input_features`, this argument is preserved for compatibility,
+                but it is not used. By default the silence in the input log mel spectrogram are ignored.
+            head_mask (`torch.Tensor` of shape `(encoder_layers, encoder_attention_heads)`, *optional*):
+                Mask to nullify selected heads of the attention modules. Mask values selected in `[0, 1]`:
+
+                - 1 indicates the head is **not masked**,
+                - 0 indicates the head is **masked**.
+            output_attentions (`bool`, *optional*):
+                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
+                returned tensors for more detail.
+            output_hidden_states (`bool`, *optional*):
+                Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
+                for more detail.
+            return_dict (`bool`, *optional*):
+                Whether or not to return a [`~utils.ModelOutput`] instead of a plain tuple.
+        """
+        logging.get_logger(__name__)
 
-        logger = logging.get_logger(__name__)
+        stage = stage_manager.stage
+        at_first_stage = stage == 0
+        at_last_stage = stage == decoder_starting_stage - 1
 
-        # TODO(baizhou): left the recording kv-value tensors as () or None type, this feature may be added in the future.
-        if past_key_values:
-            logger.warning_once("Non-empty past_key_values is not supported for pipeline models at the moment.")
-            past_key_values = None
-        if output_attentions:
-            logger.warning_once("output_attentions=True is not supported for pipeline models at the moment.")
-            output_attentions = False
-        if output_hidden_states:
-            logger.warning_once("output_hidden_states=True is not supported for pipeline models at the moment.")
-            output_hidden_states = False
-        if use_cache:
-            logger.warning_once("use_cache=True is not supported for pipeline models at the moment.")
-            use_cache = False
-        if use_cache is True:
-            if not in_decoder:
-                raise ValueError(f"`use_cache` can only be set to `True` if {self} is used as a decoder")
-        if self.gradient_checkpointing and self.training:
-            if use_cache:
-                logger.warning_once(
-                    "`use_cache=True` is incompatible with gradient checkpointing. Setting `use_cache=False`..."
+        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        output_hidden_states = (
+            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+        )
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        # Process inputs if at the first stage of encoder.
+        if at_first_stage:
+            inputs_embeds = nn.functional.gelu(self.conv1(input_features))
+            inputs_embeds = nn.functional.gelu(self.conv2(inputs_embeds))
+
+            inputs_embeds = inputs_embeds.permute(0, 2, 1)
+            embed_pos = self.embed_positions.weight
+
+            hidden_states = inputs_embeds + embed_pos
+            hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
+
+            encoder_states = () if output_hidden_states else None
+            all_attentions = () if output_attentions else None
+
+            # check if head_mask has a correct number of layers specified if desired
+            if head_mask is not None:
+                assert head_mask.size()[0] == (
+                    len(self.layers)
+                ), f"The head_mask should be specified for {len(self.layers)} layers, but it is for {head_mask.size()[0]}."
+
+        else:
+            if hidden_states is None:
+                raise ValueError(
+                    "hidden_states shouldn't be None for stages other than the first stage of encoder/decoder."
                 )
-                use_cache = False
 
+        start_idx, end_idx = stage_index[0], stage_index[1]
+
+        for idx in range(start_idx, end_idx):
+            encoder_layer = self.layers[idx]
+
+            if output_hidden_states:
+                encoder_states = encoder_states + (hidden_states,)
+            # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
+            dropout_probability = random.uniform(0, 1)
+            if self.training and (dropout_probability < self.layerdrop):  # skip the layer
+                layer_outputs = (None, None)
+            else:
+                if self.gradient_checkpointing and self.training:
+                    layer_outputs = self._gradient_checkpointing_func(
+                        encoder_layer.__call__,
+                        hidden_states,
+                        None,
+                        (head_mask[idx] if head_mask is not None else None),
+                        output_attentions,
+                    )
+                else:
+                    layer_outputs = encoder_layer(
+                        hidden_states,
+                        None,
+                        layer_head_mask=(head_mask[idx] if head_mask is not None else None),
+                        output_attentions=output_attentions,
+                    )
+
+                hidden_states = layer_outputs[0]
+
+            if output_attentions:
+                all_attentions = all_attentions + (layer_outputs[1],)
+
+        if at_last_stage:
+            hidden_states = self.layer_norm(hidden_states)
+            if output_hidden_states:
+                encoder_states = encoder_states + (hidden_states,)
+
+            if not return_dict:
+                return tuple(v for v in [hidden_states, encoder_states, all_attentions] if v is not None)
+            return BaseModelOutput(
+                last_hidden_state=hidden_states,
+                hidden_states=encoder_states,
+                attentions=all_attentions,
+            )
+
+        else:
+            return {"hidden_states": hidden_states, "head_mask": head_mask}
+
+    @staticmethod
+    def whisper_decoder_forward(
+        self: WhisperDecoder,
+        input_ids=None,
+        attention_mask=None,
+        encoder_hidden_states=None,
+        head_mask=None,
+        cross_attn_head_mask=None,
+        past_key_values=None,
+        inputs_embeds=None,
+        use_cache=None,
+        output_attentions=None,
+        output_hidden_states=None,
+        return_dict=None,
+        stage_manager: Optional[PipelineStageManager] = None,
+        hidden_states: Optional[torch.FloatTensor] = None,
+        stage_index: Optional[List[int]] = None,
+        decoder_starting_stage: Optional[int] = None,
+        shard_config: Optional[ShardConfig] = None,
+    ):
+        r"""
+        Args:
+            input_ids (`torch.LongTensor` of shape `(batch_size, sequence_length)`):
+                Indices of input sequence tokens in the vocabulary. Padding will be ignored by default should you
+                provide it.
+
+                Indices can be obtained using [`WhisperTokenizer`]. See [`PreTrainedTokenizer.encode`] and
+                [`PreTrainedTokenizer.__call__`] for details.
+
+                [What are input IDs?](../glossary#input-ids)
+            attention_mask (`torch.Tensor` of shape `(batch_size, sequence_length)`, *optional*):
+                Mask to avoid performing attention on padding token indices. Mask values selected in `[0, 1]`:
+
+                - 1 for tokens that are **not masked**,
+                - 0 for tokens that are **masked**.
+
+                [What are attention masks?](../glossary#attention-mask)
+            encoder_hidden_states (`torch.FloatTensor` of shape `(batch_size, encoder_sequence_length, hidden_size)`, *optional*):
+                Sequence of hidden-states at the output of the last layer of the encoder. Used in the cross-attention
+                of the decoder.
+            head_mask (`torch.Tensor` of shape `(decoder_layers, decoder_attention_heads)`, *optional*):
+                Mask to nullify selected heads of the attention modules. Mask values selected in `[0, 1]`:
+
+                - 1 indicates the head is **not masked**,
+                - 0 indicates the head is **masked**.
+
+            cross_attn_head_mask (`torch.Tensor` of shape `(decoder_layers, decoder_attention_heads)`, *optional*):
+                Mask to nullify selected heads of the attention modules in encoder to avoid performing cross-attention
+                on hidden heads. Mask values selected in `[0, 1]`:
+
+                - 1 indicates the head is **not masked**,
+                - 0 indicates the head is **masked**.
+
+            past_key_values (`tuple(tuple(torch.FloatTensor))`, *optional*, returned when `use_cache=True` is passed or when `config.use_cache=True`):
+                Tuple of `tuple(torch.FloatTensor)` of length `config.n_layers`, with each tuple having 2 tensors of
+                shape `(batch_size, num_heads, sequence_length, embed_size_per_head)`) and 2 additional tensors of
+                shape `(batch_size, num_heads, encoder_sequence_length, embed_size_per_head)`.
+
+                Contains pre-computed hidden-states (key and values in the self-attention blocks and in the
+                cross-attention blocks) that can be used (see `past_key_values` input) to speed up sequential decoding.
+
+                If `past_key_values` are used, the user can optionally input only the last `decoder_input_ids` (those
+                that don't have their past key value states given to this model) of shape `(batch_size, 1)` instead of
+                all `decoder_input_ids` of shape `(batch_size, sequence_length)`. inputs_embeds (`torch.FloatTensor` of
+                shape `(batch_size, sequence_length, hidden_size)`, *optional*): Optionally, instead of passing
+                `input_ids` you can choose to directly pass an embedded representation. This is useful if you want more
+                control over how to convert `input_ids` indices into associated vectors than the model's internal
+                embedding lookup matrix.
+            output_attentions (`bool`, *optional*):
+                Whether or not to return the attentions tensors of all attention layers. See `attentions` under
+                returned tensors for more detail.
+            output_hidden_states (`bool`, *optional*):
+                Whether or not to return the hidden states of all layers. See `hidden_states` under returned tensors
+                for more detail.
+            return_dict (`bool`, *optional*):
+                Whether or not to return a [`~utils.ModelOutput`] instead of a plain tuple.
+        """
+        logger = logging.get_logger(__name__)
         stage = stage_manager.stage
-        in_decoder = self.is_decoder
-        if in_decoder != (stage >= decoder_starting_stage):
-            raise ValueError("Config in T5Stack is not aligned with pipeline setting.")
-
-        # at_first_stage: current stage is the first stage of encoder/decoder, taking input_ids/input_embeds
-        # at_last_stage: current stage is the last stage of encoder/decoder, making outputs the same form as huggingface
-        at_first_stage = (stage == 0) or (stage == decoder_starting_stage)
-        at_last_stage = (stage == decoder_starting_stage - 1) or (stage == stage_manager.num_stages - 1)
+        at_first_stage = stage == decoder_starting_stage
+        at_last_stage = stage == stage_manager.num_stages - 1
+
+        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        output_hidden_states = (
+            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+        )
+        use_cache = use_cache if use_cache is not None else self.config.use_cache
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+
+        # decoder layers
+        all_hidden_states = () if output_hidden_states else None
+        all_self_attns = () if output_attentions else None
+        all_cross_attentions = () if (output_attentions and encoder_hidden_states is not None) else None
+        next_decoder_cache = () if use_cache else None
+
+        # check if head_mask/cross_attn_head_mask has a correct number of layers specified if desired
+        for attn_mask, mask_name in zip([head_mask, cross_attn_head_mask], ["head_mask", "cross_attn_head_mask"]):
+            if attn_mask is not None:
+                assert attn_mask.size()[0] == (len(self.layers)), (
+                    f"The `{mask_name}` should be specified for {len(self.layers)} layers, but it is for"
+                    f" {head_mask.size()[0]}."
+                )
+
+        # past_key_values_length
+        past_key_values_length = past_key_values[0][0].shape[2] if past_key_values is not None else 0
 
-        # Process inputs if at the first stage of encoder/decoder.
         if at_first_stage:
+            # retrieve input_ids and inputs_embeds
             if input_ids is not None and inputs_embeds is not None:
-                err_msg_prefix = "decoder_" if in_decoder else ""
-                raise ValueError(
-                    f"You cannot specify both {err_msg_prefix}input_ids and {err_msg_prefix}inputs_embeds at the same time"
-                )
+                raise ValueError("You cannot specify both decoder_input_ids and decoder_inputs_embeds at the same time")
             elif input_ids is not None:
                 input_shape = input_ids.size()
                 input_ids = input_ids.view(-1, input_shape[-1])
             elif inputs_embeds is not None:
                 input_shape = inputs_embeds.size()[:-1]
             else:
-                err_msg_prefix = "decoder_" if in_decoder else ""
-                raise ValueError(
-                    f"You have to specify either {err_msg_prefix}input_ids or {err_msg_prefix}inputs_embeds"
-                )
+                raise ValueError("You have to specify either decoder_input_ids or decoder_inputs_embeds")
+
             if inputs_embeds is None:
-                if self.embed_tokens is None:
-                    raise ValueError("You have to initialize the model with valid token embeddings")
                 inputs_embeds = self.embed_tokens(input_ids)
-            batch_size, seq_length = input_shape
-            device = inputs_embeds.device
-            hidden_states = self.dropout(inputs_embeds)
+
+            attention_mask = _get_attention_mask(
+                self, shard_config, inputs_embeds, past_key_values_length, attention_mask
+            )
+
+            # embed positions
+            if input_ids is not None:
+                positions = self.embed_positions(input_ids, past_key_values_length=past_key_values_length)
+            else:
+                positions = self.embed_positions(inputs_embeds, past_key_values_length=past_key_values_length)
+
+            hidden_states = inputs_embeds + positions
+            hidden_states = nn.functional.dropout(hidden_states, p=self.dropout, training=self.training)
+
+            if self.gradient_checkpointing and self.training:
+                if use_cache:
+                    logger.warning_once(
+                        "`use_cache = True` is incompatible with gradient checkpointing. Setting `use_cache = False`..."
+                    )
+                    use_cache = False
+
         else:
             if hidden_states is None:
                 raise ValueError(
                     "hidden_states shouldn't be None for stages other than the first stage of encoder/decoder."
                 )
             input_shape = hidden_states.size()[:-1]
-            batch_size, seq_length = input_shape[0], input_shape[1]
-            device = hidden_states.device
-
-        # required mask seq length can be calculated via length of past
-        mask_seq_length = past_key_values[0][0].shape[2] + seq_length if past_key_values is not None else seq_length
-
-        # initialize past_key_values with `None` if past does not exist
-        if past_key_values is None:
-            past_key_values = [None] * len(self.block)
-
-        if attention_mask is None:
-            attention_mask = torch.ones(batch_size, mask_seq_length, device=device)
-
-        # We can provide a self-attention mask of dimensions [batch_size, from_seq_length, to_seq_length]
-        # ourselves in which case we just need to make it broadcastable to all heads.
-        extended_attention_mask = self.get_extended_attention_mask(attention_mask, input_shape)
-
-        # If a 2D or 3D attention mask is provided for the cross-attention
-        # we need to make broadcastable to [batch_size, num_heads, seq_length, seq_length]
-        if self.is_decoder and encoder_hidden_states is not None:
-            encoder_batch_size, encoder_sequence_length, _ = encoder_hidden_states.size()
-            encoder_hidden_shape = (encoder_batch_size, encoder_sequence_length)
-            if encoder_attention_mask is None:
-                encoder_attention_mask = torch.ones(encoder_hidden_shape, device=inputs_embeds.device, dtype=torch.long)
-            encoder_extended_attention_mask = self.invert_attention_mask(encoder_attention_mask)
-        else:
-            encoder_extended_attention_mask = None
-
-        # Prepare head mask if needed
-        head_mask = self.get_head_mask(head_mask, self.config.num_layers)
-        cross_attn_head_mask = self.get_head_mask(cross_attn_head_mask, self.config.num_layers)
-        present_key_value_states = () if use_cache else None
-        all_hidden_states = () if output_hidden_states else None
-        all_attentions = () if output_attentions else None
-        all_cross_attentions = () if (output_attentions and self.is_decoder) else None
+            attention_mask = _get_attention_mask(
+                self,
+                shard_config,
+                hidden_states,
+                past_key_values_length,
+                attention_mask,
+            )
 
-        # Going through held blocks.
         start_idx, end_idx = stage_index[0], stage_index[1]
 
-        for i in range(start_idx, end_idx):
-            past_key_value = past_key_values[i]
-            layer_module = self.block[i]
-            layer_head_mask = head_mask[i]
-            cross_attn_layer_head_mask = cross_attn_head_mask[i]
-            torch.cuda.set_device(hidden_states.device)
+        for idx in range(start_idx, end_idx):
+            # add LayerDrop (see https://arxiv.org/abs/1909.11556 for description)
+            decoder_layer = self.layers[idx]
+
+            if output_hidden_states:
+                all_hidden_states += (hidden_states,)
+            dropout_probability = random.uniform(0, 1)
+            if self.training and (dropout_probability < self.layerdrop):
+                continue
+
+            past_key_value = past_key_values[idx] if past_key_values is not None else None
 
             if self.gradient_checkpointing and self.training:
                 layer_outputs = self._gradient_checkpointing_func(
-                    layer_module.forward,
+                    decoder_layer.__call__,
                     hidden_states,
-                    extended_attention_mask,
-                    position_bias,
+                    attention_mask,
                     encoder_hidden_states,
-                    encoder_extended_attention_mask,
-                    encoder_decoder_position_bias,
-                    layer_head_mask,
-                    cross_attn_layer_head_mask,
-                    None,  # past_key_value is always None with gradient checkpointing
-                    use_cache,
+                    None,  # encoder attention mask
+                    head_mask[idx] if head_mask is not None else None,
+                    (cross_attn_head_mask[idx] if cross_attn_head_mask is not None else None),
+                    None,  # past_key_value
                     output_attentions,
+                    use_cache,
                 )
             else:
-                layer_outputs = layer_module(
+                layer_outputs = decoder_layer(
                     hidden_states,
-                    attention_mask=extended_attention_mask,
-                    position_bias=position_bias,
+                    attention_mask=attention_mask,
                     encoder_hidden_states=encoder_hidden_states,
-                    encoder_attention_mask=encoder_extended_attention_mask,
-                    encoder_decoder_position_bias=encoder_decoder_position_bias,
-                    layer_head_mask=layer_head_mask,
-                    cross_attn_layer_head_mask=cross_attn_layer_head_mask,
+                    layer_head_mask=(head_mask[idx] if head_mask is not None else None),
+                    cross_attn_layer_head_mask=(
+                        cross_attn_head_mask[idx] if cross_attn_head_mask is not None else None
+                    ),
                     past_key_value=past_key_value,
-                    use_cache=use_cache,
                     output_attentions=output_attentions,
+                    use_cache=use_cache,
                 )
+            hidden_states = layer_outputs[0]
 
-            # layer_outputs is a tuple with:
-            # hidden-states, key-value-states, (self-attention position bias), (self-attention weights), (cross-attention position bias), (cross-attention weights)
-
-            if use_cache is False or use_cache is None:
-                layer_outputs = layer_outputs[:1] + (None,) + layer_outputs[1:]
-            hidden_states, present_key_value_state = layer_outputs[:2]
-
-            # We share the position biases between the layers - the first layer store them
-            # layer_outputs = hidden-states, key-value-states (self-attention position bias), (self-attention weights),
-            # (cross-attention position bias), (cross-attention weights)
-            position_bias = layer_outputs[2]
-
-            if in_decoder and encoder_hidden_states is not None:
-                encoder_decoder_position_bias = layer_outputs[4 if output_attentions else 3]
-            # append next layer key value states
             if use_cache:
-                present_key_value_states = present_key_value_states + (present_key_value_state,)
+                next_decoder_cache += (layer_outputs[3 if output_attentions else 1],)
 
-        # last layer
-        if at_last_stage:
-            hidden_states = self.final_layer_norm(hidden_states)
-            hidden_states = self.dropout(hidden_states)
+            if output_attentions:
+                all_self_attns += (layer_outputs[1],)
 
+                if encoder_hidden_states is not None:
+                    all_cross_attentions += (layer_outputs[2],)
+
+        if at_last_stage:
+            hidden_states = self.layer_norm(hidden_states)
+            # add hidden states from the last decoder layer
+            if output_hidden_states:
+                all_hidden_states += (hidden_states,)
+            next_cache = next_decoder_cache if use_cache else None
             if not return_dict:
                 return tuple(
                     v
                     for v in [
                         hidden_states,
-                        present_key_value_states,
+                        next_cache,
                         all_hidden_states,
-                        all_attentions,
+                        all_self_attns,
                         all_cross_attentions,
                     ]
                     if v is not None
                 )
             return BaseModelOutputWithPastAndCrossAttentions(
                 last_hidden_state=hidden_states,
-                past_key_values=present_key_value_states,
+                past_key_values=next_cache,
                 hidden_states=all_hidden_states,
-                attentions=all_attentions,
+                attentions=all_self_attns,
                 cross_attentions=all_cross_attentions,
             )
+
         else:
             return {
+                "head_mask": head_mask,
+                "cross_attn_head_mask": cross_attn_head_mask,
                 "hidden_states": hidden_states,
-                "position_bias": position_bias,
-                "encoder_decoder_position_bias": encoder_decoder_position_bias,
-                "backward_tensor_keys": ["hidden_states"],
             }
 
     @staticmethod
-    def t5_model_forward(
-        self: T5Model,
-        input_ids: Optional[torch.LongTensor] = None,
-        attention_mask: Optional[torch.FloatTensor] = None,
+    def whisper_model_forward(
+        self: WhisperModel,
+        input_features: Optional[torch.FloatTensor] = None,
+        attention_mask: Optional[torch.LongTensor] = None,
         decoder_input_ids: Optional[torch.LongTensor] = None,
-        decoder_attention_mask: Optional[torch.BoolTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        decoder_head_mask: Optional[torch.FloatTensor] = None,
+        decoder_attention_mask: Optional[torch.LongTensor] = None,
+        head_mask: Optional[torch.Tensor] = None,
+        decoder_head_mask: Optional[torch.Tensor] = None,
         cross_attn_head_mask: Optional[torch.Tensor] = None,
         encoder_outputs: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
         past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
-        inputs_embeds: Optional[torch.Tensor] = None,
-        decoder_inputs_embeds: Optional[torch.Tensor] = None,
+        decoder_inputs_embeds: Optional[Tuple[torch.FloatTensor]] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
         encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
-        backward_tensor_keys: Optional[List[str]] = None,
         stage_index: Optional[List[int]] = None,
         decoder_starting_stage: Optional[int] = None,
-    ) -> Union[Tuple[torch.FloatTensor], Seq2SeqModelOutput]:
-        # This function is modified on the basis of transformers.models.t5.modeling_t5.T5Model.forward.
-        # Please refer to original code of transformers for more details.
-
-        __HEAD_MASK_WARNING_MSG = """
-        The input argument `head_mask` was split into two arguments `head_mask` and `decoder_head_mask`. Currently,
-        `decoder_head_mask` is set to copy `head_mask`, but this feature is deprecated and will be removed in future versions.
-        If you do not want to use any `decoder_head_mask` now, please set `decoder_head_mask = torch.ones(num_layers,
-        num_heads)`.
-        """
-
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-
-        logger = logging.get_logger(__name__)
+        shard_config: Optional[ShardConfig] = None,
+    ):
+        r"""
+        Returns:
 
-        # TODO(baizhou): left the recording kv-value tensors as () or None type, this feature may be added in the future.
+        Example:
+         ```python
+         >>> import torch
+         >>> from transformers import AutoFeatureExtractor, WhisperModel
+         >>> from datasets import load_dataset
+
+         >>> model = WhisperModel.from_pretrained("openai/whisper-base")
+         >>> feature_extractor = AutoFeatureExtractor.from_pretrained("openai/whisper-base")
+         >>> ds = load_dataset("hf-internal-testing/librispeech_asr_dummy", "clean", split="validation")
+         >>> inputs = feature_extractor(ds[0]["audio"]["array"], return_tensors="pt")
+         >>> input_features = inputs.input_features
+         >>> decoder_input_ids = torch.tensor([[1, 1]]) * model.config.decoder_start_token_id
+         >>> last_hidden_state = model(input_features, decoder_input_ids=decoder_input_ids).last_hidden_state
+         >>> list(last_hidden_state.shape)
+         [1, 2, 512]
+         ```"""
+        # TODO: left the recording kv-value tensors as () or None type, this feature may be added in the future.
         if past_key_values:
             logger.warning_once("Non-empty past_key_values is not supported for pipeline models at the moment.")
             past_key_values = None
         if output_attentions:
             logger.warning_once("output_attentions=True is not supported for pipeline models at the moment.")
             output_attentions = False
         if output_hidden_states:
             logger.warning_once("output_hidden_states=True is not supported for pipeline models at the moment.")
             output_hidden_states = False
         if use_cache:
             logger.warning_once("use_cache=True is not supported for pipeline models at the moment.")
             use_cache = False
 
-        # FutureWarning: head_mask was separated into two input args - head_mask, decoder_head_mask
-        if head_mask is not None and decoder_head_mask is None:
-            if self.config.num_layers == self.config.num_decoder_layers:
-                warnings.warn(__HEAD_MASK_WARNING_MSG, FutureWarning)
-                decoder_head_mask = head_mask
+        logging.get_logger(__name__)
 
+        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        output_hidden_states = (
+            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+        )
+        use_cache = use_cache if use_cache is not None else self.config.use_cache
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
         in_decoder = stage_manager.stage >= decoder_starting_stage
-        # Stage is in encoder, directly return the output of t5_stack_forward
         if not in_decoder:
-            encoder_outputs = T5PipelineForwards.t5_stack_forward(
-                self.encoder,
-                input_ids=input_ids,
-                attention_mask=attention_mask,
-                inputs_embeds=inputs_embeds,
-                head_mask=head_mask,
-                output_attentions=output_attentions,
-                output_hidden_states=output_hidden_states,
-                return_dict=return_dict,
-                stage_manager=stage_manager,
-                hidden_states=hidden_states,
-                position_bias=position_bias,
-                encoder_decoder_position_bias=encoder_decoder_position_bias,
-                stage_index=stage_index,
-                decoder_starting_stage=decoder_starting_stage,
-            )
-            if stage_manager.stage == decoder_starting_stage - 1:
-                # last stage of encoder
-                return {"encoder_hidden_states": encoder_outputs[0]}
-            else:
-                return encoder_outputs
+            if encoder_outputs is None:
+                input_features = self._mask_input_features(input_features, attention_mask=attention_mask)
+
+                encoder_outputs = WhisperPipelineForwards.whisper_encoder_forward(
+                    self.encoder,
+                    input_features,
+                    head_mask=head_mask,
+                    output_attentions=output_attentions,
+                    output_hidden_states=output_hidden_states,
+                    return_dict=return_dict,
+                    stage_manager=stage_manager,
+                    hidden_states=hidden_states,
+                    stage_index=stage_index,
+                    decoder_starting_stage=decoder_starting_stage,
+                )
+
+                if stage_manager.stage == decoder_starting_stage - 1:
+                    # last stage of encoder
+                    return {"encoder_hidden_states": encoder_outputs[0]}
+                else:
+                    return encoder_outputs
+            # If the user passed a tuple for encoder_outputs, we wrap it in a BaseModelOutput when return_dict=True
+            elif return_dict and not isinstance(encoder_outputs, BaseModelOutput):
+                encoder_outputs = BaseModelOutput(
+                    last_hidden_state=encoder_outputs[0],
+                    hidden_states=(encoder_outputs[1] if len(encoder_outputs) > 1 else None),
+                    attentions=encoder_outputs[2] if len(encoder_outputs) > 2 else None,
+                )
 
         at_last_decoder_stage = stage_manager.is_last_stage()
         at_first_decoder_stage = stage_manager.stage == decoder_starting_stage
-
         if encoder_outputs is not None:
             encoder_hidden_states = encoder_outputs[0]
         elif encoder_hidden_states is None:
             raise ValueError("Non-empty encoder_hidden_states should be passed in at decoder stages.")
 
         if not at_first_decoder_stage and hidden_states is None:
             raise ValueError("If not at the first layer of decoder, non-empty hidden_states must be provided.")
 
-        # Decode
-        decoder_outputs = T5PipelineForwards.t5_stack_forward(
+        # decoder outputs consists of (dec_features, past_key_value, dec_hidden, dec_attn)
+        decoder_outputs = WhisperPipelineForwards.whisper_decoder_forward(
             self.decoder,
             input_ids=decoder_input_ids,
             attention_mask=decoder_attention_mask,
-            inputs_embeds=decoder_inputs_embeds,
-            past_key_values=past_key_values,
             encoder_hidden_states=encoder_hidden_states,
-            encoder_attention_mask=attention_mask,
             head_mask=decoder_head_mask,
             cross_attn_head_mask=cross_attn_head_mask,
+            past_key_values=past_key_values,
+            inputs_embeds=decoder_inputs_embeds,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             stage_manager=stage_manager,
             hidden_states=hidden_states,
-            position_bias=position_bias,
-            encoder_decoder_position_bias=encoder_decoder_position_bias,
             stage_index=stage_index,
             decoder_starting_stage=decoder_starting_stage,
+            shard_config=shard_config,
         )
 
-        # Directly return outputs of overloaded T5Stack forward if not at last stage.
+        # Directly return outputs of overloaded Whisper forward if not at last stage.
         if not at_last_decoder_stage:
             # encoder_hidden_states should be passed to the next stage
             decoder_outputs["encoder_hidden_states"] = encoder_hidden_states
             return decoder_outputs
 
         if not return_dict:
-            return decoder_outputs + encoder_hidden_states
-        else:
-            return Seq2SeqModelOutput(
-                last_hidden_state=decoder_outputs.last_hidden_state,
-                past_key_values=decoder_outputs.past_key_values,
-                decoder_hidden_states=decoder_outputs.hidden_states,
-                decoder_attentions=decoder_outputs.attentions,
-                cross_attentions=decoder_outputs.cross_attentions,
-                encoder_last_hidden_state=encoder_hidden_states,
-            )
+            return decoder_outputs + encoder_outputs
+
+        return Seq2SeqModelOutput(
+            last_hidden_state=decoder_outputs.last_hidden_state,
+            past_key_values=decoder_outputs.past_key_values,
+            decoder_hidden_states=decoder_outputs.hidden_states,
+            decoder_attentions=decoder_outputs.attentions,
+            cross_attentions=decoder_outputs.cross_attentions,
+            encoder_last_hidden_state=encoder_hidden_states,
+        )
 
     @staticmethod
-    def t5_for_conditional_generation_forward(
-        self: T5ForConditionalGeneration,
-        input_ids: Optional[torch.LongTensor] = None,
-        attention_mask: Optional[torch.FloatTensor] = None,
+    def whisper_for_conditional_generation_forward(
+        self: WhisperForConditionalGeneration,
+        input_features: Optional[torch.FloatTensor] = None,
+        attention_mask: Optional[torch.LongTensor] = None,
         decoder_input_ids: Optional[torch.LongTensor] = None,
-        decoder_attention_mask: Optional[torch.BoolTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        decoder_head_mask: Optional[torch.FloatTensor] = None,
+        decoder_attention_mask: Optional[torch.LongTensor] = None,
+        head_mask: Optional[torch.Tensor] = None,
+        decoder_head_mask: Optional[torch.Tensor] = None,
         cross_attn_head_mask: Optional[torch.Tensor] = None,
-        encoder_outputs: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-        past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
-        decoder_inputs_embeds: Optional[torch.FloatTensor] = None,
+        encoder_outputs: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        decoder_inputs_embeds: Optional[Tuple[torch.FloatTensor]] = None,
         labels: Optional[torch.LongTensor] = None,
         use_cache: Optional[bool] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
         encoder_hidden_states: Optional[torch.FloatTensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
-        backward_tensor_keys: Optional[List[str]] = None,
         stage_index: Optional[List[int]] = None,
         decoder_starting_stage: Optional[int] = None,
-    ) -> Union[Tuple[torch.FloatTensor], Seq2SeqLMOutput]:
-        # This function is modified on the basis of transformers.models.t5.modeling_t5.T5ForConditionalGeneration.forward.
-        # Please refer to original code of transformers for more details.
-
-        __HEAD_MASK_WARNING_MSG = """
-        The input argument `head_mask` was split into two arguments `head_mask` and `decoder_head_mask`. Currently,
-        `decoder_head_mask` is set to copy `head_mask`, but this feature is deprecated and will be removed in future versions.
-        If you do not want to use any `decoder_head_mask` now, please set `decoder_head_mask = torch.ones(num_layers,
-        num_heads)`.
-        """
+        shard_config: Optional[ShardConfig] = None,
+    ) -> Union[Tuple[torch.Tensor], Seq2SeqLMOutput]:
+        r"""
+        labels (`torch.LongTensor` of shape `(batch_size, sequence_length)`, *optional*):
+            Labels for computing the language modeling loss. Indices should either be in `[0, ..., config.vocab_size]`
+            or -100 (see `input_ids` docstring). Tokens with indices set to `-100` are ignored (masked), the loss is
+            only computed for the tokens with labels in `[0, ..., config.vocab_size]`.
 
-        use_cache = use_cache if use_cache is not None else self.config.use_cache
-        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
+        Returns:
 
-        logger = logging.get_logger(__name__)
+        Example:
 
-        # TODO(baizhou): left the recording kv-value tensors as () or None type, this feature may be added in the future.
-        if past_key_values:
-            logger.warning_once("Non-empty past_key_values is not supported for pipeline models at the moment.")
-            past_key_values = None
-        if output_attentions:
-            logger.warning_once("output_attentions=True is not supported for pipeline models at the moment.")
-            output_attentions = False
-        if output_hidden_states:
-            logger.warning_once("output_hidden_states=True is not supported for pipeline models at the moment.")
-            output_hidden_states = False
-        if use_cache:
-            logger.warning_once("use_cache=True is not supported for pipeline models at the moment.")
-            use_cache = False
+        ```python
+        >>> import torch
+        >>> from transformers import AutoProcessor, WhisperForConditionalGeneration
+        >>> from datasets import load_dataset
 
-        # FutureWarning: head_mask was separated into two input args - head_mask, decoder_head_mask
-        if head_mask is not None and decoder_head_mask is None:
-            if self.config.num_layers == self.config.num_decoder_layers:
-                warnings.warn(__HEAD_MASK_WARNING_MSG, FutureWarning)
-                decoder_head_mask = head_mask
+        >>> processor = AutoProcessor.from_pretrained("openai/whisper-tiny.en")
+        >>> model = WhisperForConditionalGeneration.from_pretrained("openai/whisper-tiny.en")
 
-        in_decoder = stage_manager.stage >= decoder_starting_stage
+        >>> ds = load_dataset("hf-internal-testing/librispeech_asr_dummy", "clean", split="validation")
 
-        # Stage is in encoder, directly return the output of t5_stack_forward
-        if not in_decoder:
-            encoder_outputs = T5PipelineForwards.t5_stack_forward(
-                self.encoder,
-                input_ids=input_ids,
-                attention_mask=attention_mask,
-                inputs_embeds=inputs_embeds,
-                head_mask=head_mask,
-                output_attentions=output_attentions,
-                output_hidden_states=output_hidden_states,
-                return_dict=return_dict,
-                stage_manager=stage_manager,
-                hidden_states=hidden_states,
-                position_bias=position_bias,
-                encoder_decoder_position_bias=encoder_decoder_position_bias,
-                stage_index=stage_index,
-                decoder_starting_stage=decoder_starting_stage,
-            )
-            if stage_manager.stage == decoder_starting_stage - 1:
-                # last stage of encoder
-                return {"encoder_hidden_states": encoder_outputs[0]}
-            else:
-                return encoder_outputs
+        >>> inputs = processor(ds[0]["audio"]["array"], return_tensors="pt")
+        >>> input_features = inputs.input_features
 
-        at_last_decoder_stage = stage_manager.is_last_stage()
-        at_first_decoder_stage = stage_manager.stage == decoder_starting_stage
-
-        if encoder_outputs is not None:
-            encoder_hidden_states = encoder_outputs[0]
-        elif encoder_hidden_states is None:
-            raise ValueError("Non-empty encoder_hidden_states should be passed in at decoder stages.")
-
-        if not at_first_decoder_stage and hidden_states is None:
-            raise ValueError("If not at the first layer of decoder, non-empty hidden_states must be provided.")
+        >>> generated_ids = model.generate(inputs=input_features)
 
-        if labels is not None and decoder_input_ids is None and decoder_inputs_embeds is None:
-            # get decoder inputs from shifting lm labels to the right
-            decoder_input_ids = self._shift_right(labels)
+        >>> transcription = processor.batch_decode(generated_ids, skip_special_tokens=True)[0]
+        >>> transcription
+        ' Mr. Quilter is the apostle of the middle classes, and we are glad to welcome his gospel.'
+        ```"""
+        return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        # Decode
-        decoder_outputs = T5PipelineForwards.t5_stack_forward(
-            self.decoder,
-            input_ids=decoder_input_ids,
-            attention_mask=decoder_attention_mask,
-            inputs_embeds=decoder_inputs_embeds,
-            past_key_values=past_key_values,
-            encoder_hidden_states=encoder_hidden_states,
-            encoder_attention_mask=attention_mask,
-            head_mask=decoder_head_mask,
+        if labels is not None:
+            if decoder_input_ids is None and decoder_inputs_embeds is None:
+                decoder_input_ids = shift_tokens_right(
+                    labels, self.config.pad_token_id, self.config.decoder_start_token_id
+                )
+        in_decoder = stage_manager.stage >= decoder_starting_stage
+        at_last_decoder_stage = stage_manager.is_last_stage()
+        outputs = WhisperPipelineForwards.whisper_model_forward(
+            self.model,
+            input_features,
+            attention_mask=attention_mask,
+            decoder_input_ids=decoder_input_ids,
+            encoder_outputs=encoder_outputs,
+            decoder_attention_mask=decoder_attention_mask,
+            head_mask=head_mask,
+            decoder_head_mask=decoder_head_mask,
             cross_attn_head_mask=cross_attn_head_mask,
+            past_key_values=past_key_values,
+            decoder_inputs_embeds=decoder_inputs_embeds,
             use_cache=use_cache,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             stage_manager=stage_manager,
             hidden_states=hidden_states,
-            position_bias=position_bias,
-            encoder_decoder_position_bias=encoder_decoder_position_bias,
+            encoder_hidden_states=encoder_hidden_states,
             stage_index=stage_index,
             decoder_starting_stage=decoder_starting_stage,
+            shard_config=shard_config,
         )
+        if not in_decoder:
+            return outputs
 
-        # Directly return outputs of overloaded T5Stack forward if not at last stage.
         if not at_last_decoder_stage:
             # encoder_hidden_states should be passed to the next stage
-            decoder_outputs["encoder_hidden_states"] = encoder_hidden_states
-            return decoder_outputs
-
-        sequence_output = decoder_outputs[0]
-
-        if self.config.tie_word_embeddings:
-            # Rescale output before projecting on vocab
-            # See https://github.com/tensorflow/mesh/blob/fa19d69eafc9a482aff0b59ddd96b025c0cb207d/mesh_tensorflow/transformer/transformer.py#L586
-            sequence_output = sequence_output * (self.model_dim**-0.5)
+            outputs["encoder_hidden_states"] = encoder_hidden_states
+            return outputs
 
-        lm_logits = self.lm_head(sequence_output)
+        lm_logits = self.proj_out(outputs[0])
 
         loss = None
         if labels is not None:
-            loss_fct = CrossEntropyLoss(ignore_index=-100)
+            loss_fct = CrossEntropyLoss()
             # move labels to correct device to enable PP
             labels = labels.to(lm_logits.device)
-            loss = loss_fct(lm_logits.view(-1, lm_logits.size(-1)), labels.view(-1))
+            loss = loss_fct(lm_logits.view(-1, self.config.vocab_size), labels.reshape(-1))
 
         if not return_dict:
-            output = (lm_logits,) + decoder_outputs[1:] + encoder_hidden_states
+            output = (lm_logits,) + outputs[1:]
             return ((loss,) + output) if loss is not None else output
 
         return Seq2SeqLMOutput(
             loss=loss,
             logits=lm_logits,
-            past_key_values=decoder_outputs.past_key_values,
-            decoder_hidden_states=decoder_outputs.hidden_states,
-            decoder_attentions=decoder_outputs.attentions,
-            cross_attentions=decoder_outputs.cross_attentions,
-            encoder_last_hidden_state=encoder_hidden_states,
+            past_key_values=outputs.past_key_values,
+            decoder_hidden_states=outputs.decoder_hidden_states,
+            decoder_attentions=outputs.decoder_attentions,
+            cross_attentions=outputs.cross_attentions,
+            encoder_last_hidden_state=outputs.encoder_last_hidden_state,
+            encoder_hidden_states=outputs.encoder_hidden_states,
+            encoder_attentions=outputs.encoder_attentions,
         )
 
     @staticmethod
-    def t5_encoder_model_forward(
-        self: T5EncoderModel,
-        input_ids: Optional[torch.LongTensor] = None,
-        attention_mask: Optional[torch.FloatTensor] = None,
-        head_mask: Optional[torch.FloatTensor] = None,
-        inputs_embeds: Optional[torch.FloatTensor] = None,
+    def whisper_for_audio_classification_forward(
+        self: WhisperForAudioClassification,
+        input_features: Optional[torch.LongTensor] = None,
+        head_mask: Optional[torch.Tensor] = None,
+        encoder_outputs: Optional[Tuple[Tuple[torch.FloatTensor]]] = None,
+        labels: Optional[torch.LongTensor] = None,
         output_attentions: Optional[bool] = None,
         output_hidden_states: Optional[bool] = None,
         return_dict: Optional[bool] = None,
         stage_manager: Optional[PipelineStageManager] = None,
         hidden_states: Optional[torch.FloatTensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        encoder_decoder_position_bias: Optional[torch.Tensor] = None,
-        backward_tensor_keys: Optional[List[str]] = None,
+        encoder_states=None,
+        all_attentions=None,
         stage_index: Optional[List[int]] = None,
         decoder_starting_stage: Optional[int] = None,
-    ) -> Union[Tuple[torch.FloatTensor], BaseModelOutput]:
+        shard_config: Optional[ShardConfig] = None,
+    ):
         r"""
-        This function is modified on the basis of transformers.models.t5.modeling_gpt2.T5EncoderModel.forward.
+        This function is modified on the basis of transformers.models.whisper.modeling_whisper.WhisperForAudioClassification.forward.
         Please refer to original code of transformers for more details.
-        ```"""
+        """
+        output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
+        output_hidden_states = (
+            output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
+        )
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
-        outputs = T5PipelineForwards.t5_stack_forward(
+        # audio_classification only holds encoder
+        encoder_outputs = WhisperPipelineForwards.whisper_encoder_forward(
             self.encoder,
-            input_ids=input_ids,
-            attention_mask=attention_mask,
-            inputs_embeds=inputs_embeds,
+            input_features,
             head_mask=head_mask,
             output_attentions=output_attentions,
             output_hidden_states=output_hidden_states,
             return_dict=return_dict,
             stage_manager=stage_manager,
             hidden_states=hidden_states,
-            position_bias=position_bias,
-            encoder_decoder_position_bias=encoder_decoder_position_bias,
             stage_index=stage_index,
             decoder_starting_stage=decoder_starting_stage,
         )
 
-        return outputs
-
-
-def get_t5_flash_attention_forward():
-    from transformers.models.t5.modeling_t5 import T5Attention
-
-    def forward(
-        self: T5Attention,
-        hidden_states: torch.Tensor,
-        mask: Optional[torch.Tensor] = None,
-        key_value_states: Optional[torch.Tensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        past_key_value: Optional[Tuple[torch.Tensor]] = None,
-        layer_head_mask: Optional[torch.Tensor] = None,
-        query_length: Optional[int] = None,
-        use_cache: bool = False,
-        output_attentions: bool = False,
-    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]:
-        """
-        Self-attention (if key_value_states is None) or attention over source sentence (provided by key_value_states).
-        """
-        # Input is (batch_size, seq_length, dim)
-        # Mask is (batch_size, key_length) (non-causal) or (batch_size, key_length, key_length)
-        # past_key_value[0] is (batch_size, n_heads, q_len - 1, dim_per_head)
-        batch_size, seq_length = hidden_states.shape[:2]
-
-        real_seq_length = seq_length
-
-        if past_key_value is not None:
-            if len(past_key_value) != 2:
-                raise ValueError(
-                    f"past_key_value should have 2 past states: keys and values. Got { len(past_key_value)} past states"
-                )
-            real_seq_length += past_key_value[0].shape[2] if query_length is None else query_length
-
-        key_length = real_seq_length if key_value_states is None else key_value_states.shape[1]
-
-        def shape(states):
-            """projection"""
-            return states.view(batch_size, -1, self.n_heads, self.key_value_proj_dim).transpose(1, 2)
-
-        def unshape(states):
-            """reshape"""
-            return states.transpose(1, 2).contiguous().view(batch_size, -1, self.inner_dim)
-
-        def project(hidden_states, proj_layer, key_value_states, past_key_value):
-            """projects hidden states correctly to key/query states"""
-            if key_value_states is None:
-                # self-attn
-                # (batch_size, n_heads, seq_length, dim_per_head)
-                hidden_states = shape(proj_layer(hidden_states))
-            elif past_key_value is None:
-                # cross-attn
-                # (batch_size, n_heads, seq_length, dim_per_head)
-                hidden_states = shape(proj_layer(key_value_states))
-
-            if past_key_value is not None:
-                if key_value_states is None:
-                    # self-attn
-                    # (batch_size, n_heads, key_length, dim_per_head)
-                    hidden_states = torch.cat([past_key_value, hidden_states], dim=2)
-                elif past_key_value.shape[2] != key_value_states.shape[1]:
-                    # checking that the `sequence_length` of the `past_key_value` is the same as
-                    # the provided `key_value_states` to support prefix tuning
-                    # cross-attn
-                    # (batch_size, n_heads, seq_length, dim_per_head)
-                    hidden_states = shape(proj_layer(key_value_states))
-                else:
-                    # cross-attn
-                    hidden_states = past_key_value
-            return hidden_states
-
-        # get query states
-        query_states = shape(self.q(hidden_states))  # (batch_size, n_heads, seq_length, dim_per_head)
-
-        # get key/value states
-        key_states = project(
-            hidden_states, self.k, key_value_states, past_key_value[0] if past_key_value is not None else None
-        )
-        value_states = project(
-            hidden_states, self.v, key_value_states, past_key_value[1] if past_key_value is not None else None
-        )
-
-        if position_bias is None:
-            if not self.has_relative_attention_bias:
-                position_bias = torch.zeros(
-                    (1, self.n_heads, real_seq_length, key_length), device=query_states.device, dtype=query_states.dtype
-                )
-                if self.gradient_checkpointing and self.training:
-                    position_bias.requires_grad = True
-            else:
-                position_bias = self.compute_bias(real_seq_length, key_length, device=query_states.device)
+        if not stage_manager.is_last_stage():
+            return encoder_outputs
 
-            # if key and values are already calculated
-            # we want only the last query position bias
-            if past_key_value is not None:
-                position_bias = position_bias[:, :, -hidden_states.size(1) :, :]
-
-            if mask is not None:
-                position_bias = position_bias + mask  # (batch_size, n_heads, seq_length, key_length)
-
-        if self.pruned_heads:
-            mask = torch.ones(position_bias.shape[1])
-            mask[list(self.pruned_heads)] = 0
-            position_bias_masked = position_bias[:, mask.bool()]
+        if self.config.use_weighted_layer_sum:
+            hidden_states = torch.stack(encoder_outputs, dim=1)
+            norm_weights = nn.functional.softmax(self.layer_weights, dim=-1)
+            hidden_states = (hidden_states * norm_weights.view(-1, 1, 1)).sum(dim=1)
         else:
-            position_bias_masked = position_bias
-
-        with torch.backends.cuda.sdp_kernel(enable_flash=True, enable_mem_efficient=True):
-            attn_output = torch.nn.functional.scaled_dot_product_attention(
-                query_states,
-                key_states,
-                value_states,
-                attn_mask=position_bias_masked,
-                dropout_p=self.dropout,
-                scale=1.0,
-            )
-        attn_output = unshape(attn_output)
-        attn_output = self.o(attn_output)
-
-        present_key_value_state = (key_states, value_states) if (self.is_decoder and use_cache) else None
-
-        outputs = (attn_output,) + (present_key_value_state,) + (position_bias,)
-
-        return outputs
-
-    return forward
-
-
-def get_jit_fused_T5_layer_ff_forward():
-    from transformers.models.t5.modeling_t5 import T5LayerFF
-
-    def forward(self: T5LayerFF, hidden_states: torch.Tensor) -> torch.Tensor:
-        forwarded_states = self.layer_norm(hidden_states)
-        forwarded_states = self.DenseReluDense(forwarded_states)
-        hidden_states = self.dropout_add(forwarded_states, hidden_states, self.dropout.p, self.dropout.training)
-        return hidden_states
-
-    return forward
+            hidden_states = encoder_outputs[0]
 
+        hidden_states = self.projector(hidden_states)
+        pooled_output = hidden_states.mean(dim=1)
 
-def get_T5_layer_self_attention_forward():
-    from transformers.models.t5.modeling_t5 import T5LayerSelfAttention
+        logits = self.classifier(pooled_output)
 
-    def forward(
-        self: T5LayerSelfAttention,
-        hidden_states: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        layer_head_mask: Optional[torch.Tensor] = None,
-        past_key_value: Optional[Tuple[torch.Tensor]] = None,
-        use_cache: bool = False,
-        output_attentions: bool = False,
-    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]:
-        normed_hidden_states = self.layer_norm(hidden_states)
-        attention_output = self.SelfAttention(
-            normed_hidden_states,
-            mask=attention_mask,
-            position_bias=position_bias,
-            layer_head_mask=layer_head_mask,
-            past_key_value=past_key_value,
-            use_cache=use_cache,
-            output_attentions=output_attentions,
-        )
-        hidden_states = self.dropout_add(attention_output[0], hidden_states, self.dropout.p, self.dropout.training)
-        outputs = (hidden_states,) + attention_output[1:]  # add attentions if we output them
-        return outputs
-
-    return forward
+        loss = None
 
+        if labels is not None:
+            loss_fct = CrossEntropyLoss()
+            # move labels to correct device to enable PP
+            labels = labels.to(logits.device)
+            loss = loss_fct(logits.view(-1, self.config.num_labels), labels.view(-1))
 
-def get_T5_layer_cross_attention_forward():
-    from transformers.models.t5.modeling_t5 import T5LayerCrossAttention
+        if not return_dict:
+            output = (logits,) + encoder_outputs[1:]
+            return ((loss,) + output) if loss is not None else output
 
-    def forward(
-        self: T5LayerCrossAttention,
-        hidden_states: torch.Tensor,
-        key_value_states: torch.Tensor,
-        attention_mask: Optional[torch.Tensor] = None,
-        position_bias: Optional[torch.Tensor] = None,
-        layer_head_mask: Optional[torch.Tensor] = None,
-        past_key_value: Optional[Tuple[torch.Tensor]] = None,
-        use_cache: bool = False,
-        query_length: Optional[int] = None,
-        output_attentions: bool = False,
-    ) -> Tuple[torch.Tensor, Optional[torch.Tensor], Optional[torch.Tensor]]:
-        normed_hidden_states = self.layer_norm(hidden_states)
-        attention_output = self.EncDecAttention(
-            normed_hidden_states,
-            mask=attention_mask,
-            key_value_states=key_value_states,
-            position_bias=position_bias,
-            layer_head_mask=layer_head_mask,
-            past_key_value=past_key_value,
-            use_cache=use_cache,
-            query_length=query_length,
-            output_attentions=output_attentions,
+        return SequenceClassifierOutput(
+            loss=loss,
+            logits=logits,
+            hidden_states=encoder_outputs.hidden_states,
+            attentions=encoder_outputs.attentions,
         )
-        layer_output = self.dropout_add(attention_output[0], hidden_states, self.dropout.p, self.dropout.training)
-        outputs = (layer_output,) + attention_output[1:]  # add attentions if we output them
-        return outputs
-
-    return forward
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/modeling/vit.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/modeling/vit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/auto_policy.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/auto_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,24 +178,14 @@
     ),
     "transformers.models.mistral.modeling_mistral.MistralForCausalLM": PolicyLocation(
         file_name="mistral", class_name="MistralForCausalLMPolicy"
     ),
     "transformers.models.mistral.modeling_mistral.MistralForSequenceClassification": PolicyLocation(
         file_name="mistral", class_name="MistralForSequenceClassificationPolicy"
     ),
-    # Qwen2
-    "transformers.models.qwen2.modeling_qwen2.Qwen2Model": PolicyLocation(
-        file_name="qwen2", class_name="Qwen2ModelPolicy"
-    ),
-    "transformers.models.qwen2.modeling_qwen2.Qwen2ForCausalLM": PolicyLocation(
-        file_name="qwen2", class_name="Qwen2ForCausalLMPolicy"
-    ),
-    "transformers.models.qwen2.modeling_qwen2.Qwen2ForSequenceClassification": PolicyLocation(
-        file_name="qwen2", class_name="Qwen2ForSequenceClassificationPolicy"
-    ),
 }
 
 
 def import_policy(policy_location: PolicyLocation) -> Policy:
     """
     Dynamically import a Policy class based on the policy location.
     """
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/base_policy.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/base_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/bert.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/blip2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/blip2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/bloom.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/chatglm2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/falcon.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/falcon.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/gpt2.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/gptj.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/gptj.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/llama.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/llama.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,17 @@
                 target_key=LlamaModel,
             )
 
         if self.shard_config.enable_tensor_parallelism:
             assert (
                 self.model.config.num_attention_heads % self.shard_config.tensor_parallel_size == 0
             ), f"The number of attention heads must be divisible by tensor parallel size."
-            if hasattr(self.model.config, "num_key_value_heads"):
-                assert (
-                    self.model.config.num_key_value_heads >= self.shard_config.tensor_parallel_size
-                    and self.model.config.num_key_value_heads % self.shard_config.tensor_parallel_size == 0
-                ), f"The number of key_value heads must be divisible by, and must not be less than tensor parallel size."
+            assert (
+                self.model.config.num_key_value_heads % self.shard_config.tensor_parallel_size == 0
+            ), f"The number of key_value heads must be divisible by tensor parallel size."
             decoder_attribute_replacement = {
                 "self_attn.hidden_size": self.model.config.hidden_size // self.shard_config.tensor_parallel_size,
                 "self_attn.num_heads": self.model.config.num_attention_heads // self.shard_config.tensor_parallel_size,
             }
             if getattr(self.model.config, "num_key_value_heads", False):
                 decoder_attribute_replacement["self_attn.num_key_value_heads"] = (
                     self.model.config.num_key_value_heads // self.shard_config.tensor_parallel_size
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/mistral.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/mistral.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     PaddingLMHead,
     VocabParallelEmbedding1D,
     VocabParallelLMHead1D,
 )
 
 from ..modeling.mistral import (
     MistralForwards,
-    get_lm_forward_with_dist_cross_entropy,
     get_mistral_flash_attention_forward,
     get_mistral_model_forward_for_flash_attn,
 )
 from .base_policy import ModulePolicyDescription, Policy, SubModuleReplacementDescription
 
 __all__ = ["MistralPolicy", "MistralModelPolicy", "MistralForCausalLMPolicy", "MistralForSequenceClassificationPolicy"]
 
@@ -272,26 +271,22 @@
             # add a new item for casual lm
             new_item = {
                 MistralForCausalLM: ModulePolicyDescription(
                     sub_module_replacement=[
                         SubModuleReplacementDescription(
                             suffix="lm_head",
                             target_module=VocabParallelLMHead1D,
-                            kwargs={
-                                "gather_output": not self.shard_config.parallel_output,
-                                "make_vocab_size_divisible_by": self.shard_config.make_vocab_size_divisible_by,
-                            },
+                            kwargs=dict(
+                                gather_output=True,
+                                make_vocab_size_divisible_by=self.shard_config.make_vocab_size_divisible_by,
+                            ),
                         )
                     ]
                 )
             }
-            if self.shard_config.parallel_output:
-                new_item[MistralForCausalLM].method_replacement = {
-                    "forward": get_lm_forward_with_dist_cross_entropy(self.shard_config)
-                }
         else:
             new_item = {
                 MistralForCausalLM: ModulePolicyDescription(
                     sub_module_replacement=[
                         SubModuleReplacementDescription(
                             suffix="lm_head",
                             target_module=PaddingLMHead,
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/opt.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 )
 
 from .._utils import getattr_
 from ..modeling.jit import get_jit_fused_dropout_add_func
 from ..modeling.opt import (
     OPTPipelineForwards,
     get_jit_fused_opt_decoder_layer_forward,
-    get_lm_forward_with_dist_cross_entropy,
     get_opt_decoder_forward_for_flash_attention,
     get_opt_flash_attention_forward,
 )
 from .base_policy import ModulePolicyDescription, Policy, SubModuleReplacementDescription
 
 __all__ = [
     "OPTPolicy",
@@ -266,26 +265,20 @@
         policy = super().module_policy()
         if self.shard_config.enable_tensor_parallelism:
             self.append_or_create_submodule_replacement(
                 description=SubModuleReplacementDescription(
                     suffix="lm_head",
                     target_module=VocabParallelLMHead1D,
                     kwargs=dict(
-                        gather_output=not self.shard_config.parallel_output,
-                        make_vocab_size_divisible_by=self.shard_config.make_vocab_size_divisible_by,
+                        gather_output=True, make_vocab_size_divisible_by=self.shard_config.make_vocab_size_divisible_by
                     ),
                 ),
                 policy=policy,
                 target_key=OPTForCausalLM,
             )
-            if self.shard_config.parallel_output:
-                method_replacement = {"forward": get_lm_forward_with_dist_cross_entropy(self.shard_config)}
-                self.append_or_create_method_replacement(
-                    description=method_replacement, policy=policy, target_key=OPTForCausalLM
-                )
         else:
             self.append_or_create_submodule_replacement(
                 description=SubModuleReplacementDescription(
                     suffix="lm_head",
                     target_module=PaddingLMHead,
                     kwargs=dict(make_vocab_size_divisible_by=self.shard_config.make_vocab_size_divisible_by),
                 ),
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/sam.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/sam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/t5.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/vit.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/vit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/policies/whisper.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/policies/whisper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/shard/grad_ckpt_config.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/shard/grad_ckpt_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/shard/shard_config.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/shard/shard_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/shard/sharder.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/shard/sharder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/shard/shardformer.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/shard/shardformer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/shardformer/shard/utils.py` & `colossalai-nightly-2024.5.4/colossalai/shardformer/shard/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/api.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/api.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/moe_tensor/api.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/moe_tensor/api.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/moe_tensor/moe_info.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/moe_tensor/moe_info.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/padded_tensor/api.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/padded_tensor/api.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/shape_consistency.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/tensor/utils.py` & `colossalai-nightly-2024.5.4/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/testing/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/testing/comparison.py` & `colossalai-nightly-2024.5.4/colossalai/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2024.5.4/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/testing/random.py` & `colossalai-nightly-2024.5.4/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/testing/utils.py` & `colossalai-nightly-2024.5.4/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/__init__.py` & `colossalai-nightly-2024.5.4/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/common.py` & `colossalai-nightly-2024.5.4/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/memory.py` & `colossalai-nightly-2024.5.4/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/model/utils.py` & `colossalai-nightly-2024.5.4/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2024.5.4/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2024.5.4/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2024.5.4/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/utils/timer.py` & `colossalai-nightly-2024.5.4/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,27 @@
     A manager class to manipulate the tensors in chunks.
 
     Args:
         chunk_configuration (Dict[int, Dict]): the configuration dictionary of this chunk manager.
         init_device (torch.device): optional, the device on which the chunk is initialized. The default is None.
     """
 
-    def __init__(
-        self,
-        chunk_configuration,
-        init_device: Optional[torch.device] = None,
-        reuse_fp16_chunk: bool = True,
-    ) -> None:
+    def __init__(self, chunk_configuration, init_device: Optional[torch.device] = None) -> None:
         self.device = init_device or get_accelerator().get_current_device()
         self.dp_degree_chunk_size_dict: Dict[int, int] = dict()
         self.kwargs_config = chunk_configuration
         for k, v in self.kwargs_config.items():
             self.dp_degree_chunk_size_dict[k] = v.pop("chunk_size")
             v["init_device"] = self.device
 
         self.chunk_groups: Dict[str, Deque[Chunk]] = dict()
         self.tensor_chunk_map: Dict[torch.Tensor, Chunk] = dict()
         self.accessed_chunks: Set[Chunk] = set()
         self.accessed_mem: int = 0
         self.total_mem: Dict[str, int] = {"cpu": 0, "cuda": 0}
-        self.reuse_fp16_chunk = reuse_fp16_chunk
-        # Whether model is accumulating gradients,
-        self.accumulating_grads = False
-        self.overflow_counter = 0
 
     def register_tensor(
         self,
         tensor: torch.Tensor,
         group_type: str,
         config_key: int,
         zero_group: ProcessGroup,
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/chunk/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     return a / b
 
 
 def init_chunk_manager(
     model: nn.Module,
     init_device: Optional[torch.device] = None,
     hidden_dim: Optional[int] = None,
-    reuse_fp16_chunk: bool = True,
     verbose: bool = False,
     **kwargs,
 ) -> ChunkManager:
     if hidden_dim:
         search_interval = hidden_dim
     else:
         search_interval = 1024  # defaults to 1024
@@ -47,13 +46,9 @@
             "used number: {:.2f} * 2^20, wasted number: {:.2f} * 2^20\n".format(total_size, wasted_size),
             "total wasted percentage is {:.2f}%".format(100 * safe_div(wasted_size, total_size + wasted_size)),
             sep="",
             flush=True,
         )
     dist.barrier()
 
-    chunk_manager = ChunkManager(
-        config_dict,
-        init_device,
-        reuse_fp16_chunk=reuse_fp16_chunk,
-    )
+    chunk_manager = ChunkManager(config_dict, init_device)
     return chunk_manager
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_ddp.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,35 +94,28 @@
         zero_group: Optional[ProcessGroup] = None,
         memstats: Optional[MemStats] = None,  # genimi memory stats
         master_weights: bool = True,
         extra_dp_group: Optional[ProcessGroup] = None,
         verbose: bool = False,
     ) -> None:
         assert mixed_precision in (torch.float16, torch.bfloat16)
-        reuse_fp16_chunk = master_weights if not enable_gradient_accumulation else False
-        self.enable_gradient_accumulation = enable_gradient_accumulation
         if chunk_config_dict is not None:
-            self.chunk_manager = ChunkManager(
-                chunk_config_dict,
-                chunk_init_device,
-                reuse_fp16_chunk=reuse_fp16_chunk,
-            )
+            self.chunk_manager = ChunkManager(chunk_config_dict, chunk_init_device)
         else:
             # some ugly hotfix for the compatibility with Lightning
             if search_range_m is None:
                 search_range_m = 32
             self.chunk_manager = init_chunk_manager(
                 model=module,
                 init_device=chunk_init_device,
                 hidden_dim=hidden_dim,
                 search_range_m=search_range_m,
                 min_chunk_size_m=min_chunk_size_m,
                 strict_ddp_flag=strict_ddp_mode,
                 process_group=zero_group,
-                reuse_fp16_chunk=reuse_fp16_chunk,
                 verbose=verbose,
             )
         self.gemini_manager = GeminiManager(
             placement_policy,
             self.chunk_manager,
             memstats,
             shard_param_frac=shard_param_frac,
@@ -131,24 +124,31 @@
             warmup_non_model_data_ratio=warmup_non_model_data_ratio,
             steady_cuda_cap_ratio=steady_cuda_cap_ratio,
         )
         self.force_outputs_fp32 = force_outputs_fp32
         self.param_op_hook = GeminiZeROHook(self.gemini_manager)
         self.fp32_params: List[torch.Tensor] = list()
         self.fp16_params: List[ColoParameter] = list()
+        self.overflow_counter = 0
         self.grads_device: Dict[torch.Tensor, torch.device] = dict()
         self.param2name: Dict[nn.Parameter, str] = dict()
         self.name2param: Dict[str, nn.Parameter] = dict()
         self.scatter_after_inference = scatter_after_inference
         self.mixed_precision = mixed_precision
         self.zero_group = zero_group or _get_default_group()
         self.extra_dp_group = extra_dp_group
 
+        self.reuse_fp16_chunk = master_weights
         self.master_weights = master_weights
 
+        self.enable_gradient_accumulation = enable_gradient_accumulation
+        if self.enable_gradient_accumulation:
+            self.reuse_fp16_chunk = False
+        self.accumulating_grads = False  # Whether model is accumulating gradients
+
         self._logger = get_dist_logger()
 
         if self.gemini_manager._premade_memstats_:
             # build chunk in param runtime visited order.
             param_order = self.gemini_manager.memstats()._param_runtime_order
         else:
             # build chunk in param initialized order.
@@ -174,37 +174,15 @@
         self._non_persistent_buffers_set = self._get_non_persistent_buffers_set(module)
         self._cast_buffers()
         # register grad hook
         for p in module.parameters():
             if is_ddp_ignored(p):
                 continue
             if p.requires_grad:
-                p._grad_handle = p.register_hook(
-                    partial(
-                        GeminiDDP.grad_handle,
-                        chunk_manager=self.chunk_manager,
-                        param2name=self.param2name,
-                        grads_device=self.grads_device,
-                        master_weights=self.master_weights,
-                        enable_gradient_accumulation=self.enable_gradient_accumulation,
-                        p=p,
-                    )
-                )
-
-    def remove_hooks(self):
-        for p in self.module.parameters():
-            if is_ddp_ignored(p):
-                continue
-            if p.requires_grad:
-                assert hasattr(p, "_grad_handle")
-                p._grad_handle.remove()
-                delattr(p, "_grad_handle")
-
-    def __del__(self):
-        self.remove_hooks()
+                p.register_hook(partial(self.grad_handle, p))
 
     def parameters(self, recurse: bool = True):
         return self.module.parameters(recurse)
 
     def named_parameters(self, prefix: str = "", recurse: bool = True):
         return self.module.named_parameters(prefix, recurse)
 
@@ -342,97 +320,88 @@
             error_str = "\n\t".join(error_params)
             raise RuntimeError(
                 "ZERO DDP error: the synchronization of gradients doesn't exit properly.",
                 "The most possible reason is that the model is not compatible with GeminiDDP.\n",
                 f"{error_str}",
             )
         self._setup_grads_ptr()
-        if self.enable_gradient_accumulation and not self.chunk_manager.accumulating_grads:
-            self.chunk_manager.accumulating_grads = True  # Turn on the state of gradient accumulation.
+        if self.enable_gradient_accumulation and not self.accumulating_grads:
+            self.accumulating_grads = True  # Turn on the state of gradient accumulation.
         self._logger.debug(
             f"comp cuda demand time: {self.gemini_manager._comp_cuda_demand_time}, layout time: {self.gemini_manager._layout_time}, evict time: {self.gemini_manager._evict_time}, CPU->CUDA vol: {self.gemini_manager._h2d_volume}B, CUDA->CPU vol: {self.gemini_manager._d2h_volume}"
         )
         self.gemini_manager.post_iter()
 
     def backward(self, loss: torch.Tensor):
         self._pre_backward()
         with self.param_op_hook.switch_to_backward(), ColoParamOpHookManager.use_hooks(self.param_op_hook):
             loss.backward()
         self._post_backward()
 
     def backward_by_grad(self, tensor, grad):
         raise RuntimeError("Gemini is not compatible with pipeline. backward_by_grad shoudn't be called in Gemini.")
 
-    @staticmethod
-    def grad_handle(
-        grad,
-        chunk_manager: ChunkManager,
-        param2name: Dict,
-        grads_device: Dict,
-        master_weights: bool,
-        enable_gradient_accumulation: bool,
-        p: nn.Parameter,
-    ):
+    def grad_handle(self, p, grad):
         setattr(p, "_gemini_reduced", True)
         empty_grad = torch.empty_like(grad)
         free_storage(empty_grad)
         with torch._C.DisableTorchFunction():
-            chunk = chunk_manager.get_chunk(p)
+            chunk = self.chunk_manager.get_chunk(p)
             if chunk.tensors_info[p].state != TensorState.HOLD_AFTER_BWD:
                 raise RuntimeError(
-                    f"Parameter `{param2name[p]}` failed at the gradient reduction. "
+                    f"Parameter `{self.param2name[p]}` failed at the gradient reduction. "
                     "Some unsupported torch function is operated upon this parameter."
                 )
             grad_chunk = chunk
-            if not chunk_manager.reuse_fp16_chunk:
-                if not chunk_manager.accumulating_grads:
-                    grad_chunk = chunk_manager.init_grad_chunk(chunk)
+            if not self.reuse_fp16_chunk:
+                if not self.accumulating_grads:
+                    grad_chunk = self.chunk_manager.init_grad_chunk(chunk)
                 else:
                     assert chunk.grad_chunk is not None
-                    if chunk.grad_chunk not in chunk_manager.accessed_chunks:
-                        grad_chunk = chunk_manager.rearrange_accumulated_grad_chunk(chunk)
+                    if chunk.grad_chunk not in self.chunk_manager.accessed_chunks:
+                        grad_chunk = self.chunk_manager.rearrange_accumulated_grad_chunk(chunk)
                     else:
                         grad_chunk = chunk.grad_chunk
                         chunk.grad_chunk.l2_norm = None
 
                 # hold -> compute -> hold after bwd
                 grad_chunk.tensor_trans_state(p, TensorState.COMPUTE)
                 grad_chunk.tensor_trans_state(p, TensorState.HOLD_AFTER_BWD)
                 # fp16 param chunk: hold after bwd -> ready for reduce -> hold
                 chunk.tensor_trans_state(p, TensorState.READY_FOR_REDUCE)
                 chunk.tensor_trans_state(p, TensorState.HOLD)
 
             grad_chunk.tensor_trans_state(p, TensorState.READY_FOR_REDUCE)
-            if not chunk_manager.accumulating_grads:
-                grad_chunk.copy_tensor_to_chunk_slice(p, grad, update_ptr=chunk_manager.reuse_fp16_chunk)
+            if not self.accumulating_grads:
+                grad_chunk.copy_tensor_to_chunk_slice(p, grad, update_ptr=self.reuse_fp16_chunk)
             else:
                 grad_chunk.add_tensor_to_chunk_slice(p, grad)
-            reduced = chunk_manager.reduce_chunk(grad_chunk)
+            reduced = self.chunk_manager.reduce_chunk(grad_chunk)
             if reduced:
-                if not chunk_manager.reuse_fp16_chunk:
+                if not self.reuse_fp16_chunk:
                     if chunk.keep_gathered:
-                        chunk_manager.fake_release_chunk(chunk)
+                        self.chunk_manager.fake_release_chunk(chunk)
                     else:
-                        chunk_manager.release_chunk(chunk)
+                        self.chunk_manager.release_chunk(chunk)
                 if grad_chunk.is_gathered:
                     grad_chunk.cuda_global_chunk.div_(chunk.pg_size)
-                    if chunk.extra_dp_group is not None:
+                    if self.extra_dp_group is not None:
                         grad_chunk.cuda_global_chunk.div_(chunk.extra_dp_size)
                 else:
                     grad_chunk.cuda_shard.div_(chunk.pg_size)
-                    if chunk.extra_dp_group is not None:
+                    if self.extra_dp_group is not None:
                         grad_chunk.cuda_shard.div_(chunk.extra_dp_size)
                 # check overflow elements
-                chunk_manager.overflow_counter += grad_chunk.has_inf_or_nan
+                self.overflow_counter += grad_chunk.has_inf_or_nan
                 # record l2 norm for gradient clipping. flag is bound to fp16 chunk
                 if chunk.l2_norm_flag:
                     grad_chunk.set_l2_norm()
-                chunk_manager.move_chunk(grad_chunk, grads_device[p], force_copy=True)
-                if not (master_weights) or (enable_gradient_accumulation):
-                    chunk_manager.move_chunk(chunk, grads_device[p], force_copy=True)
+                self.chunk_manager.move_chunk(grad_chunk, self.grads_device[p], force_copy=True)
+                if not (self.master_weights) or (self.enable_gradient_accumulation):
+                    self.chunk_manager.move_chunk(chunk, self.grads_device[p], force_copy=True)
         return empty_grad
 
     def zero_grad(self, set_to_none: bool = False) -> None:
         self.module.zero_grad(set_to_none=True)
 
     def set_chunk_grad_device(self, chunk: Chunk, device: torch.device) -> None:
         for tensor in chunk.get_tensors():
@@ -540,19 +509,19 @@
             prefix (str): the prefix for parameters and buffers used in this
                 module
         """
         assert keep_vars is False, "`state_dict` with parameter, `keep_vars=True`, is not supported now."
 
         # get copies of fp32 parameters in CPU
         # as memory of fp16_params may be reused by grad, it's not reliable, we should use fp32_params and convert to fp16
-        params = self.fp32_params if self.chunk_manager.reuse_fp16_chunk else self.fp16_params
+        params = self.fp32_params if self.reuse_fp16_chunk else self.fp16_params
         param_to_save_data = self._get_param_to_save_data(params, only_rank_0)
         # get the mapping between copies and fp16 parameters
         p_mapping = dict()
-        if self.chunk_manager.reuse_fp16_chunk:
+        if self.reuse_fp16_chunk:
             for p, fp32_p in zip(self.fp16_params, self.fp32_params):
                 name = self.param2name[p]
                 assert fp32_p in param_to_save_data, "Parameter '{}' is neglected in the chunk list".format(name)
                 record_parameter = param_to_save_data[fp32_p]
                 p_mapping[p] = record_parameter
         else:
             p_mapping = param_to_save_data
@@ -740,32 +709,30 @@
 
         fp32_to_name = dict()
         for p, fp32_p in zip(self.fp16_params, self.fp32_params):
             if p is not None:
                 name = self.param2name[p]
                 fp32_to_name[fp32_p] = name
 
-        params_to_load = self.fp32_params if self.chunk_manager.reuse_fp16_chunk else self.fp16_params
+        params_to_load = self.fp32_params if self.reuse_fp16_chunk else self.fp16_params
         chunk_list = self.chunk_manager.get_chunks(params_to_load)
         for chunk in chunk_list:
             temp_chunk = get_temp_total_chunk_on_cuda(chunk, self.mixed_precision)
 
             for tensor, tensor_info in chunk.tensors_info.items():
                 source_device_mesh, source_sharding_spec, shard_fn, gather_fn = None, None, None, None
                 if is_distributed_tensor(tensor):
                     # shard the input param
                     source_device_mesh = get_device_mesh(tensor)
                     source_sharding_spec = get_sharding_spec(tensor)
                 elif is_customized_distributed_tensor(tensor):
                     shard_fn = tensor.shard_fn
                     gather_fn = tensor.gather_fn
 
-                parameter_name = (
-                    fp32_to_name[tensor] if self.chunk_manager.reuse_fp16_chunk else self.param2name[tensor]
-                )
+                parameter_name = fp32_to_name[tensor] if self.reuse_fp16_chunk else self.param2name[tensor]
                 parameter_slice = temp_chunk[tensor_info.offset : tensor_info.end]
                 load(
                     parameter_name,
                     tensor,
                     partial(load_parameter, parameter_slice),
                     source_device_mesh,
                     source_sharding_spec,
@@ -929,15 +896,15 @@
         for name, param in self.name2param.items():
             if param is not None:
                 if is_ddp_ignored(param):
                     # deal with ddp ignored parameters
                     gathered_param = param if keep_vars else param.detach()
                 else:
                     # as memory of fp16 param may be reused, we should use fp32 param and then convert to fp16
-                    param_to_save = fp16_to_fp32[param] if self.chunk_manager.reuse_fp16_chunk else param
+                    param_to_save = fp16_to_fp32[param] if self.reuse_fp16_chunk else param
                     if param_to_save not in gathered_param_buffer:
                         chunk = self.chunk_manager.get_chunk(param_to_save)
                         gathered_param_buffer.update(self._get_chunk_to_save_data(chunk, only_rank_0))
                     gathered_param = gathered_param_buffer.pop(param_to_save)
 
                 block, block_size = sharder.append_param(prefix + name, gathered_param)
                 if block is not None:
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,18 @@
     ) -> None:
         super().__init__(
             initial_scale, min_scale, growth_factor, backoff_factor, growth_interval, hysteresis, max_scale
         )
         self.module = module
 
     def check_local_overflow(self) -> bool:
-        return self.module.chunk_manager.overflow_counter > 0
+        return self.module.overflow_counter > 0
 
     def pre_zero_grad(self) -> None:
-        self.module.chunk_manager.overflow_counter = 0
+        self.module.overflow_counter = 0
 
 
 class GeminiOptimizer(OptimizerWrapper):
     """A wrapper for optimizer. ``GeminiDDP`` and ``GeminiOptimizer`` implement Zero Redundancy Optimizer (ZeRO state-3).
 
     Note:
         You must use ``GeminiDDP`` with ``GeminiOptimizer``.
@@ -198,15 +198,15 @@
 
     def _set_grad_ptr(self):
         for group in self.param_groups:
             for fake_param in group["params"]:
                 chunk16 = self.param_to_chunk16[fake_param]
                 begin, end = self.param_to_range[fake_param]
 
-                grad_chunk16 = chunk16 if self.module.chunk_manager.reuse_fp16_chunk else chunk16.grad_chunk
+                grad_chunk16 = chunk16 if self.module.reuse_fp16_chunk else chunk16.grad_chunk
                 fake_param.data = grad_chunk16.payload[begin:end]
                 fake_param.grad = fake_param.data
 
                 to_update_chunk = chunk16.paired_chunk if self.module.master_weights else chunk16
                 fake_param.data = to_update_chunk.payload[begin:end]
 
     def _update_fp16_params(self):
@@ -217,22 +217,22 @@
                 fake_param.data = none_tensor.to(fake_param.device)
 
         for chunk16 in self.chunk16_set:
             chunk16.optim_update()
 
     def _clear_global_norm(self) -> None:
         for c16 in self.chunk16_set:
-            grad_chunk = c16 if self.module.chunk_manager.reuse_fp16_chunk else c16.grad_chunk
+            grad_chunk = c16 if self.module.reuse_fp16_chunk else c16.grad_chunk
             grad_chunk.l2_norm = None
 
     def _calc_global_norm(self) -> float:
         norm_sqr: float = 0.0
         group_to_norm = dict()
         for c16 in self.chunk16_set:
-            grad_chunk = c16 if self.module.chunk_manager.reuse_fp16_chunk else c16.grad_chunk
+            grad_chunk = c16 if self.module.reuse_fp16_chunk else c16.grad_chunk
             assert grad_chunk.l2_norm is not None
 
             if grad_chunk.is_gathered:
                 norm_sqr += grad_chunk.l2_norm
             else:
                 # this chunk is sharded, use communication to collect total norm
                 if grad_chunk.torch_pg not in group_to_norm:
@@ -271,28 +271,28 @@
         self._set_grad_ptr()
 
         if self.mix_precision_mixin.should_skip_step():
             if self.verbose:
                 self._logger.info(f"Found overflow. Skip step")
             self._clear_global_norm()  # clear recorded norm
             self.zero_grad()  # reset all gradients
-            if self.module.chunk_manager.reuse_fp16_chunk:
+            if self.module.reuse_fp16_chunk:
                 self._update_fp16_params()
             return
 
         # get combined scale. combined scale = loss scale * clipping norm
         # so that gradient = gradient / combined scale
         combined_scale = self._get_combined_scale()
 
         ret = self.optim.step(div_scale=combined_scale, *args, **kwargs)
         self._register_states()
         self.zero_grad()
         if self.module.master_weights:
             self._update_fp16_params()
-        self.module.chunk_manager.accumulating_grads = False
+        self.module.accumulating_grads = False
         return ret
 
     def clip_grad_norm(self, model: torch.nn.Module, max_norm: float, norm_type: float = 2.0):
         raise NotImplementedError
 
     def backward(self, loss: torch.Tensor):
         loss = self.mix_precision_mixin.pre_backward(loss)
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2024.5.4/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2024.5.4/colossalai/zero/low_level/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,29 @@
 
 from torch import Tensor
 
 from .base_store import BaseStore
 
 
 class GradientStore(BaseStore):
-    def __init__(self, *args, partition_grad: bool = False, require_grad_sync: bool = True):
+    def __init__(self, *args, partition_grad: bool = False):
         super().__init__(*args)
         """
         self._grads_of_params mapping the parameter and its gradient slices
         data structure:
         {
          group_id:{
             param_id: [grad_rank0, grad_rank1, ...]
           }
         }
         """
         self._grads_of_params = dict()
-        # stage 2
-        self._partition_grads = partition_grad
-        # grad accumulation
-        self.require_grad_sync = require_grad_sync
-        self._working_index = 0 if partition_grad else self._local_rank
         # for zero2, it's `param_id: [grad_local_rank]`
+        self._working_index = 0 if partition_grad else self._local_rank
+
         self.grad_to_param_mapping = dict()
 
     def get_partitioned_gradients_by_param_id(self, group_id: int, param_id: int) -> List:
         """Return list of gradient slices of a specific parameter
 
         Args:
             group_id (int): The index of a parameter group
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2024.5.4/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2024.5.4/colossalai/zero/low_level/low_level_optim.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,20 +86,46 @@
     ):
         super(LowLevelZeroOptimizer, self).__init__(optim=optimizer)
 
         self._dtype = self.optim.param_groups[0]["params"][0].dtype
         self._logger = get_dist_logger()
         self._verbose = verbose
 
+        # stage 2
+        self._partition_grads = partition_grad
+
         self._cpu_offload = cpu_offload
 
+        # grad accumulation
+        self.require_grad_sync = True
+
+        # if process_group is none, will use the default one
+        self.dp_pg = dp_process_group
+        self._local_rank = dist.get_rank(group=self.dp_pg)
+        self._world_size = dist.get_world_size(group=self.dp_pg)
+
+        # extra dp
+        # This group is used to sync moe param, dp_world_size = moe_duplicates * extra_dp_size.
+        # Non moe param will be sync by global dp pg, moe param will be sync by extra dp pg.
+        # Moe param grad is be split as non moe param by global dp pg, and grad will be merged in step.
+        # And moe working and master param are split by extra dp pg.
+        self.moe_extra_dp_pg = moe_extra_dp_process_group
+        if self.moe_extra_dp_pg is not None:
+            self.moe_extra_dp_pg_size = dist.get_world_size(group=self.moe_extra_dp_pg)
+            self.moe_extra_dp_pg_rank = dist.get_rank(group=self.moe_extra_dp_pg)
+
         # working and master params for mixed precision training
         self._working_param_groups = dict()
         self._master_param_groups_of_current_rank = dict()
 
+        # communication params
+        self._overlap_communication = overlap_communication
+        self._reduce_bucket_size = reduce_bucket_size
+        self._communication_dtype = communication_dtype
+
         # gradient clipping
         self._clip_grad_norm = clip_grad_norm
 
         # master weights copy
         self._master_weights = master_weights
 
         if forced_dtype:
@@ -110,34 +136,32 @@
             self._dtype = forced_dtype
 
         # check argument conflict
         self._sanity_checks()
 
         # ParameterStore will manage the tensor buffers used for zero
         # it will not manage the tensors used by mixed precision training
-        self._param_store = ParameterStore(dp_process_group)
-        self._grad_store = GradientStore(dp_process_group, partition_grad=partition_grad, require_grad_sync=True)
-        self._bucket_store = BucketStore(
-            dp_process_group, reduce_bucket_size, overlap_communication, communication_dtype, moe_extra_dp_process_group
-        )
+        self._param_store = ParameterStore(self.dp_pg)
+        self._grad_store = GradientStore(self.dp_pg, partition_grad=partition_grad)
+        self._bucket_store = BucketStore(self.dp_pg)
 
         # moe param should not be stored in working_groups
         # because they have different parallel strategy
         # so we need to store them separately in param_groups
         # instead of working_groups
         self.working_moe_params = list()
 
         # iterate over the param group in the optimizer
         # partition these param groups for data parallel training
         # and add buffers to parameter store for future access
         for group_id, param_group in enumerate(self.optim.param_groups):
             group_params = list()
             for param in param_group["params"]:
                 if param.requires_grad:
-                    if self._bucket_store.moe_extra_dp_pg is None:
+                    if self.moe_extra_dp_pg is None:
                         # skip moe param
                         if is_moe_tensor(param):
                             self.working_moe_params.append(param)
                             continue
                     group_params.append(param)
 
             # add the working params to working_param_groups for bookkeeping
@@ -166,18 +190,23 @@
             self.moe_master_to_working_map = {}
             for master_moe_param, working_moe_param in zip(self.master_moe_params, self.working_moe_params):
                 self.moe_master_to_working_map[id(master_moe_param)] = working_moe_param
             # add to optim
             param_group["params"] = self.master_moe_params
             self.optim.param_groups.append(param_group)
 
+        # initialize communication stream for
+        # communication-computation overlapping
+        if self._overlap_communication:
+            self._comm_stream = get_accelerator().Stream()
+
         # reduction hook is only used if overlapping communication
         # or stage 2 is used
         # if it is stage 1 without overlapping, no hook will be attached
-        if self._bucket_store._overlap_communication or self._grad_store._partition_grads:
+        if self._overlap_communication or self._partition_grads:
             self._attach_reduction_hook()
 
         # initialize mixed precision mixin
         self.mixed_precision_mixin: Optional[MixedPrecisionMixin] = None
         if self._dtype is torch.float16:
             self.mixed_precision_mixin = LowLevelZeroFP16MixedPrecisionMixin(
                 self.num_param_groups,
@@ -189,17 +218,14 @@
                 growth_interval=growth_interval,
                 hysteresis=hysteresis,
                 max_scale=max_scale,
             )
         elif self._dtype is torch.bfloat16:
             self.mixed_precision_mixin = BF16MixedPrecisionMixin()
 
-    def __del__(self):
-        self.remove_hooks()
-
     @property
     def dtype(self):
         return self._dtype
 
     @property
     def num_param_groups(self):
         return len(self._working_param_groups)
@@ -216,36 +242,32 @@
 
     def _create_master_param_current_rank(self, param_list):
         # split each param evenly by world size
         params_current_rank = []
         device = "cpu" if self._cpu_offload else get_accelerator().get_current_device()
 
         for param in param_list:
-            padding_size = (
-                self._bucket_store.zero_world_size - param.numel() % self._bucket_store.zero_world_size
-            ) % self._bucket_store.zero_world_size
+            padding_size = (self._world_size - param.numel() % self._world_size) % self._world_size
             self._param_store.record_param_padding_size(param, padding_size)
 
             with torch.no_grad():
                 if padding_size > 0:
                     padding_param = torch.nn.functional.pad(param.data.view(-1), [0, padding_size])
                     # reset working params' ptr when no master weights
                     if self._master_weights == False:
                         param.data = padding_param[: param.numel()].view(param.shape)
                 else:
                     padding_param = param.data.view(-1)
 
-                if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(param):
-                    splited_params = padding_param.split(
-                        padding_param.numel() // self._bucket_store.moe_extra_dp_pg_size
-                    )
-                    splited_params = splited_params[self._bucket_store.moe_extra_dp_pg_rank]
+                if self.moe_extra_dp_pg is not None and is_moe_tensor(param):
+                    splited_params = padding_param.split(padding_param.numel() // self.moe_extra_dp_pg_size)
+                    splited_params = splited_params[self.moe_extra_dp_pg_rank]
                 else:
-                    splited_params = padding_param.split(padding_param.numel() // self._bucket_store.zero_world_size)
-                    splited_params = splited_params[self._bucket_store.zero_local_rank]
+                    splited_params = padding_param.split(padding_param.numel() // self._world_size)
+                    splited_params = splited_params[self._local_rank]
 
                 # use fp32 when master_weights is True
                 if self._master_weights is True:
                     splited_param_current_rank = splited_params.detach().float().to(device)
                 else:
                     splited_param_current_rank = splited_params
 
@@ -254,63 +276,49 @@
 
         return params_current_rank
 
     ###########################
     # Backward Reduction Hook #
     ###########################
 
-    @staticmethod
-    def grad_handler(
-        param: nn.Parameter,
-        group_id: int,
-        bucket_store: BucketStore,
-        param_store: ParameterStore,
-        grad_store: GradientStore,
-    ):
+    def _grad_handler(self, group_id, param):
         # if run with no_sync context, would not sync grad when backward
-        if grad_store.require_grad_sync:
-            LowLevelZeroOptimizer.add_to_bucket(param, group_id, bucket_store, param_store, grad_store)
+        if self.require_grad_sync:
+            self._add_to_bucket(param, group_id)
 
     def _attach_reduction_hook(self):
         # we iterate over the working params
         # on each param, we register a hook to its AccumulateGrad object
         for group_id in range(self.num_param_groups):
             param_group = self._working_param_groups[group_id]
             for param in param_group:
                 if param.requires_grad:
-                    param._grad_handle = param.register_post_accumulate_grad_hook(
-                        partial(
-                            LowLevelZeroOptimizer.grad_handler,
-                            group_id=group_id,
-                            bucket_store=self._bucket_store,
-                            param_store=self._param_store,
-                            grad_store=self._grad_store,
-                        )
-                    )
+                    param.register_post_accumulate_grad_hook(partial(self._grad_handler, group_id))
 
     #######################
     # Reduction Functions #
     #######################
-    @staticmethod
-    def run_reduction(bucket_store: BucketStore, grad_store: GradientStore):
-        if bucket_store.num_elements_in_bucket() > 0:
-            bucket_store.build_grad_in_bucket()
-            if bucket_store.moe_extra_dp_pg is None:
-                flat_grads = bucket_store.get_flatten_grad()
-                flat_grads /= bucket_store.zero_world_size
+
+    def _run_reduction(self):
+        if self._bucket_store.num_elements_in_bucket() > 0:
+            self._bucket_store.build_grad_in_bucket()
+
+            if self.moe_extra_dp_pg is None:
+                flat_grads = self._bucket_store.get_flatten_grad()
+                flat_grads /= self._world_size
             else:
                 # record moe and non moe param
                 moe_list = []
-                for param in bucket_store._param_list:
+                for param in self._bucket_store._param_list:
                     moe_list.append(is_moe_tensor(param))
 
                 # divide them into different groups
                 moe_grad_list = []
                 non_moe_grad_list = []
-                for grad_list in bucket_store._grad_in_bucket.values():
+                for grad_list in self._bucket_store._grad_in_bucket.values():
                     non_moe_cur_grad = []
                     moe_cur_grad = []
                     for i in range(len(grad_list)):
                         if moe_list[i] == True:
                             moe_cur_grad.append(grad_list[i])
                         else:
                             non_moe_cur_grad.append(grad_list[i])
@@ -320,249 +328,218 @@
                         non_moe_grad_list.append(non_moe_cur_grad)
 
                 if len(non_moe_grad_list) > 0:
                     non_moe_flat_grads = []
                     for grad_list in non_moe_grad_list:
                         non_moe_flat_grads.append(_flatten_dense_tensors(grad_list))
                     non_moe_flat_grads = _flatten_dense_tensors(non_moe_flat_grads)
-                    non_moe_flat_grads /= bucket_store.zero_world_size
+                    non_moe_flat_grads /= self._world_size
 
                 if len(moe_grad_list) > 0:
                     moe_flat_grads = []
                     for grad_list in moe_grad_list:
                         moe_flat_grads.append(_flatten_dense_tensors(grad_list))
                     moe_flat_grads = _flatten_dense_tensors(moe_flat_grads)
 
             # ready to add other tensors to bucket
-            bucket_store.reset_num_elements_in_bucket()
+            self._bucket_store.reset_num_elements_in_bucket()
 
-            if bucket_store._overlap_communication:
-                stream = bucket_store.comm_stream
+            if self._overlap_communication:
+                stream = self._comm_stream
                 # in case of the memory being reused in the default stream
-                if bucket_store.moe_extra_dp_pg is None:
+                if self.moe_extra_dp_pg is None:
                     flat_grads.record_stream(stream)
                 else:
                     if len(non_moe_grad_list) > 0:
                         non_moe_flat_grads.record_stream(stream)
                     if len(moe_grad_list) > 0:
                         moe_flat_grads.record_stream(stream)
                 # waiting for ops in the default stream finishing
                 stream.wait_stream(get_accelerator().current_stream())
             else:
                 stream = get_accelerator().current_stream()
 
             with get_accelerator().stream(stream):
-                group_id = bucket_store.current_group_id
+                group_id = self._bucket_store.current_group_id
 
-                if bucket_store.moe_extra_dp_pg is None:
+                if self.moe_extra_dp_pg is None:
                     grad_dtype = flat_grads.dtype
-                    if bucket_store._communication_dtype is not None:
-                        flat_grads = flat_grads.to(bucket_store._communication_dtype)
+                    if self._communication_dtype is not None:
+                        flat_grads = flat_grads.to(self._communication_dtype)
 
-                if not grad_store._partition_grads:
-                    if bucket_store.moe_extra_dp_pg is None:
-                        dist.all_reduce(flat_grads, group=bucket_store.torch_pg)
+                if not self._partition_grads:
+                    if self.moe_extra_dp_pg is None:
+                        dist.all_reduce(flat_grads, group=self.dp_pg)
                         if flat_grads.dtype != grad_dtype:
                             flat_grads = flat_grads.to(grad_dtype)
 
-                        flat_grads_per_rank = flat_grads.split(flat_grads.numel() // bucket_store.zero_world_size)
-                        grad_in_bucket = bucket_store.get_grad()
-                        LowLevelZeroOptimizer.update_unpartitoned_grad(
-                            bucket_store, grad_store, grad_in_bucket.values(), flat_grads_per_rank, group_id
-                        )
+                        flat_grads_per_rank = flat_grads.split(flat_grads.numel() // self._world_size)
+                        grad_in_bucket = self._bucket_store.get_grad()
+                        self._update_unpartitoned_grad(grad_in_bucket.values(), flat_grads_per_rank, group_id)
 
                     # sync extra zero group
                     else:
                         # sync non moe param in global dp group
                         if len(non_moe_grad_list) > 0:
-                            dist.all_reduce(non_moe_flat_grads, group=bucket_store.torch_pg)
+                            dist.all_reduce(non_moe_flat_grads, group=self.dp_pg)
                             flat_grads_per_rank = non_moe_flat_grads.split(
-                                non_moe_flat_grads.numel() // bucket_store.zero_world_size
-                            )
-                            LowLevelZeroOptimizer.update_unpartitoned_grad(
-                                bucket_store, grad_store, non_moe_grad_list, flat_grads_per_rank, group_id
+                                non_moe_flat_grads.numel() // self._world_size
                             )
+                            self._update_unpartitoned_grad(non_moe_grad_list, flat_grads_per_rank, group_id)
 
                         # sync moe param only in zero group
                         if len(moe_grad_list) > 0:
-                            dist.all_reduce(moe_flat_grads, group=bucket_store.moe_extra_dp_pg)
-                            flat_grads_per_rank = moe_flat_grads.split(
-                                moe_flat_grads.numel() // bucket_store.zero_world_size
-                            )
-                            LowLevelZeroOptimizer.update_unpartitoned_grad(
-                                bucket_store, grad_store, moe_grad_list, flat_grads_per_rank, group_id
-                            )
+                            dist.all_reduce(moe_flat_grads, group=self.moe_extra_dp_pg)
+                            flat_grads_per_rank = moe_flat_grads.split(moe_flat_grads.numel() // self._world_size)
+                            self._update_unpartitoned_grad(moe_grad_list, flat_grads_per_rank, group_id)
 
                 else:
-                    if bucket_store.moe_extra_dp_pg is None:
-                        flat_grads_list = list(flat_grads.split(len(flat_grads) // bucket_store.zero_world_size))
+                    if self.moe_extra_dp_pg is None:
+                        flat_grads_list = list(flat_grads.split(len(flat_grads) // self._world_size))
                         recieved_grad = torch.zeros_like(flat_grads_list[0])
-                        dist.reduce_scatter(recieved_grad, flat_grads_list, group=bucket_store.torch_pg)
+                        dist.reduce_scatter(recieved_grad, flat_grads_list, group=self.dp_pg)
 
                         if recieved_grad.dtype != grad_dtype:
                             recieved_grad = recieved_grad.to(grad_dtype)
 
-                        grad_in_bucket_current_rank = bucket_store.get_grad()[bucket_store.zero_local_rank]
-                        LowLevelZeroOptimizer.update_partitoned_grad(
-                            bucket_store, grad_store, grad_in_bucket_current_rank, recieved_grad, group_id, 1
-                        )
+                        grad_in_bucket_current_rank = self._bucket_store.get_grad()[self._local_rank]
+                        self._update_partitoned_grad(grad_in_bucket_current_rank, recieved_grad, group_id, 1)
                     else:
                         # categorize moe and non moe param
-                        grad_in_bucket_current_rank = bucket_store.get_grad()[bucket_store.zero_local_rank]
+                        grad_in_bucket_current_rank = self._bucket_store.get_grad()[self._local_rank]
                         moe_grad_in_bucket_current_rank = []
                         non_moe_grad_in_bucket_current_rank = []
                         for idx, grad in enumerate(grad_in_bucket_current_rank):
                             if moe_list[idx] == True:
                                 moe_grad_in_bucket_current_rank.append(grad)
                             else:
                                 non_moe_grad_in_bucket_current_rank.append(grad)
 
                         if len(non_moe_grad_list) > 0:
                             flat_grads_list = list(
-                                non_moe_flat_grads.split(len(non_moe_flat_grads) // bucket_store.zero_world_size)
+                                non_moe_flat_grads.split(len(non_moe_flat_grads) // self._world_size)
                             )
                             recieved_grad = torch.zeros_like(flat_grads_list[0])
-                            dist.reduce_scatter(recieved_grad, flat_grads_list, group=bucket_store.torch_pg)
-                            LowLevelZeroOptimizer.update_partitoned_grad(
-                                bucket_store,
-                                grad_store,
+                            dist.reduce_scatter(recieved_grad, flat_grads_list, group=self.dp_pg)
+                            self._update_partitoned_grad(
                                 non_moe_grad_in_bucket_current_rank,
                                 recieved_grad,
                                 group_id,
                                 1,
                             )
 
                         if len(moe_grad_list) > 0:
                             flat_grads_list = list(
-                                moe_flat_grads.split(len(moe_flat_grads) // bucket_store.moe_extra_dp_pg_size)
+                                moe_flat_grads.split(len(moe_flat_grads) // self.moe_extra_dp_pg_size)
                             )
                             recieved_grad = torch.zeros_like(flat_grads_list[0])
                             dist.reduce_scatter(
                                 recieved_grad,
                                 flat_grads_list,
-                                group=bucket_store.moe_extra_dp_pg,
+                                group=self.moe_extra_dp_pg,
                             )
-                            param_slice = bucket_store.zero_world_size // bucket_store.moe_extra_dp_pg_size
+                            param_slice = self._world_size // self.moe_extra_dp_pg_size
                             recieved_grad = list(recieved_grad.split(len(recieved_grad) // param_slice))
                             for split_recieved_grad in recieved_grad:
                                 split_recieved_grad = _unflatten_dense_tensors(
                                     split_recieved_grad, moe_grad_in_bucket_current_rank
                                 )
                                 for real_grad, grad in zip(split_recieved_grad, moe_grad_in_bucket_current_rank):
-                                    param_id = bucket_store.get_param_id_of_grad(grad)
-                                    LowLevelZeroOptimizer.add_grad(
-                                        grad_store, real_grad, param_slice, group_id, param_id
-                                    )
-
-                bucket_store.reset()
-
-    @staticmethod
-    def update_unpartitoned_grad(
-        bucket_store: BucketStore,
-        grad_store: GradientStore,
-        origin_grad_list: List,
-        flat_grad_list: List,
-        group_id: int,
-    ) -> None:
+                                    param_id = self._bucket_store.get_param_id_of_grad(grad)
+                                    self._add_grad(real_grad, param_slice, group_id, param_id)
+
+                self._bucket_store.reset()
+
+    def _update_unpartitoned_grad(self, origin_grad_list: List, flat_grad_list: List, group_id: int) -> None:
         for rank, grad_list in enumerate(origin_grad_list):
             sync_tensor(flat_grad_list[rank], grad_list)
             for grad in grad_list:
-                param_id = bucket_store.get_param_id_of_grad(grad)
-                LowLevelZeroOptimizer.add_grad(grad_store, grad, bucket_store.zero_world_size, group_id, param_id, rank)
+                param_id = self._bucket_store.get_param_id_of_grad(grad)
+                self._add_grad(grad, self._world_size, group_id, param_id, rank)
 
-    @staticmethod
-    def update_partitoned_grad(
-        bucket_store: BucketStore,
-        grad_store: GradientStore,
+    def _update_partitoned_grad(
+        self,
         origin_grad_list: List,
         flat_grad: torch.Tensor,
         group_id: int,
         partition_num: int,
     ) -> None:
         sync_tensor(flat_grad, origin_grad_list)
         for grad in origin_grad_list:
-            param_id = bucket_store.get_param_id_of_grad(grad)
-            LowLevelZeroOptimizer.add_grad(grad_store, grad, partition_num, group_id, param_id)
+            param_id = self._bucket_store.get_param_id_of_grad(grad)
+            self._add_grad(grad, partition_num, group_id, param_id)
 
-    @staticmethod
-    def add_grad(
-        grad_store: GradientStore,
+    def _add_grad(
+        self,
         grad: torch.Tensor,
         partition_num: int,
         group_id: int,
         param_id: int,
         rank: int = 0,
     ) -> None:
-        if len(grad_store.get_partitioned_gradients_by_param_id(group_id, param_id)) < partition_num:
-            grad_store.append_gradients_by_param_id(grad, group_id, param_id)
+        if len(self._grad_store.get_partitioned_gradients_by_param_id(group_id, param_id)) < partition_num:
+            self._grad_store.append_gradients_by_param_id(grad, group_id, param_id)
         else:
-            grad_store.add_gradients_by_param_id(grad, rank, group_id, param_id)
+            self._grad_store.add_gradients_by_param_id(grad, rank, group_id, param_id)
 
-    @staticmethod
-    def add_to_bucket(
-        param: nn.Parameter,
-        group_id: int,
-        bucket_store: BucketStore,
-        param_store: ParameterStore,
-        grad_store: GradientStore,
-    ):
+    def _add_to_bucket(self, param, group_id):
         param_size = param.numel()
 
         # check if the bucket is full
         # if full, will reduce the grads already in the bucket
         # or got a grad of param from another group
         # after reduction, the bucket will be empty
         if (
-            bucket_store.num_elements_in_bucket() + param_size > bucket_store.reduce_bucket_size
-            or group_id != bucket_store.current_group_id
+            self._bucket_store.num_elements_in_bucket() + param_size > self._reduce_bucket_size
+            or group_id != self._bucket_store.current_group_id
         ):
-            LowLevelZeroOptimizer.run_reduction(bucket_store, grad_store)
+            self._run_reduction()
 
-        padding_size = param_store.get_param_padding_size(param)
-        bucket_store.add_param_grad(group_id, param, padding_size)
+        padding_size = self._param_store.get_param_padding_size(param)
+        self._bucket_store.add_param_grad(group_id, param, padding_size)
 
     ################################
     # torch.optim.Optimizer methods
     ################################
 
     def backward(self, loss, retain_graph=False):
         assert not (
-            self._grad_store._partition_grads and not self._grad_store.require_grad_sync
+            self._partition_grads and not self.require_grad_sync
         ), "ZeRO2(partition_grads) and no_sync are not compatible"
 
         if self.mixed_precision_mixin is not None:
             loss = self.mixed_precision_mixin.pre_backward(loss)
 
         loss.backward(retain_graph=retain_graph)
 
-        if not self._grad_store.require_grad_sync:
+        if not self.require_grad_sync:
             return
 
-        self._reduce_grad(self._grad_store._partition_grads)
+        self._reduce_grad(self._partition_grads)
 
         # clear reduced grads
-        if self._bucket_store._overlap_communication:
+        if self._overlap_communication:
             get_accelerator().synchronize()
         self.zero_grad()
 
     def backward_by_grad(self, tensor, grad):
         assert not (
-            self._grad_store._partition_grads and not self._grad_store.require_grad_sync
+            self._partition_grads and not self.require_grad_sync
         ), "ZeRO2(partition_grads) and gradient accumulation(no_sync) are not compatible"
 
         if self.mixed_precision_mixin is not None:
             grad = self.mixed_precision_mixin.pre_backward_by_grad(tensor, grad)
         torch.autograd.backward(tensor, grad)
 
-        if not self._grad_store.require_grad_sync:
+        if not self.require_grad_sync:
             return
-        self._reduce_grad(self._grad_store._partition_grads)
+        self._reduce_grad(self._partition_grads)
 
         # clear reduced grads
-        if self._bucket_store._overlap_communication:
+        if self._overlap_communication:
             get_accelerator().synchronize()
 
         self.zero_grad()
 
     def zero_grad(self, set_to_none=True):
         """
         Set parameter gradients to zero. If set_to_none = True, gradient
@@ -585,15 +562,15 @@
 
     ####################
     # Update Parameter #
     ####################
 
     def step(self, closure=None):
         assert closure is None, "closure is not supported by step()"
-        if not self._grad_store.require_grad_sync:
+        if not self.require_grad_sync:
             return
 
         if self.mixed_precision_mixin is not None and self.mixed_precision_mixin.should_skip_step():
             self._grad_store.reset_all_gradients()
             if self._verbose:
                 self._logger.info(f"Found overflow. Skip step")
             self.zero_grad()
@@ -604,37 +581,35 @@
         norm_groups = []
 
         # sometimes not all params are 'really' working
         # for instance, when layer drop, the dropped layer has no grad
         # and should not be updated
         real_working_params = dict()
         real_master_params = dict()
-        grad_index = 0 if self._grad_store._partition_grads else self._bucket_store.zero_local_rank
+        grad_index = 0 if self._partition_grads else self._local_rank
         for group_id in range(self.num_param_groups):
             master_params = self._master_param_groups_of_current_rank[group_id]
             real_working_params[group_id] = []
             real_master_params[group_id] = []
             for splited_param in master_params:
                 working_param = self._param_store.master_to_working_param[id(splited_param)]
                 # if a working param requires grad and has no grad
                 # it is not 'really' working, e.g. the droped layer
                 # else the splited grad should be attached to the splited param
                 grads = self._grad_store.get_partitioned_gradients_by_param_id(group_id, id(working_param))
                 if len(grads) > 0:
                     # moe hybrid zero
-                    if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(working_param):
+                    if self.moe_extra_dp_pg is not None and is_moe_tensor(working_param):
                         real_working_params[group_id].append(working_param)
-                        if self._grad_store._partition_grads:
+                        if self._partition_grads:
                             grad = grads
                         else:
-                            param_slice = self._bucket_store.zero_world_size // self._bucket_store.moe_extra_dp_pg_size
+                            param_slice = self._world_size // self.moe_extra_dp_pg_size
                             grad = grads[
-                                self._bucket_store.moe_extra_dp_pg_rank
-                                * param_slice : (self._bucket_store.moe_extra_dp_pg_rank + 1)
-                                * param_slice
+                                self.moe_extra_dp_pg_rank * param_slice : (self.moe_extra_dp_pg_rank + 1) * param_slice
                             ]
                         grad = flatten(grad)
                     else:
                         real_working_params[group_id].append(working_param)
                         grad = grads[grad_index]
                     # no need to copy fp32 grad if master_weights is False
                     if self._master_weights:
@@ -695,33 +670,33 @@
 
         # update working partition updated by the current rank
         device = get_accelerator().get_current_device()
         for group_id in range(self.num_param_groups):
             master_working_param = self.optim.param_groups[group_id]["params"]
             for idx, splited_param in enumerate(master_working_param):
                 working_param = real_working_params[group_id][idx]
-                if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(working_param):
+                if self.moe_extra_dp_pg is not None and is_moe_tensor(working_param):
                     all_splited_param = [
                         torch.zeros(splited_param.shape, device=device, dtype=self._dtype)
-                        for _ in range(self._bucket_store.moe_extra_dp_pg_size)
+                        for _ in range(self.moe_extra_dp_pg_size)
                     ]
                     dist.all_gather(
                         all_splited_param,
                         splited_param.to(device).to(self._dtype),
-                        group=self._bucket_store.moe_extra_dp_pg,
+                        group=self.moe_extra_dp_pg,
                     )
                 else:
                     all_splited_param = [
                         torch.zeros(splited_param.shape, device=device, dtype=self._dtype)
-                        for _ in range(self._bucket_store.zero_world_size)
+                        for _ in range(self._world_size)
                     ]
                     dist.all_gather(
                         all_splited_param,
                         splited_param.to(device).to(self._dtype),
-                        group=self._bucket_store.torch_pg,
+                        group=self.dp_pg,
                     )
                 working_param.data.copy_(flatten(all_splited_param)[: working_param.numel()].reshape_as(working_param))
             self.optim.param_groups[group_id]["params"] = self._master_param_groups_of_current_rank[group_id]
 
     def _compute_grad_norm(self, gradients: List[Tensor], norm_type: int = 2) -> float:
         r"""
         Compute and return the gradient norm for gradient clipping.
@@ -741,15 +716,15 @@
         if norm_type == inf:
             total_norm = max(grad.data.abs().max() for grad in gradients)
             total_norm_cuda = torch.tensor(
                 [float(total_norm)],
                 device=get_accelerator().get_current_device(),
                 dtype=torch.float,
             )
-            dist.all_reduce(total_norm_cuda, op=torch.distributed.ReduceOp.MAX, group=self._bucket_store.torch_pg)
+            dist.all_reduce(total_norm_cuda, op=torch.distributed.ReduceOp.MAX, group=self.dp_pg)
             total_norm = total_norm_cuda.item()
 
         else:
             total_norm_exponentiated = 0.0
             for grad in gradients:
                 grad_norm_exponentiated = grad.data.double().norm(norm_type) ** norm_type
                 total_norm_exponentiated += grad_norm_exponentiated
@@ -759,15 +734,15 @@
                 [float(total_norm_exponentiated)],
                 device=get_accelerator().get_current_device(),
                 dtype=torch.float,
             )
             torch.distributed.all_reduce(
                 total_norm_exponentiated_cuda,
                 op=torch.distributed.ReduceOp.SUM,
-                group=self._bucket_store.torch_pg,
+                group=self.dp_pg,
             )
             total_norm = total_norm_exponentiated_cuda.item() ** (1.0 / norm_type)
 
         return total_norm
 
     #############################
     # Mixed Precision Utilities #
@@ -794,41 +769,35 @@
 
     # this method is used to sync gradient manually
     def _sync_grad(self):
         for group_id in range(self.num_param_groups):
             param_group = self._working_param_groups[group_id]
             for param in param_group:
                 if param.requires_grad and param.grad is not None:
-                    LowLevelZeroOptimizer.add_to_bucket(
-                        param,
-                        group_id,
-                        self._bucket_store,
-                        self._param_store,
-                        self._grad_store,
-                    )
+                    self._add_to_bucket(param, group_id)
 
-        LowLevelZeroOptimizer.run_reduction(self._bucket_store, self._grad_store)
+        self._run_reduction()
 
     def _reduce_grad(self, partition_grad):
         # if not overlapping communication (no reduction hook is attached) when zero1
         # we need to manually reduce these gradients
-        if not partition_grad and not self._bucket_store._overlap_communication:
+        if not partition_grad and not self._overlap_communication:
             self._sync_grad()
         else:
-            LowLevelZeroOptimizer.run_reduction(self._bucket_store, self._grad_store)
+            self._run_reduction()
 
     # this context comes from pytorch DDP
     @contextmanager
     def no_sync(self):
-        old_require_grad_sync = self._grad_store.require_grad_sync
-        self._grad_store.require_grad_sync = False
+        old_require_grad_sync = self.require_grad_sync
+        self.require_grad_sync = False
         try:
             yield
         finally:
-            self._grad_store.require_grad_sync = old_require_grad_sync
+            self.require_grad_sync = old_require_grad_sync
 
     ##############
     # State Dict #
     ##############
 
     def _pack_state(self, state: Dict) -> Dict:
         # comes from pytorch optimizer.state_dict()
@@ -860,26 +829,24 @@
         zero_state = dict()
         device = get_accelerator().get_current_device()
         for param, state in self.optim.state.items():
             zero_state[param] = copy.deepcopy(state)
             for k, v in state.items():
                 if isinstance(v, torch.Tensor) and k != "step":
                     working_param = self._param_store.master_to_working_param[id(param)]
-                    if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(v):
+                    if self.moe_extra_dp_pg is not None and is_moe_tensor(v):
                         gather_tensor = [
-                            torch.zeros(v.shape, device=device, dtype=v.dtype)
-                            for _ in range(self._bucket_store.moe_extra_dp_pg_size)
+                            torch.zeros(v.shape, device=device, dtype=v.dtype) for _ in range(self.moe_extra_dp_pg_size)
                         ]
-                        dist.all_gather(gather_tensor, v.to(device), group=self._bucket_store.moe_extra_dp_pg)
+                        dist.all_gather(gather_tensor, v.to(device), group=self.moe_extra_dp_pg)
                     else:
                         gather_tensor = [
-                            torch.zeros(v.shape, device=device, dtype=v.dtype)
-                            for _ in range(self._bucket_store.zero_world_size)
+                            torch.zeros(v.shape, device=device, dtype=v.dtype) for _ in range(self._world_size)
                         ]
-                        dist.all_gather(gather_tensor, v.to(device), group=self._bucket_store.torch_pg)
+                        dist.all_gather(gather_tensor, v.to(device), group=self.dp_pg)
                     param_state = (
                         torch.stack(gather_tensor).view(-1)[: working_param.numel()].reshape_as(working_param).cpu()
                     )
                     zero_state[param][k] = param_state
 
         states_dict = self._pack_state(zero_state)
 
@@ -891,31 +858,25 @@
         Args:
             state_dict (dict): A pytorch form state_dict
         """
         zero_state_dict = copy.deepcopy(state_dict)
         for param_idx, state in zero_state_dict["state"].items():
             for k, v in state.items():
                 if isinstance(v, torch.Tensor) and k != "step":
-                    padding_size = (
-                        self._bucket_store.zero_world_size - v.numel() % self._bucket_store.zero_world_size
-                    ) % self._bucket_store.zero_world_size
+                    padding_size = (self._world_size - v.numel() % self._world_size) % self._world_size
                     with torch.no_grad():
                         v = v.flatten()
                         if padding_size > 0:
                             v = torch.nn.functional.pad(v, [0, padding_size])
-                        if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(v):
-                            v_list = v.split(v.numel() // self._bucket_store.moe_extra_dp_pg_size)
-                            zero_state_dict["state"][param_idx][k] = (
-                                v_list[self._bucket_store.moe_extra_dp_pg_rank].detach().clone()
-                            )
+                        if self.moe_extra_dp_pg is not None and is_moe_tensor(v):
+                            v_list = v.split(v.numel() // self.moe_extra_dp_pg_size)
+                            zero_state_dict["state"][param_idx][k] = v_list[self.moe_extra_dp_pg_rank].detach().clone()
                         else:
-                            v_list = v.split(v.numel() // self._bucket_store.zero_world_size)
-                            zero_state_dict["state"][param_idx][k] = (
-                                v_list[self._bucket_store.zero_local_rank].detach().clone()
-                            )
+                            v_list = v.split(v.numel() // self._world_size)
+                            zero_state_dict["state"][param_idx][k] = v_list[self._local_rank].detach().clone()
 
         self.optim.load_state_dict(zero_state_dict)
 
     def state_dict_shard(self, max_shard_size: int = 1024) -> Iterator[Tuple[Dict, int]]:
         """Returns dictionaries containing a whole state of the module one by one. The max size of dictionary shard is specified by ``max_shard_size``.
            Only include the 'state' in state_dict.
 
@@ -939,26 +900,24 @@
                 if (group_id + 1) * len(pg) < param_idx:
                     continue
                 master_param = pg[param_idx - (group_id) * len(pg)]
                 working_param = self._param_store.master_to_working_param[id(master_param)]
 
             for k, v in states.items():
                 if isinstance(v, torch.Tensor) and k != "step":
-                    if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(v):
+                    if self.moe_extra_dp_pg is not None and is_moe_tensor(v):
                         state_tensor = [
-                            torch.zeros(v.shape, device=device, dtype=v.dtype)
-                            for _ in range(self._bucket_store.moe_extra_dp_pg_size)
+                            torch.zeros(v.shape, device=device, dtype=v.dtype) for _ in range(self.moe_extra_dp_pg_size)
                         ]
-                        dist.all_gather(state_tensor, v.to(device), group=self._bucket_store.moe_extra_dp_pg)
+                        dist.all_gather(state_tensor, v.to(device), group=self.moe_extra_dp_pg)
                     else:
                         state_tensor = [
-                            torch.zeros(v.shape, device=device, dtype=v.dtype)
-                            for _ in range(self._bucket_store.zero_world_size)
+                            torch.zeros(v.shape, device=device, dtype=v.dtype) for _ in range(self._world_size)
                         ]
-                        dist.all_gather(state_tensor, v.to(device), group=self._bucket_store.torch_pg)
+                        dist.all_gather(state_tensor, v.to(device), group=self.dp_pg)
                     state_tensor = (
                         torch.stack(state_tensor).view(-1)[: working_param.numel()].reshape_as(working_param).cpu()
                     )
                     current_block_size += state_tensor.numel()
                     current_block[k] = state_tensor
 
             if ret_block_size + current_block_size > max_shard_size and len(ret_block) > 0:
@@ -981,38 +940,22 @@
             p_id = id(p)
             if p_id in self._param_store.working_to_master_param:
                 master_param = self._param_store.working_to_master_param[p_id]
                 padding_size = self._param_store.get_param_padding_size(p)
                 working_param = p.data.view(-1)
                 if padding_size > 0:
                     working_param = torch.nn.functional.pad(working_param, [0, padding_size])
-                if self._bucket_store.moe_extra_dp_pg is not None and is_moe_tensor(p):
+                if self.moe_extra_dp_pg is not None and is_moe_tensor(p):
                     master_param.copy_(working_param.chunk(self.extra_dp_pg_size)[self.extra_dp_pg_rank])
                 else:
-                    master_param.copy_(
-                        working_param.chunk(self._bucket_store.zero_world_size)[self._bucket_store.zero_local_rank]
-                    )
+                    master_param.copy_(working_param.chunk(self._world_size)[self._local_rank])
         if hasattr(self, "master_moe_params"):
             for master_moe_param, working_moe_param in zip(self.master_moe_params, self.working_moe_params):
                 master_moe_param.copy_(working_moe_param)
 
-    def remove_hooks(self) -> None:
-        """remove the registered hooks
-
-        Args:
-            plugin (LowLevelZeroPlugin): the plugin to bound this method.
-        """
-        for group_id in range(self.num_param_groups):
-            param_group = self._working_param_groups[group_id]
-            for param in param_group:
-                if param.requires_grad:
-                    assert hasattr(param, "_grad_handle")
-                    param._grad_handle.remove()
-                    delattr(param, "_grad_handle")
-
     def get_working_to_master_map(self) -> Dict[int, torch.Tensor]:
         return self._param_store.working_to_master_param
 
     def get_master_to_working_map(self) -> Dict[int, torch.Tensor]:
         if hasattr(self, "moe_master_to_working_map"):
             return {
                 **self._param_store.master_to_working_param,
```

### Comparing `colossalai-nightly-2024.5.11/colossalai/zero/wrapper.py` & `colossalai-nightly-2024.5.4/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2024.5.11
+Version: 2024.5.4
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2024.5.11 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2024.5.4 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2024.5.11/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2024.5.4/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -688,15 +688,14 @@
 colossalai/shardformer/modeling/falcon.py
 colossalai/shardformer/modeling/gpt2.py
 colossalai/shardformer/modeling/gptj.py
 colossalai/shardformer/modeling/jit.py
 colossalai/shardformer/modeling/llama.py
 colossalai/shardformer/modeling/mistral.py
 colossalai/shardformer/modeling/opt.py
-colossalai/shardformer/modeling/qwen2.py
 colossalai/shardformer/modeling/sam.py
 colossalai/shardformer/modeling/t5.py
 colossalai/shardformer/modeling/vit.py
 colossalai/shardformer/modeling/whisper.py
 colossalai/shardformer/modeling/chatglm2_6b/__init__.py
 colossalai/shardformer/modeling/chatglm2_6b/configuration_chatglm.py
 colossalai/shardformer/modeling/chatglm2_6b/modeling_chatglm.py
@@ -709,15 +708,14 @@
 colossalai/shardformer/policies/chatglm2.py
 colossalai/shardformer/policies/falcon.py
 colossalai/shardformer/policies/gpt2.py
 colossalai/shardformer/policies/gptj.py
 colossalai/shardformer/policies/llama.py
 colossalai/shardformer/policies/mistral.py
 colossalai/shardformer/policies/opt.py
-colossalai/shardformer/policies/qwen2.py
 colossalai/shardformer/policies/sam.py
 colossalai/shardformer/policies/t5.py
 colossalai/shardformer/policies/vit.py
 colossalai/shardformer/policies/whisper.py
 colossalai/shardformer/shard/__init__.py
 colossalai/shardformer/shard/grad_ckpt_config.py
 colossalai/shardformer/shard/shard_config.py
@@ -883,15 +881,14 @@
 tests/kit/model_zoo/transformers/chatglm2.py
 tests/kit/model_zoo/transformers/falcon.py
 tests/kit/model_zoo/transformers/gpt.py
 tests/kit/model_zoo/transformers/gptj.py
 tests/kit/model_zoo/transformers/llama.py
 tests/kit/model_zoo/transformers/mistral.py
 tests/kit/model_zoo/transformers/opt.py
-tests/kit/model_zoo/transformers/qwen2.py
 tests/kit/model_zoo/transformers/sam.py
 tests/kit/model_zoo/transformers/t5.py
 tests/kit/model_zoo/transformers/vit.py
 tests/kit/model_zoo/transformers/whisper.py
 tests/test_analyzer/__init__.py
 tests/test_analyzer/test_fx/__init__.py
 tests/test_analyzer/test_fx/test_bias_addition.py
@@ -962,12 +959,11 @@
 tests/test_shardformer/test_model/test_shard_chatglm2.py
 tests/test_shardformer/test_model/test_shard_falcon.py
 tests/test_shardformer/test_model/test_shard_gpt2.py
 tests/test_shardformer/test_model/test_shard_gptj.py
 tests/test_shardformer/test_model/test_shard_llama.py
 tests/test_shardformer/test_model/test_shard_mistral.py
 tests/test_shardformer/test_model/test_shard_opt.py
-tests/test_shardformer/test_model/test_shard_qwen2.py
 tests/test_shardformer/test_model/test_shard_sam.py
 tests/test_shardformer/test_model/test_shard_t5.py
 tests/test_shardformer/test_model/test_shard_vit.py
 tests/test_shardformer/test_model/test_shard_whisper.py
```

### Comparing `colossalai-nightly-2024.5.11/examples/language/data_utils.py` & `colossalai-nightly-2024.5.4/examples/language/data_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/examples/language/model_utils.py` & `colossalai-nightly-2024.5.4/examples/language/model_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/examples/language/performance_evaluator.py` & `colossalai-nightly-2024.5.4/examples/language/performance_evaluator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/__init__.py` & `colossalai-nightly-2024.5.4/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/base_extension.py` & `colossalai-nightly-2024.5.4/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/cpp_extension.py` & `colossalai-nightly-2024.5.4/extensions/cpp_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/cpu_adam/cpu_adam_arm.py` & `colossalai-nightly-2024.5.4/extensions/cpu_adam/cpu_adam_arm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/cpu_adam/cpu_adam_x86.py` & `colossalai-nightly-2024.5.4/extensions/cpu_adam/cpu_adam_x86.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/arm/cpu_adam_arm.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/arm/cpu_adam_arm.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/arm/cpu_adam_arm.h` & `colossalai-nightly-2024.5.4/extensions/csrc/arm/cpu_adam_arm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/colossal_C_frontend.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/cpu_adam.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/cpu_adam.h` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/include/block_reduce.h` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/layer_norm_cuda.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/moe_cuda.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/moe_cuda_kernel.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_adam.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_apply.cuh` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_lamb.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_masked_softmax.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_masked_softmax.h` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/cuda/type_shim.h` & `colossalai-nightly-2024.5.4/extensions/csrc/cuda/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/csrc/scaled_softmax.py` & `colossalai-nightly-2024.5.4/extensions/csrc/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/cuda_extension.py` & `colossalai-nightly-2024.5.4/extensions/cuda_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/flash_attention/flash_attention_dao_cuda.py` & `colossalai-nightly-2024.5.4/extensions/flash_attention/flash_attention_dao_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/flash_attention/flash_attention_npu.py` & `colossalai-nightly-2024.5.4/extensions/flash_attention/flash_attention_npu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/flash_attention/flash_attention_sdpa_cuda.py` & `colossalai-nightly-2024.5.4/extensions/flash_attention/flash_attention_sdpa_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/layernorm/layernorm_cuda.py` & `colossalai-nightly-2024.5.4/extensions/layernorm/layernorm_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/moe/moe_cuda.py` & `colossalai-nightly-2024.5.4/extensions/moe/moe_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/optimizer/fused_optimizer_cuda.py` & `colossalai-nightly-2024.5.4/extensions/optimizer/fused_optimizer_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/softmax/scaled_masked_softmax_cuda.py` & `colossalai-nightly-2024.5.4/extensions/softmax/scaled_masked_softmax_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py` & `colossalai-nightly-2024.5.4/extensions/softmax/scaled_upper_triangle_masked_softmax_cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/triton_extension.py` & `colossalai-nightly-2024.5.4/extensions/triton_extension.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/extensions/utils.py` & `colossalai-nightly-2024.5.4/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/requirements/requirements-test.txt` & `colossalai-nightly-2024.5.4/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/setup.py` & `colossalai-nightly-2024.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         raise RuntimeError("[extension] Could not find any kernel compatible with the current environment.")
     else:
         op_name_list = ", ".join(op_names)
         print(f"[extension] Building extensions{op_name_list}")
 else:
     ext_modules = []
 
-version = "2024.05.11"
+version = "2024.05.04"
 package_name = "colossalai-nightly"
 
 setup(
     name=package_name,
     version=version,
     packages=find_packages(
         exclude=(
```

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/__init__.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/base.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/hanging_param_model.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/nested_model.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/repeated_computed_layers.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/custom/simple_net.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/custom/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/executor.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/blip2.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/blip2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/bloom.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/chatglm2.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/falcon.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/falcon.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/gptj.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/gptj.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/llama.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/mistral.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/mistral.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/qwen2.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/vit.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,70 @@
 import torch
 import transformers
 
 from ..registry import ModelAttribute, model_zoo
 
-try:
-    from transformers import Qwen2Config
-
-    HAS_QWEN2 = True
-except ImportError:
-    HAS_QWEN2 = False
-
-if HAS_QWEN2:
-    # ===============================
-    # Register Qwen2
-    # ===============================
-
-    def data_gen():
-        # the input ids are corresponding to the sentence
-        # 'Hello, my dog is cute'
-        #
-        # the code is give below:
-        # -----------------------------------
-        # from transformers import Qwen2TokenizerFast
-        # tokenizer = Qwen2TokenizerFast.from_pretrained("Qwen/Qwen1.5-7B-Chat")
-        # input = 'Hello, my dog is cute'
-        # tokenized_input = tokenizer(input, return_tensors='pt').to('cuda')
-        # -----------------------------------
-
-        input_ids = torch.Tensor(
-            [[9707, 11, 847, 5562, 374, 13, 123, 18838], [9707, 11, 847, 5562, 374, 17, 89, 18838]]
-        ).long()
-        attention_mask = torch.Tensor([[1, 1, 1, 1, 1, 1, 1, 1], [1, 1, 1, 1, 1, 1, 1, 1]]).long()
-        return dict(input_ids=input_ids, attention_mask=attention_mask)
-
-    # label is needed for casual lm
-    def data_gen_for_casual_lm():
-        data = data_gen()
-        labels = data["input_ids"].clone()
-        data["labels"] = labels
-        return data
-
-    # transform the output to a dict
-    output_transform_fn = lambda x: x
-
-    # function to get the loss
-    loss_fn = lambda output: output["last_hidden_state"].mean()
-    loss_fn_for_casual_lm = lambda output: output["loss"]
-    loss_fn_for_seq_classification = lambda output: output["logits"].mean()
-
-    config = Qwen2Config(
-        hidden_size=128,
-        intermediate_size=256,
-        max_window_layers=4,
-        num_attention_heads=16,
-        num_hidden_layers=4,
-        num_key_value_heads=16,
-    )
-
-    config.pad_token_id = 0
-
-    # register the following models
-    # transformers.Qwen2Model,
-    # transformers.Qwen2ForCausalLM,
-    # transformers.Qwen2ForSequenceClassification,
-    model_zoo.register(
-        name="transformers_qwen2",
-        model_fn=lambda: transformers.Qwen2Model(config),
-        data_gen_fn=data_gen,
-        output_transform_fn=output_transform_fn,
-        loss_fn=loss_fn,
-        model_attribute=ModelAttribute(has_control_flow=True),
-    )
-    model_zoo.register(
-        name="transformers_qwen2_for_casual_lm",
-        model_fn=lambda: transformers.Qwen2ForCausalLM(config),
-        data_gen_fn=data_gen_for_casual_lm,
-        output_transform_fn=output_transform_fn,
-        loss_fn=loss_fn_for_casual_lm,
-        model_attribute=ModelAttribute(has_control_flow=True),
-    )
-    model_zoo.register(
-        name="transformers_qwen2_for_sequence_classification",
-        model_fn=lambda: transformers.Qwen2ForSequenceClassification(config),
-        data_gen_fn=data_gen,
-        output_transform_fn=output_transform_fn,
-        loss_fn=loss_fn_for_seq_classification,
-        model_attribute=ModelAttribute(has_control_flow=True),
-    )
+# ===============================
+# Register single-sentence VIT
+# ===============================
+
+config = transformers.ViTConfig(num_hidden_layers=4, hidden_size=128, intermediate_size=256, num_attention_heads=4)
+
+
+# define data gen function
+def data_gen():
+    pixel_values = torch.randn(1, 3, 224, 224)
+    return dict(pixel_values=pixel_values)
+
+
+def data_gen_for_image_classification():
+    data = data_gen()
+    data["labels"] = torch.tensor([0])
+    return data
+
+
+def data_gen_for_masked_image_modeling():
+    data = data_gen()
+    num_patches = (config.image_size // config.patch_size) ** 2
+    bool_masked_pos = torch.randint(low=0, high=2, size=(1, num_patches)).bool()
+    data["bool_masked_pos"] = bool_masked_pos
+    return data
+
+
+# define output transform function
+output_transform_fn = lambda x: x
+
+# function to get the loss
+loss_fn_for_vit_model = lambda x: x["pooler_output"].mean()
+loss_fn_for_image_classification = lambda x: x["logits"].mean()
+loss_fn_for_masked_image_modeling = lambda x: x["loss"]
+
+# register the following models
+# transformers.ViTModel,
+# transformers.ViTForMaskedImageModeling,
+# transformers.ViTForImageClassification,
+model_zoo.register(
+    name="transformers_vit",
+    model_fn=lambda: transformers.ViTModel(config),
+    data_gen_fn=data_gen,
+    output_transform_fn=output_transform_fn,
+    loss_fn=loss_fn_for_vit_model,
+    model_attribute=ModelAttribute(has_control_flow=True),
+)
+
+model_zoo.register(
+    name="transformers_vit_for_masked_image_modeling",
+    model_fn=lambda: transformers.ViTForMaskedImageModeling(config),
+    data_gen_fn=data_gen_for_masked_image_modeling,
+    output_transform_fn=output_transform_fn,
+    loss_fn=loss_fn_for_masked_image_modeling,
+    model_attribute=ModelAttribute(has_control_flow=True),
+)
+
+model_zoo.register(
+    name="transformers_vit_for_image_classification",
+    model_fn=lambda: transformers.ViTForImageClassification(config),
+    data_gen_fn=data_gen_for_image_classification,
+    output_transform_fn=output_transform_fn,
+    loss_fn=loss_fn_for_image_classification,
+    model_attribute=ModelAttribute(has_control_flow=True),
+)
```

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/sam.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/sam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/kit/model_zoo/transformers/whisper.py` & `colossalai-nightly-2024.5.4/tests/kit/model_zoo/transformers/whisper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2024.5.4/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2024.5.4/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_flash_attention.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/_utils.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_bert.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_blip2.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_blip2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_bloom.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_chatglm2.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_chatglm2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_falcon.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_falcon.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_gpt2.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_gptj.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_gptj.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_llama.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,15 @@
         booster.plugin.zero_stage in [1, 2]
         and booster.plugin.shard_config.enable_sequence_parallelism
         and booster.plugin.shard_config.sequence_parallelism_mode == "all_to_all"
     ):
         for p1, p2 in zip(llama_model.parameters(), sharded_optimizer._master_param_groups_of_current_rank[0]):
             working_p = sharded_optimizer._param_store.master_to_working_param[id(p2)]
             grads = sharded_optimizer._grad_store.get_partitioned_gradients_by_param_id(0, id(working_p))
-            grad_index = (
-                0 if sharded_optimizer._grad_store._partition_grads else sharded_optimizer._bucket_store.zero_local_rank
-            )
+            grad_index = 0 if sharded_optimizer._partition_grads else sharded_optimizer._local_rank
             grad = grads[grad_index]
             sharded_grad = p1.grad.view(-1).chunk(dist.get_world_size())[dist.get_rank()]
             assert_close(sharded_grad, grad[: sharded_grad.shape[0]], atol=5e-3, rtol=5e-3, check_dtype=False)
 
     # Save gradient tensors for comparison between the original model and the sharded model before optimizer step.
     grads_to_check = {}
     if (stage_manager is None or stage_manager.is_first_stage(ignore_chunk=True)) and booster.plugin.zero_stage == 0:
```

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_mistral.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_mistral.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_opt.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_qwen2.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_t5.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
-
 import pytest
 import torch
-import transformers
 
 import colossalai
 from colossalai.logging import disable_existing_loggers
 from colossalai.shardformer.layer.utils import Randomizer
 from colossalai.tensor.d_tensor.api import clear_layout_converter
 from colossalai.testing import clear_cache_before_run, parameterize, rerun_if_address_is_in_use, spawn
 from tests.kit.model_zoo import model_zoo
@@ -17,76 +14,83 @@
     check_output_hidden_state,
     check_weight,
     get_grad_tensors_for_check,
     run_forward_backward_with_hybrid_plugin,
     unwrap_model,
 )
 
-os.environ["TRANSFORMERS_NO_ADVISORY_WARNINGS"] = "true"
-
 
 def check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config):
     org_model, org_optimizer, sharded_model, sharded_optimizer, criterion, booster = build_model_from_hybrid_plugin(
         model_fn, loss_fn, test_config
     )
 
     org_loss, org_output, sharded_loss, sharded_output = run_forward_backward_with_hybrid_plugin(
-        org_model, sharded_model, sharded_optimizer, data_gen_fn, output_transform_fn, criterion, booster
+        org_model,
+        sharded_model,
+        sharded_optimizer,
+        data_gen_fn,
+        output_transform_fn,
+        criterion,
+        booster,
     )
 
     stage_manager = booster.plugin.stage_manager
     tp_group = booster.plugin.tp_group
 
     # unwrap model
-    qwen2_model = unwrap_model(org_model, "Qwen2Model", "model")
-    shard_qwen2_model = unwrap_model(sharded_model, "Qwen2Model", "model")
+    t5 = unwrap_model(org_model)
+    sharded_t5 = unwrap_model(sharded_model)
 
-    row_layer_for_check = ["layers[0].self_attn.q_proj", "embed_tokens"]
-    col_layer_for_check = ["layers[0].self_attn.o_proj"]
+    row_layer_for_check = ["shared", "encoder.block[0].layer[0].SelfAttention.q"]
 
     # Save gradient tensors for comparison between the original model and the sharded model before optimizer step.
     grads_to_check = {}
-    if (stage_manager is None or stage_manager.is_first_stage(ignore_chunk=True)) and booster.plugin.zero_stage == 0:
-        if test_config["precision"] == "fp32":
-            atol, rtol = 1e-6, 1e-4
-        else:
-            atol, rtol = 5e-3, 5e-3
+    if test_config["precision"] == "fp32":
+        atol, rtol = 1e-5, 1e-3
+    else:
+        atol, rtol = 5e-3, 5e-3
+    if (stage_manager is None or stage_manager.is_first_stage()) and booster.plugin.zero_stage == 0:
         row_layer_grads = get_grad_tensors_for_check(
-            qwen2_model, shard_qwen2_model, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0, verbose=False
-        )
-        col_layer_grads = get_grad_tensors_for_check(
-            qwen2_model, shard_qwen2_model, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
+            t5, sharded_t5, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0
         )
-        grads_to_check.update(col_layer_grads)
         grads_to_check.update(row_layer_grads)
 
     # optimizer executes step
     org_optimizer.step()
     sharded_optimizer.step()
 
     # check last hidden state & loss
-    if stage_manager is None or stage_manager.is_last_stage(ignore_chunk=True):
+    if stage_manager is None or stage_manager.is_last_stage():
         if test_config["precision"] == "fp32":
             atol, rtol = 1e-5, 1e-3
         else:
             atol, rtol = 5e-3, 5e-3
 
-        if org_model.__class__.__name__ == "Qwen2Model":
+        if org_model.__class__.__name__ != "T5ForConditionalGeneration":
             check_output_hidden_state(org_output, sharded_output, stage_manager, atol=atol, rtol=rtol)
 
         check_loss(org_loss, sharded_loss, atol=atol, rtol=rtol)
 
     # check weights
-    if stage_manager is None or stage_manager.is_first_stage(ignore_chunk=True):
-        if test_config["precision"] == "fp32":
-            atol, rtol = 1e-4, 1e-3
-        else:
-            atol, rtol = 5e-3, 5e-3
+    if test_config["precision"] == "fp32":
+        # TODO he precision in weight checking is too significant.
+        atol, rtol = 1e-3, 1e-3
+    else:
+        atol, rtol = 5e-3, 5e-3
+    if stage_manager is None or stage_manager.is_first_stage():
         check_weight(
-            qwen2_model, shard_qwen2_model, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
+            t5,
+            sharded_t5,
+            row_layer_for_check,
+            tp_group,
+            atol=atol,
+            rtol=rtol,
+            dim=0,
+            verbose=False,
         )
 
     # check grads
     check_all_grad_tensors(grads_to_check)
 
     torch.cuda.empty_cache()
 
@@ -94,142 +98,165 @@
 @parameterize(
     "test_config",
     [
         {
             "tp_size": 2,
             "pp_size": 2,
             "num_microbatches": 2,
+            "enable_metadata_cache": False,
             "enable_all_optimization": True,
             "use_lazy_init": True,
             "precision": "fp16",
             "initial_scale": 1,
         },
         {
             "tp_size": 1,
             "pp_size": 2,
             "num_microbatches": 4,
+            "enable_metadata_cache": False,
             "use_lazy_init": False,
-            "precision": "fp32",
+            "precision": "fp16",
+            "initial_scale": 1,
         },
         {
             "tp_size": 4,
             "pp_size": 1,
-            "enable_all_optimization": True,
+            "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp32",
         },
         {
             "tp_size": 1,
             "pp_size": 4,
             "num_microbatches": 4,
+            "enable_metadata_cache": False,
             "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp32",
         },
-        {"tp_size": 2, "pp_size": 1, "enable_all_optimization": True, "use_lazy_init": False, "precision": "fp32"},
         {
             "tp_size": 2,
             "pp_size": 1,
             "enable_all_optimization": True,
             "use_lazy_init": True,
             "zero_stage": 2,
             "precision": "fp16",
             "initial_scale": 1,
         },
         {
             "tp_size": 1,
             "pp_size": 2,
             "num_microbatches": 2,
+            "enable_metadata_cache": False,
             "enable_all_optimization": True,
             "use_lazy_init": True,
             "zero_stage": 1,
             "precision": "fp16",
             "initial_scale": 1,
         },
     ],
 )
-def run_qwen2_test(test_config):
-    sub_model_zoo = model_zoo.get_sub_registry("transformers_qwen2")
+@clear_cache_before_run()
+def run_t5_test(test_config):
+    sub_model_zoo = model_zoo.get_sub_registry("transformers_t5")
+
+    for name, (
+        model_fn,
+        data_gen_fn,
+        output_transform_fn,
+        loss_fn,
+        _,
+    ) in sub_model_zoo.items():
+        # skip 4-stage pp test for t5_encoder
+        if test_config["pp_size"] > 2 and name == "transformers_t5_encoder_model":
+            continue
 
-    for name, (model_fn, data_gen_fn, output_transform_fn, loss_fn, _) in sub_model_zoo.items():
         check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config)
 
     clear_layout_converter()
     Randomizer.reset_index()
     torch.cuda.empty_cache()
 
 
 @parameterize(
     "test_config",
     [
         {
             "tp_size": 2,
             "pp_size": 2,
             "num_microbatches": 4,
+            "enable_metadata_cache": False,
             "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp32",
             "initial_scale": 1,
         },
         {
             "tp_size": 2,
             "pp_size": 2,
             "num_microbatches": 4,
+            "enable_metadata_cache": False,
             "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp16",
             "zero_stage": 1,
             "initial_scale": 1,
         },
-        {
-            "tp_size": 2,
-            "pp_size": 2,
-            "pp_style": "interleaved",
-            "num_model_chunks": 2,
-            "num_microbatches": 4,
-            "enable_all_optimization": False,
-            "precision": "fp16",
-            "zero_stage": 1,
-            "initial_scale": 1,
-        },
     ],
 )
-def run_qwen2_3d_test(test_config):
-    sub_model_zoo = model_zoo.get_sub_registry("transformers_qwen2")
+def run_t5_3d_test(test_config):
+    sub_model_zoo = model_zoo.get_sub_registry("transformers_t5")
 
-    for name, (model_fn, data_gen_fn, output_transform_fn, loss_fn, _) in sub_model_zoo.items():
+    for name, (
+        model_fn,
+        data_gen_fn,
+        output_transform_fn,
+        loss_fn,
+        _,
+    ) in sub_model_zoo.items():
         check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config)
 
     clear_layout_converter()
-    Randomizer.reset_index()
     torch.cuda.empty_cache()
 
 
-def check_qwen2(rank, world_size, port):
+def check_t5(rank, world_size, port):
     disable_existing_loggers()
-    colossalai.launch(rank=rank, world_size=world_size, host="localhost", port=port, backend="nccl")
-    run_qwen2_test()
+    colossalai.launch(
+        rank=rank,
+        world_size=world_size,
+        host="localhost",
+        port=port,
+        backend="nccl",
+    )
+    run_t5_test()
 
 
-def check_qwen2_3d(rank, world_size, port):
+def check_t5_3d(rank, world_size, port):
     disable_existing_loggers()
-    colossalai.launch(rank=rank, world_size=world_size, host="localhost", port=port, backend="nccl")
-    run_qwen2_3d_test()
+    colossalai.launch(
+        rank=rank,
+        world_size=world_size,
+        host="localhost",
+        port=port,
+        backend="nccl",
+    )
+    run_t5_3d_test()
 
 
-@pytest.mark.skipif(transformers.__version__ < "4.39.1", reason="Requires transformers version 4.39.1 or later")
+@pytest.mark.dist
 @rerun_if_address_is_in_use()
 @clear_cache_before_run()
-def test_qwen2():
-    spawn(check_qwen2, 4)
+def test_t5():
+    spawn(check_t5, 4)
 
 
-@pytest.mark.skipif(transformers.__version__ < "4.39.1", reason="Requires transformers version 4.39.1 or later")
+@pytest.mark.largedist
 @rerun_if_address_is_in_use()
 @clear_cache_before_run()
-def test_qwen2_3d():
-    spawn(check_qwen2_3d, 8)
+def test_t5_3d():
+    spawn(check_t5_3d, 8)
 
 
 if __name__ == "__main__":
-    test_qwen2()
-    test_qwen2_3d()
+    test_t5()
+    test_t5_3d()
```

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_sam.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_sam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_t5.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_vit.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,242 +21,177 @@
 
 def check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config):
     org_model, org_optimizer, sharded_model, sharded_optimizer, criterion, booster = build_model_from_hybrid_plugin(
         model_fn, loss_fn, test_config
     )
 
     org_loss, org_output, sharded_loss, sharded_output = run_forward_backward_with_hybrid_plugin(
-        org_model,
-        sharded_model,
-        sharded_optimizer,
-        data_gen_fn,
-        output_transform_fn,
-        criterion,
-        booster,
+        org_model, sharded_model, sharded_optimizer, data_gen_fn, output_transform_fn, criterion, booster
     )
 
     stage_manager = booster.plugin.stage_manager
     tp_group = booster.plugin.tp_group
 
     # unwrap model
-    t5 = unwrap_model(org_model)
-    sharded_t5 = unwrap_model(sharded_model)
+    vit_model = unwrap_model(org_model, "ViTModel", "vit")
+    shard_vit_model = unwrap_model(sharded_model, "ViTModel", "vit")
 
-    row_layer_for_check = ["shared", "encoder.block[0].layer[0].SelfAttention.q"]
+    # check grad
+    row_layer_for_check = ["encoder.layer[0].attention.attention.query", "embeddings.patch_embeddings.projection"]
+    col_layer_for_check = ["encoder.layer[0].attention.output.dense"]
 
     # Save gradient tensors for comparison between the original model and the sharded model before optimizer step.
     grads_to_check = {}
-    if test_config["precision"] == "fp32":
-        atol, rtol = 1e-5, 1e-3
-    else:
-        atol, rtol = 5e-3, 5e-3
     if (stage_manager is None or stage_manager.is_first_stage()) and booster.plugin.zero_stage == 0:
+        if test_config["precision"] == "fp32":
+            atol, rtol = 2e-5, 1e-3
+        else:
+            atol, rtol = 5e-3, 5e-3
         row_layer_grads = get_grad_tensors_for_check(
-            t5, sharded_t5, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0
+            vit_model, shard_vit_model, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0, verbose=False
         )
+        col_layer_grads = get_grad_tensors_for_check(
+            vit_model, shard_vit_model, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
+        )
+        grads_to_check.update(col_layer_grads)
         grads_to_check.update(row_layer_grads)
 
     # optimizer executes step
     org_optimizer.step()
     sharded_optimizer.step()
 
     # check last hidden state & loss
     if stage_manager is None or stage_manager.is_last_stage():
         if test_config["precision"] == "fp32":
-            atol, rtol = 1e-5, 1e-3
+            atol, rtol = 2e-3, 1e-3
         else:
             atol, rtol = 5e-3, 5e-3
 
-        if org_model.__class__.__name__ != "T5ForConditionalGeneration":
+        if org_model.__class__.__name__ == "ViTModel":
             check_output_hidden_state(org_output, sharded_output, stage_manager, atol=atol, rtol=rtol)
-
         check_loss(org_loss, sharded_loss, atol=atol, rtol=rtol)
 
     # check weights
-    if test_config["precision"] == "fp32":
-        # TODO he precision in weight checking is too significant.
-        atol, rtol = 1e-3, 1e-3
-    else:
-        atol, rtol = 5e-3, 5e-3
     if stage_manager is None or stage_manager.is_first_stage():
+        if test_config["precision"] == "fp32":
+            atol, rtol = 5e-3, 1e-3
+        else:
+            atol, rtol = 5e-3, 5e-3
         check_weight(
-            t5,
-            sharded_t5,
-            row_layer_for_check,
-            tp_group,
-            atol=atol,
-            rtol=rtol,
-            dim=0,
-            verbose=False,
+            vit_model, shard_vit_model, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
         )
 
     # check grads
     check_all_grad_tensors(grads_to_check)
 
     torch.cuda.empty_cache()
 
 
+# TODO: num_microbatch size = 2 inf loss
 @parameterize(
     "test_config",
     [
         {
             "tp_size": 2,
             "pp_size": 2,
-            "num_microbatches": 2,
-            "enable_metadata_cache": False,
-            "enable_all_optimization": True,
-            "use_lazy_init": True,
-            "precision": "fp16",
-            "initial_scale": 1,
-        },
-        {
-            "tp_size": 1,
-            "pp_size": 2,
             "num_microbatches": 4,
-            "enable_metadata_cache": False,
+            "enable_all_optimization": True,
             "use_lazy_init": False,
             "precision": "fp16",
             "initial_scale": 1,
         },
         {
-            "tp_size": 4,
-            "pp_size": 1,
-            "enable_all_optimization": False,
-            "use_lazy_init": False,
-            "precision": "fp32",
-        },
-        {
             "tp_size": 1,
-            "pp_size": 4,
+            "pp_size": 2,
             "num_microbatches": 4,
-            "enable_metadata_cache": False,
             "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp32",
         },
+        {"tp_size": 4, "pp_size": 1, "enable_all_optimization": True, "use_lazy_init": False, "precision": "fp32"},
+        {"tp_size": 2, "pp_size": 1, "enable_all_optimization": True, "use_lazy_init": False, "precision": "fp32"},
         {
             "tp_size": 2,
             "pp_size": 1,
             "enable_all_optimization": True,
-            "use_lazy_init": True,
+            "use_lazy_init": False,
             "zero_stage": 2,
             "precision": "fp16",
             "initial_scale": 1,
         },
         {
             "tp_size": 1,
             "pp_size": 2,
-            "num_microbatches": 2,
-            "enable_metadata_cache": False,
+            "num_microbatches": 4,
             "enable_all_optimization": True,
-            "use_lazy_init": True,
+            "use_lazy_init": False,
             "zero_stage": 1,
             "precision": "fp16",
             "initial_scale": 1,
         },
     ],
 )
-@clear_cache_before_run()
-def run_t5_test(test_config):
-    sub_model_zoo = model_zoo.get_sub_registry("transformers_t5")
-
-    for name, (
-        model_fn,
-        data_gen_fn,
-        output_transform_fn,
-        loss_fn,
-        _,
-    ) in sub_model_zoo.items():
-        # skip 4-stage pp test for t5_encoder
-        if test_config["pp_size"] > 2 and name == "transformers_t5_encoder_model":
-            continue
+def run_vit_test(test_config):
+    # TODO: fix bug when settign lazy_init for Conv2D Layers in ViT models
 
+    sub_model_zoo = model_zoo.get_sub_registry("transformers_vit")
+    for name, (model_fn, data_gen_fn, output_transform_fn, loss_fn, _) in sub_model_zoo.items():
         check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config)
 
     clear_layout_converter()
     Randomizer.reset_index()
     torch.cuda.empty_cache()
 
 
 @parameterize(
     "test_config",
     [
         {
             "tp_size": 2,
             "pp_size": 2,
             "num_microbatches": 4,
-            "enable_metadata_cache": False,
             "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp32",
             "initial_scale": 1,
         },
-        {
-            "tp_size": 2,
-            "pp_size": 2,
-            "num_microbatches": 4,
-            "enable_metadata_cache": False,
-            "enable_all_optimization": False,
-            "use_lazy_init": False,
-            "precision": "fp16",
-            "zero_stage": 1,
-            "initial_scale": 1,
-        },
     ],
 )
-def run_t5_3d_test(test_config):
-    sub_model_zoo = model_zoo.get_sub_registry("transformers_t5")
+def run_vit_3d_test(test_config):
+    sub_model_zoo = model_zoo.get_sub_registry("transformers_vit")
 
-    for name, (
-        model_fn,
-        data_gen_fn,
-        output_transform_fn,
-        loss_fn,
-        _,
-    ) in sub_model_zoo.items():
+    for name, (model_fn, data_gen_fn, output_transform_fn, loss_fn, _) in sub_model_zoo.items():
         check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config)
 
     clear_layout_converter()
     torch.cuda.empty_cache()
 
 
-def check_t5(rank, world_size, port):
+def check_vit(rank, world_size, port):
     disable_existing_loggers()
-    colossalai.launch(
-        rank=rank,
-        world_size=world_size,
-        host="localhost",
-        port=port,
-        backend="nccl",
-    )
-    run_t5_test()
+    colossalai.launch(rank=rank, world_size=world_size, host="localhost", port=port, backend="nccl")
+    run_vit_test()
 
 
-def check_t5_3d(rank, world_size, port):
+def check_vit_3d(rank, world_size, port):
     disable_existing_loggers()
-    colossalai.launch(
-        rank=rank,
-        world_size=world_size,
-        host="localhost",
-        port=port,
-        backend="nccl",
-    )
-    run_t5_3d_test()
+    colossalai.launch(rank=rank, world_size=world_size, host="localhost", port=port, backend="nccl")
+    run_vit_3d_test()
 
 
 @pytest.mark.dist
 @rerun_if_address_is_in_use()
 @clear_cache_before_run()
-def test_t5():
-    spawn(check_t5, 4)
+def test_vit():
+    spawn(check_vit, 4)
 
 
 @pytest.mark.largedist
 @rerun_if_address_is_in_use()
 @clear_cache_before_run()
-def test_t5_3d():
-    spawn(check_t5_3d, 8)
+def test_vit_3d():
+    spawn(check_vit_3d, 8)
 
 
 if __name__ == "__main__":
-    test_t5()
-    test_t5_3d()
+    test_vit()
+    test_vit_3d()
```

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_model/test_shard_vit.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_model/test_shard_whisper.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,187 +11,215 @@
     build_model_from_hybrid_plugin,
     check_all_grad_tensors,
     check_loss,
     check_output_hidden_state,
     check_weight,
     get_grad_tensors_for_check,
     run_forward_backward_with_hybrid_plugin,
-    unwrap_model,
 )
 
 
 def check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config):
+    # check forward
     org_model, org_optimizer, sharded_model, sharded_optimizer, criterion, booster = build_model_from_hybrid_plugin(
         model_fn, loss_fn, test_config
     )
 
     org_loss, org_output, sharded_loss, sharded_output = run_forward_backward_with_hybrid_plugin(
         org_model, sharded_model, sharded_optimizer, data_gen_fn, output_transform_fn, criterion, booster
     )
 
     stage_manager = booster.plugin.stage_manager
     tp_group = booster.plugin.tp_group
 
-    # unwrap model
-    vit_model = unwrap_model(org_model, "ViTModel", "vit")
-    shard_vit_model = unwrap_model(sharded_model, "ViTModel", "vit")
+    # unwarp the model
+    if org_model.__class__.__name__ == "WhisperForConditionalGeneration":
+        whisper = org_model.model
+        sharded_whisper = sharded_model.unwrap().model
+    else:
+        whisper = org_model
+        sharded_whisper = sharded_model.unwrap()
 
     # check grad
-    row_layer_for_check = ["encoder.layer[0].attention.attention.query", "embeddings.patch_embeddings.projection"]
-    col_layer_for_check = ["encoder.layer[0].attention.output.dense"]
+    if org_model.__class__.__name__ == "WhisperForAudioClassification":
+        col_layer_for_check = ["encoder.layers[0].self_attn.q_proj"]
+        row_layer_for_check = ["encoder.layers[0].self_attn.out_proj"]
+    else:
+        col_layer_for_check = [
+            "encoder.layers[0].self_attn.q_proj",
+            # 'decoder.layers[0].self_attn.q_proj'
+        ]
+        row_layer_for_check = [
+            "encoder.layers[0].self_attn.out_proj",
+            #'decoder.layers[0].self_attn.out_proj'
+        ]
 
     # Save gradient tensors for comparison between the original model and the sharded model before optimizer step.
     grads_to_check = {}
-    if (stage_manager is None or stage_manager.is_first_stage()) and booster.plugin.zero_stage == 0:
-        if test_config["precision"] == "fp32":
-            atol, rtol = 2e-5, 1e-3
-        else:
-            atol, rtol = 5e-3, 5e-3
+    if test_config["precision"] == "fp32":
+        atol, rtol = 2e-4, 2e-4
+    else:
+        atol, rtol = 5e-3, 5e-3
+
+    if stage_manager is None or stage_manager.is_first_stage():
         row_layer_grads = get_grad_tensors_for_check(
-            vit_model, shard_vit_model, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0, verbose=False
+            whisper, sharded_whisper, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1
         )
         col_layer_grads = get_grad_tensors_for_check(
-            vit_model, shard_vit_model, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
+            whisper, sharded_whisper, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0
         )
         grads_to_check.update(col_layer_grads)
         grads_to_check.update(row_layer_grads)
 
     # optimizer executes step
     org_optimizer.step()
     sharded_optimizer.step()
 
     # check last hidden state & loss
     if stage_manager is None or stage_manager.is_last_stage():
         if test_config["precision"] == "fp32":
-            atol, rtol = 2e-3, 1e-3
+            atol, rtol = 2e-4, 2e-4
         else:
             atol, rtol = 5e-3, 5e-3
 
-        if org_model.__class__.__name__ == "ViTModel":
+        if org_model.__class__.__name__ == "WhisperModel":
             check_output_hidden_state(org_output, sharded_output, stage_manager, atol=atol, rtol=rtol)
+
         check_loss(org_loss, sharded_loss, atol=atol, rtol=rtol)
 
     # check weights
+    if test_config["precision"] == "fp32":
+        atol, rtol = 1e-3, 1e-3
+    else:
+        atol, rtol = 5e-3, 5e-3
     if stage_manager is None or stage_manager.is_first_stage():
-        if test_config["precision"] == "fp32":
-            atol, rtol = 5e-3, 1e-3
-        else:
-            atol, rtol = 5e-3, 5e-3
         check_weight(
-            vit_model, shard_vit_model, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
+            whisper, sharded_whisper, row_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=1, verbose=False
+        )
+        check_weight(
+            whisper, sharded_whisper, col_layer_for_check, tp_group, atol=atol, rtol=rtol, dim=0, verbose=False
         )
 
     # check grads
     check_all_grad_tensors(grads_to_check)
 
     torch.cuda.empty_cache()
 
 
-# TODO: num_microbatch size = 2 inf loss
+# TODO fix WhisperForConditionalGeneration enable jit fused operato
+# TODO（jianghai) fix fp16
 @parameterize(
     "test_config",
     [
         {
             "tp_size": 2,
             "pp_size": 2,
-            "num_microbatches": 4,
+            "num_microbatches": 2,
+            "enable_metadata_cache": False,
             "enable_all_optimization": True,
             "use_lazy_init": False,
-            "precision": "fp16",
+            "precision": "fp32",
             "initial_scale": 1,
         },
         {
             "tp_size": 1,
             "pp_size": 2,
             "num_microbatches": 4,
-            "enable_all_optimization": False,
+            "enable_metadata_cache": False,
             "use_lazy_init": False,
             "precision": "fp32",
+            "initial_scale": 1,
         },
-        {"tp_size": 4, "pp_size": 1, "enable_all_optimization": True, "use_lazy_init": False, "precision": "fp32"},
-        {"tp_size": 2, "pp_size": 1, "enable_all_optimization": True, "use_lazy_init": False, "precision": "fp32"},
         {
-            "tp_size": 2,
+            "tp_size": 4,
             "pp_size": 1,
             "enable_all_optimization": True,
             "use_lazy_init": False,
-            "zero_stage": 2,
-            "precision": "fp16",
-            "initial_scale": 1,
+            "precision": "fp32",
         },
         {
             "tp_size": 1,
-            "pp_size": 2,
+            "pp_size": 4,
             "num_microbatches": 4,
-            "enable_all_optimization": True,
+            "enable_metadata_cache": False,
             "use_lazy_init": False,
-            "zero_stage": 1,
-            "precision": "fp16",
-            "initial_scale": 1,
+            "precision": "fp32",
         },
+        # whisper is not supported fp16 for now.
     ],
 )
-def run_vit_test(test_config):
-    # TODO: fix bug when settign lazy_init for Conv2D Layers in ViT models
-
-    sub_model_zoo = model_zoo.get_sub_registry("transformers_vit")
+def run_whisper_test(test_config):
+    sub_model_zoo = model_zoo.get_sub_registry("transformers_whisper")
     for name, (model_fn, data_gen_fn, output_transform_fn, loss_fn, _) in sub_model_zoo.items():
+        if test_config["pp_size"] > 2 and name == "transformers_whisper_for_audio_classification":
+            continue
         check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config)
 
     clear_layout_converter()
     Randomizer.reset_index()
     torch.cuda.empty_cache()
 
 
 @parameterize(
     "test_config",
     [
         {
             "tp_size": 2,
             "pp_size": 2,
             "num_microbatches": 4,
+            "enable_metadata_cache": False,
+            "enable_all_optimization": False,
+            "use_lazy_init": False,
+            "precision": "fp32",
+            "initial_scale": 1,
+        },
+        {
+            "tp_size": 2,
+            "pp_size": 2,
+            "num_microbatches": 2,
+            "enable_metadata_cache": False,
             "enable_all_optimization": False,
             "use_lazy_init": False,
             "precision": "fp32",
             "initial_scale": 1,
         },
     ],
 )
-def run_vit_3d_test(test_config):
-    sub_model_zoo = model_zoo.get_sub_registry("transformers_vit")
+def run_whisper_3d_test(test_config):
+    sub_model_zoo = model_zoo.get_sub_registry("transformers_whisper")
 
     for name, (model_fn, data_gen_fn, output_transform_fn, loss_fn, _) in sub_model_zoo.items():
         check_forward_backward(model_fn, data_gen_fn, output_transform_fn, loss_fn, test_config)
 
     clear_layout_converter()
     torch.cuda.empty_cache()
 
 
-def check_vit(rank, world_size, port):
+def check_whisper(rank, world_size, port):
     disable_existing_loggers()
     colossalai.launch(rank=rank, world_size=world_size, host="localhost", port=port, backend="nccl")
-    run_vit_test()
+    run_whisper_test()
 
 
-def check_vit_3d(rank, world_size, port):
+def check_whisper_3d(rank, world_size, port):
     disable_existing_loggers()
     colossalai.launch(rank=rank, world_size=world_size, host="localhost", port=port, backend="nccl")
-    run_vit_3d_test()
+    run_whisper_3d_test()
 
 
 @pytest.mark.dist
 @rerun_if_address_is_in_use()
 @clear_cache_before_run()
-def test_vit():
-    spawn(check_vit, 4)
+def test_whisper():
+    spawn(check_whisper, 4)
 
 
 @pytest.mark.largedist
 @rerun_if_address_is_in_use()
 @clear_cache_before_run()
-def test_vit_3d():
-    spawn(check_vit_3d, 8)
+def test_whisper_3d():
+    spawn(check_whisper_3d, 8)
 
 
 if __name__ == "__main__":
-    test_vit()
-    test_vit_3d()
+    test_whisper()
+    test_whisper_3d()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_shard_utils.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2024.5.11/tests/test_shardformer/test_with_torch_ddp.py` & `colossalai-nightly-2024.5.4/tests/test_shardformer/test_with_torch_ddp.py`

 * *Files identical despite different names*

