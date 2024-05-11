# Comparing `tmp/paradance-0.4.8.tar.gz` & `tmp/paradance-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradance-0.4.8.tar", max compression
+gzip compressed data, was "paradance-0.4.9.tar", max compression
```

## Comparing `paradance-0.4.8.tar` & `paradance-0.4.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2023-09-05 13:42:40.066553 paradance-0.4.8/LICENSE
--rw-r--r--   0        0        0     1403 2024-03-14 02:53:00.152563 paradance-0.4.8/README.md
--rw-r--r--   0        0        0     1214 2024-03-20 09:53:12.759441 paradance-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      157 2024-03-18 02:46:04.558833 paradance-0.4.8/src/paradance/__init__.py
--rw-r--r--   0        0        0      211 2024-03-18 02:46:04.559311 paradance-0.4.8/src/paradance/dataloader/__init__.py
--rw-r--r--   0        0        0     5427 2024-03-18 02:46:04.560057 paradance-0.4.8/src/paradance/dataloader/base.py
--rw-r--r--   0        0        0     1084 2024-03-18 02:46:04.560166 paradance-0.4.8/src/paradance/dataloader/load_config.py
--rw-r--r--   0        0        0     1453 2024-03-18 02:46:04.560338 paradance-0.4.8/src/paradance/dataloader/load_csv.py
--rw-r--r--   0        0        0     1422 2024-03-18 02:46:04.560517 paradance-0.4.8/src/paradance/dataloader/load_excel.py
--rw-r--r--   0        0        0      225 2024-03-15 09:04:12.105095 paradance-0.4.8/src/paradance/evaluation/__init__.py
--rw-r--r--   0        0        0     1058 2023-09-06 22:42:02.517216 paradance-0.4.8/src/paradance/evaluation/auc_triple_parameters_evaluator.py
--rw-r--r--   0        0        0     2017 2024-03-18 02:46:04.560783 paradance-0.4.8/src/paradance/evaluation/base_calculator.py
--rw-r--r--   0        0        0     5147 2024-03-18 02:46:04.560987 paradance-0.4.8/src/paradance/evaluation/calculator.py
--rw-r--r--   0        0        0     2171 2024-03-08 05:57:47.721822 paradance-0.4.8/src/paradance/evaluation/distinct_portfolio_evaluator.py
--rw-r--r--   0        0        0     4588 2024-03-15 09:04:17.211942 paradance-0.4.8/src/paradance/evaluation/inverse_pair_evaluator.py
--rw-r--r--   0        0        0      463 2023-09-06 22:42:02.518308 paradance-0.4.8/src/paradance/evaluation/log_mse_evaluator.py
--rw-r--r--   0        0        0     1689 2024-03-18 06:58:52.562487 paradance-0.4.8/src/paradance/evaluation/logarithm_pca_calculator.py
--rw-r--r--   0        0        0      781 2023-09-08 16:12:38.464108 paradance-0.4.8/src/paradance/evaluation/neg_rank_ratio_evaluator.py
--rw-r--r--   0        0        0     1925 2024-03-08 05:57:47.722034 paradance-0.4.8/src/paradance/evaluation/portfolio_evaluator.py
--rw-r--r--   0        0        0     2956 2023-12-25 11:16:45.191926 paradance-0.4.8/src/paradance/evaluation/tau_evaluator.py
--rw-r--r--   0        0        0     2441 2023-12-25 11:16:45.192984 paradance-0.4.8/src/paradance/evaluation/woauc_evaluator.py
--rw-r--r--   0        0        0     1372 2024-03-14 02:53:00.154767 paradance-0.4.8/src/paradance/evaluation/wuauc_evaluator.py
--rw-r--r--   0        0        0      207 2024-03-15 08:55:30.647753 paradance-0.4.8/src/paradance/optimization/__init__.py
--rw-r--r--   0        0        0     6761 2024-03-18 02:46:04.561282 paradance-0.4.8/src/paradance/optimization/base.py
--rw-r--r--   0        0        0     5156 2024-03-20 03:44:56.223265 paradance-0.4.8/src/paradance/optimization/construct_weights.py
--rw-r--r--   0        0        0     2935 2024-03-18 02:46:04.561723 paradance-0.4.8/src/paradance/optimization/evaluate_targets.py
--rw-r--r--   0        0        0      827 2023-09-08 05:57:18.230023 paradance-0.4.8/src/paradance/optimization/get_processors.py
--rw-r--r--   0        0        0     5787 2024-03-20 03:52:08.937188 paradance-0.4.8/src/paradance/optimization/multiple_objective.py
--rw-r--r--   0        0        0     2056 2024-03-18 02:46:04.562095 paradance-0.4.8/src/paradance/optimization/optimize_parallel.py
--rw-r--r--   0        0        0     5094 2024-03-18 02:46:04.562282 paradance-0.4.8/src/paradance/optimization/save_study.py
--rw-r--r--   0        0        0     1041 2023-09-11 09:36:36.398890 paradance-0.4.8/src/paradance/optimization/set_path.py
--rw-r--r--   0        0        0      208 2024-03-18 02:46:04.562441 paradance-0.4.8/src/paradance/pipeline/__init__.py
--rw-r--r--   0        0        0     3582 2024-03-20 07:13:28.457804 paradance-0.4.8/src/paradance/pipeline/base.py
--rw-r--r--   0        0        0     2944 2024-03-18 02:46:04.562632 paradance-0.4.8/src/paradance/pipeline/classical.py
--rw-r--r--   0        0        0     2373 2024-03-20 08:57:15.983155 paradance-0.4.8/src/paradance/pipeline/logarithm_pca.py
--rw-r--r--   0        0        0      174 2023-09-05 13:42:40.070975 paradance-0.4.8/src/paradance/sampling/__init__.py
--rw-r--r--   0        0        0     1068 2023-09-05 13:42:40.071067 paradance-0.4.8/src/paradance/sampling/base.py
--rw-r--r--   0        0        0     1383 2023-09-05 13:42:40.071153 paradance-0.4.8/src/paradance/sampling/frequency_sampler.py
--rw-r--r--   0        0        0     2510 2023-09-05 13:42:40.071252 paradance-0.4.8/src/paradance/sampling/gini_sampler.py
--rw-r--r--   0        0        0      371 2023-09-05 13:42:40.071386 paradance-0.4.8/src/paradance/visualization/__init__.py
--rw-r--r--   0        0        0     8779 2023-09-05 13:42:40.071516 paradance-0.4.8/src/paradance/visualization/lorenz_curve.py
--rw-r--r--   0        0        0     3371 2023-09-05 13:42:40.071617 paradance-0.4.8/src/paradance/visualization/plot_trisurf.py
--rw-r--r--   0        0        0     3664 2023-09-05 13:42:40.071709 paradance-0.4.8/src/paradance/visualization/portfolio_curve.py
--rw-r--r--   0        0        0     3929 2023-09-05 13:42:40.071835 paradance-0.4.8/src/paradance/visualization/venn2.py
--rw-r--r--   0        0        0     6601 2023-09-05 13:42:40.071906 paradance-0.4.8/src/paradance/visualization/venn3.py
--rw-r--r--   0        0        0     2758 2023-09-05 13:42:40.071988 paradance-0.4.8/src/paradance/visualization/venn_base.py
--rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 paradance-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-09-05 13:42:40.066553 paradance-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1403 2024-03-14 02:53:00.152563 paradance-0.4.9/README.md
+-rw-r--r--   0        0        0     1214 2024-03-20 11:07:17.928366 paradance-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      157 2024-03-18 02:46:04.558833 paradance-0.4.9/src/paradance/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-18 02:46:04.559311 paradance-0.4.9/src/paradance/dataloader/__init__.py
+-rw-r--r--   0        0        0     5427 2024-03-18 02:46:04.560057 paradance-0.4.9/src/paradance/dataloader/base.py
+-rw-r--r--   0        0        0     1084 2024-03-18 02:46:04.560166 paradance-0.4.9/src/paradance/dataloader/load_config.py
+-rw-r--r--   0        0        0     1453 2024-03-18 02:46:04.560338 paradance-0.4.9/src/paradance/dataloader/load_csv.py
+-rw-r--r--   0        0        0     1422 2024-03-18 02:46:04.560517 paradance-0.4.9/src/paradance/dataloader/load_excel.py
+-rw-r--r--   0        0        0      225 2024-03-15 09:04:12.105095 paradance-0.4.9/src/paradance/evaluation/__init__.py
+-rw-r--r--   0        0        0     1058 2023-09-06 22:42:02.517216 paradance-0.4.9/src/paradance/evaluation/auc_triple_parameters_evaluator.py
+-rw-r--r--   0        0        0     2017 2024-03-18 02:46:04.560783 paradance-0.4.9/src/paradance/evaluation/base_calculator.py
+-rw-r--r--   0        0        0     5147 2024-03-18 02:46:04.560987 paradance-0.4.9/src/paradance/evaluation/calculator.py
+-rw-r--r--   0        0        0     2171 2024-03-08 05:57:47.721822 paradance-0.4.9/src/paradance/evaluation/distinct_portfolio_evaluator.py
+-rw-r--r--   0        0        0     4588 2024-03-15 09:04:17.211942 paradance-0.4.9/src/paradance/evaluation/inverse_pair_evaluator.py
+-rw-r--r--   0        0        0      463 2023-09-06 22:42:02.518308 paradance-0.4.9/src/paradance/evaluation/log_mse_evaluator.py
+-rw-r--r--   0        0        0     1689 2024-03-18 06:58:52.562487 paradance-0.4.9/src/paradance/evaluation/logarithm_pca_calculator.py
+-rw-r--r--   0        0        0      781 2023-09-08 16:12:38.464108 paradance-0.4.9/src/paradance/evaluation/neg_rank_ratio_evaluator.py
+-rw-r--r--   0        0        0     1925 2024-03-08 05:57:47.722034 paradance-0.4.9/src/paradance/evaluation/portfolio_evaluator.py
+-rw-r--r--   0        0        0     2956 2023-12-25 11:16:45.191926 paradance-0.4.9/src/paradance/evaluation/tau_evaluator.py
+-rw-r--r--   0        0        0     2441 2023-12-25 11:16:45.192984 paradance-0.4.9/src/paradance/evaluation/woauc_evaluator.py
+-rw-r--r--   0        0        0     1372 2024-03-14 02:53:00.154767 paradance-0.4.9/src/paradance/evaluation/wuauc_evaluator.py
+-rw-r--r--   0        0        0      207 2024-03-15 08:55:30.647753 paradance-0.4.9/src/paradance/optimization/__init__.py
+-rw-r--r--   0        0        0     6761 2024-03-18 02:46:04.561282 paradance-0.4.9/src/paradance/optimization/base.py
+-rw-r--r--   0        0        0     5156 2024-03-20 03:44:56.223265 paradance-0.4.9/src/paradance/optimization/construct_weights.py
+-rw-r--r--   0        0        0     2935 2024-03-18 02:46:04.561723 paradance-0.4.9/src/paradance/optimization/evaluate_targets.py
+-rw-r--r--   0        0        0      827 2023-09-08 05:57:18.230023 paradance-0.4.9/src/paradance/optimization/get_processors.py
+-rw-r--r--   0        0        0     5787 2024-03-20 03:52:08.937188 paradance-0.4.9/src/paradance/optimization/multiple_objective.py
+-rw-r--r--   0        0        0     2056 2024-03-18 02:46:04.562095 paradance-0.4.9/src/paradance/optimization/optimize_parallel.py
+-rw-r--r--   0        0        0     5094 2024-03-18 02:46:04.562282 paradance-0.4.9/src/paradance/optimization/save_study.py
+-rw-r--r--   0        0        0     1041 2023-09-11 09:36:36.398890 paradance-0.4.9/src/paradance/optimization/set_path.py
+-rw-r--r--   0        0        0      208 2024-03-18 02:46:04.562441 paradance-0.4.9/src/paradance/pipeline/__init__.py
+-rw-r--r--   0        0        0     3582 2024-03-20 07:13:28.457804 paradance-0.4.9/src/paradance/pipeline/base.py
+-rw-r--r--   0        0        0     2944 2024-03-18 02:46:04.562632 paradance-0.4.9/src/paradance/pipeline/classical.py
+-rw-r--r--   0        0        0     2373 2024-03-20 08:57:15.983155 paradance-0.4.9/src/paradance/pipeline/logarithm_pca.py
+-rw-r--r--   0        0        0      174 2023-09-05 13:42:40.070975 paradance-0.4.9/src/paradance/sampling/__init__.py
+-rw-r--r--   0        0        0     1068 2023-09-05 13:42:40.071067 paradance-0.4.9/src/paradance/sampling/base.py
+-rw-r--r--   0        0        0     1383 2023-09-05 13:42:40.071153 paradance-0.4.9/src/paradance/sampling/frequency_sampler.py
+-rw-r--r--   0        0        0     2510 2023-09-05 13:42:40.071252 paradance-0.4.9/src/paradance/sampling/gini_sampler.py
+-rw-r--r--   0        0        0      371 2023-09-05 13:42:40.071386 paradance-0.4.9/src/paradance/visualization/__init__.py
+-rw-r--r--   0        0        0     8779 2023-09-05 13:42:40.071516 paradance-0.4.9/src/paradance/visualization/lorenz_curve.py
+-rw-r--r--   0        0        0     3371 2023-09-05 13:42:40.071617 paradance-0.4.9/src/paradance/visualization/plot_trisurf.py
+-rw-r--r--   0        0        0     3664 2023-09-05 13:42:40.071709 paradance-0.4.9/src/paradance/visualization/portfolio_curve.py
+-rw-r--r--   0        0        0     3929 2023-09-05 13:42:40.071835 paradance-0.4.9/src/paradance/visualization/venn2.py
+-rw-r--r--   0        0        0     6601 2023-09-05 13:42:40.071906 paradance-0.4.9/src/paradance/visualization/venn3.py
+-rw-r--r--   0        0        0     2758 2023-09-05 13:42:40.071988 paradance-0.4.9/src/paradance/visualization/venn_base.py
+-rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 paradance-0.4.9/PKG-INFO
```

### Comparing `paradance-0.4.8/LICENSE` & `paradance-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/README.md` & `paradance-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/pyproject.toml` & `paradance-0.4.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paradance"
-version = "0.4.8"
+version = "0.4.9"
 description = "Offers a toolset for comprehensive, multi-faceted large-scale data analysis and optimizations."
 authors = ["Yin Cheng <yin.sjtu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/yinsn/paradance"
 repository = "https://github.com/yinsn/paradance"
 packages = [{ include = "paradance", from = "src" }]
@@ -13,15 +13,15 @@
 imageio = "^2.34.0"
 ipykernel = "^6.29.3"
 ipywidgets = "^8.1.2"
 joblib = "^1.3.2"
 jupyter = "^1.0.0"
 matplotlib = "^3.8.3"
 matplotlib-venn = "^0.11.10"
-mixician = "^0.1.13"
+mixician = "^0.1.14"
 numpy = "^1.26.4"
 openpyxl = "^3.1.2"
 optuna = "^3.5.0"
 pandas = "^2.2.1"
 pydantic = "^2.6.4"
 python = "^3.9"
 scikit-learn = "^1.4.1.post1"
```

### Comparing `paradance-0.4.8/src/paradance/dataloader/base.py` & `paradance-0.4.9/src/paradance/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/dataloader/load_config.py` & `paradance-0.4.9/src/paradance/dataloader/load_config.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/dataloader/load_csv.py` & `paradance-0.4.9/src/paradance/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/dataloader/load_excel.py` & `paradance-0.4.9/src/paradance/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/auc_triple_parameters_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/auc_triple_parameters_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/base_calculator.py` & `paradance-0.4.9/src/paradance/evaluation/base_calculator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/calculator.py` & `paradance-0.4.9/src/paradance/evaluation/calculator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/distinct_portfolio_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/distinct_portfolio_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/inverse_pair_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/inverse_pair_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/logarithm_pca_calculator.py` & `paradance-0.4.9/src/paradance/evaluation/logarithm_pca_calculator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/neg_rank_ratio_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/neg_rank_ratio_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/portfolio_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/portfolio_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/tau_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/tau_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/woauc_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/woauc_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/evaluation/wuauc_evaluator.py` & `paradance-0.4.9/src/paradance/evaluation/wuauc_evaluator.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/base.py` & `paradance-0.4.9/src/paradance/optimization/base.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/construct_weights.py` & `paradance-0.4.9/src/paradance/optimization/construct_weights.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/evaluate_targets.py` & `paradance-0.4.9/src/paradance/optimization/evaluate_targets.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/get_processors.py` & `paradance-0.4.9/src/paradance/optimization/get_processors.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/multiple_objective.py` & `paradance-0.4.9/src/paradance/optimization/multiple_objective.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/optimize_parallel.py` & `paradance-0.4.9/src/paradance/optimization/optimize_parallel.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/save_study.py` & `paradance-0.4.9/src/paradance/optimization/save_study.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/optimization/set_path.py` & `paradance-0.4.9/src/paradance/optimization/set_path.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/pipeline/base.py` & `paradance-0.4.9/src/paradance/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/pipeline/classical.py` & `paradance-0.4.9/src/paradance/pipeline/classical.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/pipeline/logarithm_pca.py` & `paradance-0.4.9/src/paradance/pipeline/logarithm_pca.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/sampling/base.py` & `paradance-0.4.9/src/paradance/sampling/base.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/sampling/frequency_sampler.py` & `paradance-0.4.9/src/paradance/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/sampling/gini_sampler.py` & `paradance-0.4.9/src/paradance/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/visualization/lorenz_curve.py` & `paradance-0.4.9/src/paradance/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/visualization/plot_trisurf.py` & `paradance-0.4.9/src/paradance/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/visualization/portfolio_curve.py` & `paradance-0.4.9/src/paradance/visualization/portfolio_curve.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/visualization/venn2.py` & `paradance-0.4.9/src/paradance/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/visualization/venn3.py` & `paradance-0.4.9/src/paradance/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/src/paradance/visualization/venn_base.py` & `paradance-0.4.9/src/paradance/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `paradance-0.4.8/PKG-INFO` & `paradance-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradance
-Version: 0.4.8
+Version: 0.4.9
 Summary: Offers a toolset for comprehensive, multi-faceted large-scale data analysis and optimizations.
 Home-page: https://github.com/yinsn/paradance
 License: MIT
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: imageio (>=2.34.0,<3.0.0)
 Requires-Dist: ipykernel (>=6.29.3,<7.0.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: matplotlib-venn (>=0.11.10,<0.12.0)
-Requires-Dist: mixician (>=0.1.13,<0.2.0)
+Requires-Dist: mixician (>=0.1.14,<0.2.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: optuna (>=3.5.0,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
```

