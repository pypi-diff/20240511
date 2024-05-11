# Comparing `tmp/sy_riskmodels-0.0.7.tar.gz` & `tmp/sy_riskmodels-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sy_riskmodels-0.0.7.tar", last modified: Wed May  8 03:16:07 2024, max compression
+gzip compressed data, was "sy_riskmodels-0.0.8.tar", last modified: Sat May 11 03:37:31 2024, max compression
```

## Comparing `sy_riskmodels-0.0.7.tar` & `sy_riskmodels-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 03:16:07.469816 sy_riskmodels-0.0.7/
--rw-rw-rw-   0        0        0     1084 2022-10-17 15:08:18.000000 sy_riskmodels-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5775 2024-05-08 03:16:07.469816 sy_riskmodels-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     5123 2022-11-03 09:30:24.000000 sy_riskmodels-0.0.7/README.md
--rw-rw-rw-   0        0        0      596 2024-05-08 03:15:49.000000 sy_riskmodels-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-08 03:16:07.469816 sy_riskmodels-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-08 03:16:07.445728 sy_riskmodels-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-08 03:16:07.457826 sy_riskmodels-0.0.7/src/riskmodels/
--rw-rw-rw-   0        0        0     1032 2024-05-08 03:13:12.000000 sy_riskmodels-0.0.7/src/riskmodels/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:16:07.457826 sy_riskmodels-0.0.7/src/riskmodels/contrib/
--rw-rw-rw-   0        0        0        0 2022-10-19 08:42:16.000000 sy_riskmodels-0.0.7/src/riskmodels/contrib/__init__.py
--rw-rw-rw-   0        0        0    13485 2023-09-03 15:09:23.000000 sy_riskmodels-0.0.7/src/riskmodels/contrib/build_scorecard.py
--rw-rw-rw-   0        0        0     1623 2024-05-08 01:19:02.000000 sy_riskmodels-0.0.7/src/riskmodels/contrib/var_select.py
--rw-rw-rw-   0        0        0     4241 2024-05-08 01:19:02.000000 sy_riskmodels-0.0.7/src/riskmodels/detector.py
--rw-rw-rw-   0        0        0     9080 2023-09-03 15:09:23.000000 sy_riskmodels-0.0.7/src/riskmodels/evaluate.py
--rw-rw-rw-   0        0        0     4162 2023-09-03 15:09:23.000000 sy_riskmodels-0.0.7/src/riskmodels/logging.py
--rw-rw-rw-   0        0        0     3044 2023-09-03 07:52:41.000000 sy_riskmodels-0.0.7/src/riskmodels/models.py
--rw-rw-rw-   0        0        0     2713 2023-09-03 15:09:23.000000 sy_riskmodels-0.0.7/src/riskmodels/rule.py
--rw-rw-rw-   0        0        0    52640 2024-05-08 03:13:12.000000 sy_riskmodels-0.0.7/src/riskmodels/scorecard.py
--rw-rw-rw-   0        0        0     3422 2022-10-21 05:55:38.000000 sy_riskmodels-0.0.7/src/riskmodels/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-08 03:16:07.465820 sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/
--rw-rw-rw-   0        0        0     5775 2024-05-08 03:16:07.000000 sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      560 2024-05-08 03:16:07.000000 sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 03:16:07.000000 sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 03:16:07.000000 sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 03:16:07.465820 sy_riskmodels-0.0.7/test/
--rw-rw-rw-   0        0        0      563 2023-09-03 15:09:23.000000 sy_riskmodels-0.0.7/test/test_detect.py
--rw-rw-rw-   0        0        0     1837 2023-09-03 07:52:42.000000 sy_riskmodels-0.0.7/test/test_scorecard.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:37:31.154415 sy_riskmodels-0.0.8/
+-rw-rw-rw-   0        0        0     1084 2022-10-17 15:08:18.000000 sy_riskmodels-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5775 2024-05-11 03:37:31.153415 sy_riskmodels-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5123 2022-11-03 09:30:24.000000 sy_riskmodels-0.0.8/README.md
+-rw-rw-rw-   0        0        0      596 2024-05-11 03:34:00.000000 sy_riskmodels-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-11 03:37:31.154415 sy_riskmodels-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-11 03:37:31.132788 sy_riskmodels-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-11 03:37:31.145414 sy_riskmodels-0.0.8/src/sy_riskmodels/
+-rw-rw-rw-   0        0        0     1080 2024-05-11 03:34:00.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:37:31.151423 sy_riskmodels-0.0.8/src/sy_riskmodels/contrib/
+-rw-rw-rw-   0        0        0        0 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/contrib/__init__.py
+-rw-rw-rw-   0        0        0    13850 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/contrib/build_scorecard.py
+-rw-rw-rw-   0        0        0     1632 2024-05-11 03:34:00.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/contrib/var_select.py
+-rw-rw-rw-   0        0        0     4241 2024-05-11 03:34:00.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/detector.py
+-rw-rw-rw-   0        0        0     9356 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/evaluate.py
+-rw-rw-rw-   0        0        0     4294 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/logging.py
+-rw-rw-rw-   0        0        0     3463 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/models.py
+-rw-rw-rw-   0        0        0     2814 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/rule.py
+-rw-rw-rw-   0        0        0    52100 2024-05-11 03:34:00.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/scorecard.py
+-rw-rw-rw-   0        0        0     3556 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/src/sy_riskmodels/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 03:37:31.153415 sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/
+-rw-rw-rw-   0        0        0     5775 2024-05-11 03:37:31.000000 sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      593 2024-05-11 03:37:31.000000 sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 03:37:31.000000 sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-11 03:37:31.000000 sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-11 03:37:31.152415 sy_riskmodels-0.0.8/test/
+-rw-rw-rw-   0        0        0      591 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/test/test_detect.py
+-rw-rw-rw-   0        0        0     1908 2024-05-11 03:33:59.000000 sy_riskmodels-0.0.8/test/test_scorecard.py
```

### Comparing `sy_riskmodels-0.0.7/LICENSE` & `sy_riskmodels-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sy_riskmodels-0.0.7/PKG-INFO` & `sy_riskmodels-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sy-riskmodels
-Version: 0.0.7
+Name: sy_riskmodels
+Version: 0.0.8
 Summary: 信用风险模型工具包
 Author-email: YAO Siyuan <siyuan89@163.com>
 Project-URL: Homepage, https://github.com/siyuany/riskmodels
 Project-URL: Bug Tracker, https://github.com/siyuany/riskmodels/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sy_riskmodels-0.0.7/README.md` & `sy_riskmodels-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/__init__.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-__version__ = '0.0.7'
+# -*- encoding: utf-8 -*-
+__version__ = '0.0.8'
 
