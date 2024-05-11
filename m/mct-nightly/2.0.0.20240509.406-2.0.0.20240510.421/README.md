# Comparing `tmp/mct-nightly-2.0.0.20240509.406.tar.gz` & `tmp/mct-nightly-2.0.0.20240510.421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-2.0.0.20240509.406.tar", last modified: Thu May  9 00:04:07 2024, max compression
+gzip compressed data, was "mct-nightly-2.0.0.20240510.421.tar", last modified: Fri May 10 00:04:23 2024, max compression
```

## Comparing `mct-nightly-2.0.0.20240509.406.tar` & `mct-nightly-2.0.0.20240510.421.tar`

### file list

```diff
@@ -1,607 +1,607 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17752 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.569401 mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19733 2024-05-09 00:04:07.000000 mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-05-09 00:04:07.000000 mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:04:07.000000 mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-09 00:04:07.000000 mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 00:04:07.000000 mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.569401 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-09 00:04:06.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.569401 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.573402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.573402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.573402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.573402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.573402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38326 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.577401 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.577401 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/hessian_info_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.577401 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.581402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.581402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.581402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.581402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.585402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/channels_grouping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.585402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.585402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/memory_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/prune_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.585402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.589402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.589402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.589402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.593402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.593402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/graph_prep_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.593402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.593402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/custom_layer_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.593402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.597402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.597402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    29716 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/keras_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.597402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.597402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.601402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.601402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.601402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.601402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.601402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.601402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.605402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.605402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.605402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pytorch_device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/quantization_prep_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.609402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.613402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/data_generation_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/model_info_exctractors.py
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.613402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/keras_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.613402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.613402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.613402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20937 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/defaultdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.617402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.621402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/keras/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/pytorch/pruning_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.625402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.629402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.633402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.637402 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-09 00:03:36.000000 mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 00:04:07.641403 mct-nightly-2.0.0.20240509.406/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-09 00:04:06.000000 mct-nightly-2.0.0.20240509.406/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.128475 mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-10 00:04:22.000000 mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    37478 2024-05-10 00:04:23.000000 mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 00:04:22.000000 mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-10 00:04:22.000000 mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 00:04:22.000000 mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.132475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-10 00:04:21.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.132475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.132475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.132475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.132475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7930 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.136475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.136475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38326 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29079 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4744 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5128 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.136475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.136475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/hessian_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/hessian_info_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/trace_hessian_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.140475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3091 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2210 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3706 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1773 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2745 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.140475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37578 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.140475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13820 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.140475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16592 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28519 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.140475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19594 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.144475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/channels_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.144475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14027 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.144475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5978 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19523 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/memory_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/prune_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.144475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26733 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.148475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23305 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41524 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8902 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.148475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.148475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.152475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29865 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.152475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22510 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/graph_prep_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.152475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.152475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15587 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/custom_layer_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.156475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.156475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26771 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.156475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29716 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/keras_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7906 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.160475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.164475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.164475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.164475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38459 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pytorch_device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12626 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/quantization_prep_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.168475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.172475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/data_generation_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/model_info_exctractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.172475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7623 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21539 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/keras_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.172475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21146 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.172475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/image_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21238 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/defaultdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.176475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9348 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19123 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.180475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16509 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12347 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/keras/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/pytorch/pruning_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.184475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9012 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10789 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.188475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10712 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9910 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.192475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10369 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.196475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-10 00:03:51.000000 mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-10 00:04:23.200475 mct-nightly-2.0.0.20240510.421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-10 00:04:21.000000 mct-nightly-2.0.0.20240510.421/setup.py
```

### Comparing `mct-nightly-2.0.0.20240509.406/LICENSE.md` & `mct-nightly-2.0.0.20240510.421/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/PKG-INFO` & `mct-nightly-2.0.0.20240510.421/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240509.406
+Version: 2.0.0.20240510.421
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -43,17 +43,17 @@
         
         
         ### Quick start & tutorials 
         
         Explore the Model Compression Toolkit (MCT) through our tutorials, 
         covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
         for hands-on learning. For example:
