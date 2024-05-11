# Comparing `tmp/xtuner-0.1.8.tar.gz` & `tmp/xtuner-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtuner-0.1.8.tar", last modified: Wed Nov 15 10:37:49 2023, max compression
+gzip compressed data, was "xtuner-0.1.9.tar", last modified: Thu Nov 16 05:59:46 2023, max compression
```

## Comparing `xtuner-0.1.8.tar` & `xtuner-0.1.9.tar`

### file list

```diff
@@ -1,455 +1,456 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-15 10:37:47.000000 xtuner-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-15 10:37:47.000000 xtuner-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14376 2023-11-15 10:37:49.899417 xtuner-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2023-11-15 10:37:47.000000 xtuner-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      421 2023-11-15 10:37:49.899417 xtuner-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-11-15 10:37:47.000000 xtuner-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.835417 xtuner-0.1.8/xtuner/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.835417 xtuner-0.1.8/xtuner/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.839417 xtuner-0.1.8/xtuner/apis/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/alpaca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/code_alpaca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/colorist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/lawyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/medical.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/moss_003_sft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/oasst1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/open_orca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/tiny_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/datasets/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/apis/training_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.839417 xtuner-0.1.8/xtuner/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.831417 xtuner-0.1.8/xtuner/configs/baichuan/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.839417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_sql_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.843417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6890 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_open_platypus_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.843417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_sql_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.847417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7244 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_open_platypus_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.847417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e2_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_plugins_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.851417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.855417 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6882 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e2_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_plugins_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.831417 xtuner-0.1.8/xtuner/configs/chatglm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.855417 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.859417 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.859417 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8574 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.863417 xtuner-0.1.8/xtuner/configs/deepspeed/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/deepspeed/deepspeed_zero2.json
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/deepspeed/deepspeed_zero2_offload.json
--rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/deepspeed/deepspeed_zero3.json
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/deepspeed/deepspeed_zero3_offload.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.831417 xtuner-0.1.8/xtuner/configs/internlm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.863417 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_msagent_react_e3_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_sql_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.867417 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e2_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_plugins_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_msagent_react_e3_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_mmlu_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.867417 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_open_platypus_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.871417 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.831417 xtuner-0.1.8/xtuner/configs/llama/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.871417 xtuner-0.1.8/xtuner/configs/llama/llama2_70b/
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1_hf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.875417 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_full_wizardlm_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e2_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_plugins_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7728 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_msagent_react_e3_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.879417 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.879417 xtuner-0.1.8/xtuner/configs/llama/llama_7b/
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e2_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_plugins_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.879417 xtuner-0.1.8/xtuner/configs/mistral/
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/mistral/mistral_7b_qlora_skypile_pretrain_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.831417 xtuner-0.1.8/xtuner/configs/qwen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.883417 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7394 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6317 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e2_gpu8.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_plugins_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_zh_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8599 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_arxiv_gentitle_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_code_alpaca_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_colorist_e5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7286 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_lawyer_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_medical_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_512_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_open_platypus_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6267 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_openorca_e1.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_sql_e3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_tiny_codes_e1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/configs/starcoder/
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/starcoder/starcoder_qlora_stack_exchange_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.831417 xtuner-0.1.8/xtuner/configs/yi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/configs/yi/yi_34b/
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/yi/yi_34b/yi_34b_qlora_alpaca_enzh_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/configs/yi/yi_6b/
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/yi/yi_6b/yi_6b_qlora_alpaca_enzh_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/configs/zephyr/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/configs/zephyr/zephyr_7b_beta_qlora_alpaca_e3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/dataset/collate_fns/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/collate_fns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/collate_fns/defalut_collate_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/collate_fns/mmlu_collate_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/concat_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.887417 xtuner-0.1.8/xtuner/dataset/map_fns/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.891417 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/alpaca_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/alpaca_zh_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/arxiv_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/code_alpaca_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/colors_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/crime_kg_assitant_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/default_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/law_reference_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/medical_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/msagent_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/oasst1_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/openai_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/openorca_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/pretrain_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/sql_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/stack_exchange_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/tiny_codes_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/wizardlm_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/map_fns/template_map_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/modelscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/moss_sft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.891417 xtuner-0.1.8/xtuner/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.891417 xtuner-0.1.8/xtuner/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/engine/hooks/dataset_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/engine/hooks/evaluate_chat_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/entry_point.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.891417 xtuner-0.1.8/xtuner/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/evaluation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.891417 xtuner-0.1.8/xtuner/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/evaluation/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/evaluation/metrics/mmlu_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.891417 xtuner-0.1.8/xtuner/model/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/xtuner/model/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/baichuan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/internlm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/internlm_attn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/modules/yi.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/xtuner/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/check_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/copy_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/xtuner/tools/data_preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/data_preprocess/arxiv.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/list_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/log_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/xtuner/tools/model_converters/
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/model_converters/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/model_converters/pth_to_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/model_converters/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/xtuner/tools/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/plugins/calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/plugins/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/plugins/solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.895417 xtuner-0.1.8/xtuner/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/utils/stop_criteria.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-11-15 10:37:47.000000 xtuner-0.1.8/xtuner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-15 10:37:49.835417 xtuner-0.1.8/xtuner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14376 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25464 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-15 10:37:49.000000 xtuner-0.1.8/xtuner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.782738 xtuner-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-16 05:59:44.000000 xtuner-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-16 05:59:44.000000 xtuner-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2023-11-16 05:59:46.782738 xtuner-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2023-11-16 05:59:44.000000 xtuner-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2023-11-16 05:59:46.782738 xtuner-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2023-11-16 05:59:44.000000 xtuner-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.722737 xtuner-0.1.9/xtuner/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.722737 xtuner-0.1.9/xtuner/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.722737 xtuner-0.1.9/xtuner/apis/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/code_alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/colorist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/lawyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/medical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/moss_003_sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/oasst1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/open_orca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/tiny_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/datasets/wizardlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/apis/training_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.722737 xtuner-0.1.9/xtuner/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.714737 xtuner-0.1.9/xtuner/configs/baichuan/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.726737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_sql_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.726737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6890 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7352 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_open_platypus_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.730737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_sql_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.730737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7244 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_open_platypus_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.734737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e2_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_plugins_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.734737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6234 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.738737 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6882 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e2_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_plugins_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.714737 xtuner-0.1.9/xtuner/configs/chatglm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.742738 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.742738 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6901 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8569 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.746738 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8574 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.746738 xtuner-0.1.9/xtuner/configs/deepspeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/deepspeed/deepspeed_zero1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/deepspeed/deepspeed_zero2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/deepspeed/deepspeed_zero2_offload.json
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/deepspeed/deepspeed_zero3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/deepspeed/deepspeed_zero3_offload.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.714737 xtuner-0.1.9/xtuner/configs/internlm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.750738 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_msagent_react_e3_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_sql_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.754738 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6554 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e2_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_plugins_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_msagent_react_e3_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_mmlu_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.754738 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_open_platypus_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.758738 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8551 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.718737 xtuner-0.1.9/xtuner/configs/llama/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.758738 xtuner-0.1.9/xtuner/configs/llama/llama2_70b/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1_hf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.758738 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_full_wizardlm_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e2_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_plugins_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_msagent_react_e3_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6449 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.762738 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.766738 xtuner-0.1.9/xtuner/configs/llama/llama_7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e2_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_plugins_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.766738 xtuner-0.1.9/xtuner/configs/mistral/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/mistral/mistral_7b_qlora_skypile_pretrain_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.718737 xtuner-0.1.9/xtuner/configs/qwen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.766738 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7394 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6317 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e2_gpu8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_plugins_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.770738 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_zh_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8599 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_arxiv_gentitle_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_code_alpaca_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_colorist_e5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_lawyer_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_medical_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_512_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_open_platypus_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6267 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_openorca_e1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_sql_e3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_tiny_codes_e1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.770738 xtuner-0.1.9/xtuner/configs/starcoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/starcoder/starcoder_qlora_stack_exchange_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.718737 xtuner-0.1.9/xtuner/configs/yi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.770738 xtuner-0.1.9/xtuner/configs/yi/yi_34b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/yi/yi_34b/yi_34b_qlora_alpaca_enzh_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.770738 xtuner-0.1.9/xtuner/configs/yi/yi_6b/
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/yi/yi_6b/yi_6b_qlora_alpaca_enzh_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.770738 xtuner-0.1.9/xtuner/configs/zephyr/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/configs/zephyr/zephyr_7b_beta_qlora_alpaca_e3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.770738 xtuner-0.1.9/xtuner/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.774738 xtuner-0.1.9/xtuner/dataset/collate_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/collate_fns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/collate_fns/defalut_collate_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/collate_fns/mmlu_collate_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/concat_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.774738 xtuner-0.1.9/xtuner/dataset/map_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.774738 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/alpaca_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/alpaca_zh_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/arxiv_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/code_alpaca_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/colors_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/crime_kg_assitant_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/default_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/law_reference_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/medical_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/msagent_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/oasst1_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/openai_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/openorca_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/pretrain_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/sql_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/stack_exchange_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/tiny_codes_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/wizardlm_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/map_fns/template_map_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/modelscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/moss_sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.774738 xtuner-0.1.9/xtuner/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/engine/hooks/dataset_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/engine/hooks/evaluate_chat_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/entry_point.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/evaluation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/evaluation/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/evaluation/metrics/mmlu_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/model/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/baichuan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/internlm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/internlm_attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/modules/yi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/check_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/copy_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/tools/data_preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/data_preprocess/arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/list_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/log_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.778738 xtuner-0.1.9/xtuner/tools/model_converters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/model_converters/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/model_converters/pth_to_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/model_converters/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.782738 xtuner-0.1.9/xtuner/tools/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/plugins/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/plugins/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/plugins/solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.782738 xtuner-0.1.9/xtuner/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/utils/stop_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2023-11-16 05:59:44.000000 xtuner-0.1.9/xtuner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 05:59:46.722737 xtuner-0.1.9/xtuner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25510 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-16 05:59:46.000000 xtuner-0.1.9/xtuner.egg-info/top_level.txt
```

### Comparing `xtuner-0.1.8/LICENSE` & `xtuner-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/PKG-INFO` & `xtuner-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtuner
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolkit for efficiently fine-tuning LLM
 Home-page: https://github.com/InternLM/xtuner
 Author: XTuner Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="https://github.com/InternLM/lmdeploy/assets/36994684/0cf8d00f-e86b-40ba-9b54-dc8f1bc6c8d8" width="600"/>