-import riskmodels.contrib as contrib
-import riskmodels.detector as detector
-import riskmodels.evaluate as evaluate
-import riskmodels.logging as logging
-import riskmodels.models as models
-import riskmodels.scorecard as scorecard
-import riskmodels.utils as utils
+import sy_riskmodels.contrib as contrib
+import sy_riskmodels.detector as detector
+import sy_riskmodels.evaluate as evaluate
+import sy_riskmodels.logging as logging
+import sy_riskmodels.models as models
+import sy_riskmodels.scorecard as scorecard
+import sy_riskmodels.utils as utils
 from .detector import detect
 from .evaluate import gains_table
 from .evaluate import ks_score
 from .evaluate import model_eval
 from .models import stepwise_lr
 from .scorecard import make_scorecard
 from .scorecard import woebin
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/contrib/build_scorecard.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/contrib/build_scorecard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-# -*- encoding: utf-8 -*-
-import os
-
-import numpy as np
-import pandas as pd
-import statsmodels.api as sm
-from pandas.io.excel import ExcelWriter
-from statsmodels.stats.outliers_influence import variance_inflation_factor
-
-from riskmodels.contrib.var_select import risk_trends_consistency
-from riskmodels.evaluate import (model_eval, gains_table, psi,
-                                 swap_analysis_simple)
-from riskmodels.models import group_split_cv, stepwise_lr
-from riskmodels.scorecard import (make_scorecard, sc_bins_to_df, woebin,
-                                  woebin_plot, woebin_ply, woebin_psi)
-from riskmodels.utils import str_to_list, sample_stats
-
-
-def build_scorecard(sample_df,
-                    features,
-                    target,
-                    train_filter,
-                    oot_filter,
-                    output_excel_file,
-                    variable_iv_limit=0.02,
-                    sample_stat_group_fields=None,
-                    alternative_target=None,
-                    regression_p_limit=0.05,
-                    random_test_set=0.2,
-                    special_values=None,
-                    binning_methods=None,
-                    binning_kwargs=None,
-                    cv=None,
-                    base_points=600,
-                    base_odds=50,
-                    pdo=20,
-                    compare_model_fields=None,
-                    random_state=0):
-    """
-
-    Args:
-        sample_df:
-        features:
-        target:
-        train_filter:
-        oot_filter:
-        output_excel_file:
-        variable_iv_limit:
-        sample_stat_group_fields:
-        alternative_target:
-        regression_p_limit:
-        random_test_set:
-        special_values:
-        binning_methods:
-        binning_kwargs:
-        cv:
-        base_points:
-        base_odds:
-        pdo:
-        compare_model_fields:
-        random_state:
-
-    Returns:
-
-    """
-    if binning_methods is None:
-        binning_methods = ['quantile', 'tree']
-
-    if cv is None:
-        cv = 3
-
-    # check features
-    features = list(set(features).intersection(sample_df.columns.tolist()))
-
-    # check target
-    assert target in sample_df.columns.tolist(), f'数据集中不存在目标字段{target}'
-
-    # open excel file
-    excel_file = ExcelWriter(output_excel_file)
-
-    # 1. 样本统计
-    if sample_stat_group_fields is not None:
-        sample_stat_group_fields = str_to_list(sample_stat_group_fields)
-        sample_stat_group_fields = list(
-            set(sample_stat_group_fields).intersection(
-                sample_df.columns.tolist()))
-
-    row_cnt = 0
-    if sample_stat_group_fields:
-        for field in sample_stat_group_fields:
-            tmp_df = sample_df.groupby(field).apply(sample_stats, target=target)
-            tmp_df.to_excel(excel_file, sheet_name=f'样本统计', startrow=row_cnt)
-            row_cnt += len(tmp_df) + 2
-
-    # 2. 样本拆分
-    sample_df['_train_test_flag_'] = np.where(
-        train_filter(sample_df), '01_train',
-        np.where(oot_filter(sample_df), '03_oot', ''))
-
-    rng = np.random.default_rng(random_state)
-
-    if random_test_set:
-
-        sample_df['_rand_'] = rng.random(len(sample_df))
-        sample_df['_train_test_flag_'] = np.where(
-            (sample_df['_train_test_flag_'] == '01_train') &
-            (sample_df['_rand_'] < random_test_set), '02_test',
-            sample_df['_train_test_flag_'])
-
-    tmp_df = sample_df.groupby('_train_test_flag_').apply(sample_stats,
-                                                          target=target)
-    tmp_df.to_excel(excel_file, sheet_name='样本统计', startrow=row_cnt)
-
-    train_df = sample_df[(sample_df['_train_test_flag_'] == '01_train') &
-                         (sample_df[target].isin([0, 1]))].copy().reset_index(
-                             drop=True)
-    oot_df = sample_df[(sample_df['_train_test_flag_'] == '03_oot') &
-                       (sample_df[target].isin([0, 1]))].copy().reset_index(
-                           drop=True)
-
-    # 3. 变量分箱
-    if binning_kwargs is None:
-        binning_kwargs = {}
-    bins = woebin(train_df,
-                  x=features,
-                  y=target,
-                  special_values=special_values,
-                  methods=binning_methods,
-                  **binning_kwargs)
-    woe_df, iv_df = sc_bins_to_df(bins)
-    woe_df.to_excel(excel_file, sheet_name='WOE分析', index_label='index')
-    iv_df.to_excel(excel_file, sheet_name='IV分析', index_label='变量')
-
-    # 变量筛选
-    selected_variables = iv_df[
-        (iv_df['IV'] > variable_iv_limit) &
-        iv_df['单调性'].isin(['increasing', 'decreasing'])].index.tolist()
-
-    var_risk_consist = risk_trends_consistency(
-        oot_df, sc_bins={v: bins[v] for v in selected_variables}, target=target)
-    selected_variables = [k for k, v in var_risk_consist.items() if v == 1.0]
-
-    # 4.逐步回归
-    train_X = woebin_ply(train_df[selected_variables], bins, value='woe')
-    train_y = train_df[target]
-
-    _, selected_variables = stepwise_lr(
-        train_X,
-        train_y.values,
-        cv=(lambda: group_split_cv(train_df[cv]))
-        if isinstance(cv, str) else cv,
-        x=[f + '_woe' for f in selected_variables],
-        max_num_features=30)
-
-    print(f'selected variables: {",".join(selected_variables)}')
-
-    # 5. fine tuning
-    while True:
-        X = train_X[selected_variables].copy()
-        X = sm.add_constant(X)
-        lr_model = sm.GLM(endog=train_y, exog=X, family=sm.families.Binomial())
-        lr_model_result = lr_model.fit()
-
-        if np.any(lr_model_result.params > 0) or np.any(
-                lr_model_result.pvalues > regression_p_limit):
-            t_values = lr_model_result.tvalues
-            rm_var = t_values.index[t_values == t_values.max()].item()
-            selected_variables.remove(rm_var)
-        else:
-            break
-
-    print(selected_variables)
-    print(lr_model_result.summary())
-    model_summary = pd.DataFrame(
-        {'': lr_model_result.summary().as_text().split('\n')})
-    model_summary.to_excel(excel_file,
-                           sheet_name='模型表达',
-                           index=False,
-                           header=False)
-
-    # 计算VIF
-    vif = {}
-    for idx, feature in enumerate(X.columns[1:].tolist()):
-        vif[feature] = variance_inflation_factor(train_X, idx)
-    vif = pd.Series(vif).rename('VIF').to_frame()
-    vif = vif.loc[selected_variables,]
-    print(vif)
-    vif.to_excel(excel_file,
-                 sheet_name='模型表达',
-                 index=False,
-                 startcol=11,
-                 startrow=14)
-
-    scorecard = make_scorecard(bins,
-                               lr_model_result.params.to_dict(),
-                               base_points=base_points,
-                               base_odds=base_odds,
-                               pdo=pdo)
-    print(scorecard)
-    scorecard.to_excel(excel_file,
-                       sheet_name='模型表达',
-                       index=False,
-                       startrow=len(model_summary) + 3)
-
-    # 模型评估
-    all_sample_X = woebin_ply(
-        sample_df[[var[:-4] for var in selected_variables]], bins)
-    # 这一步非常重要！！
-    all_sample_X = all_sample_X[selected_variables]
-    all_sample_X = sm.add_constant(all_sample_X)
-
-    sample_df['prob'] = lr_model_result.predict(all_sample_X)
-    perf = sample_df.groupby('_train_test_flag_').apply(model_eval,
-                                                        target=target,
-                                                        pred='prob')
-    print(perf)
-    perf.to_excel(excel_file, sheet_name='模型评估')
-
-    row_cnt = len(perf) + 2
-    if sample_stat_group_fields is not None:
-        for field in sample_stat_group_fields:
-            perf = sample_df.groupby(field).apply(model_eval,
-                                                  target=target,
-                                                  pred='prob')
-            print(perf)
-            perf.to_excel(excel_file, sheet_name='模型评估', startrow=row_cnt)
-            row_cnt += len(perf) + 2
-
-    A = pdo / np.log(2)
-    B = base_points - A * np.log(base_odds)
-
-    sample_df['score'] = np.round(A * np.log(
-        (1 - sample_df['prob']) / sample_df['prob']) + B)
-    train_df = sample_df[(sample_df['_train_test_flag_'] == '01_train') &
-                         sample_df[target].isin([0, 1])]
-    _, breaks = gains_table(train_df[target],
-                            train_df['score'],
-                            return_breaks=True)
-    breaks[0] = -np.inf
-    breaks[-1] = np.inf
-    train_gains_table = gains_table(train_df[target],
-                                    train_df['score'],
-                                    breaks=breaks)
-    pd.DataFrame(['Train Gains Table']).to_excel(excel_file,
-                                                 sheet_name='模型评估',
-                                                 index=False,
-                                                 header=False,
-                                                 startrow=row_cnt)
-    train_gains_table.to_excel(excel_file,
-                               sheet_name='模型评估',
-                               startrow=row_cnt + 1)
-    row_cnt += len(train_gains_table) + 3
-
-    if random_test_set:
-        test_df = sample_df[(sample_df['_train_test_flag_'] == '02_test') &
-                            sample_df[target].isin([0, 1])]
-        test_gains_table = gains_table(test_df[target],
-                                       test_df['score'],
-                                       breaks=breaks)
-        pd.DataFrame(['Test Gains Table']).to_excel(excel_file,
-                                                    sheet_name='模型评估',
-                                                    index=False,
-                                                    header=False,
-                                                    startrow=row_cnt)
-        test_gains_table.to_excel(excel_file,
-                                  sheet_name='模型评估',
-                                  startrow=row_cnt + 1)
-        row_cnt += len(train_gains_table) + 3
-
-    oot_df = sample_df[(sample_df['_train_test_flag_'] == '03_oot') &
-                       sample_df[target].isin([0, 1])]
-    oot_gains_table = gains_table(oot_df[target],
-                                  oot_df['score'],
-                                  breaks=breaks)
-    pd.DataFrame(['OOT Gains Table']).to_excel(excel_file,
-                                               sheet_name='模型评估',
-                                               index=False,
-                                               header=False,
-                                               startrow=row_cnt)
-    oot_gains_table.to_excel(excel_file,
-                             sheet_name='模型评估',
-                             startrow=row_cnt + 1)
-    row_cnt += len(oot_gains_table) + 3
-
-    # 其他标签
-    if alternative_target is not None:
-        alternative_target = str_to_list(alternative_target)
-
-        for y in alternative_target:
-            perf = sample_df.groupby('_train_test_flag_').apply(model_eval,
-                                                                target=y,
-                                                                pred='prob')
-            pd.DataFrame([y]).to_excel(excel_file,
-                                       sheet_name='模型评估',
-                                       index=False,
-                                       header=False,
-                                       startrow=row_cnt)
-            perf.to_excel(excel_file, sheet_name='模型评估', startrow=row_cnt + 1)
-            row_cnt += len(perf) + 3
-
-    # PSI
-    var_psi = woebin_psi(
-        train_df,
-        oot_df,
-        bins={
-            k: v for k, v in bins.items() if k + '_woe' in selected_variables
-        })
-    model_psi = pd.DataFrame({
-        'variable': 'model_score',
-        'bin': train_gains_table.index,
-        'base_distr': train_gains_table['TotalPercent'],
-        'cmp_distr': oot_gains_table['TotalPercent']
-    }).assign(psi=lambda x: psi(x['base_distr'], x['cmp_distr']))
-
-    psi_df = pd.concat([var_psi, model_psi], ignore_index=True)
-    print(psi_df)
-    psi_df.to_excel(excel_file, sheet_name='PSI分析', index=False)
-
-    # Swap分析（如有）
-    compare_model_fields = str_to_list(compare_model_fields)
-    row_cnt = 0
-    if compare_model_fields:
-        for model in compare_model_fields:
-            print(f'新模型 vs {model.upper()}\n')
-            swap_tbl = swap_analysis_simple(sample_df,
-                                            benchmark_model='score',
-                                            challenger_model=model,
-                                            target_col=target,
-                                            reject_ratio=0.2)
-            swap_tbl.to_excel(excel_file, sheet_name='Swap分析', startrow=row_cnt)
-            row_cnt += len(swap_tbl) + 5
-            print(swap_tbl, '\n\n')
-
-    excel_file.close()
-
-    woe_plots = woebin_plot({k[:-4]: bins[k[:-4]] for k in selected_variables})
-    if not os.path.exists('pic'):
-        os.mkdir('pic')
-
-    if not os.path.isdir('pic'):
-        raise NotADirectoryError('当前目录下pic路径不是目录，无法保存WOE图')
-    else:
-        for v, plt in woe_plots.items():
-            plt.savefig(f'pic/{v}.png')
+# -*- encoding: utf-8 -*-
+import os
+
+import numpy as np
+import pandas as pd
+import statsmodels.api as sm
+from pandas.io.excel import ExcelWriter
+from statsmodels.stats.outliers_influence import variance_inflation_factor
+
+from sy_riskmodels.contrib.var_select import risk_trends_consistency
+from sy_riskmodels.evaluate import (model_eval, gains_table, psi,
+                                    swap_analysis_simple)
+from sy_riskmodels.models import group_split_cv, stepwise_lr
+from sy_riskmodels.scorecard import (make_scorecard, sc_bins_to_df, woebin,
+                                     woebin_plot, woebin_ply, woebin_psi)
+from sy_riskmodels.utils import str_to_list, sample_stats
+
+
+def build_scorecard(sample_df,
+                    features,
+                    target,
+                    train_filter,
+                    oot_filter,
+                    output_excel_file,
+                    variable_iv_limit=0.02,
+                    sample_stat_group_fields=None,
+                    alternative_target=None,
+                    regression_p_limit=0.05,
+                    random_test_set=0.2,
+                    special_values=None,
+                    binning_methods=None,
+                    binning_kwargs=None,
+                    cv=None,
+                    base_points=600,
+                    base_odds=50,
+                    pdo=20,
+                    compare_model_fields=None,
+                    random_state=0):
+    """
+
+    Args:
+        sample_df:
+        features:
+        target:
+        train_filter:
+        oot_filter:
+        output_excel_file:
+        variable_iv_limit:
+        sample_stat_group_fields:
+        alternative_target:
+        regression_p_limit:
+        random_test_set:
+        special_values:
+        binning_methods:
+        binning_kwargs:
+        cv:
+        base_points:
+        base_odds:
+        pdo:
+        compare_model_fields:
+        random_state:
+
+    Returns:
+
+    """
+    if binning_methods is None:
+        binning_methods = ['quantile', 'tree']
+
+    if cv is None:
+        cv = 3
+
+    # check features
+    features = list(set(features).intersection(sample_df.columns.tolist()))
+
+    # check target
+    assert target in sample_df.columns.tolist(), f'数据集中不存在目标字段{target}'
+
+    # open excel file
+    excel_file = ExcelWriter(output_excel_file)
+
+    # 1. 样本统计
+    if sample_stat_group_fields is not None:
+        sample_stat_group_fields = str_to_list(sample_stat_group_fields)
+        sample_stat_group_fields = list(
+            set(sample_stat_group_fields).intersection(
+                sample_df.columns.tolist()))
+
+    row_cnt = 0
+    if sample_stat_group_fields:
+        for field in sample_stat_group_fields:
+            tmp_df = sample_df.groupby(field).apply(sample_stats, target=target)
+            tmp_df.to_excel(excel_file, sheet_name=f'样本统计', startrow=row_cnt)
+            row_cnt += len(tmp_df) + 2
+
+    # 2. 样本拆分
+    sample_df['_train_test_flag_'] = np.where(
+        train_filter(sample_df), '01_train',
+        np.where(oot_filter(sample_df), '03_oot', ''))
+
+    rng = np.random.default_rng(random_state)
+
+    if random_test_set:
+
+        sample_df['_rand_'] = rng.random(len(sample_df))
+        sample_df['_train_test_flag_'] = np.where(
+            (sample_df['_train_test_flag_'] == '01_train') &
+            (sample_df['_rand_'] < random_test_set), '02_test',
+            sample_df['_train_test_flag_'])
+
+    tmp_df = sample_df.groupby('_train_test_flag_').apply(sample_stats,
+                                                          target=target)
+    tmp_df.to_excel(excel_file, sheet_name='样本统计', startrow=row_cnt)
+
+    train_df = sample_df[(sample_df['_train_test_flag_'] == '01_train') &
+                         (sample_df[target].isin([0, 1]))].copy().reset_index(
+                             drop=True)
+    oot_df = sample_df[(sample_df['_train_test_flag_'] == '03_oot') &
+                       (sample_df[target].isin([0, 1]))].copy().reset_index(
+                           drop=True)
+
+    # 3. 变量分箱
+    if binning_kwargs is None:
+        binning_kwargs = {}
+    bins = woebin(train_df,
+                  x=features,
+                  y=target,
+                  special_values=special_values,
+                  methods=binning_methods,
+                  **binning_kwargs)
+    woe_df, iv_df = sc_bins_to_df(bins)
+    woe_df.to_excel(excel_file, sheet_name='WOE分析', index_label='index')
+    iv_df.to_excel(excel_file, sheet_name='IV分析', index_label='变量')
+
+    # 变量筛选
+    selected_variables = iv_df[
+        (iv_df['IV'] > variable_iv_limit) &
+        iv_df['单调性'].isin(['increasing', 'decreasing'])].index.tolist()
+
+    var_risk_consist = risk_trends_consistency(
+        oot_df, sc_bins={v: bins[v] for v in selected_variables}, target=target)
+    selected_variables = [k for k, v in var_risk_consist.items() if v == 1.0]
+
+    # 4.逐步回归
+    train_X = woebin_ply(train_df[selected_variables], bins, value='woe')
+    train_y = train_df[target]
+
+    _, selected_variables = stepwise_lr(
+        train_X,
+        train_y.values,
+        cv=(lambda: group_split_cv(train_df[cv]))
+        if isinstance(cv, str) else cv,
+        x=[f + '_woe' for f in selected_variables],
+        max_num_features=30)
+
+    print(f'selected variables: {",".join(selected_variables)}')
+
+    # 5. fine tuning
+    while True:
+        X = train_X[selected_variables].copy()
+        X = sm.add_constant(X)
+        lr_model = sm.GLM(endog=train_y, exog=X, family=sm.families.Binomial())
+        lr_model_result = lr_model.fit()
+
+        if np.any(lr_model_result.params > 0) or np.any(
+                lr_model_result.pvalues > regression_p_limit):
+            t_values = lr_model_result.tvalues
+            rm_var = t_values.index[t_values == t_values.max()].item()
+            selected_variables.remove(rm_var)
+        else:
+            break
+
+    print(selected_variables)
+    print(lr_model_result.summary())
+    model_summary = pd.DataFrame(
+        {'': lr_model_result.summary().as_text().split('\n')})
+    model_summary.to_excel(excel_file,
+                           sheet_name='模型表达',
+                           index=False,
+                           header=False)
+
+    # 计算VIF
+    vif = {}
+    for idx, feature in enumerate(X.columns[1:].tolist()):
+        vif[feature] = variance_inflation_factor(train_X, idx)
+    vif = pd.Series(vif).rename('VIF').to_frame()
+    vif = vif.loc[selected_variables,]
+    print(vif)
+    vif.to_excel(excel_file,
+                 sheet_name='模型表达',
+                 index=False,
+                 startcol=11,
+                 startrow=14)
+
+    scorecard = make_scorecard(bins,
+                               lr_model_result.params.to_dict(),
+                               base_points=base_points,
+                               base_odds=base_odds,
+                               pdo=pdo)
+    print(scorecard)
+    scorecard.to_excel(excel_file,
+                       sheet_name='模型表达',
+                       index=False,
+                       startrow=len(model_summary) + 3)
+
+    # 模型评估
+    all_sample_X = woebin_ply(
+        sample_df[[var[:-4] for var in selected_variables]], bins)
+    # 这一步非常重要！！
+    all_sample_X = all_sample_X[selected_variables]
+    all_sample_X = sm.add_constant(all_sample_X)
+
+    sample_df['prob'] = lr_model_result.predict(all_sample_X)
+    perf = sample_df.groupby('_train_test_flag_').apply(model_eval,
+                                                        target=target,
+                                                        pred='prob')
+    print(perf)
+    perf.to_excel(excel_file, sheet_name='模型评估')
+
+    row_cnt = len(perf) + 2
+    if sample_stat_group_fields is not None:
+        for field in sample_stat_group_fields:
+            perf = sample_df.groupby(field).apply(model_eval,
+                                                  target=target,
+                                                  pred='prob')
+            print(perf)
+            perf.to_excel(excel_file, sheet_name='模型评估', startrow=row_cnt)
+            row_cnt += len(perf) + 2
+
+    A = pdo / np.log(2)
+    B = base_points - A * np.log(base_odds)
+
+    sample_df['score'] = np.round(A * np.log(
+        (1 - sample_df['prob']) / sample_df['prob']) + B)
+    train_df = sample_df[(sample_df['_train_test_flag_'] == '01_train') &
+                         sample_df[target].isin([0, 1])]
+    _, breaks = gains_table(train_df[target],
+                            train_df['score'],
+                            return_breaks=True)
+    breaks[0] = -np.inf
+    breaks[-1] = np.inf
+    train_gains_table = gains_table(train_df[target],
+                                    train_df['score'],
+                                    breaks=breaks)
+    pd.DataFrame(['Train Gains Table']).to_excel(excel_file,
+                                                 sheet_name='模型评估',
+                                                 index=False,
+                                                 header=False,
+                                                 startrow=row_cnt)
+    train_gains_table.to_excel(excel_file,
+                               sheet_name='模型评估',
+                               startrow=row_cnt + 1)
+    row_cnt += len(train_gains_table) + 3
+
+    if random_test_set:
+        test_df = sample_df[(sample_df['_train_test_flag_'] == '02_test') &
+                            sample_df[target].isin([0, 1])]
+        test_gains_table = gains_table(test_df[target],
+                                       test_df['score'],
+                                       breaks=breaks)
+        pd.DataFrame(['Test Gains Table']).to_excel(excel_file,
+                                                    sheet_name='模型评估',
+                                                    index=False,
+                                                    header=False,
+                                                    startrow=row_cnt)
+        test_gains_table.to_excel(excel_file,
+                                  sheet_name='模型评估',
+                                  startrow=row_cnt + 1)
+        row_cnt += len(train_gains_table) + 3
+
+    oot_df = sample_df[(sample_df['_train_test_flag_'] == '03_oot') &
+                       sample_df[target].isin([0, 1])]
+    oot_gains_table = gains_table(oot_df[target],
+                                  oot_df['score'],
+                                  breaks=breaks)
+    pd.DataFrame(['OOT Gains Table']).to_excel(excel_file,
+                                               sheet_name='模型评估',
+                                               index=False,
+                                               header=False,
+                                               startrow=row_cnt)
+    oot_gains_table.to_excel(excel_file,
+                             sheet_name='模型评估',
+                             startrow=row_cnt + 1)
+    row_cnt += len(oot_gains_table) + 3
+
+    # 其他标签
+    if alternative_target is not None:
+        alternative_target = str_to_list(alternative_target)
+
+        for y in alternative_target:
+            perf = sample_df.groupby('_train_test_flag_').apply(model_eval,
+                                                                target=y,
+                                                                pred='prob')
+            pd.DataFrame([y]).to_excel(excel_file,
+                                       sheet_name='模型评估',
+                                       index=False,
+                                       header=False,
+                                       startrow=row_cnt)
+            perf.to_excel(excel_file, sheet_name='模型评估', startrow=row_cnt + 1)
+            row_cnt += len(perf) + 3
+
+    # PSI
+    var_psi = woebin_psi(
+        train_df,
+        oot_df,
+        bins={
+            k: v for k, v in bins.items() if k + '_woe' in selected_variables
+        })
+    model_psi = pd.DataFrame({
+        'variable': 'model_score',
+        'bin': train_gains_table.index,
+        'base_distr': train_gains_table['TotalPercent'],
+        'cmp_distr': oot_gains_table['TotalPercent']
+    }).assign(psi=lambda x: psi(x['base_distr'], x['cmp_distr']))
+
+    psi_df = pd.concat([var_psi, model_psi], ignore_index=True)
+    print(psi_df)
+    psi_df.to_excel(excel_file, sheet_name='PSI分析', index=False)
+
+    # Swap分析（如有）
+    compare_model_fields = str_to_list(compare_model_fields)
+    row_cnt = 0
+    if compare_model_fields:
+        for model in compare_model_fields:
+            print(f'新模型 vs {model.upper()}\n')
+            swap_tbl = swap_analysis_simple(sample_df,
+                                            benchmark_model='score',
+                                            challenger_model=model,
+                                            target_col=target,
+                                            reject_ratio=0.2)
+            swap_tbl.to_excel(excel_file, sheet_name='Swap分析', startrow=row_cnt)
+            row_cnt += len(swap_tbl) + 5
+            print(swap_tbl, '\n\n')
+
+    excel_file.close()
+
+    woe_plots = woebin_plot({k[:-4]: bins[k[:-4]] for k in selected_variables})
+    if not os.path.exists('pic'):
+        os.mkdir('pic')
+
+    if not os.path.isdir('pic'):
+        raise NotADirectoryError('当前目录下pic路径不是目录，无法保存WOE图')
+    else:
+        for v, plt in woe_plots.items():
+            plt.savefig(f'pic/{v}.png')
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/contrib/var_select.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/contrib/var_select.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- encoding: utf-8 -*-
 
 import pandas as pd
 