-        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/keras/ptq/example_keras_imagenet.ipynb)
-        * [Post training quantization with PyTorch](tutorials/notebooks/pytorch/ptq/example_pytorch_quantization_mnist.ipynb)
-        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/pytorch/data_generation/example_pytorch_data_generation.ipynb).
+        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+        * [Post training quantization with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
         
         
         ### Supported Versions
         
         Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
         
         |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
@@ -148,16 +148,14 @@
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
         |---------------------------|-----------------|-----------------|-------------------------|
         | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
         | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
         | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
         
-        For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
-        
         
         #### Pruning Results
         
         Results for applying pruning to reduce the parameters of the following models by 50%:
         
         | Model           | Dense Model Accuracy | Pruned Model Accuracy |
         |-----------------|----------------------|-----------------------|
```

### Comparing `mct-nightly-2.0.0.20240509.406/README.md` & `mct-nightly-2.0.0.20240510.421/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 
 
 ### Quick start & tutorials 
 
 Explore the Model Compression Toolkit (MCT) through our tutorials, 
 covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
 for hands-on learning. For example:
-* [Keras MobileNetV2 post training quantization](tutorials/notebooks/keras/ptq/example_keras_imagenet.ipynb)
-* [Post training quantization with PyTorch](tutorials/notebooks/pytorch/ptq/example_pytorch_quantization_mnist.ipynb)
-* [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/pytorch/data_generation/example_pytorch_data_generation.ipynb).
+* [Keras MobileNetV2 post training quantization](tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+* [Post training quantization with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+* [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
 
 
 ### Supported Versions
 
 Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
 
 |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
@@ -142,16 +142,14 @@
 
 | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
 |---------------------------|-----------------|-----------------|-------------------------|
 | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
 | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
 | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
 
-For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
-
 
 #### Pruning Results
 
 Results for applying pruning to reduce the parameters of the following models by 50%:
 
 | Model           | Dense Model Accuracy | Pruned Model Accuracy |
 |-----------------|----------------------|-----------------------|
```

### Comparing `mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 2.0.0.20240509.406
+Version: 2.0.0.20240510.421
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -43,17 +43,17 @@
         
         
         ### Quick start & tutorials 
         
         Explore the Model Compression Toolkit (MCT) through our tutorials, 
         covering compression techniques for Keras and PyTorch models. Access interactive [notebooks](tutorials/README.md) 
         for hands-on learning. For example:
-        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/keras/ptq/example_keras_imagenet.ipynb)
-        * [Post training quantization with PyTorch](tutorials/notebooks/pytorch/ptq/example_pytorch_quantization_mnist.ipynb)
-        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/pytorch/data_generation/example_pytorch_data_generation.ipynb).
+        * [Keras MobileNetV2 post training quantization](tutorials/notebooks/imx500_notebooks/keras/example_keras_mobilenetv2_for_imx500.ipynb)
+        * [Post training quantization with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_ptq_mnist.ipynb)
+        * [Data Generation for ResNet18 with PyTorch](tutorials/notebooks/mct_features_notebooks/pytorch/example_pytorch_data_generation.ipynb).
         
         
         ### Supported Versions
         
         Currently, MCT is being tested on various Python, Pytorch and TensorFlow versions:
         
         |             |  PyTorch 1.13                                                                                                                                                                                                               | PyTorch 2.0                                                                                                                                                                                                              | PyTorch 2.1                                                                                                                                                                                                              |
@@ -148,16 +148,14 @@
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | Data-Free 8Bit Accuracy |
         |---------------------------|-----------------|-----------------|-------------------------|
         | MobileNet V2 [3]          | 71.886          | 71.444          |71.29|
         | ResNet-18 [3]             | 69.86           | 69.63           |69.53|
         | SqueezeNet 1.1 [3]        | 58.128          | 57.678          ||
         
-        For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
-        
         
         #### Pruning Results
         
         Results for applying pruning to reduce the parameters of the following models by 50%:
         
         | Model           | Dense Model Accuracy | Pruned Model Accuracy |
         |-----------------|----------------------|-----------------------|
```

### Comparing `mct-nightly-2.0.0.20240509.406/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-2.0.0.20240510.421/mct_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 from model_compression_toolkit import qat
 from model_compression_toolkit import exporter
 from model_compression_toolkit import gptq
 from model_compression_toolkit import data_generation
 from model_compression_toolkit import pruning
 from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-__version__ = "2.0.0.20240509.000406"
+__version__ = "2.0.0.20240510.000421"
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import importlib
 
 # Supported frameworks in MCT:
 TENSORFLOW = 'tensorflow'
 PYTORCH = 'pytorch'
 FOUND_TF = importlib.util.find_spec(TENSORFLOW) is not None
 FOUND_TORCH = importlib.util.find_spec("torch") is not None
+FOUND_TORCHVISION = importlib.util.find_spec("torchvision") is not None
 FOUND_ONNX = importlib.util.find_spec("onnx") is not None
 FOUND_ONNXRUNTIME = importlib.util.find_spec("onnxruntime") is not None
 FOUND_SONY_CUSTOM_LAYERS = importlib.util.find_spec('sony_custom_layers') is not None
 
 # Metadata fields
 MCT_VERSION = 'mct_version'
 TPC_VERSION = 'tpc_version'
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/analyzer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/hessian_info_service.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/hessian_info_service.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/hessian_info_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/hessian_info_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/trace_hessian_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/hessian/trace_hessian_request.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/hessian/trace_hessian_request.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/configurable_quant_id.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/configurable_quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/resource_utilization_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/resource_utilization_tools/ru_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/channels_grouping.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/channels_grouping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/greedy_mask_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/base_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/importance_metric_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/importance_metrics/lfh_importance_metric.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/per_channel_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/mask/per_simd_group_mask.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/memory_calculator.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/memory_calculator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/prune_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/prune_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruner.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/pruning/pruning_section.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/pruning/pruning_section.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     # Create protobuf for the node's output shapes
     if output_shapes is not None:
         tshape_protos = []
         for output_shape in output_shapes:  # create protobuf for each output shape
             proto_dims_list = []
             for dim in output_shape:
-                proto_dims_list.append(TensorShapeProto.Dim(size=dim))
+                proto_dims_list.append(TensorShapeProto.Dim(size=dim))  # dim is expected to be an integer
             tshape_proto = TensorShapeProto(dim=proto_dims_list)
             tshape_protos.append(tshape_proto)
         node_properties['_output_shapes'] = AttrValue(list=AttrValue.ListValue(shape=tshape_protos))
     return node_properties
 
 
 class TensorboardWriter(object):
@@ -259,15 +259,21 @@
 
             Returns:
                 A list of tuples where each tuple is an output shape of the node.
             """
 
             # For nodes with an "empty" output shape.
             output_shape = (None,) if n.output_shape == () else n.output_shape
-
+            if 'CombinedNonMaxSuppression' in str(output_shape):
+                # output_shapes is expected to be a list of tuples where each tuple is an output shape.
+                # For NMS layers, we need to align the node's output shapes before creating the node's properties.
+                output_shape = [output_shape.nmsed_boxes,
+                                output_shape.nmsed_scores,
+                                output_shape.nmsed_classes,
+                                output_shape.valid_detections]
             dims = []
             if isinstance(output_shape, list):
                 for o in output_shape:
                     shape_wo_none = (-1,) + o[1:] if o[0] is None else o
                     dims.append(shape_wo_none)
             else:
                 dims = [(-1,) + output_shape[1:] if output_shape[0] is None else output_shape]
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/graph_prep_runner.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/graph_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/custom_layer_validation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/custom_layer_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/dwconv_to_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/matmul_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/activation_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/hessian/weights_trace_hessian_calculator_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/pruning/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/pruning/pruning_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/concat_threshold_update.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_batch_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/functional_layer_norm.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/remove_identity.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/activation_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/hessian/weights_trace_hessian_calculator_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/configurable_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/mixed_precision/configurable_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pruning/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pruning/pruning_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pytorch_device_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pytorch_device_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/resource_utilization_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/quantization_prep_runner.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/quantization_prep_runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/core/runner.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.constants import FOUND_TORCH, FOUND_TF
+from model_compression_toolkit.constants import FOUND_TORCH, FOUND_TF, FOUND_TORCHVISION
 from model_compression_toolkit.data_generation.common.data_generation_config import DataGenerationConfig
 from model_compression_toolkit.data_generation.common.enums import ImageGranularity, DataInitType, SchedulerType, BNLayerWeightingType, OutputLossType, BatchNormAlignemntLossType, ImagePipelineType, ImageNormalizationType
 
 if FOUND_TF:
     from model_compression_toolkit.data_generation.keras.keras_data_generation import (
         keras_data_generation_experimental, get_keras_data_generation_config)
 
-if FOUND_TORCH:
+if FOUND_TORCH and FOUND_TORCHVISION:
     from model_compression_toolkit.data_generation.pytorch.pytorch_data_generation import (
         pytorch_data_generation_experimental, get_pytorch_data_generation_config)
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/data_generation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/data_generation_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/data_generation_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/enums.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/enums.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/image_pipeline.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/model_info_exctractors.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/common/optimization_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/common/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/image_pipeline.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/keras_data_generation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/keras_data_generation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/model_info_exctractors.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/keras/optimization_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/keras/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/image_pipeline.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/image_pipeline.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/model_info_exctractors.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/batchnorm_alignment_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/bn_layer_weighting_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/image_initilization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/output_loss_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_functions/scheduler_step_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/optimization_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/optimization_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/data_generation/pytorch/pytorch_data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 import time
 from typing import Callable, Any, Tuple, List
 
 from tqdm import tqdm
 
-from model_compression_toolkit.constants import FOUND_TORCH
+from model_compression_toolkit.constants import FOUND_TORCH, FOUND_TORCHVISION
 from model_compression_toolkit.core.pytorch.utils import set_model
 from model_compression_toolkit.data_generation.common.constants import DEFAULT_N_ITER, DEFAULT_DATA_GEN_BS
 from model_compression_toolkit.data_generation.common.data_generation import get_data_generation_classes
 from model_compression_toolkit.data_generation.common.data_generation_config import DataGenerationConfig
 from model_compression_toolkit.data_generation.common.enums import ImageGranularity, SchedulerType, \
     BatchNormAlignemntLossType, DataInitType, BNLayerWeightingType, ImagePipelineType, ImageNormalizationType, \
     OutputLossType
@@ -40,15 +40,15 @@
 from model_compression_toolkit.data_generation.pytorch.optimization_functions.output_loss_functions import \
     output_loss_function_dict
 from model_compression_toolkit.data_generation.pytorch.optimization_functions.scheduler_step_functions import \
     scheduler_step_function_dict
 from model_compression_toolkit.data_generation.pytorch.optimization_utils import PytorchImagesOptimizationHandler
 from model_compression_toolkit.logger import Logger
 
-if FOUND_TORCH:
+if FOUND_TORCH and FOUND_TORCHVISION:
     # Importing necessary libraries
     import torch
     from torch import Tensor
     from torch.nn import Module
     from torch.optim import RAdam, Optimizer
     from torch.fx import symbolic_trace
 
@@ -350,14 +350,13 @@
         finalized_imgs = all_imgs_opt_handler.get_finalized_images()
         Logger.info(f'Total time to generate {len(finalized_imgs)} images (seconds): {int(time.time() - total_time)}')
         return finalized_imgs
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
     def get_pytorch_data_generation_config(*args, **kwargs):
-        Logger.critical('PyTorch must be installed to use get_pytorch_data_generation_config. '
-                        "The 'torch' package is missing.")  # pragma: no cover
-
+        msg = f"PyTorch and torchvision must be installed to use get_pytorch_data_generation_config. " + ("" if FOUND_TORCH else "The 'torch' package is missing. ") + ("" if FOUND_TORCHVISION else "The 'torchvision' package is missing. ") # pragma: no cover
+        Logger.critical(msg)  # pragma: no cover
 
     def pytorch_data_generation_experimental(*args, **kwargs):
-        Logger.critical("PyTorch must be installed to use 'pytorch_data_generation_experimental'. "
-                        "The 'torch' package is missing.")  # pragma: no cover
+        msg = f"PyTorch and torchvision must be installed to use pytorch_data_generation_experimental. " + ("" if FOUND_TORCH else "The 'torch' package is missing. ") + ("" if FOUND_TORCHVISION else "The 'torchvision' package is missing. ") # pragma: no cover
+        Logger.critical(msg)  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/defaultdict.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/fw_agonstic/quantization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/keras/mctq_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,121 +12,127 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable
 from io import BytesIO
 
 import torch.nn
-import onnx
 
 from mct_quantizers import PytorchActivationQuantizationHolder, PytorchQuantizationWrapper
+from model_compression_toolkit.constants import FOUND_ONNX
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.exporter.model_exporter.pytorch.base_pytorch_exporter import BasePyTorchExporter
 from mct_quantizers import pytorch_quantizers
-from mct_quantizers.pytorch.metadata import add_onnx_metadata
 
-DEFAULT_ONNX_OPSET_VERSION=15
 
-
-class FakelyQuantONNXPyTorchExporter(BasePyTorchExporter):
-    """
-    Exporter for fakely-quant PyTorch models.
-    The exporter expects to receive an exportable model (where each layer's full quantization parameters
-    can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
-    format) and fake-quant layers for the activations.
-    """
-
-    def __init__(self,
-                 model: torch.nn.Module,
-                 is_layer_exportable_fn: Callable,
-                 save_model_path: str,
-                 repr_dataset: Callable,
-                 use_onnx_custom_quantizer_ops: bool = False,
-                 onnx_opset_version=DEFAULT_ONNX_OPSET_VERSION):
-        """
-
-        Args:
-            model: Model to export.
-            is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
-            save_model_path: Path to save the exported model.
-            repr_dataset: Representative dataset (needed for creating torch script).
-            use_onnx_custom_quantizer_ops: Whether to export quantizers custom ops in ONNX or not.
-            onnx_opset_version: ONNX opset version to use for exported ONNX model.
-        """
-
-        super().__init__(model,
-                         is_layer_exportable_fn,
-                         save_model_path,
-                         repr_dataset)
-
-        self._use_onnx_custom_quantizer_ops = use_onnx_custom_quantizer_ops
-        self._onnx_opset_version = onnx_opset_version
-
-    def export(self) -> None:
-        """
-        Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
-        (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
-
-        Returns:
-            Fake-quant PyTorch model.
-        """
-        for layer in self.model.children():
-            self.is_layer_exportable_fn(layer)
-
-        # Set forward that is used during onnx export.
-        # If _use_onnx_custom_quantizer_ops is set to True, the quantizer forward function will use
-        # the custom implementation when exporting the operator into onnx model. If not, it removes the
-        # wraps and quantizes the ops in place (for weights, for activation torch quantization function is
-        # exported since it's used during forward).
-        if self._use_onnx_custom_quantizer_ops:
-            self._enable_onnx_custom_ops_export()
-        else:
-            self._substitute_fully_quantized_model()
-
-        if self._use_onnx_custom_quantizer_ops:
-            Logger.info(f"Exporting onnx model with MCTQ quantizers: {self.save_model_path}")
-        else:
-            Logger.info(f"Exporting fake-quant onnx model: {self.save_model_path}")
-
-        model_input = to_torch_tensor(next(self.repr_dataset())[0])
-
-        if hasattr(self.model, 'metadata'):
-            onnx_bytes = BytesIO()
-            torch.onnx.export(self.model,
-                              model_input,
-                              onnx_bytes,
-                              opset_version=self._onnx_opset_version,
-                              verbose=False,
-                              input_names=['input'],
-                              output_names=['output'],
-                              dynamic_axes={'input': {0: 'batch_size'},
-                                            'output': {0: 'batch_size'}})
-            onnx_model = onnx.load_from_string(onnx_bytes.getvalue())
-            onnx_model = add_onnx_metadata(onnx_model, self.model.metadata)
-            onnx.save_model(onnx_model, self.save_model_path)
-        else:
-            torch.onnx.export(self.model,
-                              model_input,
-                              self.save_model_path,
-                              opset_version=self._onnx_opset_version,
-                              verbose=False,
-                              input_names=['input'],
-                              output_names=['output'],
-                              dynamic_axes={'input': {0: 'batch_size'},
-                                            'output': {0: 'batch_size'}})
-
-    def _enable_onnx_custom_ops_export(self):
-        """
-        Enable the custom implementation forward in quantizers, so it is exported
-        with custom quantizers.
-        """
-
-        for n, m in self.model.named_modules():
-            if isinstance(m, PytorchActivationQuantizationHolder):
-                assert isinstance(m.activation_holder_quantizer, pytorch_quantizers.BasePyTorchInferableQuantizer)
-                m.activation_holder_quantizer.enable_custom_impl()
-
-            if isinstance(m, PytorchQuantizationWrapper):
-                for wq in m.weights_quantizers.values():
-                    assert isinstance(wq, pytorch_quantizers.BasePyTorchInferableQuantizer)
-                    wq.enable_custom_impl()
+if FOUND_ONNX:
+    import onnx
+    from mct_quantizers.pytorch.metadata import add_onnx_metadata
+
+    class FakelyQuantONNXPyTorchExporter(BasePyTorchExporter):
+        """
+        Exporter for fakely-quant PyTorch models.
+        The exporter expects to receive an exportable model (where each layer's full quantization parameters
+        can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
+        format) and fake-quant layers for the activations.
+        """
+
+        def __init__(self,
+                     model: torch.nn.Module,
+                     is_layer_exportable_fn: Callable,
+                     save_model_path: str,
+                     repr_dataset: Callable,
+                     onnx_opset_version: int,
+                     use_onnx_custom_quantizer_ops: bool = False):
+            """
+
+            Args:
+                model: Model to export.
+                is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
+                save_model_path: Path to save the exported model.
+                repr_dataset: Representative dataset (needed for creating torch script).
+                onnx_opset_version: ONNX opset version to use for exported ONNX model.
+                use_onnx_custom_quantizer_ops: Whether to export quantizers custom ops in ONNX or not.
+            """
+
+            super().__init__(model,
+                             is_layer_exportable_fn,
+                             save_model_path,
+                             repr_dataset)
+
+            self._use_onnx_custom_quantizer_ops = use_onnx_custom_quantizer_ops
+            self._onnx_opset_version = onnx_opset_version
+
+        def export(self) -> None:
+            """
+            Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
+            (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
+
+            Returns:
+                Fake-quant PyTorch model.
+            """
+            for layer in self.model.children():
+                self.is_layer_exportable_fn(layer)
+
+            # Set forward that is used during onnx export.
+            # If _use_onnx_custom_quantizer_ops is set to True, the quantizer forward function will use
+            # the custom implementation when exporting the operator into onnx model. If not, it removes the
+            # wraps and quantizes the ops in place (for weights, for activation torch quantization function is
+            # exported since it's used during forward).
+            if self._use_onnx_custom_quantizer_ops:
+                self._enable_onnx_custom_ops_export()
+            else:
+                self._substitute_fully_quantized_model()
+
+            if self._use_onnx_custom_quantizer_ops:
+                Logger.info(f"Exporting onnx model with MCTQ quantizers: {self.save_model_path}")
+            else:
+                Logger.info(f"Exporting fake-quant onnx model: {self.save_model_path}")
+
+            model_input = to_torch_tensor(next(self.repr_dataset())[0])
+
+            if hasattr(self.model, 'metadata'):
+                onnx_bytes = BytesIO()
+                torch.onnx.export(self.model,
+                                  model_input,
+                                  onnx_bytes,
+                                  opset_version=self._onnx_opset_version,
+                                  verbose=False,
+                                  input_names=['input'],
+                                  output_names=['output'],
+                                  dynamic_axes={'input': {0: 'batch_size'},
+                                                'output': {0: 'batch_size'}})
+                onnx_model = onnx.load_from_string(onnx_bytes.getvalue())
+                onnx_model = add_onnx_metadata(onnx_model, self.model.metadata)
+                onnx.save_model(onnx_model, self.save_model_path)
+            else:
+                torch.onnx.export(self.model,
+                                  model_input,
+                                  self.save_model_path,
+                                  opset_version=self._onnx_opset_version,
+                                  verbose=False,
+                                  input_names=['input'],
+                                  output_names=['output'],
+                                  dynamic_axes={'input': {0: 'batch_size'},
+                                                'output': {0: 'batch_size'}})
+
+        def _enable_onnx_custom_ops_export(self):
+            """
+            Enable the custom implementation forward in quantizers, so it is exported
+            with custom quantizers.
+            """
+
+            for n, m in self.model.named_modules():
+                if isinstance(m, PytorchActivationQuantizationHolder):
+                    assert isinstance(m.activation_holder_quantizer, pytorch_quantizers.BasePyTorchInferableQuantizer)
+                    m.activation_holder_quantizer.enable_custom_impl()
+
+                if isinstance(m, PytorchQuantizationWrapper):
+                    for wq in m.weights_quantizers.values():
+                        assert isinstance(wq, pytorch_quantizers.BasePyTorchInferableQuantizer)
+                        wq.enable_custom_impl()
+
+else:
+    def FakelyQuantONNXPyTorchExporter(*args, **kwargs):
+        Logger.critical("ONNX must be installed to use 'FakelyQuantONNXPyTorchExporter'. "
+                        "The 'onnx' package is missing.")  # pragma: no cover
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 from typing import Callable
 
 from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.exporter.model_exporter.fw_agonstic.quantization_format import QuantizationFormat
 from model_compression_toolkit.exporter.model_exporter.pytorch.export_serialization_format import \
     PytorchExportSerializationFormat
 from model_compression_toolkit.logger import Logger
-from model_compression_toolkit.target_platform_capabilities.target_platform import TargetPlatformCapabilities
+
+
+DEFAULT_ONNX_OPSET_VERSION = 15
 
 
 if FOUND_TORCH:
     import torch.nn
-    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_onnx_pytorch_exporter import \
-    FakelyQuantONNXPyTorchExporter, DEFAULT_ONNX_OPSET_VERSION
-    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_torchscript_pytorch_exporter import \
-        FakelyQuantTorchScriptPyTorchExporter
+    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_onnx_pytorch_exporter import FakelyQuantONNXPyTorchExporter
+    from model_compression_toolkit.exporter.model_exporter.pytorch.fakely_quant_torchscript_pytorch_exporter import FakelyQuantTorchScriptPyTorchExporter
     from model_compression_toolkit.exporter.model_wrapper.pytorch.validate_layer import is_pytorch_layer_exportable
 
     supported_serialization_quantization_export_dict = {
         PytorchExportSerializationFormat.TORCHSCRIPT: [QuantizationFormat.FAKELY_QUANT],
         PytorchExportSerializationFormat.ONNX: [QuantizationFormat.FAKELY_QUANT, QuantizationFormat.MCTQ]
     }
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/fw_agnostic/get_inferable_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/gptq/runner.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/logger.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/metadata.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/keras/pruning_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/keras/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/pruning/pytorch/pruning_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/pruning/pytorch/pruning_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/ptq/runner.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/common/qat_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/symmetric_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/lsq/uniform_lsq.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/immutable.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1_pot/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tp_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -148,27 +148,14 @@
     """
     # Create a QuantizationConfigOptions, which defines a set
     # of possible configurations to consider when quantizing a set of operations (in mixed-precision, for example).
     # If the QuantizationConfigOptions contains only one configuration,
     # this configuration will be used for the operation quantization:
     default_configuration_options = tp.QuantizationConfigOptions([default_config])
 
-    # Create a QuantizationConfigOptions for quantizing constants in functional ops.
-    # Constant configuration is similar to the default eight bit configuration except for PoT
-    # quantization method for the constant.
-    # Since the constants are not named attributes of the layer, we use the default_weight_attr_config to
-    # define the desired quantization properties for them.
-    const_config = default_config.clone_and_edit(
-        default_weight_attr_config=default_config.default_weight_attr_config.clone_and_edit(
-            enable_weights_quantization=True))
-    if not (const_config.default_weight_attr_config.weights_quantization_method == tp.QuantizationMethod.POWER_OF_TWO and
-            const_config.default_weight_attr_config.weights_per_channel_threshold is False):
-        mct.logger.Logger.error('Constant quantization config should be per-tensor PoT.')
-    const_configuration_options = tp.QuantizationConfigOptions([const_config])
-
     # Create a TargetPlatformModel and set its default quantization config.
     # This default configuration will be used for all operations
     # unless specified otherwise (see OperatorsSet, for example):
     generated_tpm = tp.TargetPlatformModel(default_configuration_options, add_metadata=True, name=name)
 
     # To start defining the model's components (such as operator sets, and fusing patterns),
     # use 'with' the TargetPlatformModel instance, and create them as below:
@@ -194,18 +181,18 @@
         # Define operator sets that use mixed_precision_configuration_options:
         conv = tp.OperatorsSet("Conv", mixed_precision_configuration_options)
         fc = tp.OperatorsSet("FullyConnected", mixed_precision_configuration_options)
 
         # Define operations sets without quantization configuration
         # options (useful for creating fusing patterns, for example):
         any_relu = tp.OperatorsSet("AnyReLU")
-        add = tp.OperatorsSet("Add", const_configuration_options)
-        sub = tp.OperatorsSet("Sub", const_configuration_options)
-        mul = tp.OperatorsSet("Mul", const_configuration_options)
-        div = tp.OperatorsSet("Div", const_configuration_options)
+        add = tp.OperatorsSet("Add")
+        sub = tp.OperatorsSet("Sub")
+        mul = tp.OperatorsSet("Mul")
+        div = tp.OperatorsSet("Div")
         prelu = tp.OperatorsSet("PReLU")
         swish = tp.OperatorsSet("Swish")
         sigmoid = tp.OperatorsSet("Sigmoid")
         tanh = tp.OperatorsSet("Tanh")
 
         # Combine multiple operators into a single operator to avoid quantization between
         # them. To do this we define fusing patterns using the OperatorsSets that were created.
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tp_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,27 +147,14 @@
     """
     # Create a QuantizationConfigOptions, which defines a set
     # of possible configurations to consider when quantizing a set of operations (in mixed-precision, for example).
     # If the QuantizationConfigOptions contains only one configuration,
     # this configuration will be used for the operation quantization:
     default_configuration_options = tp.QuantizationConfigOptions([default_config])
 
-    # Create a QuantizationConfigOptions for quantizing constants in functional ops.
-    # Constant configuration is similar to the default eight bit configuration except for PoT
-    # quantization method for the constant.
-    # Since the constants are not named attributes of the layer, we use the default_weight_attr_config to
-    # define the desired quantization properties for them.
-    const_config = default_config.clone_and_edit(
-        default_weight_attr_config=default_config.default_weight_attr_config.clone_and_edit(
-            enable_weights_quantization=True))
-    if not (const_config.default_weight_attr_config.weights_quantization_method == tp.QuantizationMethod.POWER_OF_TWO and
-            const_config.default_weight_attr_config.weights_per_channel_threshold is False):
-        mct.logger.Logger.error('Constant quantization config should be per-tensor PoT.')
-    const_configuration_options = tp.QuantizationConfigOptions([const_config])
-
     # Create a TargetPlatformModel and set its default quantization config.
     # This default configuration will be used for all operations
     # unless specified otherwise (see OperatorsSet, for example):
     generated_tpm = tp.TargetPlatformModel(default_configuration_options, add_metadata=True, name=name)
 
     # To start defining the model's components (such as operator sets, and fusing patterns),
     # use 'with' the TargetPlatformModel instance, and create them as below:
@@ -191,18 +178,18 @@
         # Define operator sets that use mixed_precision_configuration_options:
         conv = tp.OperatorsSet("Conv", mixed_precision_configuration_options)
         fc = tp.OperatorsSet("FullyConnected", mixed_precision_configuration_options)
 
         # Define operations sets without quantization configuration
         # options (useful for creating fusing patterns, for example):
         any_relu = tp.OperatorsSet("AnyReLU")
-        add = tp.OperatorsSet("Add", const_configuration_options)
-        sub = tp.OperatorsSet("Sub", const_configuration_options)
-        mul = tp.OperatorsSet("Mul", const_configuration_options)
-        div = tp.OperatorsSet("Div", const_configuration_options)
+        add = tp.OperatorsSet("Add")
+        sub = tp.OperatorsSet("Sub")
+        mul = tp.OperatorsSet("Mul")
+        div = tp.OperatorsSet("Div")
         prelu = tp.OperatorsSet("PReLU")
         swish = tp.OperatorsSet("Swish")
         sigmoid = tp.OperatorsSet("Sigmoid")
         tanh = tp.OperatorsSet("Tanh")
 
         # Combine multiple operators into a single operator to avoid quantization between
         # them. To do this we define fusing patterns using the OperatorsSets that were created.
```

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v2_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/constants.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/load_model.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-2.0.0.20240510.421/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-2.0.0.20240509.406/setup.py` & `mct-nightly-2.0.0.20240510.421/setup.py`

 * *Files identical despite different names*

