# Comparing `tmp/auto_circuit-0.1.3.tar.gz` & `tmp/auto_circuit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_circuit-0.1.3.tar", max compression
+gzip compressed data, was "auto_circuit-0.1.4.tar", max compression
```

## Comparing `auto_circuit-0.1.3.tar` & `auto_circuit-0.1.4.tar`

### file list

```diff
@@ -1,62 +1,56 @@
--rw-r--r--   0        0        0     1276 2024-05-08 23:47:50.241213 auto_circuit-0.1.3/README.md
--rw-r--r--   0        0        0    14880 2024-05-08 23:47:50.241213 auto_circuit-0.1.3/auto_circuit/data.py
--rw-r--r--   0        0        0     8438 2024-05-08 23:47:50.241213 auto_circuit-0.1.3/auto_circuit/experiment_utils.py
--rw-r--r--   0        0        0    10338 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/experiments.py
--rw-r--r--   0        0        0    13917 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/language_rotations.py
--rw-r--r--   0        0        0     6259 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/area_under_curve.py
--rw-r--r--   0        0        0     3741 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/avoid_edges.py
--rw-r--r--   0        0        0     9754 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py
--rw-r--r--   0        0        0     8595 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py
--rw-r--r--   0        0        0     8888 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/docstring_official.py
--rw-r--r--   0        0        0     5322 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py
--rw-r--r--   0        0        0    11697 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/ioi_official.py
--rw-r--r--   0        0        0     8481 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py
--rw-r--r--   0        0        0     4896 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py
--rw-r--r--   0        0        0     4648 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py
--rw-r--r--   0        0        0     4396 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/measure_roc.py
--rw-r--r--   0        0        0     4070 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/roc_plot.py
--rw-r--r--   0        0        0     2091 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff.py
--rw-r--r--   0        0        0     5344 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff_percent.py
--rw-r--r--   0        0        0     2208 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_value.py
--rw-r--r--   0        0        0     2709 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/correct_answer_percent.py
--rw-r--r--   0        0        0     2264 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/kl_div.py
--rw-r--r--   0        0        0     7097 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py
--rw-r--r--   0        0        0     6360 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics.py
--rw-r--r--   0        0        0     3896 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py
--rw-r--r--   0        0        0     6359 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/metrics/prune_scores_similarity.py
--rw-r--r--   0        0        0     5426 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/micro_model_utils.py
--rw-r--r--   0        0        0     6135 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py
--rw-r--r--   0        0        0    11781 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py
--rw-r--r--   0        0        0     7190 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py
--rw-r--r--   0        0        0     9123 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/projector_transformer.py
--rw-r--r--   0        0        0     5846 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector.py
--rw-r--r--   0        0        0    12255 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector_training.py
--rw-r--r--   0        0        0     7950 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/tracr_model_utils.py
--rw-r--r--   0        0        0     7694 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/model_utils/transformer_lens_utils.py
--rw-r--r--   0        0        0    14863 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/playground.py
--rw-r--r--   0        0        0     5123 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune.py
--rw-r--r--   0        0        0     7888 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/ACDC.py
--rw-r--r--   0        0        0     1718 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/activation_magnitude.py
--rw-r--r--   0        0        0     3759 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/circuit_probing.py
--rw-r--r--   0        0        0     4373 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/edge_attribution_patching.py
--rw-r--r--   0        0        0     1054 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/ground_truth.py
--rw-r--r--   0        0        0     5064 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/mask_gradient.py
--rw-r--r--   0        0        0     2699 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/parameter_integrated_gradients.py
--rw-r--r--   0        0        0    10248 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/prune_algos.py
--rw-r--r--   0        0        0      994 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/random_edges.py
--rw-r--r--   0        0        0    11955 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/prune_algos/subnetwork_probing.py
--rw-r--r--   0        0        0     7465 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/pythia-2_8b-sports.py
--rw-r--r--   0        0        0    16984 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/tasks.py
--rw-r--r--   0        0        0     3729 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/tracr_experiments.py
--rw-r--r--   0        0        0    11715 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/types.py
--rw-r--r--   0        0        0     6091 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/uniqueness_experiments.py
--rw-r--r--   0        0        0     6775 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/ablation_activations.py
--rw-r--r--   0        0        0      590 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/custom_tqdm.py
--rw-r--r--   0        0        0    19341 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/graph_utils.py
--rw-r--r--   0        0        0     7165 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/misc.py
--rw-r--r--   0        0        0     6295 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/patch_wrapper.py
--rw-r--r--   0        0        0     9609 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/patchable_model.py
--rw-r--r--   0        0        0     9933 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/utils/tensor_ops.py
--rw-r--r--   0        0        0    11460 2024-05-08 23:47:50.245213 auto_circuit-0.1.3/auto_circuit/visualize.py
--rw-r--r--   0        0        0     1397 2024-05-08 23:49:49.105869 auto_circuit-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 auto_circuit-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1465 2024-05-11 19:46:07.777976 auto_circuit-0.1.4/README.md
+-rw-r--r--   0        0        0    14880 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/data.py
+-rw-r--r--   0        0        0     8406 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/experiment_utils.py
+-rw-r--r--   0        0        0     6259 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/area_under_curve.py
+-rw-r--r--   0        0        0     3741 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/avoid_edges.py
+-rw-r--r--   0        0        0     9754 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py
+-rw-r--r--   0        0        0     8595 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py
+-rw-r--r--   0        0        0     8888 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/docstring_official.py
+-rw-r--r--   0        0        0     5322 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py
+-rw-r--r--   0        0        0    11697 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/ioi_official.py
+-rw-r--r--   0        0        0     8481 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py
+-rw-r--r--   0        0        0     4896 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py
+-rw-r--r--   0        0        0     4648 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py
+-rw-r--r--   0        0        0     4396 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/measure_roc.py
+-rw-r--r--   0        0        0     4070 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/roc_plot.py
+-rw-r--r--   0        0        0     2091 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/answer_diff.py
+-rw-r--r--   0        0        0     5344 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/answer_diff_percent.py
+-rw-r--r--   0        0        0     2208 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/answer_value.py
+-rw-r--r--   0        0        0     2709 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/correct_answer_percent.py
+-rw-r--r--   0        0        0     2264 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/kl_div.py
+-rw-r--r--   0        0        0     7097 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py
+-rw-r--r--   0        0        0     6360 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/prune_metrics.py
+-rw-r--r--   0        0        0     3896 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py
+-rw-r--r--   0        0        0     6359 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/metrics/prune_scores_similarity.py
+-rw-r--r--   0        0        0     5426 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/micro_model_utils.py
+-rw-r--r--   0        0        0     6135 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py
+-rw-r--r--   0        0        0    11781 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py
+-rw-r--r--   0        0        0     7190 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py
+-rw-r--r--   0        0        0     9123 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/task_projectors/projector_transformer.py
+-rw-r--r--   0        0        0     5846 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/task_projectors/task_projector.py
+-rw-r--r--   0        0        0    12255 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/task_projectors/task_projector_training.py
+-rw-r--r--   0        0        0     7950 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/tracr_model_utils.py
+-rw-r--r--   0        0        0     7694 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/model_utils/transformer_lens_utils.py
+-rw-r--r--   0        0        0     5135 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune.py
+-rw-r--r--   0        0        0     7932 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/ACDC.py
+-rw-r--r--   0        0        0     1718 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/activation_magnitude.py
+-rw-r--r--   0        0        0     3759 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/circuit_probing.py
+-rw-r--r--   0        0        0     4373 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/edge_attribution_patching.py
+-rw-r--r--   0        0        0     1054 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/ground_truth.py
+-rw-r--r--   0        0        0     5064 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/mask_gradient.py
+-rw-r--r--   0        0        0     2699 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/parameter_integrated_gradients.py
+-rw-r--r--   0        0        0    10248 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/prune_algos.py
+-rw-r--r--   0        0        0      994 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/random_edges.py
+-rw-r--r--   0        0        0    11955 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/prune_algos/subnetwork_probing.py
+-rw-r--r--   0        0        0    16984 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/tasks.py
+-rw-r--r--   0        0        0    11715 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/types.py
+-rw-r--r--   0        0        0     6775 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/ablation_activations.py
+-rw-r--r--   0        0        0      590 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/custom_tqdm.py
+-rw-r--r--   0        0        0    19408 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/graph_utils.py
+-rw-r--r--   0        0        0     7165 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/misc.py
+-rw-r--r--   0        0        0     6295 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/patch_wrapper.py
+-rw-r--r--   0        0        0    10564 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/patchable_model.py
+-rw-r--r--   0        0        0     9933 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/utils/tensor_ops.py
+-rw-r--r--   0        0        0    13620 2024-05-11 19:46:07.781976 auto_circuit-0.1.4/auto_circuit/visualize.py
+-rw-r--r--   0        0        0     1397 2024-05-11 19:48:06.712140 auto_circuit-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 auto_circuit-0.1.4/PKG-INFO
```

### Comparing `auto_circuit-0.1.3/README.md` & `auto_circuit-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 
 ## Getting Started
 
 ```bash
 pip install auto-circuit
 ```
 