-from riskmodels.scorecard import woebin
-from riskmodels.scorecard import woebin_breaks
+from sy_riskmodels.scorecard import woebin
+from sy_riskmodels.scorecard import woebin_breaks
 
 
 def risk_trends_consistency(df, sc_bins, target):
     """
     判断变量在不同数据集上风险趋势与分箱结果中风险趋势是否一致
 
     Args:
         df: pd.DataFrame
-        sc_bins: riskmodels.scorecard.woebin 返回的结果
+        sc_bins: sy_riskmodels.scorecard.woebin 返回的结果
         target: 目标变量的列名
 
     Returns:
         {变量名: 分箱badprob序列的 Spearman 秩相关系数}，秩相关系数有效区间 [-1,1]；
         其中 -1 代表趋势完全相反，1 代表趋势完全一致。
 
     """
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/detector.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/detector.py`

 * *Files identical despite different names*

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/logging.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/logging.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,132 +1,132 @@
-# -*- encoding: utf-8 -*-
-"""
-logging.py: 日志模块
-"""
-
-import logging as _logging
-import sys
-from logging import DEBUG, INFO, WARN, ERROR, FATAL
-
-if sys.version_info[0] == 3 and sys.version_info[1] >= 8:
-    pass
-elif sys.version_info[0] == 3 and sys.version_info[1] in [6, 7]:
-    import io
-    import os
-    import traceback
-
-    def findCaller(self, stack_info=False, stacklevel=1):
-        """
-        Find the stack frame of the caller so that we can note the source
-        file name, line number and function name.
-        """
-        f = _logging.currentframe()
-        #On some versions of IronPython, currentframe() returns None if
-        #IronPython isn't run with -X:Frames.
-        if f is not None:
-            f = f.f_back
-        orig_f = f
-        while f and stacklevel > 1:
-            f = f.f_back
-            stacklevel -= 1
-        if not f:
-            f = orig_f
-        rv = "(unknown file)", 0, "(unknown function)", None
-        while hasattr(f, "f_code"):
-            co = f.f_code
-            filename = os.path.normcase(co.co_filename)
-            if filename == _logging._srcfile:
-                f = f.f_back
-                continue
-            sinfo = None
-            if stack_info:
-                sio = io.StringIO()
-                sio.write('Stack (most recent call last):\n')
-                traceback.print_stack(f, file=sio)
-                sinfo = sio.getvalue()
-                if sinfo[-1] == '\n':
-                    sinfo = sinfo[:-1]
-                sio.close()
-            rv = (co.co_filename, f.f_lineno, co.co_name, sinfo)
-            break
-        return rv
-
-    def _log(self,
-             level,
-             msg,
-             args,
-             exc_info=None,
-             extra=None,
-             stack_info=False,
-             stacklevel=1):
-        """
-        Low-level logging routine which creates a LogRecord and then calls
-        all the handlers of this logger to handle the record.
-        """
-        sinfo = None
-        if _logging._srcfile:
-            #IronPython doesn't track Python frames, so findCaller raises an
-            #exception on some versions of IronPython. We trap it here so that
-            #IronPython can use logging.
-            try:
-                fn, lno, func, sinfo = self.findCaller(stack_info, stacklevel)
-            except ValueError:  # pragma: no cover
-                fn, lno, func = "(unknown file)", 0, "(unknown function)"
-        else:  # pragma: no cover
-            fn, lno, func = "(unknown file)", 0, "(unknown function)"
-        if exc_info:
-            if isinstance(exc_info, BaseException):
-                exc_info = (type(exc_info), exc_info, exc_info.__traceback__)
-            elif not isinstance(exc_info, tuple):
-                exc_info = sys.exc_info()
-        record = self.makeRecord(self.name, level, fn, lno, msg, args, exc_info,
-                                 func, extra, sinfo)
-        self.handle(record)
-
-    _logging.Logger.findCaller = findCaller
-    _logging.Logger._log = _log
-else:
-    raise RuntimeError(
-        'Not support Python with version earlier than 3.6, get %s.%s' %
-        (sys.version_info[0], sys.version_info[1]))
-
-_logging.basicConfig(format='[%(asctime)s] %(levelname)s - '
-                     '%(name)s.%(funcName)s(%(lineno)s): %(message)s',
-                     level=ERROR)
-
-
-def set_verbosity(level):
-    logger = _logging.getLogger()
-    logger.setLevel(level)
-
-
-def _log(level, msg, *args, **kwargs):
-    # DO NOT USE THIS FUNCTION DIRECTLY!
-    module_name = sys._getframe(2).f_globals['__name__']
-    logger = _logging.getLogger(module_name)
-    logger.log(level, msg, stacklevel=3, *args, **kwargs)
-
-
-def debug(msg, *args, **kwargs):
-    _log(DEBUG, msg, *args, **kwargs)
-
-
-def info(msg, *args, **kwargs):
-    _log(INFO, msg, *args, **kwargs)
-
-
-def warn(msg, *args, **kwargs):
-    _log(WARN, msg, *args, **kwargs)
-
-
-def error(msg, *args, **kwargs):
-    _log(ERROR, msg, *args, **kwargs)
-
-
-def fatal(msg, *args, **kwargs):
-    _log(FATAL, msg, *args, **kwargs)
-
-
-__all__ = [
-    'DEBUG', 'INFO', 'WARN', 'ERROR', 'FATAL', 'debug', 'info', 'warn', 'error',
-    'fatal', 'set_verbosity'
-]
+# -*- encoding: utf-8 -*-
+"""
+logging.py: 日志模块
+"""
+
+import logging as _logging
+import sys
+from logging import DEBUG, INFO, WARN, ERROR, FATAL
+
+if sys.version_info[0] == 3 and sys.version_info[1] >= 8:
+    pass
+elif sys.version_info[0] == 3 and sys.version_info[1] in [6, 7]:
+    import io
+    import os
+    import traceback
+
+    def findCaller(self, stack_info=False, stacklevel=1):
+        """
+        Find the stack frame of the caller so that we can note the source
+        file name, line number and function name.
+        """
+        f = _logging.currentframe()
+        #On some versions of IronPython, currentframe() returns None if
+        #IronPython isn't run with -X:Frames.
+        if f is not None:
+            f = f.f_back
+        orig_f = f
+        while f and stacklevel > 1:
+            f = f.f_back
+            stacklevel -= 1
+        if not f:
+            f = orig_f
+        rv = "(unknown file)", 0, "(unknown function)", None
+        while hasattr(f, "f_code"):
+            co = f.f_code
+            filename = os.path.normcase(co.co_filename)
+            if filename == _logging._srcfile:
+                f = f.f_back
+                continue
+            sinfo = None
+            if stack_info:
+                sio = io.StringIO()
+                sio.write('Stack (most recent call last):\n')
+                traceback.print_stack(f, file=sio)
+                sinfo = sio.getvalue()
+                if sinfo[-1] == '\n':
+                    sinfo = sinfo[:-1]
+                sio.close()
+            rv = (co.co_filename, f.f_lineno, co.co_name, sinfo)
+            break
+        return rv
+
+    def _log(self,
+             level,
+             msg,
+             args,
+             exc_info=None,
+             extra=None,
+             stack_info=False,
+             stacklevel=1):
+        """
+        Low-level logging routine which creates a LogRecord and then calls
+        all the handlers of this logger to handle the record.
+        """
+        sinfo = None
+        if _logging._srcfile:
+            #IronPython doesn't track Python frames, so findCaller raises an
+            #exception on some versions of IronPython. We trap it here so that
+            #IronPython can use logging.
+            try:
+                fn, lno, func, sinfo = self.findCaller(stack_info, stacklevel)
+            except ValueError:  # pragma: no cover
+                fn, lno, func = "(unknown file)", 0, "(unknown function)"
+        else:  # pragma: no cover
+            fn, lno, func = "(unknown file)", 0, "(unknown function)"
+        if exc_info:
+            if isinstance(exc_info, BaseException):
+                exc_info = (type(exc_info), exc_info, exc_info.__traceback__)
+            elif not isinstance(exc_info, tuple):
+                exc_info = sys.exc_info()
+        record = self.makeRecord(self.name, level, fn, lno, msg, args, exc_info,
+                                 func, extra, sinfo)
+        self.handle(record)
+
+    _logging.Logger.findCaller = findCaller
+    _logging.Logger._log = _log
+else:
+    raise RuntimeError(
+        'Not support Python with version earlier than 3.6, get %s.%s' %
+        (sys.version_info[0], sys.version_info[1]))
+
+_logging.basicConfig(format='[%(asctime)s] %(levelname)s - '
+                     '%(name)s.%(funcName)s(%(lineno)s): %(message)s',
+                     level=ERROR)
+
+
+def set_verbosity(level):
+    logger = _logging.getLogger()
+    logger.setLevel(level)
+
+
+def _log(level, msg, *args, **kwargs):
+    # DO NOT USE THIS FUNCTION DIRECTLY!
+    module_name = sys._getframe(2).f_globals['__name__']
+    logger = _logging.getLogger(module_name)
+    logger.log(level, msg, stacklevel=3, *args, **kwargs)
+
+
+def debug(msg, *args, **kwargs):
+    _log(DEBUG, msg, *args, **kwargs)
+
+
+def info(msg, *args, **kwargs):
+    _log(INFO, msg, *args, **kwargs)
+
+
+def warn(msg, *args, **kwargs):
+    _log(WARN, msg, *args, **kwargs)
+
+
+def error(msg, *args, **kwargs):
+    _log(ERROR, msg, *args, **kwargs)
+
+
+def fatal(msg, *args, **kwargs):
+    _log(FATAL, msg, *args, **kwargs)
+
+
+__all__ = [
+    'DEBUG', 'INFO', 'WARN', 'ERROR', 'FATAL', 'debug', 'info', 'warn', 'error',
+    'fatal', 'set_verbosity'
+]
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/models.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-# -*- encoding: utf-8 -*-
-
-import numpy as np
-
-from sklearn.linear_model import LogisticRegression
-from sklearn.metrics import roc_auc_score
-from sklearn.model_selection import check_cv
-
-import riskmodels.logging as logging
-
-
-class LogisticRegressionCV(object):
-
-    def __init__(self, *, cv=3, **logistic_kwargs):
-        self._cv = cv
-        self._logistic_kwargs = logistic_kwargs
-
-    def fit_and_eval(self, X, y):
-        y_predicted = None
-        y_actual = None
-
-        cv_wrapper = check_cv(self._cv, y=y, classifier=True)
-
-        for train_index, test_index in cv_wrapper.split(X, y):
-            X_train, X_test = X[train_index], X[test_index]
-            y_train, y_test = y[train_index], y[test_index]
-
-            logistic_regressor = LogisticRegression(**self._logistic_kwargs)
-            logistic_regressor.fit(X_train, y_train)
-
-            y_pred = logistic_regressor.predict_proba(X_test)[:, 1]
-
-            if y_predicted is None:
-                y_predicted = y_pred
-                y_actual = y_test
-            else:
-                y_predicted = np.concatenate([y_predicted, y_pred])
-                y_actual = np.concatenate([y_actual, y_test])
-
-        auc = roc_auc_score(y_actual, y_predicted)
-        return auc
-
-
-def group_split_cv(group_arr):
-    group_arr = np.asarray(group_arr)
-    groups = np.unique(group_arr)
-
-    for g in groups:
-        train = group_arr != g
-        yield np.argwhere(train).ravel(), np.argwhere(~train).ravel()
-
-
-def stepwise_lr(df, y, x, cv=3, max_num_features=30, **lr_kwargs):
-    feature_pool = x
-    selected_features = []
-    best_metrics = None
-
-    def get_features_perf(feature_list):
-        lr_cv = LogisticRegressionCV(cv=cv, **lr_kwargs)
-        auc = lr_cv.fit_and_eval(df[feature_list].values, y)
-        return auc
-
-    step = 0
-    while True:
-        perf_records = {}
-        improved = False
-        step += 1
-
-        for feature in feature_pool:
-            train_features = selected_features + [feature]
-            perf_records[tuple(train_features)] = get_features_perf(
-                train_features)
-
-        if len(selected_features) > 1:
-            for feature in selected_features:
-                train_features = selected_features.copy()
-                train_features.remove(feature)
-                perf_records[tuple(train_features)] = get_features_perf(
-                    train_features)
-
-        for key, value in perf_records.items():
-            if best_metrics is None \
-                    or (best_metrics < value and len(key) <= max_num_features):
-                selected_features = list(key)
-                best_metrics = value
-                improved = True
-                feature_pool = [f for f in x if f not in selected_features]
-
-        if improved:
-            logging.info(
-                f'Step {step}:\nSelected features: {selected_features}\n'
-                f'Performance: auc={best_metrics}')
-        else:
-            logging.info('No improve. Exit.')
-            break
-
-    return best_metrics, selected_features
+# -*- encoding: utf-8 -*-
+
+import numpy as np
+
+from sklearn.linear_model import LogisticRegression
+from sklearn.metrics import roc_auc_score
+from sklearn.model_selection import check_cv
+
+import sy_riskmodels.logging as logging
+
+
+class LogisticRegressionCV(object):
+
+  def __init__(self, *, cv=3, **logistic_kwargs):
+    self._cv = cv
+    self._logistic_kwargs = logistic_kwargs
+
+  def fit_and_eval(self, X, y):
+    train_predicted = None
+    train_actual = None
+    valid_predicted = None
+    valid_actual = None
+
+    cv_wrapper = check_cv(self._cv, y=y, classifier=True)
+
+    for train_index, test_index in cv_wrapper.split(X, y):
+      X_train, X_valid = X[train_index], X[test_index]
+      y_train, y_valid = y[train_index], y[test_index]
+
+      logistic_regressor = LogisticRegression(**self._logistic_kwargs)
+      logistic_regressor.fit(X_train, y_train)
+
+      train_pred = logistic_regressor.predict_proba(X_train)[:, 1]
+      if train_predicted is None:
+        train_predicted = train_pred
+        train_actual = y_train
+      else:
+        train_predicted = np.concatenate([train_predicted, train_pred])
+        train_actual = np.concatenate([train_actual, y_train])
+
+      valid_pred = logistic_regressor.predict_proba(X_valid)[:, 1]
+      if valid_predicted is None:
+        valid_predicted = valid_pred
+        valid_actual = y_valid
+      else:
+        valid_predicted = np.concatenate([valid_predicted, valid_pred])
+        valid_actual = np.concatenate([valid_actual, y_valid])
+
+    train_auc = roc_auc_score(train_actual, train_predicted)
+    valid_auc = roc_auc_score(valid_actual, valid_predicted)
+    logging.info(f'训练集 AUC={train_auc:.2%}，测试集 AUC={valid_auc:.2%}')
+
+    return min(train_auc, valid_auc) - abs(train_auc - valid_auc)
+
+
+def group_split_cv(group_arr):
+  group_arr = np.asarray(group_arr)
+  groups = np.unique(group_arr)
+
+  for g in groups:
+    train = group_arr != g
+    yield np.argwhere(train).ravel(), np.argwhere(~train).ravel()
+
+
+def stepwise_lr(df, y, x, cv=3, max_num_features=30, **lr_kwargs):
+  feature_pool = x
+  selected_features = []
+  best_metrics = None
+
+  def get_features_perf(feature_list):
+    lr_cv = LogisticRegressionCV(cv=cv, **lr_kwargs)
+    auc = lr_cv.fit_and_eval(df[feature_list].values, y)
+    return auc
+
+  step = 0
+  while True:
+    perf_records = {}
+    improved = False
+    step += 1
+
+    for feature in feature_pool:
+      train_features = selected_features + [feature]
+      perf_records[tuple(train_features)] = get_features_perf(train_features)
+
+    if len(selected_features) > 1:
+      for feature in selected_features:
+        train_features = selected_features.copy()
+        train_features.remove(feature)
+        perf_records[tuple(train_features)] = get_features_perf(train_features)
+
+    for key, value in perf_records.items():
+      if best_metrics is None or (best_metrics < value and
+                                  len(key) <= max_num_features):
+        selected_features = list(key)
+        best_metrics = value
+        improved = True
+        feature_pool = [f for f in x if f not in selected_features]
+
+    if improved:
+      logging.info(f'Step {step}:\nSelected features: {selected_features}\n'
+                   f'Performance: auc={best_metrics}')
+    else:
+      logging.info('No improve. Exit.')
+      break
+
+  return best_metrics, selected_features
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/rule.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/rule.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-# -*- encoding: utf-8 -*-
-
-import numpy as np
-import pandas as pd
-
-
-def make_rule_stat(bad_cnt_fn, good_cnt_fn):
-
-    def rule_stat(df):
-        cnt = len(df)
-        bad = bad_cnt_fn(df)
-        good = good_cnt_fn(df)
-        badrate = bad / (bad + good)
-        return pd.Series({
-            'cnt': cnt,
-            'bad': bad,
-            'good': good,
-            'badrate': badrate
-        })
-
-    return rule_stat
-
-
-def foil_gain(pos0, neg0, pos1, neg1):
-    """FOIL增益计算"""
-    if pos0 == 0:
-        return -np.inf
-    if neg0 == 0:
-        neg0 += 0.5
-
-    info1 = np.log2(pos0 / (pos0 + neg0))
-    info2 = np.log2(pos1 / (pos1 + neg1))
-
-    return pos0 * (info1 - info2)
-
-
-def eval_rules(df, stat_fn, *rule):
-    rules = list(rule)
-    metrics = []
-
-    for rule in rules:
-        hit_metric = df.groupby(rule(df)).apply(stat_fn)
-
-        if np.any(hit_metric.index):
-            hit_rate = hit_metric['cnt'][
-                hit_metric.index].item() / hit_metric['cnt'].sum()
-            hit_bad = hit_metric['bad'][hit_metric.index].item()
-            hit_good = hit_metric['good'][hit_metric.index].item()
-            all_bad = hit_metric['bad'].sum()
-            all_good = hit_metric['good'].sum()
-
-            if hit_bad + hit_good == 0:
-                hit_badrate = 0
-                foil = np.inf
-            else:
-                hit_badrate = hit_bad / (hit_bad + hit_good)
-                foil = foil_gain(hit_bad, hit_good, all_bad, all_good)
-
-            metrics.append({
-                'rule': rule.__name__,
-                'hit': hit_rate,
-                'badrate': hit_badrate,
-                'foil': foil
-            })
-        else:
-            metrics.append({
-                'rule': rule.__name__,
-                'hit': 0,
-                'badrate': np.nan,
-                'foil': 0
-            })
-
-    return pd.DataFrame(metrics)
-
-
-def rule_optimize(df, stat_fn, *rule):
-    rules = list(rule)
-    named_rules = {rule.__name__: rule for rule in rules}
-    opt_result = None
-    tmp_df = df.copy()
-
-    while len(tmp_df) > 0 and len(named_rules) > 0:
-        rule_result = eval_rules(tmp_df, stat_fn, *named_rules.values())
-        best_rule = rule_result.sort_values(
-            'foil', ascending=False).iloc[0, ]
-        best_rule_name = best_rule['rule']
-
-        if best_rule['foil'] > 0:
-            rule = named_rules.pop(best_rule_name)
-            tmp_df = tmp_df[~rule(tmp_df)]
-
-            if opt_result is None:
-                opt_result = best_rule.to_frame().T
-
-            else:
-                opt_result = pd.concat(
-                    [opt_result, best_rule.to_frame().T], ignore_index=True)
-        else:
-            break
-
-    return opt_result
+# -*- encoding: utf-8 -*-
+
+import numpy as np
+import pandas as pd
+
+
+def make_rule_stat(bad_cnt_fn, good_cnt_fn):
+
+    def rule_stat(df):
+        cnt = len(df)
+        bad = bad_cnt_fn(df)
+        good = good_cnt_fn(df)
+        badrate = bad / (bad + good)
+        return pd.Series({
+            'cnt': cnt,
+            'bad': bad,
+            'good': good,
+            'badrate': badrate
+        })
+
+    return rule_stat
+
+
+def foil_gain(pos0, neg0, pos1, neg1):
+    """FOIL增益计算"""
+    if pos0 == 0:
+        return -np.inf
+    if neg0 == 0:
+        neg0 += 0.5
+
+    info1 = np.log2(pos0 / (pos0 + neg0))
+    info2 = np.log2(pos1 / (pos1 + neg1))
+
+    return pos0 * (info1 - info2)
+
+
+def eval_rules(df, stat_fn, *rule):
+    rules = list(rule)
+    metrics = []
+
+    for rule in rules:
+        hit_metric = df.groupby(rule(df)).apply(stat_fn)
+
+        if np.any(hit_metric.index):
+            hit_rate = hit_metric['cnt'][
+                hit_metric.index].item() / hit_metric['cnt'].sum()
+            hit_bad = hit_metric['bad'][hit_metric.index].item()
+            hit_good = hit_metric['good'][hit_metric.index].item()
+            all_bad = hit_metric['bad'].sum()
+            all_good = hit_metric['good'].sum()
+
+            if hit_bad + hit_good == 0:
+                hit_badrate = 0
+                foil = np.inf
+            else:
+                hit_badrate = hit_bad / (hit_bad + hit_good)
+                foil = foil_gain(hit_bad, hit_good, all_bad, all_good)
+
+            metrics.append({
+                'rule': rule.__name__,
+                'hit': hit_rate,
+                'badrate': hit_badrate,
+                'foil': foil
+            })
+        else:
+            metrics.append({
+                'rule': rule.__name__,
+                'hit': 0,
+                'badrate': np.nan,
+                'foil': 0
+            })
+
+    return pd.DataFrame(metrics)
+
+
+def rule_optimize(df, stat_fn, *rule):
+    rules = list(rule)
+    named_rules = {rule.__name__: rule for rule in rules}
+    opt_result = None
+    tmp_df = df.copy()
+
+    while len(tmp_df) > 0 and len(named_rules) > 0:
+        rule_result = eval_rules(tmp_df, stat_fn, *named_rules.values())
+        best_rule = rule_result.sort_values(
+            'foil', ascending=False).iloc[0, ]
+        best_rule_name = best_rule['rule']
+
+        if best_rule['foil'] > 0:
+            rule = named_rules.pop(best_rule_name)
+            tmp_df = tmp_df[~rule(tmp_df)]
+
+            if opt_result is None:
+                opt_result = best_rule.to_frame().T
+
+            else:
+                opt_result = pd.concat(
+                    [opt_result, best_rule.to_frame().T], ignore_index=True)
+        else:
+            break
+
+    return opt_result
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/scorecard.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/scorecard.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,53 +26,53 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from pandas.core.dtypes.common import is_numeric_dtype
 from scipy.stats import chi2
 from scipy.stats import chi2_contingency
 
-import riskmodels.logging as logging
-from riskmodels.evaluate import psi
-from riskmodels.utils import monotonic, round_, str_to_list
+import sy_riskmodels.logging as logging
+from sy_riskmodels.evaluate import psi
+from sy_riskmodels.utils import monotonic, round_, str_to_list
 
 
 def check_const_cols(dat):
   # remove only 1 unique values variable
   unique1_cols = [i for i in list(dat) if len(dat[i].unique()) == 1]
   if len(unique1_cols) > 0:
     logging.warn("There are {} columns have only one unique values, which are "
                  "removed from input dataset. \n (ColumnNames: {})".format(
-                     len(unique1_cols), ', '.join(unique1_cols)))
+      len(unique1_cols), ', '.join(unique1_cols)))
     dat = dat.drop(unique1_cols, axis=1)
   return dat
 
 
 def check_datetime_cols(dat):
   datetime_cols = dat.apply(
-      pd.to_numeric, errors='ignore').select_dtypes(object).apply(
-          pd.to_datetime,
-          errors='ignore').select_dtypes('datetime64').columns.tolist()
+    pd.to_numeric, errors='ignore').select_dtypes(object).apply(
+    pd.to_datetime,
+    errors='ignore').select_dtypes('datetime64').columns.tolist()
   if len(datetime_cols) > 0:
     logging.warn("There are {} date/time type columns are removed from input "
                  "dataset. \n (ColumnNames: {})".format(
-                     len(datetime_cols), ', '.join(datetime_cols)))
+      len(datetime_cols), ', '.join(datetime_cols)))
     dat = dat.drop(datetime_cols, axis=1)
   return dat
 
 
 def check_cat_var_uniques(dat: pd.DataFrame,
                           unique_limits: int = 50,
                           var_skip: List = None):
   # character columns with too many unique values
   char_cols = [i for i in list(dat) if not is_numeric_dtype(dat[i])]
   if var_skip is not None:
     var_skip = str_to_list(var_skip)
     char_cols = list(set(char_cols) - set(str_to_list(var_skip)))
   cat_var_too_many_unique = [
-      i for i in char_cols if len(dat[i].unique()) >= unique_limits
+    i for i in char_cols if len(dat[i].unique()) >= unique_limits
   ]
   if len(cat_var_too_many_unique) > 0:
     print(f'>>> There are {cat_var_too_many_unique} categorical variables '
           f'with too many unique values (>= {unique_limits}). Please double '
           'check the following  variables: \n'
           f'{", ".join(cat_var_too_many_unique)}')
     print('>>> Skip these variables?')
@@ -90,25 +90,25 @@
 
 def rep_blank_na(dat):
   # cant replace blank string in categorical value with nan
   # remove duplicated index
   if dat.index.duplicated().any():
     dat = dat.reset_index(drop=True)
     logging.warn(
-        'There are duplicated index in dataset. The index has been reset.')
+      'There are duplicated index in dataset. The index has been reset.')
 
   blank_cols = [
-      i for i in list(dat) if dat[i].astype(str).str.findall(r'^\s*$').apply(
-          lambda x: 0 if len(x) == 0 else 1).sum() > 0
+    i for i in list(dat) if dat[i].astype(str).str.findall(r'^\s*$').apply(
+      lambda x: 0 if len(x) == 0 else 1).sum() > 0
   ]
   if len(blank_cols) > 0:
     logging.warn(
-        'There are blank strings in {} columns, which are replaced with '
-        'NaN. \n (ColumnNames: {})'.format(
-            len(blank_cols), ', '.join(blank_cols)))
+      'There are blank strings in {} columns, which are replaced with '
+      'NaN. \n (ColumnNames: {})'.format(
+        len(blank_cols), ', '.join(blank_cols)))
 
     dat.replace(r'^\s*$', np.nan, regex=True)
 
   return dat
 
 
 def check_y(dat: pd.DataFrame, y: str, *, positive: Union[int, float] = 1):
@@ -136,15 +136,15 @@
       logging.error(f'positive value ({positive}) not in the target column.')
       raise ValueError(f'positive value ({positive}) not in the target column.')
 
     dat[y] = np.where(dat[y] == positive, 1, 0)
 
   except KeyError as err:
     logging.error(
-        "Incorrect inputs; there is no \'{}\' column in dat.".format(y))
+      "Incorrect inputs; there is no \'{}\' column in dat.".format(y))
     raise KeyError(y) from err
 
   return dat
 
 
 def x_variable(dat, y, x, var_skip=None):
   y = str_to_list(y)
@@ -160,15 +160,15 @@
     if any([i in list(x_all) for i in x]) is False:
       x = x_all
     else:
       x_not_in_x_all = set(x).difference(x_all)
       if len(x_not_in_x_all) > 0:
         logging.warn("Incorrect inputs; there are {} x variables are not exist "
                      "in input data, which are removed from x. \n({})".format(
-                         len(x_not_in_x_all), ', '.join(x_not_in_x_all)))
+          len(x_not_in_x_all), ', '.join(x_not_in_x_all)))
         x = set(x).intersection(x_all)
 
   return list(x)
 
 
 def check_breaks_list(breaks_list) -> dict:
   if breaks_list is not None:
@@ -186,24 +186,24 @@
 def check_special_values(special_values, xs) -> dict:
   if special_values is not None:
     # # is string
     # if isinstance(special_values, str):
     #     special_values = eval(special_values)
     if isinstance(special_values, list):
       logging.warn(
-          "The special_values should be a dict. Make sure special values "
-          "are exactly the same in all variables if special_values is "
-          "a list.")
+        "The special_values should be a dict. Make sure special values "
+        "are exactly the same in all variables if special_values is "
+        "a list.")
       sv_dict = {}
       for i in xs:
         sv_dict[i] = special_values
       special_values = sv_dict
     elif not isinstance(special_values, dict):
       raise Exception(
-          "Incorrect inputs; special_values should be a list or dict.")
+        "Incorrect inputs; special_values should be a list or dict.")
   else:
     special_values = {}
   return special_values
 
 
 def woebin(
     dt,
@@ -256,49 +256,49 @@
   special_values = check_special_values(special_values, xs)
 
   # binning for each x variable
   # loop on xs
   if (no_cores is None) or (no_cores < 1):
     all_cores = mp.cpu_count() - 1
     no_cores = int(
-        np.ceil(xs_len / 5 if xs_len / 5 < all_cores else all_cores * 0.9))
+      np.ceil(xs_len / 5 if xs_len / 5 < all_cores else all_cores * 0.9))
 
   # y list to str
   y = y[0]
 
   woe_bin = WOEBinFactory.build(methods, **kwargs)
 
   tasks = [
-      (
-          # dtm definition
-          pd.DataFrame({
-              'y': dt[y],
-              'variable': x_i,
-              'value': dt[x_i]
-          }),
-          # breaks_list
-          breaks_list.get(x_i),
-          # special_values
-          special_values.get(x_i)) for x_i in xs
+    (
+      # dtm definition
+      pd.DataFrame({
+        'y': dt[y],
+        'variable': x_i,
+        'value': dt[x_i]
+      }),
+      # breaks_list
+      breaks_list.get(x_i),
+      # special_values
+      special_values.get(x_i)) for x_i in xs
   ]
 
   logging.info(f'开始分箱，特征数 {len(tasks)}，样本数 {len(dt)}')
 
   if no_cores == 1:
     bins = dict(zip(xs, itertools.starmap(woe_bin, tasks)))
   else:
     pool = mp.Pool(processes=no_cores)
     bins = dict(zip(xs, pool.starmap(woe_bin, tasks)))
     pool.close()
 
   # running time
   running_time = time.time() - start_time
   logging.info('分箱完成：Binning on {} rows and {} columns in {}'.format(
-      dt.shape[0], len(xs), time.strftime("%H:%M:%S",
-                                          time.gmtime(running_time))))
+    dt.shape[0], len(xs), time.strftime("%H:%M:%S",
+                                        time.gmtime(running_time))))
 
   return bins
 
 
 class WOEBinFactory(object):
   """WOEBin工厂方法类，与ComposedWOEBin配合，提供WOEBin子类的组装功能。
 
@@ -381,15 +381,15 @@
 
         >>> woe_bin = WOEBinFactory.build (['quantile', 'tree'],
         ...                               initial_bins=20,
         ...                               bin_num_limit=8,
         ...                               min_iv_inc=0.1,
         ...                               count_distr_limit=0.05)
         >>> woe_bin
-        <riskmodels.scorecard.ComposedWOEBin object at 0x1009776a0>
+        <sy_riskmodels.scorecard.ComposedWOEBin object at 0x1009776a0>
 
         Args:
             bin_classes: WOEBin子类或子类注册名列表
             **kwargs: 子类初始化的关键字参数
 
         Returns:
             ComposedWOEBin实例
@@ -477,17 +477,17 @@
             pd.DataFrame，包含如下四列 'bin_char', 'rowid', 'value'
 
         """
     assert vec is not None, 'vec cannot be None'
     vec = [str(i) for i in vec]
     a = pd.DataFrame({'bin_chr': vec}).assign(rowid=lambda x: x.index)
     b = pd.DataFrame([i.split('%,%') for i in vec], index=vec) \
-        .stack().replace('missing', np.nan) \
-        .reset_index(name='value') \
-        .rename(columns={'level_0': 'bin_chr'})[['bin_chr', 'value']]
+      .stack().replace('missing', np.nan) \
+      .reset_index(name='value') \
+      .rename(columns={'level_0': 'bin_chr'})[['bin_chr', 'value']]
 
     df = pd.merge(a, b, on='bin_chr')
     return df
 
   @classmethod
   def split_special_values(cls, dtm, spl_val):
     dtm['idx'] = dtm.index
@@ -495,36 +495,36 @@
     if spl_val is not None:
       sv_df = cls.split_vec_to_df(spl_val)
       # value
       if is_numeric_dtype(dtm['value']):
         sv_df['value'] = sv_df['value'].astype(dtm['value'].dtypes)
         # TODO: 此处是否必要？？
         sv_df['bin_chr'] = np.where(
-            np.isnan(sv_df['value']), sv_df['bin_chr'],
-            sv_df['value'].astype(str))
+          np.isnan(sv_df['value']), sv_df['bin_chr'],
+          sv_df['value'].astype(str))
       # dtm_sv & dtm
       dtm_merge = pd.merge(
-          dtm.fillna("missing"),
-          sv_df[['value', 'rowid']].fillna("missing"),
-          how='left',
-          on='value')
+        dtm.fillna("missing"),
+        sv_df[['value', 'rowid']].fillna("missing"),
+        how='left',
+        on='value')
       dtm_sv = dtm_merge[~dtm_merge['rowid'].isna()][
-          dtm.columns.tolist()].reset_index(drop=True)
+        dtm.columns.tolist()].reset_index(drop=True)
       dtm_ns = dtm_merge[dtm_merge['rowid'].isna()][
-          dtm.columns.tolist()].reset_index(drop=True)
+        dtm.columns.tolist()].reset_index(drop=True)
       if len(dtm_ns) == 0:
         dtm_ns = None
       else:
         dtm_ns['value'] = dtm_ns['value'].astype(dtm['value'].dtypes)
 
       if dtm_sv.shape[0] == 0:
         dtm_sv = None
       else:
         dtm_sv = pd.merge(
-            dtm_sv.fillna('missing'), sv_df.fillna('missing'), on='value')
+          dtm_sv.fillna('missing'), sv_df.fillna('missing'), on='value')
     else:
       dtm_sv = None
       dtm_ns = dtm.copy()
 
     if dtm_sv is not None:
       dtm_sv.set_index(dtm_sv['idx'], drop=True, inplace=True)
 
@@ -532,33 +532,33 @@
       dtm_ns.set_index(dtm_ns['idx'], drop=True, inplace=True)
 
     return {'dtm_sv': dtm_sv, 'dtm_ns': dtm_ns}
 
   @classmethod
   def dtm_binning_sv(cls, dtm, spl_val):
     """
-        将原数据集拆分为特殊值数据集、非特殊值数据集，特殊值列表有spl_val参数给出。
+    将原数据集拆分为特殊值数据集、非特殊值数据集，特殊值列表有spl_val参数给出。
 
-        Specifications:
-        1、当dtm['value']为数值类型时，每个特殊数值会单独成为一箱。例如：
-        >>> vec = ['missing', '-9999%,%-999']
-        如果dtm['value']为数值类型，在此函数中，-9999和-999会分开成为两箱；如果dtm['value']为
-        非数值类型，则-9999和-999会合并到同一分箱。
-        2、如果spl_val为None，或者dtm['value']中不存在特殊值，则返回的binning_sv为None。
-        3、如果dtm['value']全为spl_val中的特殊值，则返回的dtm为None。
-        4、如果入参breaks中包含'missing'，则spl_val中将不包含'missing'。
+    Specifications:
+    1、当dtm['value']为数值类型时，每个特殊数值会单独成为一箱。例如：
+    >>> vec = ['missing', '-9999%,%-999']
+    如果dtm['value']为数值类型，在此函数中，-9999和-999会分开成为两箱；如果dtm['value']为
+    非数值类型，则-9999和-999会合并到同一分箱。
+    2、如果spl_val为None，或者dtm['value']中不存在特殊值，则返回的binning_sv为None。
+    3、如果dtm['value']全为spl_val中的特殊值，则返回的dtm为None。
+    4、如果入参breaks中包含'missing'，则spl_val中将不包含'missing'。
 
-        Args:
-            dtm: 应包含['y', 'variable', 'value']三列的DataFrame，详见WEOBin类文档
-            spl_val: 特殊值列表
+    Args:
+        dtm: 应包含['y', 'variable', 'value']三列的DataFrame，详见WEOBin类文档
+        spl_val: 特殊值列表
 
-        Returns:
-            {'binning_sv': 特殊值分箱统计结果, 'ns_dtm': dtm中除去特殊值外的部分}
+    Returns:
+        {'binning_sv': 特殊值分箱统计结果, 'ns_dtm': dtm中除去特殊值外的部分}
 
-        """
+    """
     split_dtm = cls.split_special_values(dtm, spl_val)
 
     dtm_sv = split_dtm['dtm_sv']
     dtm_ns = split_dtm['dtm_ns']
 
     if dtm_sv is None or dtm_sv.shape[0] == 0:
       binning_sv = None
@@ -609,15 +609,15 @@
       return np.sum(x == 0)
 
     def _n1(x):
       return np.sum(x == 1)
 
     bin_chr = bin_chr.rename(index='bin_chr')
     binning = dtm.groupby(['variable', bin_chr], observed=False)['y'].agg(
-        good=_n0, bad=_n1)
+      good=_n0, bad=_n1)
     binning = binning.reset_index()
 
     return binning
 
   @classmethod
   def apply(cls, dtm, bin_res, value='woe'):
     """
@@ -644,23 +644,23 @@
       dtm_sv = dtm_sv[['idx', 'bin_chr', 'value', 'y']]
 
     if dtm_ns is not None:
       break_df = cls.split_vec_to_df(breaks)
       # TO-DO: 以下代码与binning_breaks重复，需要进行精简
       if is_numeric_dtype(dtm_ns['value']):
         break_list = ['-inf'] + list(
-            set(break_df.value.tolist()).difference(
-                {np.nan, '-inf', 'inf', 'Inf', '-Inf'})) + ['inf']
+          set(break_df.value.tolist()).difference(
+            {np.nan, '-inf', 'inf', 'Inf', '-Inf'})) + ['inf']
         break_list = sorted(list(map(float, break_list)))
         labels = [
-            '[{},{})'.format(break_list[i], break_list[i + 1])
-            for i in range(len(break_list) - 1)
+          '[{},{})'.format(break_list[i], break_list[i + 1])
+          for i in range(len(break_list) - 1)
         ]
         dtm_ns['bin_chr'] = pd.cut(
-            dtm_ns['value'], break_list, right=False, labels=labels).astype(str)
+          dtm_ns['value'], break_list, right=False, labels=labels).astype(str)
       else:
         dtm_ns = pd.merge(dtm_ns, break_df, how='left', on='value')
 
       dtm_ns = dtm_ns[['idx', 'bin_chr', 'value', 'y']]
 
     new_dtm = pd.concat([dtm_sv, dtm_ns], ignore_index=True)
     dtm = pd.merge(dtm, new_dtm[['idx', 'bin_chr']], on='idx', how='left')
@@ -677,20 +677,20 @@
   def binning_breaks(self, dtm, breaks):
     """按照给定的breaks进行分箱"""
     break_df = self.split_vec_to_df(breaks)
 
     # binning
     if is_numeric_dtype(dtm['value']):
       break_list = ['-inf'] + list(
-          set(break_df.value.tolist()).difference(
-              {np.nan, '-inf', 'inf', 'Inf', '-Inf'})) + ['inf']
+        set(break_df.value.tolist()).difference(
+          {np.nan, '-inf', 'inf', 'Inf', '-Inf'})) + ['inf']
       break_list = sorted(list(map(float, break_list)))
       labels = [
-          '[{},{})'.format(break_list[i], break_list[i + 1])
-          for i in range(len(break_list) - 1)
+        '[{},{})'.format(break_list[i], break_list[i + 1])
+        for i in range(len(break_list) - 1)
       ]
       bin_chr = pd.cut(dtm['value'], break_list, right=False, labels=labels)
 
       binning = self.binning(dtm, bin_chr)
 
       # 不缺定经过正常流程是否还会产生空值，故注释掉下面代码，后续测试中如果发现确实
       # 存在空值再行处理。不建议在此处强行合并到missing中。
@@ -714,16 +714,16 @@
       #               'bad': sum}) \
       #         .reset_index()
     else:
       dtm = pd.merge(dtm, break_df, how='left', on='value')
       binning = self.binning(dtm, dtm['bin_chr'])
       # 保持分箱顺序与传入参数一致
       binning['bin_chr'] = binning['bin_chr'].astype(
-          'category').cat.set_categories(
-              breaks, ordered=True)
+        'category').cat.set_categories(
+        breaks, ordered=True)
       binning = binning.sort_values(by='bin_chr').reset_index(drop=True)
 
     return binning
 
   def binning_format(self, binning):
     """"""
 
@@ -736,33 +736,33 @@
     def _extract_breaks(x):
       gp23 = _pattern.match(x)
       breaks_string = x if gp23 is None else gp23.group(2)
       return breaks_string
 
     # yapf: disable
     binning = binning.assign(
-        count=lambda x: x['good'] + x['bad'],
-        bad_dist=lambda x: sub0(x['bad']) / sub0(x['bad']).sum(),
-        good_dist=lambda x: sub0(x['good']) / sub0(x['good']).sum()
+      count=lambda x: x['good'] + x['bad'],
+      bad_dist=lambda x: sub0(x['bad']) / sub0(x['bad']).sum(),
+      good_dist=lambda x: sub0(x['good']) / sub0(x['good']).sum()
     ).assign(
-        count_distr=lambda x: x['count'] / x['count'].sum(),
-        badprob=lambda x: x['bad'] / x['count'],
-        woe=lambda x: np.log(x['good_dist'] / x['bad_dist'])
+      count_distr=lambda x: x['count'] / x['count'].sum(),
+      badprob=lambda x: x['bad'] / x['count'],
+      woe=lambda x: np.log(x['good_dist'] / x['bad_dist'])
     ).assign(
-        bin_iv=lambda x: (x['good_dist'] - x['bad_dist']) * x['woe']
+      bin_iv=lambda x: (x['good_dist'] - x['bad_dist']) * x['woe']
     ).assign(total_iv=lambda x: x['bin_iv'].sum())
     # yapf: enable
 
     binning['breaks'] = binning['bin_chr'].apply(_extract_breaks)
     binning['is_special_values'] = binning['is_sv']
     binning['bin'] = binning['bin_chr'].astype('str')
 
     return binning[[
-        'variable', 'bin', 'count', 'count_distr', 'good', 'bad', 'badprob',
-        'woe', 'bin_iv', 'total_iv', 'breaks', 'is_special_values'
+      'variable', 'bin', 'count', 'count_distr', 'good', 'bad', 'badprob',
+      'woe', 'bin_iv', 'total_iv', 'breaks', 'is_special_values'
     ]]
 
 
 class ComposedWOEBin(WOEBin):
   """
     组合型分箱方法，将多个分箱方法按顺序进行调用。详细说明请见WOEBin。
 
@@ -787,16 +787,16 @@
   def check_empty_bins(dtm, breaks):
     """针对数值型变量检查空分箱"""
     bins = pd.cut(dtm['value'], breaks, right=False)
     bin_sample_count = bins.value_counts()
     if np.any(bin_sample_count == 0):
       bin_sample_count = bin_sample_count[bin_sample_count != 0]
       bin_right = set([
-          re.match(r'\[(.+),(.+)\)', i).group(1)
-          for i in bin_sample_count.index.astype('str')
+        re.match(r'\[(.+),(.+)\)', i).group(1)
+        for i in bin_sample_count.index.astype('str')
       ]).difference({'-inf', 'inf'})
       breaks = sorted(list(map(float, ['-inf'] + list(bin_right) + ['inf'])))
     return breaks
 
 
 @WOEBinFactory.register('quantile')
 class QuantileInitBin(InitBin):
@@ -896,20 +896,20 @@
       if len_uniq_x < n_bins:
         n_bins = len_uniq_x
       # initial breaks
       if len_uniq_x == n_bins:
         breaks = np.unique(xvalue_rm_outlier)
       else:
         breaks = self._pretty(
-            low=min(xvalue_rm_outlier),
-            high=max(xvalue_rm_outlier),
-            n=self.n_bins)
+          low=min(xvalue_rm_outlier),
+          high=max(xvalue_rm_outlier),
+          n=self.n_bins)
 
       breaks = list(
-          filter(lambda x: np.nanmin(xvalue) < x <= np.nanmax(xvalue), breaks))
+        filter(lambda x: np.nanmin(xvalue) < x <= np.nanmax(xvalue), breaks))
       breaks = [float('-inf')] + sorted(breaks) + [float('inf')]
       breaks = self.check_empty_bins(dtm, breaks)
     else:
       breaks = np.unique(dtm['value'])
     return breaks
 
   def __init__(self, initial_bins=20, **kwargs):
@@ -924,15 +924,15 @@
     binning = self.binning_breaks(dtm, breaks)
     binning['count'] = binning['good'] + binning['bad']
     binning['count_distr'] = binning['count'] / binning['count'].sum()
 
     if not is_numeric_dtype(dtm['value']):
       binning['badprob'] = binning['bad'] / binning['count']
       binning = binning.sort_values(
-          by='badprob', ascending=False).reset_index(drop=True)
+        by='badprob', ascending=False).reset_index(drop=True)
 
     return binning
 
 
 @WOEBinFactory.register(['chi2', 'chimerge'])
 class ChiMergeOptimBin(WOEBin, OptimBinMixin):
   """
@@ -972,17 +972,17 @@
         return np.nan
       elif np.any(np.sum(arr, axis=1) == 0) or np.any(np.sum(arr, axis=0) == 0):
         return 0.0
       else:
         return chi2_contingency(arr, correction=True)[0]
 
     binning['chi2'] = binning.apply(
-        lambda x: chi2_cont_tbl([[x['good'], x['bad']],
-                                 [x['good_lag'], x['bad_lag']]]),
-        axis=1)
+      lambda x: chi2_cont_tbl([[x['good'], x['bad']],
+                               [x['good_lag'], x['bad_lag']]]),
+      axis=1)
     del binning['good_lag']
     del binning['bad_lag']
 
     return binning
 
   def woebin(self, dtm, breaks=None):
     assert breaks is not None, f"使用{self.__class__.__name__}类进行分箱，" \
@@ -1013,16 +1013,16 @@
         idx = binning_chi2[binning_chi2['chi2'] == min_chi2].index[0]
       else:
         # 结束合并操作
         break
 
       # yapf: disable
       binning_chi2.loc[idx - 1, 'bin_chr'] = '%,%'.join(
-          [binning_chi2.loc[idx - 1, 'bin_chr'],
-           binning_chi2.loc[idx, 'bin_chr']])
+        [binning_chi2.loc[idx - 1, 'bin_chr'],
+         binning_chi2.loc[idx, 'bin_chr']])
       binning_chi2.loc[idx - 1, 'count'] = (
           binning_chi2.loc[idx - 1, 'count'] +
           binning_chi2.loc[idx, 'count'])
       binning_chi2.loc[idx - 1, 'count_distr'] = (
           binning_chi2.loc[idx - 1, 'count_distr'] +
           binning_chi2.loc[idx, 'count_distr'])
       binning_chi2.loc[idx - 1, 'good'] = (
@@ -1033,20 +1033,20 @@
           binning_chi2.loc[idx, 'bad'])
       # yapf: enable
 
       if is_numeric_dtype(dtm['value']):
         # 数值类型分箱合并
         # [a,b)%,%[b,c) → [a,c)
         binning_chi2['bin_chr'] = binning_chi2['bin_chr'].apply(
-            lambda x: re.sub(r',[.\d]+\)%,%\[[.\d]+,', ',', x))
+          lambda x: re.sub(r',[.\d]+\)%,%\[[.\d]+,', ',', x))
 
       index = binning_chi2.index.tolist()
       index.remove(idx)
       binning_chi2 = binning_chi2.iloc[
-          index,
+        index,
       ].reset_index(drop=True)
       binning_chi2 = self.chi2_stat(binning_chi2)
     # End of loop
 
     # 切分点提取
     if is_numeric_dtype(dtm['value']):
       _pattern = re.compile(r"^\[(.*), *(.*)\)")
@@ -1127,36 +1127,36 @@
       else:
         break
 
     best_binning = self.merge_binning(binning_tree, binning_tree['node_id'])
 
     if is_numeric_dtype(dtm['value']):
       best_binning['bin_chr'] = best_binning['bin_chr'].apply(
-          lambda x: re.sub(r',[.\d]+\)%,%\[[.\d]+,', ',', x))
+        lambda x: re.sub(r',[.\d]+\)%,%\[[.\d]+,', ',', x))
       _pattern = re.compile(r"^\[(.*), *(.*)\)")
       breaks = best_binning['bin_chr'].apply(lambda x: _pattern.match(x)[2])
       breaks = pd.to_numeric(breaks)
     else:
       breaks = best_binning['bin_chr']
 
     return breaks
 
   def merge_binning(self, binning, node_ids):
     # yapf: disable
     new_binning = binning.groupby([
-        'variable',
-        node_ids,
+      'variable',
+      node_ids,
     ]).agg(bin_chr=('bin_chr', lambda x: '%,%'.join(x.tolist())),
            count=('count', 'sum'),
            count_distr=('count_distr', 'sum'),
            good=('good', 'sum'),
            bad=('bad', 'sum')
            ).assign(
-        bad_prob=lambda x: x['bad'] / x['count'],
-        total_iv=lambda x: self.iv(x['good'], x['bad']))
+      bad_prob=lambda x: x['bad'] / x['count'],
+      total_iv=lambda x: self.iv(x['good'], x['bad']))
     # yapf: enable
 
     return new_binning
 
   @staticmethod
   def node_split(node_ids, idx):
     new_node_ids = np.where(node_ids.index <= idx, node_ids, node_ids + 1)
@@ -1214,37 +1214,37 @@
 
   if no_cores is None or no_cores < 1:
     all_cores = mp.cpu_count() - 1
     no_cores = int(np.ceil(n_x / 5 if n_x / 5 < all_cores else all_cores * 0.9))
   no_cores = max(no_cores, 1)
 
   tasks = [
-      (
-          pd.DataFrame({
-              'y': 0,  # 不重要
-              'variable': var,
-              'value': dt[var]
-          }),
-          bins[var],
-          value) for var in x_vars
+    (
+      pd.DataFrame({
+        'y': 0,  # 不重要
+        'variable': var,
+        'value': dt[var]
+      }),
+      bins[var],
+      value) for var in x_vars
   ]
 
   if no_cores == 1:
     dat_suffix = list(itertools.starmap(WOEBin.apply, tasks))
   else:
     pool = mp.Pool(processes=no_cores)
     dat_suffix = pool.starmap(WOEBin.apply, tasks)
     pool.close()
 
   dat = pd.concat([dat] + dat_suffix, axis=1)
 
   # running time
   running_time = time.time() - start_time
   logging.info('Woe transformation on {} rows and {} columns in {}'.format(
-      dt.shape[0], n_x, time.strftime("%H:%M:%S", time.gmtime(running_time))))
+    dt.shape[0], n_x, time.strftime("%H:%M:%S", time.gmtime(running_time))))
   return dat
 
 
 def plot_bin(binx, title, show_iv):
   y_right_max = np.ceil(binx['badprob'].max() * 10)
   if y_right_max % 2 == 1:
     y_right_max = y_right_max + 1
@@ -1257,50 +1257,50 @@
   # y_left_max
   y_left_max = np.ceil(binx['count_distr'].max() * 10) / 10
   if (y_left_max > 1 or y_left_max <= 0 or y_left_max is np.nan or
       y_left_max is None):
     y_left_max = 1
   # title
   title_string = binx.loc[0, 'variable'] + "  (iv:" + str(
-      round(binx.loc[0,
-                     'total_iv'], 4)) + ")" if show_iv else binx.loc[0,
-                                                                     'variable']
+    round(binx.loc[0,
+    'total_iv'], 4)) + ")" if show_iv else binx.loc[0,
+  'variable']
   title_string = (
-      title + '-' + title_string if title is not None else title_string)
+    title + '-' + title_string if title is not None else title_string)
   # param
   ind = np.arange(len(binx.index))  # the x locations for the groups
   width = 0.35  # the width of the bars: can also be len(x) sequence
   # plot
   fig, ax1 = plt.subplots()
   ax2 = ax1.twinx()
   # ax1
   p1 = ax1.bar(
-      ind, binx['good_distr'], width, color=(24 / 254, 192 / 254, 196 / 254))
+    ind, binx['good_distr'], width, color=(24 / 254, 192 / 254, 196 / 254))
   p2 = ax1.bar(
-      ind,
-      binx['bad_distr'],
-      width,
-      bottom=binx['good_distr'],
-      color=(246 / 254, 115 / 254, 109 / 254))
+    ind,
+    binx['bad_distr'],
+    width,
+    bottom=binx['good_distr'],
+    color=(246 / 254, 115 / 254, 109 / 254))
   for i in ind:
     ax1.text(
-        i,
-        binx.loc[i, 'count_distr'] * 1.02,
-        str(round(binx.loc[i, 'count_distr'] * 100, 1)) + '%, ' +
-        str(binx.loc[i, 'count']),
-        ha='center')
+      i,
+      binx.loc[i, 'count_distr'] * 1.02,
+      str(round(binx.loc[i, 'count_distr'] * 100, 1)) + '%, ' +
+      str(binx.loc[i, 'count']),
+      ha='center')
   # ax2
   ax2.plot(ind, binx['badprob'], marker='o', color='blue')
   for i in ind:
     ax2.text(
-        i,
-        binx.loc[i, 'badprob'] * 1.02,
-        str(round(binx.loc[i, 'badprob'] * 100, 1)) + '%',
-        color='blue',
-        ha='center')
+      i,
+      binx.loc[i, 'badprob'] * 1.02,
+      str(round(binx.loc[i, 'badprob'] * 100, 1)) + '%',
+      color='blue',
+      ha='center')
   # settings
   ax1.set_ylabel('Bin count distribution')
   ax2.set_ylabel('Bad probability', color='blue')
   ax1.set_yticks(np.arange(0, y_left_max + 0.2, 0.2))
   ax2.set_yticks(np.arange(0, y_right_max + 0.2, 0.2))
   ax2.tick_params(axis='y', colors='blue')
   plt.xticks(ind, binx['bin'])
@@ -1365,41 +1365,40 @@
     elif iv < 0.1:
       iv_interval = '[0.08, 0.1)'
     elif iv < 0.2:
       iv_interval = '[0.1, 0.2)'
     else:
       iv_interval = '[0.2, +)'
 
-    # fix bugs
-    woe = x[~x.is_special_is_special_valuesvalues].woe
-    monotonic_type = monotonic(woe)
+    badrate = x[~x.is_special_values].badprob
+    monotonic_type = monotonic(badrate)
 
     return pd.Series(
-        [iv, iv_interval, monotonic_type,
-         lift.max(), lift.min()],
-        index=['IV', 'IV区间', '单调性', '最大Lift', '最小Lift'],
-        dtype='object')
+      [iv, iv_interval, monotonic_type,
+       lift.max(), lift.min()],
+      index=['IV', 'IV区间', '单调性', '最大Lift', '最小Lift'],
+      dtype='object')
 
   iv_df = woe_df.groupby(by='variable').apply(iv_stats)
   iv_df.sort_values(by='IV', ascending=False, inplace=True)
   return woe_df, iv_df
 
 
 def make_scorecard(sc_bins, coef, *, base_points=600, base_odds=50, pdo=20):
   a = pdo / np.log(2)
   b = base_points - a * np.log(base_odds)
 
   base_score = -a * coef['const'] + b
   score_df = [
-      pd.DataFrame({
-          'variable': ['base score'],
-          'bin': [''],
-          'woe': [''],
-          'score': [base_score]
-      })
+    pd.DataFrame({
+      'variable': ['base score'],
+      'bin': [''],
+      'woe': [''],
+      'score': [base_score]
+    })
   ]
 
   for var in coef.keys():
     if var != 'const':
       woe_df = sc_bins[var[:-4]][['variable', 'bin', 'woe']].copy()
       woe_df['score'] = -a * coef[var] * woe_df['woe']
       score_df.append(woe_df)
@@ -1442,15 +1441,15 @@
     breaks = binning[~binning['is_special_values']]['breaks']
     breaks = breaks.tolist()
     return {'breaks': breaks, 'special_values': special_values}
 
   brk_spcs = {key: get_breaks(value) for key, value in bins.items()}
   breaks = {k: v['breaks'] for k, v in brk_spcs.items()}
   special_values = {
-      k: v['special_values'] for k, v in brk_spcs.items() if v['special_values']
+    k: v['special_values'] for k, v in brk_spcs.items() if v['special_values']
   }
   return breaks, special_values
 
 
 def woebin_psi(df_base, df_cmp, bins):
   """
     计算变量PSI
@@ -1481,22 +1480,22 @@
   dat = pd.concat([X_base, X_cmp])
   dat['idx'] = dat.index
 
   psi_dfs = []
 
   for variable in variables:
     psi_df = pd.pivot_table(
-        dat, index=variable, columns=['set'], values=['idx'], aggfunc='count')
+      dat, index=variable, columns=['set'], values=['idx'], aggfunc='count')
     psi_df.columns = ['base', 'cmp']
     psi_df['variable'] = variable[:-4]
     psi_df['bin'] = psi_df.index
     psi_df.reset_index(drop=True, inplace=True)
 
     psi_df = psi_df.assign(
-        base_distr=lambda x: x['base'] / x['base'].sum(),
-        cmp_distr=lambda x: x['cmp'] / x['cmp'].sum()).assign(
-            psi=lambda x: psi(x['base_distr'], x['cmp_distr']))[[
-                'variable', 'bin', 'base_distr', 'cmp_distr', 'psi'
-            ]]
+      base_distr=lambda x: x['base'] / x['base'].sum(),
+      cmp_distr=lambda x: x['cmp'] / x['cmp'].sum()).assign(
+      psi=lambda x: psi(x['base_distr'], x['cmp_distr']))[[
+      'variable', 'bin', 'base_distr', 'cmp_distr', 'psi'
+    ]]
     psi_dfs.append(psi_df)
 
   return pd.concat(psi_dfs, ignore_index=True)
```

