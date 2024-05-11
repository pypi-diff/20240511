# Comparing `tmp/onediff-1.0.0.dev202405090127.tar.gz` & `tmp/onediff-1.0.0.dev202405100127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.0.0.dev202405090127.tar", last modified: Thu May  9 01:27:21 2024, max compression
+gzip compressed data, was "onediff-1.0.0.dev202405100127.tar", last modified: Fri May 10 01:27:31 2024, max compression
```

## Comparing `onediff-1.0.0.dev202405090127.tar` & `onediff-1.0.0.dev202405100127.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.518631 onediff-1.0.0.dev202405090127/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.522631 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.522631 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.522631 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.522631 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.522631 onediff-1.0.0.dev202405090127/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-09 01:27:16.000000 onediff-1.0.0.dev202405090127/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.522631 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.526631 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/backends/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.526631 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.526631 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.526631 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/with_fx_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/with_fx_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-09 01:27:21.000000 onediff-1.0.0.dev202405090127/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-09 01:27:21.000000 onediff-1.0.0.dev202405090127/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:27:21.000000 onediff-1.0.0.dev202405090127/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 01:27:21.000000 onediff-1.0.0.dev202405090127/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 01:27:21.000000 onediff-1.0.0.dev202405090127/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:27:21.530631 onediff-1.0.0.dev202405090127/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-09 01:27:15.000000 onediff-1.0.0.dev202405090127/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.953646 onediff-1.0.0.dev202405100127/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.953646 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/backends/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.957646 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.961645 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.961645 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.961645 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/with_fx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/with_fx_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-10 01:27:31.000000 onediff-1.0.0.dev202405100127/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-10 01:27:31.000000 onediff-1.0.0.dev202405100127/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 01:27:31.000000 onediff-1.0.0.dev202405100127/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-10 01:27:31.000000 onediff-1.0.0.dev202405100127/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-10 01:27:31.000000 onediff-1.0.0.dev202405100127/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 01:27:31.965645 onediff-1.0.0.dev202405100127/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-10 01:27:26.000000 onediff-1.0.0.dev202405100127/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.0.0.dev202405090127/LICENSE` & `onediff-1.0.0.dev202405100127/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/PKG-INFO` & `onediff-1.0.0.dev202405100127/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405090127
+Version: 1.0.0.dev202405100127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -85,15 +85,15 @@
 <!-- toc -->
 - [About OneDiff](#about-onediff)
   - [Architecture](#architecture)
   - [State-of-the-art performance](#state-of-the-art-performance)
   - [Features](#features)
   - [Acceleration for State-of-the-art models](#acceleration-for-state-of-the-art-models)
   - [Acceleration for production environment](#acceleration-for-production-environment)
-  - [OneDiff Quality Evalution](#onediff-quality-evaluation)
+  - [OneDiff Quality Evaluation](#onediff-quality-evaluation)
   - [OneDiff Enterprise Edition](#onediff-enterprise-edition)
 - [Installation](#installation)
 - [Release](#release)
 <!-- tocstop -->
 
 ## About OneDiff
 ### Architecture
@@ -117,15 +117,15 @@
 
 <img src="imgs/0_12_svd.png" height="400">
 
 Note that we haven't got the way to run SVD with TensorRT on Feb 29 2024.
 
 ### Features
 
-| Main Function | Details |
+| Functionality | Details |
 |----------------|----------------------------|
 | Compiling Time   | About 1 minute (SDXL) |
 | Deployment Methods              | Plug and Play |
 | Dynamic Image Size Support  | Support with no overhead |
 | Model Support                 | SD1.5~2.1, SDXL, SDXL Turbo, etc. |
 | Algorithm Support             | SD standard workflow, LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. |
 | SD Framework Support | ComfyUI, Diffusers, SD-webui |
@@ -172,18 +172,18 @@
 ### OneDiff Quality Evaluation
 
 We also maintain a repository for benchmarking the quality of generation after acceleration using OneDiff:
 [OneDiffGenMetrics](https://github.com/siliconflow/OneDiffGenMetrics)
 
 ### OneDiff Enterprise Edition
 If you need **Enterprise-level Support** for your system or business, you can
-- subscribe to Enterprise Edition online and get all support after the order: https://siliconflow.com/onediff.html
-- or send an email to contact@siliconflow.com and tell us about your user case, deployment scale, and requirements.
+- Subscribe to the OneDiff Enterprise Edition directly through our website. Upon purchase, you'll gain immediate access to comprehensive support: https://siliconflow.com/onediff.html
+- For a more personalized approach, please email us at contact@siliconflow.com. Include details about your use case, deployment size, and any specific needs you might have.
 
-OneDiff Enterprise Edition can be **subscripted for one month and one GPU** and the cost is low.
+The OneDiff Enterprise Edition is available for a monthly subscription and is designed to be cost-effective, even for systems utilizing a **single GPU**.
 
 |                                                                                                           | OneDiff Enterprise Edition              | OneDiff Community Edition               |
 | --------------------------------------------------------------------------------------------------------- | --------------------------------------- | --------------------------------------- |
 | Multiple Resolutions                                                                                      | Yes(No time cost for most of the cases) | Yes(No time cost for most of the cases) |
 | More Extreme and Dedicated optimization(usually another 20~100% performance gain) for the most used model | Yes                                     |                                         |
 | Tools for specific(very large scale) server side deployment                                               | Yes                                     |                                         |
 | Technical Support for deployment                                                                          | High priority support                   | Community                               |
@@ -223,15 +223,15 @@
   python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-beijing.aliyuncs.com/branch/community/cu121
   ```
 
 
 - **CUDA 12.2**
 
   For NA/EU users
-  ```bash 
+  ```bash
   python3 -m pip install -U --pre oneflow -f https://github.com/siliconflow/oneflow_releases/releases/expanded_assets/community_cu122
   ```
   For CN users
   ```bash
   python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-beijing.aliyuncs.com/branch/community/cu122
   ```
 
@@ -259,45 +259,11 @@
 cd onediff && python3 -m pip install -e .
 ```
 
 > **_NOTE:_** If you intend to utilize plugins for ComfyUI/StableDiffusion-WebUI, we highly recommend installing OneDiff from the source rather than PyPI. This is necessary as you'll need to manually copy (or create a soft link) for the relevant code into the extension folder of these UIs/Libs.
 
 #### 4. (Optional)Login huggingface-cli
 
-```
+```bash
 python3 -m pip install huggingface_hub
- ~/.local/bin/huggingface-cli login
+huggingface-cli login
 ```
-
-## Release
-
-- run examples to check it works
-
-  ```bash
-  cd onediff_diffusers_extensions
-  python3 examples/text_to_image.py
-  ```
-
-- bump version in these files:
-
-  ```
-  .github/workflows/pub.yml
-  src/onediff/__init__.py
-  ```
-
-- install build package
-  ```bash
-  python3 -m pip install build
-  ```
-
-- build wheel
-
-  ```bash
-  rm -rf dist
-  python3 -m build
-  ```
-
-- upload to pypi
-
-  ```bash
-  twine upload dist/*
-  ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405090127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405100127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -54,26 +54,26 @@
 Windows-by-WSL2). - NVIDIA GPUs - [Compatibility with Nvidia GPUs](https://
 github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs). --- The
 Full Introduction of OneDiff: - [About OneDiff](#about-onediff) -
 [Architecture](#architecture) - [State-of-the-art performance](#state-of-the-
 art-performance) - [Features](#features) - [Acceleration for State-of-the-art
 models](#acceleration-for-state-of-the-art-models) - [Acceleration for
 production environment](#acceleration-for-production-environment) - [OneDiff
-Quality Evalution](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
+Quality Evaluation](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
 (#onediff-enterprise-edition) - [Installation](#installation) - [Release]
 (#release) ## About OneDiff ### Architecture OneDiff interfaces with various
 front-end sd frameworks upward, and uses a custom virtual machine mixed with
 PyTorch as the inference engine downward. [imgs/onediff_arch.png]### State-of-
 the-art performance #### SDXL E2E time - Model stabilityai/stable-diffusion-xl-
 base-1.0; - Image size 1024*1024, batch size 1, steps 30; - NVIDIA A100 80G
 SXM4; [imgs/0_12_sdxl.png]#### SVD E2E time - Model stabilityai/stable-video-
 diffusion-img2vid-xt; - Image size 576*1024, batch size 1, steps 25, decoder
 chunk size 5; - NVIDIA A100 80G SXM4; [imgs/0_12_svd.png]Note that we haven't
-got the way to run SVD with TensorRT on Feb 29 2024. ### Features | Main
-Function | Details | |----------------|----------------------------| |
+got the way to run SVD with TensorRT on Feb 29 2024. ### Features |
+Functionality | Details | |----------------|----------------------------| |
 Compiling Time | About 1 minute (SDXL) | | Deployment Methods | Plug and Play |
 | Dynamic Image Size Support | Support with no overhead | | Model Support |
 SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm Support | SD standard workflow,
 LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. | | SD Framework Support
 | ComfyUI, Diffusers, SD-webui | | Save & Load Accelerated Models | Yes | |
 Time of LoRA Switching | Hundreds of milliseconds | | LoRA Occupancy | Tens of
 MB to hundreds of MB. | | Device Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/
@@ -107,27 +107,29 @@
 github.com/siliconflow/onediff/blob/main/onediff_diffusers_extensions/examples/
 text_to_image_sdxl_mp_load.py) - Compile at one device(such as device 0), then
 use the compiled result to other device(such as device 1~7). ### OneDiff
 Quality Evaluation We also maintain a repository for benchmarking the quality
 of generation after acceleration using OneDiff: [OneDiffGenMetrics](https://
 github.com/siliconflow/OneDiffGenMetrics) ### OneDiff Enterprise Edition If you
 need **Enterprise-level Support** for your system or business, you can -
-subscribe to Enterprise Edition online and get all support after the order:
-https://siliconflow.com/onediff.html - or send an email to
-contact@siliconflow.com and tell us about your user case, deployment scale, and
-requirements. OneDiff Enterprise Edition can be **subscripted for one month and
-one GPU** and the cost is low. | Â  | OneDiff Enterprise Edition | OneDiff
-Community Edition | | ---------------------------------------------------------
------------------------------------------------- | ----------------------------
------------ | --------------------------------------- | | Multiple Resolutions
-| Yes(No time cost for most of the cases) | Yes(No time cost for most of the
-cases) | | More Extreme and Dedicated optimization(usually another 20~100%
-performance gain) for the most used model | Yes | | | Tools for specific(very
-large scale) server side deployment | Yes | | | Technical Support for
-deployment | High priority support | Community | | Get the experimental
+Subscribe to the OneDiff Enterprise Edition directly through our website. Upon
+purchase, you'll gain immediate access to comprehensive support: https://
+siliconflow.com/onediff.html - For a more personalized approach, please email
+us at contact@siliconflow.com. Include details about your use case, deployment
+size, and any specific needs you might have. The OneDiff Enterprise Edition is
+available for a monthly subscription and is designed to be cost-effective, even
+for systems utilizing a **single GPU**. | Â  | OneDiff Enterprise Edition |
+OneDiff Community Edition | | -------------------------------------------------
+-------------------------------------------------------- | --------------------
+------------------- | --------------------------------------- | | Multiple
+Resolutions | Yes(No time cost for most of the cases) | Yes(No time cost for
+most of the cases) | | More Extreme and Dedicated optimization(usually another
+20~100% performance gain) for the most used model | Yes | | | Tools for
+specific(very large scale) server side deployment | Yes | | | Technical Support
+for deployment | High priority support | Community | | Get the experimental
 features | Yes | | ## Installation ### OneDiff Installation #### 1. Install
 OneFlow > **_NOTE:_** We have updated OneFlow frequently for OneDiff, so please
 install OneFlow by the links below. - **CUDA 11.8** For NA/EU users ```bash
 python3 -m pip install -U --pre oneflow -f https://github.com/siliconflow/
 oneflow_releases/releases/expanded_assets/community_cu118 ``` For CN users
 ```bash python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-
 beijing.aliyuncs.com/branch/community/cu118 ``` Click to get OneFlow packages
@@ -145,14 +147,9 @@
 "transformers==4.27.1" "diffusers[torch]==0.19.3" ``` #### 3. Install OneDiff -
 From PyPI ``` python3 -m pip install --pre onediff ``` - From source ``` git
 clone https://github.com/siliconflow/onediff.git cd onediff && python3 -m pip
 install -e . ``` > **_NOTE:_** If you intend to utilize plugins for ComfyUI/
 StableDiffusion-WebUI, we highly recommend installing OneDiff from the source
 rather than PyPI. This is necessary as you'll need to manually copy (or create
 a soft link) for the relevant code into the extension folder of these UIs/Libs.
-#### 4. (Optional)Login huggingface-cli ``` python3 -m pip install
-huggingface_hub ~/.local/bin/huggingface-cli login ``` ## Release - run
-examples to check it works ```bash cd onediff_diffusers_extensions python3
-examples/text_to_image.py ``` - bump version in these files: ``` .github/
-workflows/pub.yml src/onediff/__init__.py ``` - install build package ```bash
-python3 -m pip install build ``` - build wheel ```bash rm -rf dist python3 -
-m build ``` - upload to pypi ```bash twine upload dist/* ```
+#### 4. (Optional)Login huggingface-cli ```bash python3 -m pip install
+huggingface_hub huggingface-cli login ```
```

### Comparing `onediff-1.0.0.dev202405090127/README.md` & `onediff-1.0.0.dev202405100127/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 <!-- toc -->
 - [About OneDiff](#about-onediff)
   - [Architecture](#architecture)
   - [State-of-the-art performance](#state-of-the-art-performance)
   - [Features](#features)
   - [Acceleration for State-of-the-art models](#acceleration-for-state-of-the-art-models)
   - [Acceleration for production environment](#acceleration-for-production-environment)
-  - [OneDiff Quality Evalution](#onediff-quality-evaluation)
+  - [OneDiff Quality Evaluation](#onediff-quality-evaluation)
   - [OneDiff Enterprise Edition](#onediff-enterprise-edition)
 - [Installation](#installation)
 - [Release](#release)
 <!-- tocstop -->
 
 ## About OneDiff
 ### Architecture
@@ -90,15 +90,15 @@
 
 <img src="imgs/0_12_svd.png" height="400">
 
 Note that we haven't got the way to run SVD with TensorRT on Feb 29 2024.
 
 ### Features
 
-| Main Function | Details |
+| Functionality | Details |
 |----------------|----------------------------|
 | Compiling Time   | About 1 minute (SDXL) |
 | Deployment Methods              | Plug and Play |
 | Dynamic Image Size Support  | Support with no overhead |
 | Model Support                 | SD1.5~2.1, SDXL, SDXL Turbo, etc. |
 | Algorithm Support             | SD standard workflow, LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. |
 | SD Framework Support | ComfyUI, Diffusers, SD-webui |
@@ -145,18 +145,18 @@
 ### OneDiff Quality Evaluation
 
 We also maintain a repository for benchmarking the quality of generation after acceleration using OneDiff:
 [OneDiffGenMetrics](https://github.com/siliconflow/OneDiffGenMetrics)
 
 ### OneDiff Enterprise Edition
 If you need **Enterprise-level Support** for your system or business, you can
-- subscribe to Enterprise Edition online and get all support after the order: https://siliconflow.com/onediff.html
-- or send an email to contact@siliconflow.com and tell us about your user case, deployment scale, and requirements.
+- Subscribe to the OneDiff Enterprise Edition directly through our website. Upon purchase, you'll gain immediate access to comprehensive support: https://siliconflow.com/onediff.html
+- For a more personalized approach, please email us at contact@siliconflow.com. Include details about your use case, deployment size, and any specific needs you might have.
 
-OneDiff Enterprise Edition can be **subscripted for one month and one GPU** and the cost is low.
+The OneDiff Enterprise Edition is available for a monthly subscription and is designed to be cost-effective, even for systems utilizing a **single GPU**.
 
 |                                                                                                           | OneDiff Enterprise Edition              | OneDiff Community Edition               |
 | --------------------------------------------------------------------------------------------------------- | --------------------------------------- | --------------------------------------- |
 | Multiple Resolutions                                                                                      | Yes(No time cost for most of the cases) | Yes(No time cost for most of the cases) |
 | More Extreme and Dedicated optimization(usually another 20~100% performance gain) for the most used model | Yes                                     |                                         |
 | Tools for specific(very large scale) server side deployment                                               | Yes                                     |                                         |
 | Technical Support for deployment                                                                          | High priority support                   | Community                               |
@@ -196,15 +196,15 @@
   python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-beijing.aliyuncs.com/branch/community/cu121
   ```
 
 
 - **CUDA 12.2**
 
   For NA/EU users
-  ```bash 
+  ```bash
   python3 -m pip install -U --pre oneflow -f https://github.com/siliconflow/oneflow_releases/releases/expanded_assets/community_cu122
   ```
   For CN users
   ```bash
   python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-beijing.aliyuncs.com/branch/community/cu122
   ```
 
@@ -232,45 +232,11 @@
 cd onediff && python3 -m pip install -e .
 ```
 
 > **_NOTE:_** If you intend to utilize plugins for ComfyUI/StableDiffusion-WebUI, we highly recommend installing OneDiff from the source rather than PyPI. This is necessary as you'll need to manually copy (or create a soft link) for the relevant code into the extension folder of these UIs/Libs.
 
 #### 4. (Optional)Login huggingface-cli
 
-```
+```bash
 python3 -m pip install huggingface_hub
- ~/.local/bin/huggingface-cli login
+huggingface-cli login
 ```
-
-## Release
-
-- run examples to check it works
-
-  ```bash
-  cd onediff_diffusers_extensions
-  python3 examples/text_to_image.py
-  ```
-
-- bump version in these files:
-
-  ```
-  .github/workflows/pub.yml
-  src/onediff/__init__.py
-  ```
-
-- install build package
-  ```bash
-  python3 -m pip install build
-  ```
-
-- build wheel
-
-  ```bash
-  rm -rf dist
-  python3 -m build
-  ```
-
-- upload to pypi
-
-  ```bash
-  twine upload dist/*
-  ```
```

#### html2text {}

```diff
@@ -40,26 +40,26 @@
 Windows-by-WSL2). - NVIDIA GPUs - [Compatibility with Nvidia GPUs](https://
 github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs). --- The
 Full Introduction of OneDiff: - [About OneDiff](#about-onediff) -
 [Architecture](#architecture) - [State-of-the-art performance](#state-of-the-
 art-performance) - [Features](#features) - [Acceleration for State-of-the-art
 models](#acceleration-for-state-of-the-art-models) - [Acceleration for
 production environment](#acceleration-for-production-environment) - [OneDiff
-Quality Evalution](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
+Quality Evaluation](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
 (#onediff-enterprise-edition) - [Installation](#installation) - [Release]
 (#release) ## About OneDiff ### Architecture OneDiff interfaces with various
 front-end sd frameworks upward, and uses a custom virtual machine mixed with
 PyTorch as the inference engine downward. [imgs/onediff_arch.png]### State-of-
 the-art performance #### SDXL E2E time - Model stabilityai/stable-diffusion-xl-
 base-1.0; - Image size 1024*1024, batch size 1, steps 30; - NVIDIA A100 80G
 SXM4; [imgs/0_12_sdxl.png]#### SVD E2E time - Model stabilityai/stable-video-
 diffusion-img2vid-xt; - Image size 576*1024, batch size 1, steps 25, decoder
 chunk size 5; - NVIDIA A100 80G SXM4; [imgs/0_12_svd.png]Note that we haven't
-got the way to run SVD with TensorRT on Feb 29 2024. ### Features | Main
-Function | Details | |----------------|----------------------------| |
+got the way to run SVD with TensorRT on Feb 29 2024. ### Features |
+Functionality | Details | |----------------|----------------------------| |
 Compiling Time | About 1 minute (SDXL) | | Deployment Methods | Plug and Play |
 | Dynamic Image Size Support | Support with no overhead | | Model Support |
 SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm Support | SD standard workflow,
 LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. | | SD Framework Support
 | ComfyUI, Diffusers, SD-webui | | Save & Load Accelerated Models | Yes | |
 Time of LoRA Switching | Hundreds of milliseconds | | LoRA Occupancy | Tens of
 MB to hundreds of MB. | | Device Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/
@@ -93,27 +93,29 @@
 github.com/siliconflow/onediff/blob/main/onediff_diffusers_extensions/examples/
 text_to_image_sdxl_mp_load.py) - Compile at one device(such as device 0), then
 use the compiled result to other device(such as device 1~7). ### OneDiff
 Quality Evaluation We also maintain a repository for benchmarking the quality
 of generation after acceleration using OneDiff: [OneDiffGenMetrics](https://
 github.com/siliconflow/OneDiffGenMetrics) ### OneDiff Enterprise Edition If you
 need **Enterprise-level Support** for your system or business, you can -
-subscribe to Enterprise Edition online and get all support after the order:
-https://siliconflow.com/onediff.html - or send an email to
-contact@siliconflow.com and tell us about your user case, deployment scale, and
-requirements. OneDiff Enterprise Edition can be **subscripted for one month and
-one GPU** and the cost is low. | Â  | OneDiff Enterprise Edition | OneDiff
-Community Edition | | ---------------------------------------------------------
------------------------------------------------- | ----------------------------
------------ | --------------------------------------- | | Multiple Resolutions
-| Yes(No time cost for most of the cases) | Yes(No time cost for most of the
-cases) | | More Extreme and Dedicated optimization(usually another 20~100%
-performance gain) for the most used model | Yes | | | Tools for specific(very
-large scale) server side deployment | Yes | | | Technical Support for
-deployment | High priority support | Community | | Get the experimental
+Subscribe to the OneDiff Enterprise Edition directly through our website. Upon
+purchase, you'll gain immediate access to comprehensive support: https://
+siliconflow.com/onediff.html - For a more personalized approach, please email
+us at contact@siliconflow.com. Include details about your use case, deployment
+size, and any specific needs you might have. The OneDiff Enterprise Edition is
+available for a monthly subscription and is designed to be cost-effective, even
+for systems utilizing a **single GPU**. | Â  | OneDiff Enterprise Edition |
+OneDiff Community Edition | | -------------------------------------------------
+-------------------------------------------------------- | --------------------
+------------------- | --------------------------------------- | | Multiple
+Resolutions | Yes(No time cost for most of the cases) | Yes(No time cost for
+most of the cases) | | More Extreme and Dedicated optimization(usually another
+20~100% performance gain) for the most used model | Yes | | | Tools for
+specific(very large scale) server side deployment | Yes | | | Technical Support
+for deployment | High priority support | Community | | Get the experimental
 features | Yes | | ## Installation ### OneDiff Installation #### 1. Install
 OneFlow > **_NOTE:_** We have updated OneFlow frequently for OneDiff, so please
 install OneFlow by the links below. - **CUDA 11.8** For NA/EU users ```bash
 python3 -m pip install -U --pre oneflow -f https://github.com/siliconflow/
 oneflow_releases/releases/expanded_assets/community_cu118 ``` For CN users
 ```bash python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-
 beijing.aliyuncs.com/branch/community/cu118 ``` Click to get OneFlow packages
@@ -131,14 +133,9 @@
 "transformers==4.27.1" "diffusers[torch]==0.19.3" ``` #### 3. Install OneDiff -
 From PyPI ``` python3 -m pip install --pre onediff ``` - From source ``` git
 clone https://github.com/siliconflow/onediff.git cd onediff && python3 -m pip
 install -e . ``` > **_NOTE:_** If you intend to utilize plugins for ComfyUI/
 StableDiffusion-WebUI, we highly recommend installing OneDiff from the source
 rather than PyPI. This is necessary as you'll need to manually copy (or create
 a soft link) for the relevant code into the extension folder of these UIs/Libs.
-#### 4. (Optional)Login huggingface-cli ``` python3 -m pip install
-huggingface_hub ~/.local/bin/huggingface-cli login ``` ## Release - run
-examples to check it works ```bash cd onediff_diffusers_extensions python3
-examples/text_to_image.py ``` - bump version in these files: ``` .github/
-workflows/pub.yml src/onediff/__init__.py ``` - install build package ```bash
-python3 -m pip install build ``` - build wheel ```bash rm -rf dist python3 -
-m build ``` - upload to pypi ```bash twine upload dist/* ```
+#### 4. (Optional)Login huggingface-cli ```bash python3 -m pip install
+huggingface_hub huggingface-cli login ```
```

### Comparing `onediff-1.0.0.dev202405090127/setup.py` & `onediff-1.0.0.dev202405100127/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.0.0.dev202405100127/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/__init__.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/env_var.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/options.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/options.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/with_fx_graph.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/with_fx_graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/infer_compiler/with_fx_interpreter.py` & `onediff-1.0.0.dev202405100127/src/onediff/infer_compiler/with_fx_interpreter.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/optimization/attention_processor.py` & `onediff-1.0.0.dev202405100127/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/optimization/quant_optimizer.py` & `onediff-1.0.0.dev202405100127/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.0.0.dev202405100127/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/quantization/load_quantized_model.py` & `onediff-1.0.0.dev202405100127/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.0.0.dev202405100127/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.0.0.dev202405100127/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff/quantization/quantize_utils.py` & `onediff-1.0.0.dev202405100127/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/src/onediff.egg-info/PKG-INFO` & `onediff-1.0.0.dev202405100127/src/onediff.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202405090127
+Version: 1.0.0.dev202405100127
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -85,15 +85,15 @@
 <!-- toc -->
 - [About OneDiff](#about-onediff)
   - [Architecture](#architecture)
   - [State-of-the-art performance](#state-of-the-art-performance)
   - [Features](#features)
   - [Acceleration for State-of-the-art models](#acceleration-for-state-of-the-art-models)
   - [Acceleration for production environment](#acceleration-for-production-environment)
-  - [OneDiff Quality Evalution](#onediff-quality-evaluation)
+  - [OneDiff Quality Evaluation](#onediff-quality-evaluation)
   - [OneDiff Enterprise Edition](#onediff-enterprise-edition)
 - [Installation](#installation)
 - [Release](#release)
 <!-- tocstop -->
 
 ## About OneDiff
 ### Architecture
@@ -117,15 +117,15 @@
 
 <img src="imgs/0_12_svd.png" height="400">
 
 Note that we haven't got the way to run SVD with TensorRT on Feb 29 2024.
 
 ### Features
 
-| Main Function | Details |
+| Functionality | Details |
 |----------------|----------------------------|
 | Compiling Time   | About 1 minute (SDXL) |
 | Deployment Methods              | Plug and Play |
 | Dynamic Image Size Support  | Support with no overhead |
 | Model Support                 | SD1.5~2.1, SDXL, SDXL Turbo, etc. |
 | Algorithm Support             | SD standard workflow, LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. |
 | SD Framework Support | ComfyUI, Diffusers, SD-webui |
@@ -172,18 +172,18 @@
 ### OneDiff Quality Evaluation
 
 We also maintain a repository for benchmarking the quality of generation after acceleration using OneDiff:
 [OneDiffGenMetrics](https://github.com/siliconflow/OneDiffGenMetrics)
 
 ### OneDiff Enterprise Edition
 If you need **Enterprise-level Support** for your system or business, you can
-- subscribe to Enterprise Edition online and get all support after the order: https://siliconflow.com/onediff.html
-- or send an email to contact@siliconflow.com and tell us about your user case, deployment scale, and requirements.
+- Subscribe to the OneDiff Enterprise Edition directly through our website. Upon purchase, you'll gain immediate access to comprehensive support: https://siliconflow.com/onediff.html
+- For a more personalized approach, please email us at contact@siliconflow.com. Include details about your use case, deployment size, and any specific needs you might have.
 
-OneDiff Enterprise Edition can be **subscripted for one month and one GPU** and the cost is low.
+The OneDiff Enterprise Edition is available for a monthly subscription and is designed to be cost-effective, even for systems utilizing a **single GPU**.
 
 |                                                                                                           | OneDiff Enterprise Edition              | OneDiff Community Edition               |
 | --------------------------------------------------------------------------------------------------------- | --------------------------------------- | --------------------------------------- |
 | Multiple Resolutions                                                                                      | Yes(No time cost for most of the cases) | Yes(No time cost for most of the cases) |
 | More Extreme and Dedicated optimization(usually another 20~100% performance gain) for the most used model | Yes                                     |                                         |
 | Tools for specific(very large scale) server side deployment                                               | Yes                                     |                                         |
 | Technical Support for deployment                                                                          | High priority support                   | Community                               |
@@ -223,15 +223,15 @@
   python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-beijing.aliyuncs.com/branch/community/cu121
   ```
 
 
 - **CUDA 12.2**
 
   For NA/EU users
-  ```bash 
+  ```bash
   python3 -m pip install -U --pre oneflow -f https://github.com/siliconflow/oneflow_releases/releases/expanded_assets/community_cu122
   ```
   For CN users
   ```bash
   python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-beijing.aliyuncs.com/branch/community/cu122
   ```
 
@@ -259,45 +259,11 @@
 cd onediff && python3 -m pip install -e .
 ```
 
 > **_NOTE:_** If you intend to utilize plugins for ComfyUI/StableDiffusion-WebUI, we highly recommend installing OneDiff from the source rather than PyPI. This is necessary as you'll need to manually copy (or create a soft link) for the relevant code into the extension folder of these UIs/Libs.
 
 #### 4. (Optional)Login huggingface-cli
 
-```
+```bash
 python3 -m pip install huggingface_hub
- ~/.local/bin/huggingface-cli login
+huggingface-cli login
 ```
-
-## Release
-
-- run examples to check it works
-
-  ```bash
-  cd onediff_diffusers_extensions
-  python3 examples/text_to_image.py
-  ```
-
-- bump version in these files:
-
-  ```
-  .github/workflows/pub.yml
-  src/onediff/__init__.py
-  ```
-
-- install build package
-  ```bash
-  python3 -m pip install build
-  ```
-
-- build wheel
-
-  ```bash
-  rm -rf dist
-  python3 -m build
-  ```
-
-- upload to pypi
-
-  ```bash
-  twine upload dist/*
-  ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405090127 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405100127 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -54,26 +54,26 @@
 Windows-by-WSL2). - NVIDIA GPUs - [Compatibility with Nvidia GPUs](https://
 github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs). --- The
 Full Introduction of OneDiff: - [About OneDiff](#about-onediff) -
 [Architecture](#architecture) - [State-of-the-art performance](#state-of-the-
 art-performance) - [Features](#features) - [Acceleration for State-of-the-art
 models](#acceleration-for-state-of-the-art-models) - [Acceleration for
 production environment](#acceleration-for-production-environment) - [OneDiff
-Quality Evalution](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
+Quality Evaluation](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
 (#onediff-enterprise-edition) - [Installation](#installation) - [Release]
 (#release) ## About OneDiff ### Architecture OneDiff interfaces with various
 front-end sd frameworks upward, and uses a custom virtual machine mixed with
 PyTorch as the inference engine downward. [imgs/onediff_arch.png]### State-of-
 the-art performance #### SDXL E2E time - Model stabilityai/stable-diffusion-xl-
 base-1.0; - Image size 1024*1024, batch size 1, steps 30; - NVIDIA A100 80G
 SXM4; [imgs/0_12_sdxl.png]#### SVD E2E time - Model stabilityai/stable-video-
 diffusion-img2vid-xt; - Image size 576*1024, batch size 1, steps 25, decoder
 chunk size 5; - NVIDIA A100 80G SXM4; [imgs/0_12_svd.png]Note that we haven't
-got the way to run SVD with TensorRT on Feb 29 2024. ### Features | Main
-Function | Details | |----------------|----------------------------| |
+got the way to run SVD with TensorRT on Feb 29 2024. ### Features |
+Functionality | Details | |----------------|----------------------------| |
 Compiling Time | About 1 minute (SDXL) | | Deployment Methods | Plug and Play |
 | Dynamic Image Size Support | Support with no overhead | | Model Support |
 SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm Support | SD standard workflow,
 LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. | | SD Framework Support
 | ComfyUI, Diffusers, SD-webui | | Save & Load Accelerated Models | Yes | |
 Time of LoRA Switching | Hundreds of milliseconds | | LoRA Occupancy | Tens of
 MB to hundreds of MB. | | Device Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/
@@ -107,27 +107,29 @@
 github.com/siliconflow/onediff/blob/main/onediff_diffusers_extensions/examples/
 text_to_image_sdxl_mp_load.py) - Compile at one device(such as device 0), then
 use the compiled result to other device(such as device 1~7). ### OneDiff
 Quality Evaluation We also maintain a repository for benchmarking the quality
 of generation after acceleration using OneDiff: [OneDiffGenMetrics](https://
 github.com/siliconflow/OneDiffGenMetrics) ### OneDiff Enterprise Edition If you
 need **Enterprise-level Support** for your system or business, you can -
-subscribe to Enterprise Edition online and get all support after the order:
-https://siliconflow.com/onediff.html - or send an email to
-contact@siliconflow.com and tell us about your user case, deployment scale, and
-requirements. OneDiff Enterprise Edition can be **subscripted for one month and
-one GPU** and the cost is low. | Â  | OneDiff Enterprise Edition | OneDiff
-Community Edition | | ---------------------------------------------------------
------------------------------------------------- | ----------------------------
------------ | --------------------------------------- | | Multiple Resolutions
-| Yes(No time cost for most of the cases) | Yes(No time cost for most of the
-cases) | | More Extreme and Dedicated optimization(usually another 20~100%
-performance gain) for the most used model | Yes | | | Tools for specific(very
-large scale) server side deployment | Yes | | | Technical Support for
-deployment | High priority support | Community | | Get the experimental
+Subscribe to the OneDiff Enterprise Edition directly through our website. Upon
+purchase, you'll gain immediate access to comprehensive support: https://
+siliconflow.com/onediff.html - For a more personalized approach, please email
+us at contact@siliconflow.com. Include details about your use case, deployment
+size, and any specific needs you might have. The OneDiff Enterprise Edition is
+available for a monthly subscription and is designed to be cost-effective, even
+for systems utilizing a **single GPU**. | Â  | OneDiff Enterprise Edition |
+OneDiff Community Edition | | -------------------------------------------------
+-------------------------------------------------------- | --------------------
+------------------- | --------------------------------------- | | Multiple
+Resolutions | Yes(No time cost for most of the cases) | Yes(No time cost for
+most of the cases) | | More Extreme and Dedicated optimization(usually another
+20~100% performance gain) for the most used model | Yes | | | Tools for
+specific(very large scale) server side deployment | Yes | | | Technical Support
+for deployment | High priority support | Community | | Get the experimental
 features | Yes | | ## Installation ### OneDiff Installation #### 1. Install
 OneFlow > **_NOTE:_** We have updated OneFlow frequently for OneDiff, so please
 install OneFlow by the links below. - **CUDA 11.8** For NA/EU users ```bash
 python3 -m pip install -U --pre oneflow -f https://github.com/siliconflow/
 oneflow_releases/releases/expanded_assets/community_cu118 ``` For CN users
 ```bash python3 -m pip install -U --pre oneflow -f https://oneflow-pro.oss-cn-
 beijing.aliyuncs.com/branch/community/cu118 ``` Click to get OneFlow packages
@@ -145,14 +147,9 @@
 "transformers==4.27.1" "diffusers[torch]==0.19.3" ``` #### 3. Install OneDiff -
 From PyPI ``` python3 -m pip install --pre onediff ``` - From source ``` git
 clone https://github.com/siliconflow/onediff.git cd onediff && python3 -m pip
 install -e . ``` > **_NOTE:_** If you intend to utilize plugins for ComfyUI/
 StableDiffusion-WebUI, we highly recommend installing OneDiff from the source
 rather than PyPI. This is necessary as you'll need to manually copy (or create
 a soft link) for the relevant code into the extension folder of these UIs/Libs.
-#### 4. (Optional)Login huggingface-cli ``` python3 -m pip install
-huggingface_hub ~/.local/bin/huggingface-cli login ``` ## Release - run
-examples to check it works ```bash cd onediff_diffusers_extensions python3
-examples/text_to_image.py ``` - bump version in these files: ``` .github/
-workflows/pub.yml src/onediff/__init__.py ``` - install build package ```bash
-python3 -m pip install build ``` - build wheel ```bash rm -rf dist python3 -
-m build ``` - upload to pypi ```bash twine upload dist/* ```
+#### 4. (Optional)Login huggingface-cli ```bash python3 -m pip install
+huggingface_hub huggingface-cli login ```
```

### Comparing `onediff-1.0.0.dev202405090127/src/onediff.egg-info/SOURCES.txt` & `onediff-1.0.0.dev202405100127/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/tests/test_dual_module_list.py` & `onediff-1.0.0.dev202405100127/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.0.0.dev202405100127/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/tests/test_quantitative_quality.py` & `onediff-1.0.0.dev202405100127/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202405090127/tests/test_quantize_custom_model.py` & `onediff-1.0.0.dev202405100127/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