-## Easy and Efficient Edge Patching
+### Easy and Efficient Edge Patching
 https://github.com/UFO-101/auto-circuit/blob/03ce552ccdea98fc6fed3b05cfb2df9b0eb4e323/experiments/demos/zero_ablate_an_edge.py#L20-L26
 
-## Different Ablation Methods
+### Different Ablation Methods
 https://github.com/UFO-101/auto-circuit/blob/03ce552ccdea98fc6fed3b05cfb2df9b0eb4e323/experiments/demos/patch_an_edge.py#L37
 
-## Automatic Circuit Discovery
+### Automatic Circuit Discovery
 https://github.com/UFO-101/auto-circuit/blob/03ce552ccdea98fc6fed3b05cfb2df9b0eb4e323/experiments/demos/patch_an_edge.py#L49-L55
+
+### Visualization
+https://github.com/UFO-101/auto-circuit/blob/5777057b445d55b7d4695eed8aface9d6bcefbe3/experiments/demos/patch_some_edges.py#L49
+![](docs/assets/Small_Circuit_Viz.png)
```

### Comparing `auto_circuit-0.1.3/auto_circuit/data.py` & `auto_circuit-0.1.4/auto_circuit/data.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/experiment_utils.py` & `auto_circuit-0.1.4/auto_circuit/experiment_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,14 @@
         model=patchable_gpt2,
         dataloader=test_loader,
         test_edge_counts=[test_edge_counts],
         prune_scores=circuit_ps,
         patch_type=patch_type,
         ablation_type=ablation_type,
         render_graph=False,