### Comparing `sy_riskmodels-0.0.7/src/riskmodels/utils.py` & `sy_riskmodels-0.0.8/src/sy_riskmodels/utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-# -*- encoding: utf-8 -*-
-from functools import wraps
-
-import numpy as np
-import pandas as pd
-
-
-def sample_stats(df, target):
-    """
-    统计样本中好坏样本数量及坏样本占比，使用示例如下：
-
-    >>> sample_df = pd.DataFrame({
-    ...     'id': np.arange(10),
-    ...     'prod': ['a', 'a', 'a', 'b', 'b', 'b', 'b', 'c', 'c', 'c'],
-    ...     'y': [0, 0, 1, 1, 0, 1, 0, 1, 0, 0, 1]})
-    >>> sample_df
-       id prod  y
-    0   0    a  0
-    1   1    a  0
-    2   2    a  1
-    3   3    b  1
-    4   4    b  0
-    5   5    b  1
-    6   6    b  0
-    7   7    c  1
-    8   8    c  0
-    9   9    c  0
-    >>> sample_stats(sample_df, target='y')
-    TotalCnt     10
-    GoodCnt       6
-    BadCnt        4
-    BadRate     0.4
-    dtype: object
-    >>> sample_df.groupby('prod').apply(sample_stats, target='y')
-          TotalCnt  GoodCnt  BadCnt   BadRate
-    prod
-    a            3        2       1  0.333333
-    b            4        2       2  0.500000
-    c            3        2       1  0.333333
-
-    Args:
-        df: pd.DataFrame, 样本集
-        target: 目标变量名
-
-    Returns:
-        pd.Series，各个统计量组成的数列
-
-    """
-    y = df[target]
-    ttl_cnt = len(y)
-    good_cnt = np.sum(y == 0)
-    bad_cnt = np.sum(y == 1)
-    bad_rate = bad_cnt / (good_cnt + bad_cnt)
-    return pd.Series([ttl_cnt, good_cnt, bad_cnt, bad_rate],
-                     index=['TotalCnt', 'GoodCnt', 'BadCnt', 'BadRate'],
-                     dtype='object')
-
-
-def monotonic(series: pd.Series) -> str:
-    """
-    判断一组序列(pd.Series)的单调类型，包括以下五种类型：
-
-    * 'increasing' - 单调递增
-    * 'decreasing' - 单调递减
-    * 'up_u_shape' - 先单调递减，后单调递增
-    * 'down_u_shape' - 先单调递增，后单调递增
-
-    Args:
-        series: pd.Series, 数值型数组序列
-
-    Returns:
-        str, 单调类型
-
-    """
-    if series.is_monotonic_increasing:
-        return 'increasing'
-    elif series.is_monotonic_decreasing:
-        return 'decreasing'
-    else:
-        for i in range(2, len(series)):
-            if series[:i].is_monotonic_increasing and \
-                    series[i:].is_monotonic_decreasing:
-                return 'down_u_shape'
-            elif series[:i].is_monotonic_decreasing and \
-                    series[i:].is_monotonic_increasing:
-                return 'up_u_shape'
-    return 'non_monotonic'
-
-
-def round_(a, significant_figures=1):
-    """
-    按照有效数字个数进行四舍五入
-
-    Args:
-        a:
-        significant_figures:
-
-    Returns:
-
-    """
-    e = np.ceil(np.log10(np.where(a == 0, 1, np.abs(a))))
-    sig_figs = a / 10**e
-    sig_figs = np.round(sig_figs, significant_figures)
-    return sig_figs * 10**e
-
-
-def interactive_mode():
-    # noinspection PyPackageRequirements
-    import __main__ as main
-    if hasattr(main, '__file__'):
-        return False
-    else:
-        return True
-
-
-def str_to_list(x):
-    if x is not None and isinstance(x, str):
-        x = [x]
-    return x
-
-
-def exception_trace(func):
-
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        try:
-            result = func(*args, **kwargs)
-            return result
-        except Exception as e:
-            raise RuntimeError(f'Error in running {func.__name__} with '
-                               f'args={args}'
-                               f'kwargs={kwargs}')
-
-    return wrapper
+# -*- encoding: utf-8 -*-
+from functools import wraps
+
+import numpy as np
+import pandas as pd
+
+
+def sample_stats(df, target):
+    """
+    统计样本中好坏样本数量及坏样本占比，使用示例如下：
+
+    >>> sample_df = pd.DataFrame({
+    ...     'id': np.arange(10),
+    ...     'prod': ['a', 'a', 'a', 'b', 'b', 'b', 'b', 'c', 'c', 'c'],
+    ...     'y': [0, 0, 1, 1, 0, 1, 0, 1, 0, 0, 1]})
+    >>> sample_df
+       id prod  y
+    0   0    a  0
+    1   1    a  0
+    2   2    a  1
+    3   3    b  1
+    4   4    b  0
+    5   5    b  1
+    6   6    b  0
+    7   7    c  1
+    8   8    c  0
+    9   9    c  0
+    >>> sample_stats(sample_df, target='y')
+    TotalCnt     10
+    GoodCnt       6
+    BadCnt        4
+    BadRate     0.4
+    dtype: object
+    >>> sample_df.groupby('prod').apply(sample_stats, target='y')
+          TotalCnt  GoodCnt  BadCnt   BadRate
+    prod
+    a            3        2       1  0.333333
+    b            4        2       2  0.500000
+    c            3        2       1  0.333333
+
+    Args:
+        df: pd.DataFrame, 样本集
+        target: 目标变量名
+
+    Returns:
+        pd.Series，各个统计量组成的数列
+
+    """
+    y = df[target]
+    ttl_cnt = len(y)
+    good_cnt = np.sum(y == 0)
+    bad_cnt = np.sum(y == 1)
+    bad_rate = bad_cnt / (good_cnt + bad_cnt)
+    return pd.Series([ttl_cnt, good_cnt, bad_cnt, bad_rate],
+                     index=['TotalCnt', 'GoodCnt', 'BadCnt', 'BadRate'],
+                     dtype='object')
+
+
+def monotonic(series: pd.Series) -> str:
+    """
+    判断一组序列(pd.Series)的单调类型，包括以下五种类型：
+
+    * 'increasing' - 单调递增
+    * 'decreasing' - 单调递减
+    * 'up_u_shape' - 先单调递减，后单调递增
+    * 'down_u_shape' - 先单调递增，后单调递增
+
+    Args:
+        series: pd.Series, 数值型数组序列
+
+    Returns:
+        str, 单调类型
+
+    """
+    if series.is_monotonic_increasing:
+        return 'increasing'
+    elif series.is_monotonic_decreasing:
+        return 'decreasing'
+    else:
+        for i in range(2, len(series)):
+            if series[:i].is_monotonic_increasing and \
+                    series[i:].is_monotonic_decreasing:
+                return 'down_u_shape'
+            elif series[:i].is_monotonic_decreasing and \
+                    series[i:].is_monotonic_increasing:
+                return 'up_u_shape'
+    return 'non_monotonic'
+
+
+def round_(a, significant_figures=1):
+    """
+    按照有效数字个数进行四舍五入
+
+    Args:
+        a:
+        significant_figures:
+
+    Returns:
+
+    """
+    e = np.ceil(np.log10(np.where(a == 0, 1, np.abs(a))))
+    sig_figs = a / 10**e
+    sig_figs = np.round(sig_figs, significant_figures)
+    return sig_figs * 10**e
+
+
+def interactive_mode():
+    # noinspection PyPackageRequirements
+    import __main__ as main
+    if hasattr(main, '__file__'):
+        return False
+    else:
+        return True
+
+
+def str_to_list(x):
+    if x is not None and isinstance(x, str):
+        x = [x]
+    return x
+
+
+def exception_trace(func):
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            result = func(*args, **kwargs)
+            return result
+        except Exception as e:
+            raise RuntimeError(f'Error in running {func.__name__} with '
+                               f'args={args}'
+                               f'kwargs={kwargs}')
+
+    return wrapper
```

### Comparing `sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/PKG-INFO` & `sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sy-riskmodels
-Version: 0.0.7
+Name: sy_riskmodels
+Version: 0.0.8
 Summary: 信用风险模型工具包
 Author-email: YAO Siyuan <siyuan89@163.com>
 Project-URL: Homepage, https://github.com/siyuany/riskmodels
 Project-URL: Bug Tracker, https://github.com/siyuany/riskmodels/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sy_riskmodels-0.0.7/src/sy_riskmodels.egg-info/SOURCES.txt` & `sy_riskmodels-0.0.8/src/sy_riskmodels.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
-src/riskmodels/__init__.py
-src/riskmodels/detector.py
-src/riskmodels/evaluate.py
-src/riskmodels/logging.py
-src/riskmodels/models.py
-src/riskmodels/rule.py
-src/riskmodels/scorecard.py
-src/riskmodels/utils.py
-src/riskmodels/contrib/__init__.py
-src/riskmodels/contrib/build_scorecard.py
-src/riskmodels/contrib/var_select.py
+src/sy_riskmodels/__init__.py
+src/sy_riskmodels/detector.py
+src/sy_riskmodels/evaluate.py
+src/sy_riskmodels/logging.py
+src/sy_riskmodels/models.py
+src/sy_riskmodels/rule.py
+src/sy_riskmodels/scorecard.py
+src/sy_riskmodels/utils.py
 src/sy_riskmodels.egg-info/PKG-INFO
 src/sy_riskmodels.egg-info/SOURCES.txt
 src/sy_riskmodels.egg-info/dependency_links.txt
 src/sy_riskmodels.egg-info/top_level.txt
+src/sy_riskmodels/contrib/__init__.py
+src/sy_riskmodels/contrib/build_scorecard.py
+src/sy_riskmodels/contrib/var_select.py
 test/test_detect.py
 test/test_scorecard.py
```