@@ -18,15 +18,15 @@
         
         👋 join us on <a href="https://twitter.com/intern_lm" target="_blank">Twitter</a>, <a href="https://discord.gg/xa29JuW87d" target="_blank">Discord</a> and <a href="https://cdn.vansin.top/internlm/xtuner.jpg" target="_blank">WeChat</a>
         
         </div>
         
         ## 🎉 News
         
-        - **\[2023/10\]** Support [ChatGLM3-6B](https://huggingface.co/THUDM/chatglm3-6b) model!
+        - **\[2023/11\]** Support [ChatGLM3-6B](https://huggingface.co/THUDM/chatglm3-6b) model!
         - **\[2023/10\]** Support [MSAgent-Bench](https://modelscope.cn/datasets/damo/MSAgent-Bench) dataset, and the fine-tuned LLMs can be applied by [Lagent](https://github.com/InternLM/lagent)!
         - **\[2023/10\]** Optimize the data processing to accommodate `system` context. More information can be found on [Docs](docs/en/user_guides/dataset_format.md)!
         - **\[2023/09\]** Support [InternLM-20B](https://huggingface.co/internlm) models!
         - **\[2023/09\]** Support [Baichuan2](https://huggingface.co/baichuan-inc) models!
         - **\[2023/08\]** XTuner is released, with multiple fine-tuned adapters on [HuggingFace](https://huggingface.co/xtuner).
         
         ## 📖 Introduction
@@ -182,21 +182,23 @@
           xtuner train ${CONFIG_NAME_OR_PATH}
           ```
         
           For example, we can start the QLoRA fine-tuning of InternLM-7B with oasst1 dataset by
         
           ```shell
           # On a single GPU
-          xtuner train internlm_7b_qlora_oasst1_e3
+          xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2
           # On multiple GPUs
-          (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train internlm_7b_qlora_oasst1_e3
-          (SLURM) srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm
+          (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2
+          (SLURM) srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm --deepspeed deepspeed_zero2
           ```
         
-          For more examples, please see [finetune.md](./docs/en/user_guides/finetune.md).
+          - `--deepspeed` means using [DeepSpeed](https://github.com/microsoft/DeepSpeed) 🚀 to optimize the training. XTuner comes with several integrated strategies including ZeRO-1, ZeRO-2, and ZeRO-3. If you wish to disable this feature, simply remove this argument.
+        
+          - For more examples, please see [finetune.md](./docs/en/user_guides/finetune.md).
         
         - **Step 2**, convert the saved PTH model (if using DeepSpeed, it will be a directory) to HuggingFace model, by
         
           ```shell
           xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH} ${PTH} ${SAVE_PATH}
           ```
         
@@ -245,16 +247,14 @@
               --temperture 0.8 \
               --top_p 0.95 \
               --seed 0
           ```
         
           🔥 Seeking efficient inference with less GPU memory? Try 4-bit quantization from [LMDeploy](https://github.com/InternLM/lmdeploy)! For more details, see [here](https://github.com/InternLM/lmdeploy/tree/main#quantization).
         
-          🎯 We are woking closely with [LMDeploy](https://github.com/InternLM/lmdeploy), to implement the deployment of **plugin-based chat**!
-        
         ### Evaluation
         
         - We recommend using [OpenCompass](https://github.com/InternLM/opencompass), a comprehensive and systematic LLM evaluation library, which currently supports 50+ datasets with about 300,000 questions.
         
         ## 🤝 Contributing
         
         We appreciate all contributions to XTuner. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guideline.
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: xtuner Version: 0.1.8 Summary: A toolkit for
+Metadata-Version: 2.1 Name: xtuner Version: 0.1.9 Summary: A toolkit for
 efficiently fine-tuning LLM Home-page: https://github.com/InternLM/xtuner
 Author: XTuner Contributors Author-email: openmmlab@gmail.com License: Apache
 License 2.0 Description:
 [https://github.com/InternLM/lmdeploy/assets/36994684/0cf8d00f-e86b-40ba-9b54-
                                  dc8f1bc6c8d8]
 
 [![license](https://img.shields.io/github/license/InternLM/xtuner.svg)](https:/
 /github.com/InternLM/xtuner/blob/main/LICENSE) [![PyPI](https://badge.fury.io/
  py/xtuner.svg)](https://pypi.org/project/xtuner/) [![Generic badge](https://
      img.shields.io/badge/ð¤%20Huggingface-xtuner-yellow.svg)](https://
  huggingface.co/xtuner) English | [ç®ä½ä¸­æ](README_zh-CN.md) ð join us
                         on _T_w_i_t_t_e_r, _D_i_s_c_o_r_d and _W_e_C_h_a_t
-## ð News - **\[2023/10\]** Support [ChatGLM3-6B](https://huggingface.co/
+## ð News - **\[2023/11\]** Support [ChatGLM3-6B](https://huggingface.co/
 THUDM/chatglm3-6b) model! - **\[2023/10\]** Support [MSAgent-Bench](https://
 modelscope.cn/datasets/damo/MSAgent-Bench) dataset, and the fine-tuned LLMs can
 be applied by [Lagent](https://github.com/InternLM/lagent)! - **\[2023/10\]**
 Optimize the data processing to accommodate `system` context. More information
 can be found on [Docs](docs/en/user_guides/dataset_format.md)! - **\[2023/
 09\]** Support [InternLM-20B](https://huggingface.co/internlm) models! - **\
 [2023/09\]** Support [Baichuan2](https://huggingface.co/baichuan-inc) models! -
@@ -87,55 +87,57 @@
 provides many ready-to-use configs and we can view all configs by ```shell
 xtuner list-cfg ``` Or, if the provided configs cannot meet the requirements,
 please copy the provided config to the specified directory and make specific
 modifications by ```shell xtuner copy-cfg ${CONFIG_NAME} ${SAVE_PATH} ``` -
 **Step 1**, start fine-tuning. ```shell xtuner train ${CONFIG_NAME_OR_PATH} ```
 For example, we can start the QLoRA fine-tuning of InternLM-7B with oasst1
 dataset by ```shell # On a single GPU xtuner train internlm_7b_qlora_oasst1_e3
-# On multiple GPUs (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train
-internlm_7b_qlora_oasst1_e3 (SLURM) srun ${SRUN_ARGS} xtuner train
-internlm_7b_qlora_oasst1_e3 --launcher slurm ``` For more examples, please see
-[finetune.md](./docs/en/user_guides/finetune.md). - **Step 2**, convert the
-saved PTH model (if using DeepSpeed, it will be a directory) to HuggingFace
-model, by ```shell xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH} ${PTH} $
-{SAVE_PATH} ``` ### Chat [![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-144OuTVyT_GvFyDMtlSlTzcxYIfnRsklq?usp=sharing) XTuner provides tools to chat
-with pretrained / fine-tuned LLMs. ```shell xtuner chat ${NAME_OR_PATH_TO_LLM}
---adapter {NAME_OR_PATH_TO_ADAPTER} [optional arguments] ``` For example, we
-can start the chat with InternLM-7B with adapter trained from Alpaca-enzh:
-```shell xtuner chat internlm/internlm-7b --adapter xtuner/internlm-7b-qlora-
-alpaca-enzh --prompt-template internlm_chat --system-template alpaca ```
-Llama2-7b with adapter trained from MOSS-003-SFT: ```shell xtuner chat meta-
-llama/Llama-2-7b-hf --adapter xtuner/Llama-2-7b-qlora-moss-003-sft --bot-name
-Llama2 --prompt-template moss_sft --system-template moss_sft --with-plugins
-calculate solve search --command-stop-word "" --answer-stop-word "" --no-
-streamer ``` For more examples, please see [chat.md](./docs/en/user_guides/
-chat.md). ### Deployment - **Step 0**, merge the HuggingFace adapter to
-pretrained LLM, by ```shell xtuner convert merge \ ${NAME_OR_PATH_TO_LLM} \ $
-{NAME_OR_PATH_TO_ADAPTER} \ ${SAVE_PATH} \ --max-shard-size 2GB ``` - **Step
-1**, deploy fine-tuned LLM with any other framework, such as [LMDeploy](https:/
-/github.com/InternLM/lmdeploy) ð. ```shell pip install lmdeploy python -
-m lmdeploy.pytorch.chat ${NAME_OR_PATH_TO_LLM} \ --max_new_tokens 256 \ --
-temperture 0.8 \ --top_p 0.95 \ --seed 0 ``` ð¥ Seeking efficient inference
-with less GPU memory? Try 4-bit quantization from [LMDeploy](https://
-github.com/InternLM/lmdeploy)! For more details, see [here](https://github.com/
-InternLM/lmdeploy/tree/main#quantization). ð¯ We are woking closely with
-[LMDeploy](https://github.com/InternLM/lmdeploy), to implement the deployment
-of **plugin-based chat**! ### Evaluation - We recommend using [OpenCompass]
-(https://github.com/InternLM/opencompass), a comprehensive and systematic LLM
-evaluation library, which currently supports 50+ datasets with about 300,000
-questions. ## ð¤ Contributing We appreciate all contributions to XTuner.
-Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
-guideline. ## ðï¸ Acknowledgement - [Llama 2](https://github.com/
-facebookresearch/llama) - [QLoRA](https://github.com/artidoro/qlora) -
-[LMDeploy](https://github.com/InternLM/lmdeploy) ## License This project is
-released under the [Apache License 2.0](LICENSE). Please also adhere to the
-Licenses of models and datasets being used. Keywords: large language
-model,parameter-efficient fine-tuning Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: all Provides-
-Extra: deepspeed
+--deepspeed deepspeed_zero2 # On multiple GPUs (DIST) NPROC_PER_NODE=${GPU_NUM}
+xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2 (SLURM)
+srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm --
+deepspeed deepspeed_zero2 ``` - `--deepspeed` means using [DeepSpeed](https://
+github.com/microsoft/DeepSpeed) ð to optimize the training. XTuner comes
+with several integrated strategies including ZeRO-1, ZeRO-2, and ZeRO-3. If you
+wish to disable this feature, simply remove this argument. - For more examples,
+please see [finetune.md](./docs/en/user_guides/finetune.md). - **Step 2**,
+convert the saved PTH model (if using DeepSpeed, it will be a directory) to
+HuggingFace model, by ```shell xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH}
+${PTH} ${SAVE_PATH} ``` ### Chat [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/144OuTVyT_GvFyDMtlSlTzcxYIfnRsklq?usp=sharing)
+XTuner provides tools to chat with pretrained / fine-tuned LLMs. ```shell
+xtuner chat ${NAME_OR_PATH_TO_LLM} --adapter {NAME_OR_PATH_TO_ADAPTER}
+[optional arguments] ``` For example, we can start the chat with InternLM-7B
+with adapter trained from Alpaca-enzh: ```shell xtuner chat internlm/internlm-
+7b --adapter xtuner/internlm-7b-qlora-alpaca-enzh --prompt-template
+internlm_chat --system-template alpaca ``` Llama2-7b with adapter trained from
+MOSS-003-SFT: ```shell xtuner chat meta-llama/Llama-2-7b-hf --adapter xtuner/
+Llama-2-7b-qlora-moss-003-sft --bot-name Llama2 --prompt-template moss_sft --
+system-template moss_sft --with-plugins calculate solve search --command-stop-
+word "" --answer-stop-word "" --no-streamer ``` For more examples, please see
+[chat.md](./docs/en/user_guides/chat.md). ### Deployment - **Step 0**, merge
+the HuggingFace adapter to pretrained LLM, by ```shell xtuner convert merge \ $
+{NAME_OR_PATH_TO_LLM} \ ${NAME_OR_PATH_TO_ADAPTER} \ ${SAVE_PATH} \ --max-
+shard-size 2GB ``` - **Step 1**, deploy fine-tuned LLM with any other
+framework, such as [LMDeploy](https://github.com/InternLM/lmdeploy) ð.
+```shell pip install lmdeploy python -m lmdeploy.pytorch.chat $
+{NAME_OR_PATH_TO_LLM} \ --max_new_tokens 256 \ --temperture 0.8 \ --top_p 0.95
+\ --seed 0 ``` ð¥ Seeking efficient inference with less GPU memory? Try 4-bit
+quantization from [LMDeploy](https://github.com/InternLM/lmdeploy)! For more
+details, see [here](https://github.com/InternLM/lmdeploy/tree/
+main#quantization). ### Evaluation - We recommend using [OpenCompass](https://
+github.com/InternLM/opencompass), a comprehensive and systematic LLM evaluation
+library, which currently supports 50+ datasets with about 300,000 questions. ##
+ð¤ Contributing We appreciate all contributions to XTuner. Please refer to
+[CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guideline. ##
+ðï¸ Acknowledgement - [Llama 2](https://github.com/facebookresearch/llama)
+- [QLoRA](https://github.com/artidoro/qlora) - [LMDeploy](https://github.com/
+InternLM/lmdeploy) ## License This project is released under the [Apache
+License 2.0](LICENSE). Please also adhere to the Licenses of models and
+datasets being used. Keywords: large language model,parameter-efficient fine-
+tuning Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Topic :: Utilities Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: all Provides-Extra: deepspeed
```

### Comparing `xtuner-0.1.8/README.md` & `xtuner-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 👋 join us on <a href="https://twitter.com/intern_lm" target="_blank">Twitter</a>, <a href="https://discord.gg/xa29JuW87d" target="_blank">Discord</a> and <a href="https://cdn.vansin.top/internlm/xtuner.jpg" target="_blank">WeChat</a>
 
 </div>
 
 ## 🎉 News
 
-- **\[2023/10\]** Support [ChatGLM3-6B](https://huggingface.co/THUDM/chatglm3-6b) model!
+- **\[2023/11\]** Support [ChatGLM3-6B](https://huggingface.co/THUDM/chatglm3-6b) model!
 - **\[2023/10\]** Support [MSAgent-Bench](https://modelscope.cn/datasets/damo/MSAgent-Bench) dataset, and the fine-tuned LLMs can be applied by [Lagent](https://github.com/InternLM/lagent)!
 - **\[2023/10\]** Optimize the data processing to accommodate `system` context. More information can be found on [Docs](docs/en/user_guides/dataset_format.md)!
 - **\[2023/09\]** Support [InternLM-20B](https://huggingface.co/internlm) models!
 - **\[2023/09\]** Support [Baichuan2](https://huggingface.co/baichuan-inc) models!
 - **\[2023/08\]** XTuner is released, with multiple fine-tuned adapters on [HuggingFace](https://huggingface.co/xtuner).
 
 ## 📖 Introduction
@@ -174,21 +174,23 @@
   xtuner train ${CONFIG_NAME_OR_PATH}
   ```
 
   For example, we can start the QLoRA fine-tuning of InternLM-7B with oasst1 dataset by
 
   ```shell
   # On a single GPU
-  xtuner train internlm_7b_qlora_oasst1_e3
+  xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2
   # On multiple GPUs
-  (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train internlm_7b_qlora_oasst1_e3
-  (SLURM) srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm
+  (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2
+  (SLURM) srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm --deepspeed deepspeed_zero2
   ```
 
-  For more examples, please see [finetune.md](./docs/en/user_guides/finetune.md).
+  - `--deepspeed` means using [DeepSpeed](https://github.com/microsoft/DeepSpeed) 🚀 to optimize the training. XTuner comes with several integrated strategies including ZeRO-1, ZeRO-2, and ZeRO-3. If you wish to disable this feature, simply remove this argument.
+
+  - For more examples, please see [finetune.md](./docs/en/user_guides/finetune.md).
 
 - **Step 2**, convert the saved PTH model (if using DeepSpeed, it will be a directory) to HuggingFace model, by
 
   ```shell
   xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH} ${PTH} ${SAVE_PATH}
   ```
 
@@ -237,16 +239,14 @@
       --temperture 0.8 \
       --top_p 0.95 \
       --seed 0
   ```
 
   🔥 Seeking efficient inference with less GPU memory? Try 4-bit quantization from [LMDeploy](https://github.com/InternLM/lmdeploy)! For more details, see [here](https://github.com/InternLM/lmdeploy/tree/main#quantization).
 
-  🎯 We are woking closely with [LMDeploy](https://github.com/InternLM/lmdeploy), to implement the deployment of **plugin-based chat**!
-
 ### Evaluation
 
 - We recommend using [OpenCompass](https://github.com/InternLM/opencompass), a comprehensive and systematic LLM evaluation library, which currently supports 50+ datasets with about 300,000 questions.
 
 ## 🤝 Contributing
 
 We appreciate all contributions to XTuner. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guideline.
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 [![license](https://img.shields.io/github/license/InternLM/xtuner.svg)](https:/
 /github.com/InternLM/xtuner/blob/main/LICENSE) [![PyPI](https://badge.fury.io/
  py/xtuner.svg)](https://pypi.org/project/xtuner/) [![Generic badge](https://
      img.shields.io/badge/ð¤%20Huggingface-xtuner-yellow.svg)](https://
  huggingface.co/xtuner) English | [ç®ä½ä¸­æ](README_zh-CN.md) ð join us
                         on _T_w_i_t_t_e_r, _D_i_s_c_o_r_d and _W_e_C_h_a_t
-## ð News - **\[2023/10\]** Support [ChatGLM3-6B](https://huggingface.co/
+## ð News - **\[2023/11\]** Support [ChatGLM3-6B](https://huggingface.co/
 THUDM/chatglm3-6b) model! - **\[2023/10\]** Support [MSAgent-Bench](https://
 modelscope.cn/datasets/damo/MSAgent-Bench) dataset, and the fine-tuned LLMs can
 be applied by [Lagent](https://github.com/InternLM/lagent)! - **\[2023/10\]**
 Optimize the data processing to accommodate `system` context. More information
 can be found on [Docs](docs/en/user_guides/dataset_format.md)! - **\[2023/
 09\]** Support [InternLM-20B](https://huggingface.co/internlm) models! - **\
 [2023/09\]** Support [Baichuan2](https://huggingface.co/baichuan-inc) models! -
@@ -83,47 +83,50 @@
 provides many ready-to-use configs and we can view all configs by ```shell
 xtuner list-cfg ``` Or, if the provided configs cannot meet the requirements,
 please copy the provided config to the specified directory and make specific
 modifications by ```shell xtuner copy-cfg ${CONFIG_NAME} ${SAVE_PATH} ``` -
 **Step 1**, start fine-tuning. ```shell xtuner train ${CONFIG_NAME_OR_PATH} ```
 For example, we can start the QLoRA fine-tuning of InternLM-7B with oasst1
 dataset by ```shell # On a single GPU xtuner train internlm_7b_qlora_oasst1_e3
-# On multiple GPUs (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train
-internlm_7b_qlora_oasst1_e3 (SLURM) srun ${SRUN_ARGS} xtuner train
-internlm_7b_qlora_oasst1_e3 --launcher slurm ``` For more examples, please see
-[finetune.md](./docs/en/user_guides/finetune.md). - **Step 2**, convert the
-saved PTH model (if using DeepSpeed, it will be a directory) to HuggingFace
-model, by ```shell xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH} ${PTH} $
-{SAVE_PATH} ``` ### Chat [![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-144OuTVyT_GvFyDMtlSlTzcxYIfnRsklq?usp=sharing) XTuner provides tools to chat
-with pretrained / fine-tuned LLMs. ```shell xtuner chat ${NAME_OR_PATH_TO_LLM}
---adapter {NAME_OR_PATH_TO_ADAPTER} [optional arguments] ``` For example, we
-can start the chat with InternLM-7B with adapter trained from Alpaca-enzh:
-```shell xtuner chat internlm/internlm-7b --adapter xtuner/internlm-7b-qlora-
-alpaca-enzh --prompt-template internlm_chat --system-template alpaca ```
-Llama2-7b with adapter trained from MOSS-003-SFT: ```shell xtuner chat meta-
-llama/Llama-2-7b-hf --adapter xtuner/Llama-2-7b-qlora-moss-003-sft --bot-name
-Llama2 --prompt-template moss_sft --system-template moss_sft --with-plugins
-calculate solve search --command-stop-word "" --answer-stop-word "" --no-
-streamer ``` For more examples, please see [chat.md](./docs/en/user_guides/
-chat.md). ### Deployment - **Step 0**, merge the HuggingFace adapter to
-pretrained LLM, by ```shell xtuner convert merge \ ${NAME_OR_PATH_TO_LLM} \ $
-{NAME_OR_PATH_TO_ADAPTER} \ ${SAVE_PATH} \ --max-shard-size 2GB ``` - **Step
-1**, deploy fine-tuned LLM with any other framework, such as [LMDeploy](https:/
-/github.com/InternLM/lmdeploy) ð. ```shell pip install lmdeploy python -
-m lmdeploy.pytorch.chat ${NAME_OR_PATH_TO_LLM} \ --max_new_tokens 256 \ --
-temperture 0.8 \ --top_p 0.95 \ --seed 0 ``` ð¥ Seeking efficient inference
-with less GPU memory? Try 4-bit quantization from [LMDeploy](https://
-github.com/InternLM/lmdeploy)! For more details, see [here](https://github.com/
-InternLM/lmdeploy/tree/main#quantization). ð¯ We are woking closely with
-[LMDeploy](https://github.com/InternLM/lmdeploy), to implement the deployment
-of **plugin-based chat**! ### Evaluation - We recommend using [OpenCompass]
-(https://github.com/InternLM/opencompass), a comprehensive and systematic LLM
-evaluation library, which currently supports 50+ datasets with about 300,000
-questions. ## ð¤ Contributing We appreciate all contributions to XTuner.
-Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
-guideline. ## ðï¸ Acknowledgement - [Llama 2](https://github.com/
-facebookresearch/llama) - [QLoRA](https://github.com/artidoro/qlora) -
-[LMDeploy](https://github.com/InternLM/lmdeploy) ## License This project is
-released under the [Apache License 2.0](LICENSE). Please also adhere to the
-Licenses of models and datasets being used.
+--deepspeed deepspeed_zero2 # On multiple GPUs (DIST) NPROC_PER_NODE=${GPU_NUM}
+xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2 (SLURM)
+srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm --
+deepspeed deepspeed_zero2 ``` - `--deepspeed` means using [DeepSpeed](https://
+github.com/microsoft/DeepSpeed) ð to optimize the training. XTuner comes
+with several integrated strategies including ZeRO-1, ZeRO-2, and ZeRO-3. If you
+wish to disable this feature, simply remove this argument. - For more examples,
+please see [finetune.md](./docs/en/user_guides/finetune.md). - **Step 2**,
+convert the saved PTH model (if using DeepSpeed, it will be a directory) to
+HuggingFace model, by ```shell xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH}
+${PTH} ${SAVE_PATH} ``` ### Chat [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/144OuTVyT_GvFyDMtlSlTzcxYIfnRsklq?usp=sharing)
+XTuner provides tools to chat with pretrained / fine-tuned LLMs. ```shell
+xtuner chat ${NAME_OR_PATH_TO_LLM} --adapter {NAME_OR_PATH_TO_ADAPTER}
+[optional arguments] ``` For example, we can start the chat with InternLM-7B
+with adapter trained from Alpaca-enzh: ```shell xtuner chat internlm/internlm-
+7b --adapter xtuner/internlm-7b-qlora-alpaca-enzh --prompt-template
+internlm_chat --system-template alpaca ``` Llama2-7b with adapter trained from
+MOSS-003-SFT: ```shell xtuner chat meta-llama/Llama-2-7b-hf --adapter xtuner/
+Llama-2-7b-qlora-moss-003-sft --bot-name Llama2 --prompt-template moss_sft --
+system-template moss_sft --with-plugins calculate solve search --command-stop-
+word "" --answer-stop-word "" --no-streamer ``` For more examples, please see
+[chat.md](./docs/en/user_guides/chat.md). ### Deployment - **Step 0**, merge
+the HuggingFace adapter to pretrained LLM, by ```shell xtuner convert merge \ $
+{NAME_OR_PATH_TO_LLM} \ ${NAME_OR_PATH_TO_ADAPTER} \ ${SAVE_PATH} \ --max-
+shard-size 2GB ``` - **Step 1**, deploy fine-tuned LLM with any other
+framework, such as [LMDeploy](https://github.com/InternLM/lmdeploy) ð.
+```shell pip install lmdeploy python -m lmdeploy.pytorch.chat $
+{NAME_OR_PATH_TO_LLM} \ --max_new_tokens 256 \ --temperture 0.8 \ --top_p 0.95
+\ --seed 0 ``` ð¥ Seeking efficient inference with less GPU memory? Try 4-bit
+quantization from [LMDeploy](https://github.com/InternLM/lmdeploy)! For more
+details, see [here](https://github.com/InternLM/lmdeploy/tree/
+main#quantization). ### Evaluation - We recommend using [OpenCompass](https://
+github.com/InternLM/opencompass), a comprehensive and systematic LLM evaluation
+library, which currently supports 50+ datasets with about 300,000 questions. ##
+ð¤ Contributing We appreciate all contributions to XTuner. Please refer to
+[CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guideline. ##
+ðï¸ Acknowledgement - [Llama 2](https://github.com/facebookresearch/llama)
+- [QLoRA](https://github.com/artidoro/qlora) - [LMDeploy](https://github.com/
+InternLM/lmdeploy) ## License This project is released under the [Apache
+License 2.0](LICENSE). Please also adhere to the Licenses of models and
+datasets being used.
```

### Comparing `xtuner-0.1.8/setup.py` & `xtuner-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/__init__.py` & `xtuner-0.1.9/xtuner/apis/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/alpaca.py` & `xtuner-0.1.9/xtuner/apis/datasets/alpaca.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/arxiv.py` & `xtuner-0.1.9/xtuner/apis/datasets/arxiv.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/code_alpaca.py` & `xtuner-0.1.9/xtuner/apis/datasets/code_alpaca.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/colorist.py` & `xtuner-0.1.9/xtuner/apis/datasets/colorist.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/lawyer.py` & `xtuner-0.1.9/xtuner/apis/datasets/lawyer.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/medical.py` & `xtuner-0.1.9/xtuner/apis/datasets/medical.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/moss_003_sft.py` & `xtuner-0.1.9/xtuner/apis/datasets/moss_003_sft.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/oasst1.py` & `xtuner-0.1.9/xtuner/apis/datasets/oasst1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/open_orca.py` & `xtuner-0.1.9/xtuner/apis/datasets/open_orca.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/sql.py` & `xtuner-0.1.9/xtuner/apis/datasets/sql.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/tiny_codes.py` & `xtuner-0.1.9/xtuner/apis/datasets/tiny_codes.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/datasets/wizardlm.py` & `xtuner-0.1.9/xtuner/apis/datasets/wizardlm.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/model.py` & `xtuner-0.1.9/xtuner/apis/model.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/apis/training_args.py` & `xtuner-0.1.9/xtuner/apis/training_args.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/__init__.py` & `xtuner-0.1.9/xtuner/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_base/baichuan2_13b_base_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_13b_chat/baichuan2_13b_chat_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_base/baichuan2_7b_base_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan2_7b_chat/baichuan2_7b_chat_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e2_gpu8.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_all_e2_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_plugins_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_moss_sft_plugins_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_base/baichuan_13b_base_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_13b_chat/baichuan_13b_chat_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e2_gpu8.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_all_e2_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_plugins_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_moss_sft_plugins_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/baichuan/baichuan_7b/baichuan_7b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm2_6b/chatglm2_6b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b/chatglm3_6b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/deepspeed/deepspeed_zero3_offload.json` & `xtuner-0.1.9/xtuner/configs/deepspeed/deepspeed_zero3_offload.json`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_msagent_react_e3_gpu8.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_msagent_react_e3_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_full_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_full_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e2_gpu8.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_all_e2_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_plugins_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_moss_sft_plugins_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_msagent_react_e3_gpu8.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_msagent_react_e3_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3_hf.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_e3_hf.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_mmlu_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_oasst1_mmlu_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_7b/internlm_7b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_20b/internlm_chat_20b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/internlm/internlm_chat_7b/internlm_chat_7b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1_hf.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_int8_lora_open_platypus_e1_hf.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1_hf.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_70b/llama2_70b_qlora_open_platypus_e1_hf.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_full_wizardlm_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_full_wizardlm_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e2_gpu8.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_all_e2_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_plugins_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_moss_sft_plugins_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_msagent_react_e3_gpu8.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_msagent_react_e3_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b/llama2_7b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama2_7b_chat/llama2_7b_chat_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e2_gpu8.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_all_e2_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_plugins_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_moss_sft_plugins_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/llama/llama_7b/llama_7b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/llama/llama_7b/llama_7b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/mistral/mistral_7b_qlora_skypile_pretrain_e1.py` & `xtuner-0.1.9/xtuner/configs/mistral/mistral_7b_qlora_skypile_pretrain_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e2_gpu8.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_all_e2_gpu8.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_plugins_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_moss_sft_plugins_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b/qwen_7b_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_enzh_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_zh_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_alpaca_zh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_arxiv_gentitle_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_arxiv_gentitle_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_code_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_code_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_colorist_e5.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_colorist_e5.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_lawyer_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_lawyer_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_medical_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_medical_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_512_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_512_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_oasst1_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_open_platypus_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_open_platypus_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_openorca_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_openorca_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_sql_e3.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_sql_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_tiny_codes_e1.py` & `xtuner-0.1.9/xtuner/configs/qwen/qwen_7b_chat/qwen_7b_chat_qlora_tiny_codes_e1.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/starcoder/starcoder_qlora_stack_exchange_example.py` & `xtuner-0.1.9/xtuner/configs/starcoder/starcoder_qlora_stack_exchange_example.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/yi/yi_34b/yi_34b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/yi/yi_34b/yi_34b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/yi/yi_6b/yi_6b_qlora_alpaca_enzh_e3.py` & `xtuner-0.1.9/xtuner/configs/yi/yi_6b/yi_6b_qlora_alpaca_enzh_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/configs/zephyr/zephyr_7b_beta_qlora_alpaca_e3.py` & `xtuner-0.1.9/xtuner/configs/zephyr/zephyr_7b_beta_qlora_alpaca_e3.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/collate_fns/defalut_collate_fn.py` & `xtuner-0.1.9/xtuner/dataset/collate_fns/defalut_collate_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/collate_fns/mmlu_collate_fn.py` & `xtuner-0.1.9/xtuner/dataset/collate_fns/mmlu_collate_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/concat_dataset.py` & `xtuner-0.1.9/xtuner/dataset/concat_dataset.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/huggingface.py` & `xtuner-0.1.9/xtuner/dataset/huggingface.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/__init__.py` & `xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/__init__.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/msagent_map_fn.py` & `xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/msagent_map_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/oasst1_map_fn.py` & `xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/oasst1_map_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/openai_map_fn.py` & `xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/openai_map_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/map_fns/dataset_map_fns/wizardlm_map_fn.py` & `xtuner-0.1.9/xtuner/dataset/map_fns/dataset_map_fns/wizardlm_map_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/map_fns/template_map_fn.py` & `xtuner-0.1.9/xtuner/dataset/map_fns/template_map_fn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/modelscope.py` & `xtuner-0.1.9/xtuner/dataset/modelscope.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/moss_sft.py` & `xtuner-0.1.9/xtuner/dataset/moss_sft.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/dataset/utils.py` & `xtuner-0.1.9/xtuner/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/engine/hooks/dataset_info_hook.py` & `xtuner-0.1.9/xtuner/engine/hooks/dataset_info_hook.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/engine/hooks/evaluate_chat_hook.py` & `xtuner-0.1.9/xtuner/engine/hooks/evaluate_chat_hook.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/entry_point.py` & `xtuner-0.1.9/xtuner/entry_point.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/evaluation/metrics/mmlu_metric.py` & `xtuner-0.1.9/xtuner/evaluation/metrics/mmlu_metric.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/modules/baichuan.py` & `xtuner-0.1.9/xtuner/model/modules/baichuan.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/modules/dispatch.py` & `xtuner-0.1.9/xtuner/model/modules/dispatch.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/modules/internlm.py` & `xtuner-0.1.9/xtuner/model/modules/internlm.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/modules/internlm_attn.py` & `xtuner-0.1.9/xtuner/model/modules/internlm_attn.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/modules/llama.py` & `xtuner-0.1.9/xtuner/model/modules/llama.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/modules/yi.py` & `xtuner-0.1.9/xtuner/model/modules/yi.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/sft.py` & `xtuner-0.1.9/xtuner/model/sft.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/model/utils.py` & `xtuner-0.1.9/xtuner/model/utils.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/chat.py` & `xtuner-0.1.9/xtuner/tools/chat.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/check_custom_dataset.py` & `xtuner-0.1.9/xtuner/tools/check_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/copy_cfg.py` & `xtuner-0.1.9/xtuner/tools/copy_cfg.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/data_preprocess/arxiv.py` & `xtuner-0.1.9/xtuner/tools/data_preprocess/arxiv.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/list_cfg.py` & `xtuner-0.1.9/xtuner/tools/list_cfg.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/log_dataset.py` & `xtuner-0.1.9/xtuner/tools/log_dataset.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/model_converters/merge.py` & `xtuner-0.1.9/xtuner/tools/model_converters/merge.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/model_converters/pth_to_hf.py` & `xtuner-0.1.9/xtuner/tools/model_converters/pth_to_hf.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/model_converters/split.py` & `xtuner-0.1.9/xtuner/tools/model_converters/split.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/plugins/api.py` & `xtuner-0.1.9/xtuner/tools/plugins/api.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/plugins/search.py` & `xtuner-0.1.9/xtuner/tools/plugins/search.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/plugins/solve.py` & `xtuner-0.1.9/xtuner/tools/plugins/solve.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/test.py` & `xtuner-0.1.9/xtuner/tools/test.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/tools/train.py` & `xtuner-0.1.9/xtuner/tools/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,16 @@
                 grad_clip = mm_max_norm
                 ds_cfg = auto_dtype_of_deepspeed_config(ds_cfg)
                 strategy = dict(
                     type='DeepSpeedStrategy',
                     config=ds_cfg,
                     gradient_accumulation_steps=grad_accum,
                     train_micro_batch_size_per_gpu=train_bs,
-                    gradient_clipping=grad_clip)
+                    gradient_clipping=grad_clip,
+                    exclude_frozen_parameters=True)
                 cfg.__setitem__('strategy', strategy)
                 optim_wrapper = dict(
                     type='DeepSpeedOptimWrapper',
                     optimizer=cfg.optim_wrapper.optimizer)
                 cfg.__setitem__('optim_wrapper', optim_wrapper)
                 cfg.runner_type = 'FlexibleRunner'
```

### Comparing `xtuner-0.1.8/xtuner/tools/utils.py` & `xtuner-0.1.9/xtuner/tools/utils.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/utils/stop_criteria.py` & `xtuner-0.1.9/xtuner/utils/stop_criteria.py`

 * *Files identical despite different names*

### Comparing `xtuner-0.1.8/xtuner/utils/templates.py` & `xtuner-0.1.9/xtuner/utils/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     code_llama_chat=dict(
         SYSTEM='{system}\n', INSTRUCTION='[INST] {input} [/INST]'),
     chatglm2=dict(
         SYSTEM='{system}\n',
         INSTRUCTION='\n\n[Round {round}]\n\n问：{input}\n\n答：'),
     chatglm3=dict(
         SYSTEM='<|system|>\n{system}',
-        INSTRUCTION='<|user|>\n{input}<|assistant|>'),
+        INSTRUCTION='<|user|>\n{input}<|assistant|>\n'),
     qwen_chat=dict(
         SYSTEM=('\n<|im_start|>system\n{system}<|im_end|>'),
         INSTRUCTION=(
             '\n<|im_start|>user\n{input}<|im_end|>\n<|im_start|>assistant\n')),
     baichuan_chat=dict(
         SYSTEM='{system}\n',
         INSTRUCTION='<reserved_102>{input}<reserved_103>'),
```

### Comparing `xtuner-0.1.8/xtuner/version.py` & `xtuner-0.1.9/xtuner/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 short_version = __version__
 
 
 def parse_version_info(version_str):
     """Parse a version string into a tuple.
 
     Args:
```

### Comparing `xtuner-0.1.8/xtuner.egg-info/PKG-INFO` & `xtuner-0.1.9/xtuner.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtuner
-Version: 0.1.8
+Version: 0.1.9
 Summary: A toolkit for efficiently fine-tuning LLM
 Home-page: https://github.com/InternLM/xtuner
 Author: XTuner Contributors
 Author-email: openmmlab@gmail.com
 License: Apache License 2.0
 Description: <div align="center">
           <img src="https://github.com/InternLM/lmdeploy/assets/36994684/0cf8d00f-e86b-40ba-9b54-dc8f1bc6c8d8" width="600"/>
@@ -18,15 +18,15 @@
         
         👋 join us on <a href="https://twitter.com/intern_lm" target="_blank">Twitter</a>, <a href="https://discord.gg/xa29JuW87d" target="_blank">Discord</a> and <a href="https://cdn.vansin.top/internlm/xtuner.jpg" target="_blank">WeChat</a>
         
         </div>
         
         ## 🎉 News
         
-        - **\[2023/10\]** Support [ChatGLM3-6B](https://huggingface.co/THUDM/chatglm3-6b) model!
+        - **\[2023/11\]** Support [ChatGLM3-6B](https://huggingface.co/THUDM/chatglm3-6b) model!
         - **\[2023/10\]** Support [MSAgent-Bench](https://modelscope.cn/datasets/damo/MSAgent-Bench) dataset, and the fine-tuned LLMs can be applied by [Lagent](https://github.com/InternLM/lagent)!
         - **\[2023/10\]** Optimize the data processing to accommodate `system` context. More information can be found on [Docs](docs/en/user_guides/dataset_format.md)!
         - **\[2023/09\]** Support [InternLM-20B](https://huggingface.co/internlm) models!
         - **\[2023/09\]** Support [Baichuan2](https://huggingface.co/baichuan-inc) models!
         - **\[2023/08\]** XTuner is released, with multiple fine-tuned adapters on [HuggingFace](https://huggingface.co/xtuner).
         
         ## 📖 Introduction
@@ -182,21 +182,23 @@
           xtuner train ${CONFIG_NAME_OR_PATH}
           ```
         
           For example, we can start the QLoRA fine-tuning of InternLM-7B with oasst1 dataset by
         
           ```shell
           # On a single GPU
-          xtuner train internlm_7b_qlora_oasst1_e3
+          xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2
           # On multiple GPUs
-          (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train internlm_7b_qlora_oasst1_e3
-          (SLURM) srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm
+          (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2
+          (SLURM) srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm --deepspeed deepspeed_zero2
           ```
         
-          For more examples, please see [finetune.md](./docs/en/user_guides/finetune.md).
+          - `--deepspeed` means using [DeepSpeed](https://github.com/microsoft/DeepSpeed) 🚀 to optimize the training. XTuner comes with several integrated strategies including ZeRO-1, ZeRO-2, and ZeRO-3. If you wish to disable this feature, simply remove this argument.
+        
+          - For more examples, please see [finetune.md](./docs/en/user_guides/finetune.md).
         
         - **Step 2**, convert the saved PTH model (if using DeepSpeed, it will be a directory) to HuggingFace model, by
         
           ```shell
           xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH} ${PTH} ${SAVE_PATH}
           ```
         
@@ -245,16 +247,14 @@
               --temperture 0.8 \
               --top_p 0.95 \
               --seed 0
           ```
         
           🔥 Seeking efficient inference with less GPU memory? Try 4-bit quantization from [LMDeploy](https://github.com/InternLM/lmdeploy)! For more details, see [here](https://github.com/InternLM/lmdeploy/tree/main#quantization).
         
-          🎯 We are woking closely with [LMDeploy](https://github.com/InternLM/lmdeploy), to implement the deployment of **plugin-based chat**!
-        
         ### Evaluation
         
         - We recommend using [OpenCompass](https://github.com/InternLM/opencompass), a comprehensive and systematic LLM evaluation library, which currently supports 50+ datasets with about 300,000 questions.
         
         ## 🤝 Contributing
         
         We appreciate all contributions to XTuner. Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guideline.
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: xtuner Version: 0.1.8 Summary: A toolkit for
+Metadata-Version: 2.1 Name: xtuner Version: 0.1.9 Summary: A toolkit for
 efficiently fine-tuning LLM Home-page: https://github.com/InternLM/xtuner
 Author: XTuner Contributors Author-email: openmmlab@gmail.com License: Apache
 License 2.0 Description:
 [https://github.com/InternLM/lmdeploy/assets/36994684/0cf8d00f-e86b-40ba-9b54-
                                  dc8f1bc6c8d8]
 
 [![license](https://img.shields.io/github/license/InternLM/xtuner.svg)](https:/
 /github.com/InternLM/xtuner/blob/main/LICENSE) [![PyPI](https://badge.fury.io/
  py/xtuner.svg)](https://pypi.org/project/xtuner/) [![Generic badge](https://
      img.shields.io/badge/ð¤%20Huggingface-xtuner-yellow.svg)](https://
  huggingface.co/xtuner) English | [ç®ä½ä¸­æ](README_zh-CN.md) ð join us
                         on _T_w_i_t_t_e_r, _D_i_s_c_o_r_d and _W_e_C_h_a_t
-## ð News - **\[2023/10\]** Support [ChatGLM3-6B](https://huggingface.co/
+## ð News - **\[2023/11\]** Support [ChatGLM3-6B](https://huggingface.co/
 THUDM/chatglm3-6b) model! - **\[2023/10\]** Support [MSAgent-Bench](https://
 modelscope.cn/datasets/damo/MSAgent-Bench) dataset, and the fine-tuned LLMs can
 be applied by [Lagent](https://github.com/InternLM/lagent)! - **\[2023/10\]**
 Optimize the data processing to accommodate `system` context. More information
 can be found on [Docs](docs/en/user_guides/dataset_format.md)! - **\[2023/
 09\]** Support [InternLM-20B](https://huggingface.co/internlm) models! - **\
 [2023/09\]** Support [Baichuan2](https://huggingface.co/baichuan-inc) models! -
@@ -87,55 +87,57 @@
 provides many ready-to-use configs and we can view all configs by ```shell
 xtuner list-cfg ``` Or, if the provided configs cannot meet the requirements,
 please copy the provided config to the specified directory and make specific
 modifications by ```shell xtuner copy-cfg ${CONFIG_NAME} ${SAVE_PATH} ``` -
 **Step 1**, start fine-tuning. ```shell xtuner train ${CONFIG_NAME_OR_PATH} ```
 For example, we can start the QLoRA fine-tuning of InternLM-7B with oasst1
 dataset by ```shell # On a single GPU xtuner train internlm_7b_qlora_oasst1_e3
-# On multiple GPUs (DIST) NPROC_PER_NODE=${GPU_NUM} xtuner train
-internlm_7b_qlora_oasst1_e3 (SLURM) srun ${SRUN_ARGS} xtuner train
-internlm_7b_qlora_oasst1_e3 --launcher slurm ``` For more examples, please see
-[finetune.md](./docs/en/user_guides/finetune.md). - **Step 2**, convert the
-saved PTH model (if using DeepSpeed, it will be a directory) to HuggingFace
-model, by ```shell xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH} ${PTH} $
-{SAVE_PATH} ``` ### Chat [![Open In Colab](https://colab.research.google.com/
-assets/colab-badge.svg)](https://colab.research.google.com/drive/
-144OuTVyT_GvFyDMtlSlTzcxYIfnRsklq?usp=sharing) XTuner provides tools to chat
-with pretrained / fine-tuned LLMs. ```shell xtuner chat ${NAME_OR_PATH_TO_LLM}
---adapter {NAME_OR_PATH_TO_ADAPTER} [optional arguments] ``` For example, we
-can start the chat with InternLM-7B with adapter trained from Alpaca-enzh:
-```shell xtuner chat internlm/internlm-7b --adapter xtuner/internlm-7b-qlora-
-alpaca-enzh --prompt-template internlm_chat --system-template alpaca ```
-Llama2-7b with adapter trained from MOSS-003-SFT: ```shell xtuner chat meta-
-llama/Llama-2-7b-hf --adapter xtuner/Llama-2-7b-qlora-moss-003-sft --bot-name
-Llama2 --prompt-template moss_sft --system-template moss_sft --with-plugins
-calculate solve search --command-stop-word "" --answer-stop-word "" --no-
-streamer ``` For more examples, please see [chat.md](./docs/en/user_guides/
-chat.md). ### Deployment - **Step 0**, merge the HuggingFace adapter to
-pretrained LLM, by ```shell xtuner convert merge \ ${NAME_OR_PATH_TO_LLM} \ $
-{NAME_OR_PATH_TO_ADAPTER} \ ${SAVE_PATH} \ --max-shard-size 2GB ``` - **Step
-1**, deploy fine-tuned LLM with any other framework, such as [LMDeploy](https:/
-/github.com/InternLM/lmdeploy) ð. ```shell pip install lmdeploy python -
-m lmdeploy.pytorch.chat ${NAME_OR_PATH_TO_LLM} \ --max_new_tokens 256 \ --
-temperture 0.8 \ --top_p 0.95 \ --seed 0 ``` ð¥ Seeking efficient inference
-with less GPU memory? Try 4-bit quantization from [LMDeploy](https://
-github.com/InternLM/lmdeploy)! For more details, see [here](https://github.com/
-InternLM/lmdeploy/tree/main#quantization). ð¯ We are woking closely with
-[LMDeploy](https://github.com/InternLM/lmdeploy), to implement the deployment
-of **plugin-based chat**! ### Evaluation - We recommend using [OpenCompass]
-(https://github.com/InternLM/opencompass), a comprehensive and systematic LLM
-evaluation library, which currently supports 50+ datasets with about 300,000
-questions. ## ð¤ Contributing We appreciate all contributions to XTuner.
-Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing
-guideline. ## ðï¸ Acknowledgement - [Llama 2](https://github.com/
-facebookresearch/llama) - [QLoRA](https://github.com/artidoro/qlora) -
-[LMDeploy](https://github.com/InternLM/lmdeploy) ## License This project is
-released under the [Apache License 2.0](LICENSE). Please also adhere to the
-Licenses of models and datasets being used. Keywords: large language
-model,parameter-efficient fine-tuning Platform: UNKNOWN Classifier: Development
-Status :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: OS Independent Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-Python:
->=3.8 Description-Content-Type: text/markdown Provides-Extra: all Provides-
-Extra: deepspeed
+--deepspeed deepspeed_zero2 # On multiple GPUs (DIST) NPROC_PER_NODE=${GPU_NUM}
+xtuner train internlm_7b_qlora_oasst1_e3 --deepspeed deepspeed_zero2 (SLURM)
+srun ${SRUN_ARGS} xtuner train internlm_7b_qlora_oasst1_e3 --launcher slurm --
+deepspeed deepspeed_zero2 ``` - `--deepspeed` means using [DeepSpeed](https://
+github.com/microsoft/DeepSpeed) ð to optimize the training. XTuner comes
+with several integrated strategies including ZeRO-1, ZeRO-2, and ZeRO-3. If you
+wish to disable this feature, simply remove this argument. - For more examples,
+please see [finetune.md](./docs/en/user_guides/finetune.md). - **Step 2**,
+convert the saved PTH model (if using DeepSpeed, it will be a directory) to
+HuggingFace model, by ```shell xtuner convert pth_to_hf ${CONFIG_NAME_OR_PATH}
+${PTH} ${SAVE_PATH} ``` ### Chat [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/144OuTVyT_GvFyDMtlSlTzcxYIfnRsklq?usp=sharing)
+XTuner provides tools to chat with pretrained / fine-tuned LLMs. ```shell
+xtuner chat ${NAME_OR_PATH_TO_LLM} --adapter {NAME_OR_PATH_TO_ADAPTER}
+[optional arguments] ``` For example, we can start the chat with InternLM-7B
+with adapter trained from Alpaca-enzh: ```shell xtuner chat internlm/internlm-
+7b --adapter xtuner/internlm-7b-qlora-alpaca-enzh --prompt-template
+internlm_chat --system-template alpaca ``` Llama2-7b with adapter trained from
+MOSS-003-SFT: ```shell xtuner chat meta-llama/Llama-2-7b-hf --adapter xtuner/
+Llama-2-7b-qlora-moss-003-sft --bot-name Llama2 --prompt-template moss_sft --
+system-template moss_sft --with-plugins calculate solve search --command-stop-
+word "" --answer-stop-word "" --no-streamer ``` For more examples, please see
+[chat.md](./docs/en/user_guides/chat.md). ### Deployment - **Step 0**, merge
+the HuggingFace adapter to pretrained LLM, by ```shell xtuner convert merge \ $
+{NAME_OR_PATH_TO_LLM} \ ${NAME_OR_PATH_TO_ADAPTER} \ ${SAVE_PATH} \ --max-
+shard-size 2GB ``` - **Step 1**, deploy fine-tuned LLM with any other
+framework, such as [LMDeploy](https://github.com/InternLM/lmdeploy) ð.
+```shell pip install lmdeploy python -m lmdeploy.pytorch.chat $
+{NAME_OR_PATH_TO_LLM} \ --max_new_tokens 256 \ --temperture 0.8 \ --top_p 0.95
+\ --seed 0 ``` ð¥ Seeking efficient inference with less GPU memory? Try 4-bit
+quantization from [LMDeploy](https://github.com/InternLM/lmdeploy)! For more
+details, see [here](https://github.com/InternLM/lmdeploy/tree/
+main#quantization). ### Evaluation - We recommend using [OpenCompass](https://
+github.com/InternLM/opencompass), a comprehensive and systematic LLM evaluation
+library, which currently supports 50+ datasets with about 300,000 questions. ##
+ð¤ Contributing We appreciate all contributions to XTuner. Please refer to
+[CONTRIBUTING.md](.github/CONTRIBUTING.md) for the contributing guideline. ##
+ðï¸ Acknowledgement - [Llama 2](https://github.com/facebookresearch/llama)
+- [QLoRA](https://github.com/artidoro/qlora) - [LMDeploy](https://github.com/
+InternLM/lmdeploy) ## License This project is released under the [Apache
+License 2.0](LICENSE). Please also adhere to the Licenses of models and
+datasets being used. Keywords: large language model,parameter-efficient fine-
+tuning Platform: UNKNOWN Classifier: Development Status :: 4 - Beta Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Topic :: Utilities Requires-Python: >=3.8 Description-Content-Type: text/
+markdown Provides-Extra: all Provides-Extra: deepspeed
```

### Comparing `xtuner-0.1.8/xtuner.egg-info/SOURCES.txt` & `xtuner-0.1.9/xtuner.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,15 @@
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_medical_e1.py
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_512_e3.py
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_oasst1_e3.py
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_open_platypus_e3.py
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_openorca_e1.py
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_sql_e3.py
 xtuner/configs/chatglm/chatglm3_6b_base/chatglm3_6b_base_qlora_tiny_codes_e1.py
+xtuner/configs/deepspeed/deepspeed_zero1.json
 xtuner/configs/deepspeed/deepspeed_zero2.json
 xtuner/configs/deepspeed/deepspeed_zero2_offload.json
 xtuner/configs/deepspeed/deepspeed_zero3.json
 xtuner/configs/deepspeed/deepspeed_zero3_offload.json
 xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_e3.py
 xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_e3.py
 xtuner/configs/internlm/internlm_20b/internlm_20b_qlora_alpaca_enzh_oasst1_e3.py
```

### Comparing `xtuner-0.1.8/xtuner.egg-info/requires.txt` & `xtuner-0.1.9/xtuner.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 bitsandbytes>=0.40.0
 datasets
 einops
 fsspec<=2023.6.0
 lagent>=0.1.2
-mmengine>=0.9.0
+mmengine>=0.9.1
 modelscope
 peft>=0.4.0
 scipy
 SentencePiece
 tiktoken
 torch
 transformers<=4.34.0,>=4.32.1
@@ -15,36 +15,36 @@
 
 [all]
 bitsandbytes>=0.40.0
 datasets
 einops
 fsspec<=2023.6.0
 lagent>=0.1.2
-mmengine>=0.9.0
+mmengine>=0.9.1
 modelscope
 peft>=0.4.0
 scipy
 SentencePiece
 tiktoken
 torch
 transformers<=4.34.0,>=4.32.1
 transformers_stream_generator
-deepspeed
+deepspeed>=0.12.3
 mpi4py-mpich
 
 [deepspeed]
 bitsandbytes>=0.40.0
 datasets
 einops
 fsspec<=2023.6.0
 lagent>=0.1.2
-mmengine>=0.9.0
+mmengine>=0.9.1
 modelscope
 peft>=0.4.0
 scipy
 SentencePiece
 tiktoken
 torch
 transformers<=4.34.0,>=4.32.1
 transformers_stream_generator
-deepspeed
+deepspeed>=0.12.3
 mpi4py-mpich
```