-        render_all_edges=False,
     )
     (
         logit_diff_percent_mean,
         logit_diff_percent_std,
         logit_diff_percents,
     ) = answer_diff_percent(
         patchable_gpt2,
```

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/area_under_curve.py` & `auto_circuit-0.1.4/auto_circuit/metrics/area_under_curve.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/avoid_edges.py` & `auto_circuit-0.1.4/auto_circuit/metrics/avoid_edges.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py` & `auto_circuit-0.1.4/auto_circuit/metrics/completeness_metrics/same_under_knockouts.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py` & `auto_circuit-0.1.4/auto_circuit/metrics/completeness_metrics/train_same_under_knockouts.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/docstring_official.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/docstring_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/greaterthan_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/ioi_official.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/ioi_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/sports_players_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/tracr/reverse_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/circuits/tracr/xproportion_official.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/measure_roc.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/measure_roc.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/official_circuits/roc_plot.py` & `auto_circuit-0.1.4/auto_circuit/metrics/official_circuits/roc_plot.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/answer_diff.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_diff_percent.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/answer_diff_percent.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/answer_value.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/answer_value.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/correct_answer_percent.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/correct_answer_percent.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/kl_div.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/kl_div.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/measure_prune_metrics.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/prune_metrics.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_metrics/prune_metrics_plot.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/metrics/prune_scores_similarity.py` & `auto_circuit-0.1.4/auto_circuit/metrics/prune_scores_similarity.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/micro_model_utils.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/micro_model_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/sparse_autoencoders/autoencoder_training.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/sparse_autoencoders/autoencoder_transformer.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/sparse_autoencoders/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/projector_transformer.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/task_projectors/projector_transformer.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/task_projectors/task_projector.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/task_projectors/task_projector_training.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/task_projectors/task_projector_training.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/tracr_model_utils.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/tracr_model_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/model_utils/transformer_lens_utils.py` & `auto_circuit-0.1.4/auto_circuit/model_utils/transformer_lens_utils.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune.py` & `auto_circuit-0.1.4/auto_circuit/prune.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,30 +27,30 @@
     dataloader: PromptDataLoader,
     test_edge_counts: List[int],
     prune_scores: PruneScores,
     patch_type: PatchType = PatchType.EDGE_PATCH,
     ablation_type: AblationType = AblationType.RESAMPLE,
     reverse_clean_corrupt: bool = False,
     render_graph: bool = False,
-    render_all_edges: bool = False,
+    render_score_threshold: bool = False,
     render_file_path: Optional[str] = None,
 ) -> CircuitOutputs:
     """Run the model, pruning edges based on the given `prune_scores`. Runs the model
     over the given `dataloader` for each `test_edge_count`.
 
     Args:
         model: The model to run
         dataloader: The dataloader to use for input and patches
         test_edge_counts: The numbers of edges to prune.
         prune_scores: The scores that determine the ordering of edges for pruning
         patch_type: Whether to patch the circuit or the complement.
         ablation_type: The type of ablation to use.
         reverse_clean_corrupt: Reverse clean and corrupt (for input and patches).
         render_graph: Whether to render the graph using `draw_seq_graph`.
-        render_all_edges: Whether to render all edges, if `render_graph` is `True`.
+        render_score_threshold: Edge score threshold, if `render_graph` is `True`.
         render_file_path: Path to save the rendered graph, if `render_graph` is `True`.
 
     Returns:
         A dictionary mapping from the number of pruned edges to a
             [`BatchOutputs`][auto_circuit.types.BatchOutputs] object, which is a
             dictionary mapping from [`BatchKey`s][auto_circuit.types.BatchKey] to output
             tensors.
@@ -99,14 +99,14 @@
                         patch_edge_count += (1 - dest.patch_mask.int()).sum().item()
                 with t.inference_mode():
                     model_output = model(batch_input)[model.out_slice]
                 circ_outs[patch_edge_count][batch.key] = model_output.detach().clone()
             if render_graph:
                 draw_seq_graph(
                     model=model,
-                    show_all_edges=render_all_edges,
+                    score_threshold=render_score_threshold,
                     show_all_seq_pos=False,
                     seq_labels=dataloader.seq_labels,
                     file_path=render_file_path,
                 )
     del patch_src_outs
     return circ_outs
```

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/ACDC.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/ACDC.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from copy import deepcopy
 from itertools import product
 from random import random
 from typing import Callable, List, Literal, Optional, Set
 
 import torch as t
 from ordered_set import OrderedSet
+from plotly import graph_objects as go
 from torch.nn.functional import log_softmax, mse_loss
 
 from auto_circuit.data import PromptDataLoader
 from auto_circuit.types import (
     CircuitOutputs,
     Edge,
     PatchType,
@@ -31,15 +32,15 @@
     official_edges: Optional[Set[Edge]],
     tao_exps: List[int] = list(range(-5, -1)),
     tao_bases: List[int] = [1, 3, 5, 7, 9],
     faithfulness_target: Literal["kl_div", "mse"] = "kl_div",
     test_mode: bool = False,
     run_circuits_ref: Optional[Callable[..., CircuitOutputs]] = None,
     show_graphs: bool = False,
-    draw_seq_graph_ref: Optional[Callable[..., None]] = None,
+    draw_seq_graph_ref: Optional[Callable[..., go.Figure]] = None,
 ) -> PruneScores:
     """
     Run the ACDC algorithm from the paper "Towards Automated Circuit Discovery for
     Mechanistic Interpretability"
     ([Conmy et al. (2023)](https://arxiv.org/abs/2304.14997)).
 
     The algorithm does not assign scores to each edge, instead it finds the edges to be
```

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/activation_magnitude.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/activation_magnitude.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/circuit_probing.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/circuit_probing.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/edge_attribution_patching.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/edge_attribution_patching.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/ground_truth.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/ground_truth.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/mask_gradient.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/mask_gradient.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/parameter_integrated_gradients.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/parameter_integrated_gradients.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/prune_algos.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/prune_algos.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/random_edges.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/random_edges.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/prune_algos/subnetwork_probing.py` & `auto_circuit-0.1.4/auto_circuit/prune_algos/subnetwork_probing.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/tasks.py` & `auto_circuit-0.1.4/auto_circuit/tasks.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/types.py` & `auto_circuit-0.1.4/auto_circuit/types.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/ablation_activations.py` & `auto_circuit-0.1.4/auto_circuit/utils/ablation_activations.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/custom_tqdm.py` & `auto_circuit-0.1.4/auto_circuit/utils/custom_tqdm.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/graph_utils.py` & `auto_circuit-0.1.4/auto_circuit/utils/graph_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,15 @@
 
     Warning:
         This function modifies the state of the model! This is a likely source of bugs.
     """
     if curr_src_outs is None:
         curr_src_outs = t.zeros_like(patch_src_outs)
 
+    # TODO: Raise an error if one of the edge names doesn't exist.
     if edges is not None:
         set_all_masks(model, val=0.0)
         for edge in model.edges:
             if edge in edges or edge.name in edges:
                 edge.patch_mask(model).data[edge.patch_idx] = 1.0
 
     for wrapper in model.wrappers:
```

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/misc.py` & `auto_circuit-0.1.4/auto_circuit/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/patch_wrapper.py` & `auto_circuit-0.1.4/auto_circuit/utils/patch_wrapper.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/patchable_model.py` & `auto_circuit-0.1.4/auto_circuit/utils/patchable_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, List, Optional, Set, Tuple
+from collections import defaultdict
+from typing import Any, Collection, Dict, List, Optional, Set, Tuple
 
 import torch as t
 from transformer_lens.past_key_value_caching import HookedTransformerKeyValueCache
 
 from auto_circuit.types import DestNode, Edge, Node, PruneScores, SrcNode
 from auto_circuit.utils.patch_wrapper import PatchWrapperImpl
 
@@ -56,14 +57,15 @@
         wrapped_model: The model to wrap which is being made patchable.
     """
 
     nodes: Set[Node]
     srcs: Set[SrcNode]
     dests: Set[DestNode]
     edge_dict: Dict[int | None, List[Edge]]  # Key is token position or None for all
+    edge_name_dict: Dict[int | None, Dict[str, Edge]]
     edges: Set[Edge]
     n_edges: int
     seq_dim: int
     seq_len: Optional[int]
     wrappers: Set[PatchWrapperImpl]
     src_wrappers: Set[PatchWrapperImpl]
     dest_wrappers: Set[PatchWrapperImpl]
@@ -97,14 +99,17 @@
         super().__init__()
         self.nodes = nodes
         self.srcs = srcs
         self.dests = dests
         self.edge_dict = edge_dict
         self.edges = edges
         self.n_edges = len(edges)
+        self.edge_name_dict = defaultdict(dict)
+        for edge in edges:
+            self.edge_name_dict[edge.seq_idx][edge.name] = edge
         self.seq_dim = seq_dim
         self.seq_len = seq_len
         self.wrappers = wrappers
         self.src_wrappers = src_wrappers
         self.dest_wrappers = dest_wrappers
         self.patch_masks = {}
         for dest_wrapper in self.dest_wrappers:
@@ -175,33 +180,50 @@
             A new [`PruneScores`][auto_circuit.types.PruneScores] instance.
         """
         prune_scores: PruneScores = {}
         for (mod_name, mask) in self.patch_masks.items():
             prune_scores[mod_name] = t.full_like(mask.data, init_val)
         return prune_scores
 
-    def circuit_prune_scores(self, edges: Set[Edge], bool: bool = False) -> PruneScores:
+    def circuit_prune_scores(
+        self,
+        edges: Optional[Collection[Edge | str]] = None,
+        edge_dict: Optional[Dict[Edge, float] | Dict[str, float]] = None,
+        bool: bool = False,
+    ) -> PruneScores:
         """
         Convert a set of edges to a corresponding
         [`PruneScores`][auto_circuit.types.PruneScores] object.
 
         Args:
-            edges: The set of edges to convert to prune scores.
+            edges: The set of edges or edge names to convert to prune scores.
             bool: Whether to return the prune scores as boolean type tensors.
 
         Returns:
             The prune scores corresponding to the set of edges.
         """
-        prune_scores = self.new_prune_scores()
-        for edge in edges:
-            prune_scores[edge.dest.module_name][edge.patch_idx] = 1.0
+        ps = self.new_prune_scores()
+        assert not (edges is None and edge_dict is None), "Must specify edges"
+
+        # TODO: Raise an error if one of the edge names doesn't exist.
+        if edges is not None:
+            for edge in self.edges:
+                if edge in edges or edge.name in edges:
+                    ps[edge.dest.module_name][edge.patch_idx] = 1.0
+        else:
+            assert edge_dict is not None
+            for e in self.edges:
+                if e in edge_dict.keys():
+                    ps[e.dest.module_name][e.patch_idx] = edge_dict[e]  # type: ignore
+                if e.name in edge_dict.keys():
+                    ps[e.dest.module_name][e.patch_idx] = edge_dict[e]  # type: ignore
         if bool:
-            return dict([(mod, mask.bool()) for (mod, mask) in prune_scores.items()])
+            return dict([(mod, mask.bool()) for (mod, mask) in ps.items()])
         else:
-            return prune_scores
+            return ps
 
     def current_patch_masks_as_prune_scores(self) -> PruneScores:
         """
         Convert the current patch masks to a corresponding
         [`PruneScores`][auto_circuit.types.PruneScores] object.
 
         Returns:
```

### Comparing `auto_circuit-0.1.3/auto_circuit/utils/tensor_ops.py` & `auto_circuit-0.1.4/auto_circuit/utils/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `auto_circuit-0.1.3/pyproject.toml` & `auto_circuit-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-circuit"
-version = "0.1.3"  # This isn't used. Version set during Github action.
+version = "0.1.4"  # This isn't used. Version set during Github action.
 description = ""
 authors = ["UFO-101 <josephmiller101@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auto_circuit"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `auto_circuit-0.1.3/PKG-INFO` & `auto_circuit-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-circuit
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: UFO-101
 Author-email: josephmiller101@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -35,16 +35,20 @@
 
 ## Getting Started
 
 ```bash
 pip install auto-circuit
 ```
 
-## Easy and Efficient Edge Patching
+### Easy and Efficient Edge Patching
 https://github.com/UFO-101/auto-circuit/blob/03ce552ccdea98fc6fed3b05cfb2df9b0eb4e323/experiments/demos/zero_ablate_an_edge.py#L20-L26
 
-## Different Ablation Methods
+### Different Ablation Methods
 https://github.com/UFO-101/auto-circuit/blob/03ce552ccdea98fc6fed3b05cfb2df9b0eb4e323/experiments/demos/patch_an_edge.py#L37
 
-## Automatic Circuit Discovery
+### Automatic Circuit Discovery
 https://github.com/UFO-101/auto-circuit/blob/03ce552ccdea98fc6fed3b05cfb2df9b0eb4e323/experiments/demos/patch_an_edge.py#L49-L55
 
+### Visualization
+https://github.com/UFO-101/auto-circuit/blob/5777057b445d55b7d4695eed8aface9d6bcefbe3/experiments/demos/patch_some_edges.py#L49
+![](docs/assets/Small_Circuit_Viz.png)
+
```

