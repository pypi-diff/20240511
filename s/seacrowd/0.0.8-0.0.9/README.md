# Comparing `tmp/seacrowd-0.0.8.tar.gz` & `tmp/seacrowd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seacrowd-0.0.8.tar", last modified: Fri Apr 12 07:58:36 2024, max compression
+gzip compressed data, was "seacrowd-0.0.9.tar", last modified: Fri Apr 12 08:01:43 2024, max compression
```

## Comparing `seacrowd-0.0.8.tar` & `seacrowd-0.0.9.tar`

### file list

```diff
@@ -1,982 +1,982 @@
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:36.104850 seacrowd-0.0.8/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.8/LICENSE
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:58:36.101196 seacrowd-0.0.8/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.8/README.md
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.367103 seacrowd-0.0.8/seacrowd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-12 07:58:18.000000 seacrowd-0.0.8/seacrowd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/config_helper.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.461014 seacrowd-0.0.8/seacrowd/sea_datasets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.479503 seacrowd-0.0.8/seacrowd/sea_datasets/abui_wordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/abui_wordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.505652 seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.532813 seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.564798 seacrowd-0.0.8/seacrowd/sea_datasets/ara_close/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ara_close/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ara_close/ara_close.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.591189 seacrowd-0.0.8/seacrowd/sea_datasets/asr_sindodusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/asr_sindodusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.621655 seacrowd-0.0.8/seacrowd/sea_datasets/asr_smaldusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/asr_smaldusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.641516 seacrowd-0.0.8/seacrowd/sea_datasets/asr_stidusc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/asr_stidusc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.671577 seacrowd-0.0.8/seacrowd/sea_datasets/audio_keyword_spotting/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.691714 seacrowd-0.0.8/seacrowd/sea_datasets/aya_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/aya_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.710999 seacrowd-0.0.8/seacrowd/sea_datasets/barasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/barasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/barasa/barasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.730235 seacrowd-0.0.8/seacrowd/sea_datasets/beaye_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/beaye_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.759720 seacrowd-0.0.8/seacrowd/sea_datasets/belebele/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/belebele/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/belebele/belebele.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.778581 seacrowd-0.0.8/seacrowd/sea_datasets/bible_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bible_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.798068 seacrowd-0.0.8/seacrowd/sea_datasets/bible_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bible_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.819645 seacrowd-0.0.8/seacrowd/sea_datasets/bible_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bible_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.841132 seacrowd-0.0.8/seacrowd/sea_datasets/bioner_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bioner_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bioner_id/bioner_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.859881 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_captioning/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_captioning/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.893018 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_lm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_lm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.912157 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_speech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_speech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.935037 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_vist/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_vist/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.968876 seacrowd-0.0.8/seacrowd/sea_datasets/burapha_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/burapha_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/burapha_th/burapha_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:28.994323 seacrowd-0.0.8/seacrowd/sea_datasets/burmese_romanize/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/burmese_romanize/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.015045 seacrowd-0.0.8/seacrowd/sea_datasets/casa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/casa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/casa/casa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.034667 seacrowd-0.0.8/seacrowd/sea_datasets/cc100/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cc100/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cc100/cc100.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.051362 seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_doc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.074280 seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_sent/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.093947 seacrowd-0.0.8/seacrowd/sea_datasets/cebuaner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cebuaner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cebuaner/cebuaner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.116448 seacrowd-0.0.8/seacrowd/sea_datasets/coco_35l/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/coco_35l/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/coco_35l/coco_35l.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.135630 seacrowd-0.0.8/seacrowd/sea_datasets/cod/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cod/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cod/cod.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.156595 seacrowd-0.0.8/seacrowd/sea_datasets/code_mixed_jv_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.181182 seacrowd-0.0.8/seacrowd/sea_datasets/codeswitch_reddit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.201216 seacrowd-0.0.8/seacrowd/sea_datasets/commonvoice_120/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/commonvoice_120/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.219617 seacrowd-0.0.8/seacrowd/sea_datasets/copal/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/copal/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/copal/copal.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.239918 seacrowd-0.0.8/seacrowd/sea_datasets/covost2/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/covost2/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/covost2/covost2.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.260227 seacrowd-0.0.8/seacrowd/sea_datasets/creole_rc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.8/seacrowd/sea_datasets/creole_rc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/creole_rc/creole_rc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.287290 seacrowd-0.0.8/seacrowd/sea_datasets/crosssum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/crosssum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/crosssum/crosssum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.315972 seacrowd-0.0.8/seacrowd/sea_datasets/cub_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cub_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.335759 seacrowd-0.0.8/seacrowd/sea_datasets/culturax/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/culturax/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/culturax/culturax.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.357586 seacrowd-0.0.8/seacrowd/sea_datasets/cvss/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cvss/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/cvss/cvss.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.377024 seacrowd-0.0.8/seacrowd/sea_datasets/dengue_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/dengue_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.395752 seacrowd-0.0.8/seacrowd/sea_datasets/emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emot/emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.413916 seacrowd-0.0.8/seacrowd/sea_datasets/emotcmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emotcmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emotcmt/emotcmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.433220 seacrowd-0.0.8/seacrowd/sea_datasets/emotes_3k/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emotes_3k/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.460990 seacrowd-0.0.8/seacrowd/sea_datasets/emotion_id_opinion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.480194 seacrowd-0.0.8/seacrowd/sea_datasets/etos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/etos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/etos/etos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.501502 seacrowd-0.0.8/seacrowd/sea_datasets/facqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/facqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/facqa/facqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.526069 seacrowd-0.0.8/seacrowd/sea_datasets/facqa/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/facqa/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.556864 seacrowd-0.0.8/seacrowd/sea_datasets/fakenews_ph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fakenews_ph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.582842 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_gay_lang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.607137 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.625291 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_slang_norm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.657504 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_words_aoa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.682707 seacrowd-0.0.8/seacrowd/sea_datasets/filwordnet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filwordnet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/filwordnet/filwordnet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.710018 seacrowd-0.0.8/seacrowd/sea_datasets/fleurs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fleurs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13115 2024-04-12 07:50:18.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fleurs/fleurs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      800 2024-04-12 07:46:55.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fleurs/lang_config.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.729792 seacrowd-0.0.8/seacrowd/sea_datasets/flores200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/flores200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/flores200/flores200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.752088 seacrowd-0.0.8/seacrowd/sea_datasets/fsl_105/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fsl_105/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6817 2024-04-12 07:57:15.000000 seacrowd-0.0.8/seacrowd/sea_datasets/fsl_105/fsl_105.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.769982 seacrowd-0.0.8/seacrowd/sea_datasets/gatitos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/gatitos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/gatitos/gatitos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.789584 seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_newsclass/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.814145 seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.834091 seacrowd-0.0.8/seacrowd/sea_datasets/globalwoz/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/globalwoz/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/globalwoz/globalwoz.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.857279 seacrowd-0.0.8/seacrowd/sea_datasets/glotstorybook/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/glotstorybook/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.879757 seacrowd-0.0.8/seacrowd/sea_datasets/hoasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/hoasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/hoasa/hoasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.900382 seacrowd-0.0.8/seacrowd/sea_datasets/iapp_squad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/iapp_squad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.919375 seacrowd-0.0.8/seacrowd/sea_datasets/iatf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/iatf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5801 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/iatf/iatf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.946587 seacrowd-0.0.8/seacrowd/sea_datasets/icon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/icon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/icon/icon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.969595 seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive/id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:29.990163 seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive_news_comment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.011018 seacrowd-0.0.8/seacrowd/sea_datasets/id_am2ico/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_am2ico/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.029935 seacrowd-0.0.8/seacrowd/sea_datasets/id_clickbait/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_clickbait/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.049013 seacrowd-0.0.8/seacrowd/sea_datasets/id_coreference_resolution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.086273 seacrowd-0.0.8/seacrowd/sea_datasets/id_frog_story/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_frog_story/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.105146 seacrowd-0.0.8/seacrowd/sea_datasets/id_google_play_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_google_play_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.132506 seacrowd-0.0.8/seacrowd/sea_datasets/id_hatespeech/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_hatespeech/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.149994 seacrowd-0.0.8/seacrowd/sea_datasets/id_hoax_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_hoax_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.169125 seacrowd-0.0.8/seacrowd/sea_datasets/id_hsd_nofaaulia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.189944 seacrowd-0.0.8/seacrowd/sea_datasets/id_msvd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_msvd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_msvd/id_msvd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.213150 seacrowd-0.0.8/seacrowd/sea_datasets/id_multilabel_hs/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.237664 seacrowd-0.0.8/seacrowd/sea_datasets/id_panl_bppt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_panl_bppt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.267548 seacrowd-0.0.8/seacrowd/sea_datasets/id_qqp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_qqp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_qqp/id_qqp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.289060 seacrowd-0.0.8/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.310803 seacrowd-0.0.8/seacrowd/sea_datasets/id_sentiment_analysis/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.332415 seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.352236 seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.374305 seacrowd-0.0.8/seacrowd/sea_datasets/id_stance/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_stance/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_stance/id_stance.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.392128 seacrowd-0.0.8/seacrowd/sea_datasets/id_sts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_sts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_sts/id_sts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.411763 seacrowd-0.0.8/seacrowd/sea_datasets/id_vaccines_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.429970 seacrowd-0.0.8/seacrowd/sea_datasets/id_wiki_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.449447 seacrowd-0.0.8/seacrowd/sea_datasets/id_wsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_wsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/id_wsd/id_wsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.465174 seacrowd-0.0.8/seacrowd/sea_datasets/identic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/identic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/identic/identic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.487432 seacrowd-0.0.8/seacrowd/sea_datasets/identifikasi_bahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.504873 seacrowd-0.0.8/seacrowd/sea_datasets/idk_mrc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/idk_mrc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.543366 seacrowd-0.0.8/seacrowd/sea_datasets/idn_tagged_corpus_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.570584 seacrowd-0.0.8/seacrowd/sea_datasets/ijelid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ijelid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ijelid/ijelid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.601210 seacrowd-0.0.8/seacrowd/sea_datasets/imdb_jv/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/imdb_jv/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.626642 seacrowd-0.0.8/seacrowd/sea_datasets/indo4b/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo4b/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo4b/indo4b.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.657333 seacrowd-0.0.8/seacrowd/sea_datasets/indo4b_plus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo4b_plus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.683090 seacrowd-0.0.8/seacrowd/sea_datasets/indo_general_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.702944 seacrowd-0.0.8/seacrowd/sea_datasets/indo_law/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_law/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_law/indo_law.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.721836 seacrowd-0.0.8/seacrowd/sea_datasets/indo_puisi/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_puisi/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.741254 seacrowd-0.0.8/seacrowd/sea_datasets/indo_religious_mt_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.760757 seacrowd-0.0.8/seacrowd/sea_datasets/indo_story_cloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_story_cloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.781289 seacrowd-0.0.8/seacrowd/sea_datasets/indocamrest/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocamrest/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocamrest/indocamrest.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.800644 seacrowd-0.0.8/seacrowd/sea_datasets/indocollex/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocollex/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocollex/indocollex.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.822084 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/indocoref.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.871312 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/file_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.892516 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ner_ugm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.912405 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_nerui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_nerui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.931395 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ntp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ntp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.950946 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.970972 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_tweet_ordering/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:30.998910 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_gsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.020339 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_pud/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.043076 seacrowd-0.0.8/seacrowd/sea_datasets/indoler/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indoler/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indoler/indoler.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.060068 seacrowd-0.0.8/seacrowd/sea_datasets/indommlu/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indommlu/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indommlu/indommlu.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.078251 seacrowd-0.0.8/seacrowd/sea_datasets/indoner_tourism/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indoner_tourism/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.095271 seacrowd-0.0.8/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.114495 seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.137760 seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_news_dataset/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.155389 seacrowd-0.0.8/seacrowd/sea_datasets/indonesiannmt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesiannmt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.178915 seacrowd-0.0.8/seacrowd/sea_datasets/indonglish/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonglish/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonglish/indonglish.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.212932 seacrowd-0.0.8/seacrowd/sea_datasets/indonli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonli/indonli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.239261 seacrowd-0.0.8/seacrowd/sea_datasets/indonlu_nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.266051 seacrowd-0.0.8/seacrowd/sea_datasets/indoqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indoqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indoqa/indoqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.285853 seacrowd-0.0.8/seacrowd/sea_datasets/indosmd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indosmd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indosmd/indosmd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.306229 seacrowd-0.0.8/seacrowd/sea_datasets/indosum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indosum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indosum/indosum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.336006 seacrowd-0.0.8/seacrowd/sea_datasets/indotacos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indotacos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indotacos/indotacos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.359370 seacrowd-0.0.8/seacrowd/sea_datasets/indowiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indowiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indowiki/indowiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.380833 seacrowd-0.0.8/seacrowd/sea_datasets/indqner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indqner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indqner/indqner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.406037 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_digit_cdsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.439150 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.462648 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.481828 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.510658 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.541637 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.558911 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.577714 seacrowd-0.0.8/seacrowd/sea_datasets/inset_lexicon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/inset_lexicon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.621086 seacrowd-0.0.8/seacrowd/sea_datasets/jadi_ide/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/jadi_ide/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.667787 seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.697895 seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.721821 seacrowd-0.0.8/seacrowd/sea_datasets/kamus_alay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kamus_alay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.746719 seacrowd-0.0.8/seacrowd/sea_datasets/karonese_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/karonese_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.782864 seacrowd-0.0.8/seacrowd/sea_datasets/kawat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kawat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kawat/kawat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.801281 seacrowd-0.0.8/seacrowd/sea_datasets/kde4/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kde4/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kde4/kde4.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.821648 seacrowd-0.0.8/seacrowd/sea_datasets/keps/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/keps/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/keps/keps.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.841919 seacrowd-0.0.8/seacrowd/sea_datasets/kheng_info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kheng_info/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kheng_info/kheng_info.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.860217 seacrowd-0.0.8/seacrowd/sea_datasets/khmer_alt_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.896428 seacrowd-0.0.8/seacrowd/sea_datasets/khpos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/khpos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/khpos/khpos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.914379 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.949982 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc_news/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc_news/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.969677 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_nllb/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_nllb/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:31.986901 seacrowd-0.0.8/seacrowd/sea_datasets/korpus_nusantara/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/korpus_nusantara/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.007055 seacrowd-0.0.8/seacrowd/sea_datasets/lazada_review_filipino/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.032909 seacrowd-0.0.8/seacrowd/sea_datasets/librivox_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/librivox_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.055260 seacrowd-0.0.8/seacrowd/sea_datasets/limesoda/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/limesoda/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/limesoda/limesoda.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.079536 seacrowd-0.0.8/seacrowd/sea_datasets/liputan6/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/liputan6/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/liputan6/liputan6.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.101981 seacrowd-0.0.8/seacrowd/sea_datasets/local_id_abusive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/local_id_abusive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.127269 seacrowd-0.0.8/seacrowd/sea_datasets/lr_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/lr_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/lr_sum/lr_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.153683 seacrowd-0.0.8/seacrowd/sea_datasets/m3exam/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/m3exam/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/m3exam/m3exam.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.172564 seacrowd-0.0.8/seacrowd/sea_datasets/mabl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mabl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mabl/mabl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.194365 seacrowd-0.0.8/seacrowd/sea_datasets/malaysia_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/malaysia_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.213281 seacrowd-0.0.8/seacrowd/sea_datasets/malindo_morph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/malindo_morph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.237866 seacrowd-0.0.8/seacrowd/sea_datasets/malindo_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/malindo_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.255616 seacrowd-0.0.8/seacrowd/sea_datasets/massive/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/massive/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.8/seacrowd/sea_datasets/massive/massive.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.274028 seacrowd-0.0.8/seacrowd/sea_datasets/mc4_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mc4_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.293128 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_brunei/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_brunei/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.311050 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sabah/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sabah/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.328378 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sarawak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sarawak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.352206 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_standard_lisan/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.376007 seacrowd-0.0.8/seacrowd/sea_datasets/memolon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/memolon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/memolon/memolon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.394775 seacrowd-0.0.8/seacrowd/sea_datasets/minangnlp_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/minangnlp_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.414778 seacrowd-0.0.8/seacrowd/sea_datasets/miracl/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/miracl/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/miracl/miracl.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.449750 seacrowd-0.0.8/seacrowd/sea_datasets/mkqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mkqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mkqa/mkqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.483536 seacrowd-0.0.8/seacrowd/sea_datasets/mlqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mlqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mlqa/mlqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.501659 seacrowd-0.0.8/seacrowd/sea_datasets/mozilla_pontoon/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.520581 seacrowd-0.0.8/seacrowd/sea_datasets/mswc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mswc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mswc/mswc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.547507 seacrowd-0.0.8/seacrowd/sea_datasets/mtop_intent_classification/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mtop_intent_classification/labels.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.565868 seacrowd-0.0.8/seacrowd/sea_datasets/multilexnorm/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/multilexnorm/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.598178 seacrowd-0.0.8/seacrowd/sea_datasets/my_paraphrase/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/my_paraphrase/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.616469 seacrowd-0.0.8/seacrowd/sea_datasets/myanmar_rakhine_parallel/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.635490 seacrowd-0.0.8/seacrowd/sea_datasets/mypos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mypos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mypos/mypos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.653028 seacrowd-0.0.8/seacrowd/sea_datasets/mysentence/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mysentence/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/mysentence/mysentence.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.669804 seacrowd-0.0.8/seacrowd/sea_datasets/myxnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/myxnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/myxnli/myxnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.688889 seacrowd-0.0.8/seacrowd/sea_datasets/nergrit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nergrit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nergrit/nergrit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.724263 seacrowd-0.0.8/seacrowd/sea_datasets/nerp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nerp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nerp/nerp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.756468 seacrowd-0.0.8/seacrowd/sea_datasets/netifier/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/netifier/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/netifier/netifier.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.778216 seacrowd-0.0.8/seacrowd/sea_datasets/news_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/news_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/news_en_id/news_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.798415 seacrowd-0.0.8/seacrowd/sea_datasets/newsph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/newsph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/newsph/newsph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.818170 seacrowd-0.0.8/seacrowd/sea_datasets/nllb_seed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nllb_seed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.851359 seacrowd-0.0.8/seacrowd/sea_datasets/ntrex_128/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ntrex_128/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.872009 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.894748 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_rhetoric/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.933452 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_topic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.956299 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:32.981713 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.004569 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.034317 seacrowd-0.0.8/seacrowd/sea_datasets/nusax_mt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusax_mt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.062586 seacrowd-0.0.8/seacrowd/sea_datasets/nusax_senti/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusax_senti/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.096299 seacrowd-0.0.8/seacrowd/sea_datasets/oil/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/oil/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/oil/oil.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.122400 seacrowd-0.0.8/seacrowd/sea_datasets/ojw/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ojw/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ojw/ojw.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.158544 seacrowd-0.0.8/seacrowd/sea_datasets/openlid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/openlid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/openlid/openlid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.182593 seacrowd-0.0.8/seacrowd/sea_datasets/openslr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/openslr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/openslr/openslr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.208508 seacrowd-0.0.8/seacrowd/sea_datasets/orchid_pos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/orchid_pos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.233529 seacrowd-0.0.8/seacrowd/sea_datasets/oscar_2201/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/oscar_2201/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.265915 seacrowd-0.0.8/seacrowd/sea_datasets/palito/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/palito/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/palito/palito.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.285378 seacrowd-0.0.8/seacrowd/sea_datasets/paracotta_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/paracotta_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.316497 seacrowd-0.0.8/seacrowd/sea_datasets/parallel_id_nyo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.339604 seacrowd-0.0.8/seacrowd/sea_datasets/parallel_su_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/parallel_su_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.366965 seacrowd-0.0.8/seacrowd/sea_datasets/ph_fake_news_corpus/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.387560 seacrowd-0.0.8/seacrowd/sea_datasets/pho_ner_covid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/pho_ner_covid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.8/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.413297 seacrowd-0.0.8/seacrowd/sea_datasets/phomt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/phomt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/phomt/phomt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.438436 seacrowd-0.0.8/seacrowd/sea_datasets/phost/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/phost/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/phost/phost.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.463378 seacrowd-0.0.8/seacrowd/sea_datasets/posp/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/posp/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/posp/posp.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.492365 seacrowd-0.0.8/seacrowd/sea_datasets/postag_su/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/postag_su/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/postag_su/postag_su.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.514295 seacrowd-0.0.8/seacrowd/sea_datasets/prdect_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/prdect_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/prdect_id/prdect_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.551888 seacrowd-0.0.8/seacrowd/sea_datasets/qasina/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/qasina/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/qasina/qasina.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.575126 seacrowd-0.0.8/seacrowd/sea_datasets/roots_vi_ted/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/roots_vi_ted/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.610564 seacrowd-0.0.8/seacrowd/sea_datasets/sampiran/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sampiran/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sampiran/sampiran.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.632845 seacrowd-0.0.8/seacrowd/sea_datasets/sap_wat/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sap_wat/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sap_wat/sap_wat.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.651124 seacrowd-0.0.8/seacrowd/sea_datasets/sarawak_malay/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sarawak_malay/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.668743 seacrowd-0.0.8/seacrowd/sea_datasets/scb_mt_en_th/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.686972 seacrowd-0.0.8/seacrowd/sea_datasets/sea_bench/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_bench/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_bench/sea_bench.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.707566 seacrowd-0.0.8/seacrowd/sea_datasets/sea_madlad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_madlad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.749645 seacrowd-0.0.8/seacrowd/sea_datasets/sea_wiki/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_wiki/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1844 2024-04-12 07:50:53.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_wiki/lang_config.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9272 2024-04-12 07:52:13.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.777734 seacrowd-0.0.8/seacrowd/sea_datasets/seaeval/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/seaeval/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/seaeval/seaeval.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.800426 seacrowd-0.0.8/seacrowd/sea_datasets/seahorse/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/seahorse/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/seahorse/seahorse.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.819939 seacrowd-0.0.8/seacrowd/sea_datasets/sentiment_nathasa_review/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.847246 seacrowd-0.0.8/seacrowd/sea_datasets/shopee_reviews_tagalog/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.867736 seacrowd-0.0.8/seacrowd/sea_datasets/singgalang/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/singgalang/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/singgalang/singgalang.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.884428 seacrowd-0.0.8/seacrowd/sea_datasets/smsa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/smsa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/smsa/smsa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.905130 seacrowd-0.0.8/seacrowd/sea_datasets/snli_indo/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/snli_indo/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/snli_indo/snli_indo.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.929044 seacrowd-0.0.8/seacrowd/sea_datasets/spamid_pair/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/spamid_pair/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.948356 seacrowd-0.0.8/seacrowd/sea_datasets/squad_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/squad_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/squad_id/squad_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.966941 seacrowd-0.0.8/seacrowd/sea_datasets/stb_ext/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/stb_ext/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/stb_ext/stb_ext.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:33.986831 seacrowd-0.0.8/seacrowd/sea_datasets/stif_indonesia/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/stif_indonesia/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.008572 seacrowd-0.0.8/seacrowd/sea_datasets/struct_amb_ind/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/struct_amb_ind/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.031564 seacrowd-0.0.8/seacrowd/sea_datasets/su_emot/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/su_emot/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/su_emot/su_emot.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.056109 seacrowd-0.0.8/seacrowd/sea_datasets/su_id_asr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/su_id_asr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.073050 seacrowd-0.0.8/seacrowd/sea_datasets/su_id_tts/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/su_id_tts/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.091099 seacrowd-0.0.8/seacrowd/sea_datasets/talpco/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/talpco/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/talpco/talpco.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.109479 seacrowd-0.0.8/seacrowd/sea_datasets/tatabahasa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tatabahasa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.128230 seacrowd-0.0.8/seacrowd/sea_datasets/tatoeba/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tatoeba/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tatoeba/tatoeba.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.159578 seacrowd-0.0.8/seacrowd/sea_datasets/tcope/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tcope/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tcope/tcope.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.179321 seacrowd-0.0.8/seacrowd/sea_datasets/ted_en_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ted_en_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.196166 seacrowd-0.0.8/seacrowd/sea_datasets/term_a/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/term_a/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/term_a/term_a.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.213351 seacrowd-0.0.8/seacrowd/sea_datasets/tgl_profanity/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tgl_profanity/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.240952 seacrowd-0.0.8/seacrowd/sea_datasets/tha_lao_embassy_parcor/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.267356 seacrowd-0.0.8/seacrowd/sea_datasets/thai_alpaca/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_alpaca/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.286344 seacrowd-0.0.8/seacrowd/sea_datasets/thai_constitution/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_constitution/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.305876 seacrowd-0.0.8/seacrowd/sea_datasets/thai_databricks_dolly/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.323727 seacrowd-0.0.8/seacrowd/sea_datasets/thai_depression/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_depression/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_depression/thai_depression.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.342871 seacrowd-0.0.8/seacrowd/sea_datasets/thai_gpteacher/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_gpteacher/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.365620 seacrowd-0.0.8/seacrowd/sea_datasets/thai_hh_rlhf/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.386707 seacrowd-0.0.8/seacrowd/sea_datasets/thai_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_sum/thai_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.405678 seacrowd-0.0.8/seacrowd/sea_datasets/thai_toxicity_tweet/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.424339 seacrowd-0.0.8/seacrowd/sea_datasets/tico_19/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tico_19/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tico_19/tico_19.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.443050 seacrowd-0.0.8/seacrowd/sea_datasets/titml_idn/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/titml_idn/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/titml_idn/titml_idn.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.477099 seacrowd-0.0.8/seacrowd/sea_datasets/tlunified_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tlunified_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.496771 seacrowd-0.0.8/seacrowd/sea_datasets/toxicity_200/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/toxicity_200/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.515611 seacrowd-0.0.8/seacrowd/sea_datasets/tydiqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tydiqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/tydiqa/tydiqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.534919 seacrowd-0.0.8/seacrowd/sea_datasets/typhoon_yolanda_tweets/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.557472 seacrowd-0.0.8/seacrowd/sea_datasets/ucla_phonetic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ucla_phonetic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.576493 seacrowd-0.0.8/seacrowd/sea_datasets/ud_id_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ud_id_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.596687 seacrowd-0.0.8/seacrowd/sea_datasets/ud_jv_csui/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ud_jv_csui/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.615658 seacrowd-0.0.8/seacrowd/sea_datasets/udhr/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/udhr/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/udhr/udhr.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.636300 seacrowd-0.0.8/seacrowd/sea_datasets/udhr_lid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/udhr_lid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.655947 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vicov19qa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.675557 seacrowd-0.0.8/seacrowd/sea_datasets/uit_victsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_victsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.693656 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vihsd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vihsd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.712849 seacrowd-0.0.8/seacrowd/sea_datasets/uit_viic/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_viic/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_viic/uit_viic.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.729403 seacrowd-0.0.8/seacrowd/sea_datasets/uit_viocd/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_viocd/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.747762 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vion/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vion/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vion/uit_vion.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.766905 seacrowd-0.0.8/seacrowd/sea_datasets/uit_visd4sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_visd4sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.791813 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsfc/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsfc/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.819146 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsmec/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsmec/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.845386 seacrowd-0.0.8/seacrowd/sea_datasets/unimorph/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/unimorph/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/unimorph/unimorph.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.862737 seacrowd-0.0.8/seacrowd/sea_datasets/unimorph_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/unimorph_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.880304 seacrowd-0.0.8/seacrowd/sea_datasets/vi_pubmed/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vi_pubmed/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.900489 seacrowd-0.0.8/seacrowd/sea_datasets/vihealthqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vihealthqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.931308 seacrowd-0.0.8/seacrowd/sea_datasets/visobert/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/visobert/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/visobert/visobert.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.957694 seacrowd-0.0.8/seacrowd/sea_datasets/vispamreviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vispamreviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.976596 seacrowd-0.0.8/seacrowd/sea_datasets/vistec_tp_th_21/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:34.999056 seacrowd-0.0.8/seacrowd/sea_datasets/vitext2sql/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vitext2sql/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.021581 seacrowd-0.0.8/seacrowd/sea_datasets/vivos/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vivos/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vivos/vivos.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.050542 seacrowd-0.0.8/seacrowd/sea_datasets/vivqa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vivqa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vivqa/vivqa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.076833 seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_ner/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.100583 seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_sa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.157832 seacrowd-0.0.8/seacrowd/sea_datasets/vndt/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vndt/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vndt/utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/vndt/vndt.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.178150 seacrowd-0.0.8/seacrowd/sea_datasets/voxlingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/voxlingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/voxlingua/voxlingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.215764 seacrowd-0.0.8/seacrowd/sea_datasets/weathub/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/weathub/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/weathub/weathub.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.237177 seacrowd-0.0.8/seacrowd/sea_datasets/wikiann/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikiann/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikiann/wikiann.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.255708 seacrowd-0.0.8/seacrowd/sea_datasets/wikilingua/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikilingua/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikilingua/wikilingua.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.284139 seacrowd-0.0.8/seacrowd/sea_datasets/wikimatrix/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikimatrix/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.305415 seacrowd-0.0.8/seacrowd/sea_datasets/wikitext_tl_39/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.327050 seacrowd-0.0.8/seacrowd/sea_datasets/wili_2018/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wili_2018/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wili_2018/wili_2018.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.348502 seacrowd-0.0.8/seacrowd/sea_datasets/wisesight_thai_sentiment/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.367597 seacrowd-0.0.8/seacrowd/sea_datasets/wit/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wit/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wit/wit.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.389362 seacrowd-0.0.8/seacrowd/sea_datasets/wongnai_reviews/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wongnai_reviews/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.414380 seacrowd-0.0.8/seacrowd/sea_datasets/wrete/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wrete/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/wrete/wrete.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.433828 seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/__init__.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.450891 seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/x_fact.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.475679 seacrowd-0.0.8/seacrowd/sea_datasets/xcopa/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xcopa/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xcopa/xcopa.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.494349 seacrowd-0.0.8/seacrowd/sea_datasets/xl_jailbreak/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xl_jailbreak/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.513766 seacrowd-0.0.8/seacrowd/sea_datasets/xl_sum/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xl_sum/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xl_sum/xl_sum.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.532436 seacrowd-0.0.8/seacrowd/sea_datasets/xm3600/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xm3600/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xm3600/xm3600.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.553700 seacrowd-0.0.8/seacrowd/sea_datasets/xnli/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xnli/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xnli/xnli.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.573396 seacrowd-0.0.8/seacrowd/sea_datasets/xpersona_id/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xpersona_id/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.591637 seacrowd-0.0.8/seacrowd/sea_datasets/xquad/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xquad/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xquad/xquad.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.609902 seacrowd-0.0.8/seacrowd/sea_datasets/xsid/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xsid/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xsid/xsid.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.629124 seacrowd-0.0.8/seacrowd/sea_datasets/xstorycloze/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xstorycloze/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.674484 seacrowd-0.0.8/seacrowd/sea_datasets/yunshan_cup_2020/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:35.755318 seacrowd-0.0.8/seacrowd/utils/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/common_parser.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/configs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/constants.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:36.039687 seacrowd-0.0.8/seacrowd/utils/schemas/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/image_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/imqa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/kb.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/pairs.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/pairs_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/qa.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/self_supervised_pretraining.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/seq_label.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/speech_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/speech_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/speech_to_speech.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/text_multilabel.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/text_to_text.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/tod.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/tree.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.8/seacrowd/utils/schemas/video.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:36.084843 seacrowd-0.0.8/seacrowd.egg-info/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 07:58:26.000000 seacrowd-0.0.8/seacrowd.egg-info/PKG-INFO
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31367 2024-04-12 07:58:26.000000 seacrowd-0.0.8/seacrowd.egg-info/SOURCES.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-12 07:58:26.000000 seacrowd-0.0.8/seacrowd.egg-info/dependency_links.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-12 07:58:26.000000 seacrowd-0.0.8/seacrowd.egg-info/requires.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-12 07:58:26.000000 seacrowd-0.0.8/seacrowd.egg-info/top_level.txt
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      703 2024-04-12 07:58:36.112064 seacrowd-0.0.8/setup.cfg
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-12 07:28:29.000000 seacrowd-0.0.8/setup.py
-drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 07:58:36.065437 seacrowd-0.0.8/tests/
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.8/tests/__init__.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.8/tests/test_seacrowd.py
--rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.8/tests/test_seacrowd_source_only.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:43.293824 seacrowd-0.0.9/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11357 2024-04-04 06:00:44.000000 seacrowd-0.0.9/LICENSE
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 08:01:43.290315 seacrowd-0.0.9/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5757 2024-04-04 06:00:44.000000 seacrowd-0.0.9/README.md
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.040505 seacrowd-0.0.9/seacrowd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      251 2024-04-12 08:01:25.000000 seacrowd-0.0.9/seacrowd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    40451 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/config_helper.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.116258 seacrowd-0.0.9/seacrowd/sea_datasets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.136287 seacrowd-0.0.9/seacrowd/sea_datasets/abui_wordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/abui_wordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5277 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.162713 seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5692 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.189029 seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2661 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.218282 seacrowd-0.0.9/seacrowd/sea_datasets/ara_close/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ara_close/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8227 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ara_close/ara_close.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.244554 seacrowd-0.0.9/seacrowd/sea_datasets/asr_sindodusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/asr_sindodusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7231 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.275940 seacrowd-0.0.9/seacrowd/sea_datasets/asr_smaldusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/asr_smaldusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7305 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.308412 seacrowd-0.0.9/seacrowd/sea_datasets/asr_stidusc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/asr_stidusc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6979 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.329479 seacrowd-0.0.9/seacrowd/sea_datasets/audio_keyword_spotting/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/audio_keyword_spotting/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7860 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.355419 seacrowd-0.0.9/seacrowd/sea_datasets/aya_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/aya_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7482 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/aya_dataset/aya_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.384332 seacrowd-0.0.9/seacrowd/sea_datasets/barasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/barasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7224 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/barasa/barasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.421332 seacrowd-0.0.9/seacrowd/sea_datasets/beaye_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/beaye_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4357 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.445595 seacrowd-0.0.9/seacrowd/sea_datasets/belebele/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/belebele/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8610 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/belebele/belebele.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.472601 seacrowd-0.0.9/seacrowd/sea_datasets/bible_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bible_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6790 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bible_en_id/bible_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.494798 seacrowd-0.0.9/seacrowd/sea_datasets/bible_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bible_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6856 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.514992 seacrowd-0.0.9/seacrowd/sea_datasets/bible_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bible_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6632 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bible_su_id/bible_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.536390 seacrowd-0.0.9/seacrowd/sea_datasets/bioner_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bioner_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6108 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bioner_id/bioner_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.555810 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_captioning/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_captioning/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8518 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.574385 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_lm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_lm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8430 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_lm/bloom_lm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.606560 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_speech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_speech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6922 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_speech/bloom_speech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.648391 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_vist/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_vist/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9674 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/bloom_vist/bloom_vist.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.707747 seacrowd-0.0.9/seacrowd/sea_datasets/burapha_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/burapha_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6995 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/burapha_th/burapha_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.745401 seacrowd-0.0.9/seacrowd/sea_datasets/burmese_romanize/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/burmese_romanize/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4420 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.779000 seacrowd-0.0.9/seacrowd/sea_datasets/casa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/casa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5635 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/casa/casa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.813404 seacrowd-0.0.9/seacrowd/sea_datasets/cc100/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cc100/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10941 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cc100/cc100.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.840420 seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_doc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_doc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6230 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.874164 seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_sent/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_sent/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6256 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:35.941550 seacrowd-0.0.9/seacrowd/sea_datasets/cebuaner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cebuaner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7783 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cebuaner/cebuaner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.004656 seacrowd-0.0.9/seacrowd/sea_datasets/coco_35l/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/coco_35l/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9830 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/coco_35l/coco_35l.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.030188 seacrowd-0.0.9/seacrowd/sea_datasets/cod/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cod/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6239 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cod/cod.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.054875 seacrowd-0.0.9/seacrowd/sea_datasets/code_mixed_jv_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/code_mixed_jv_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8760 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.089752 seacrowd-0.0.9/seacrowd/sea_datasets/codeswitch_reddit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/codeswitch_reddit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9015 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.122762 seacrowd-0.0.9/seacrowd/sea_datasets/commonvoice_120/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/commonvoice_120/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9438 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.154539 seacrowd-0.0.9/seacrowd/sea_datasets/copal/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/copal/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5868 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/copal/copal.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.172037 seacrowd-0.0.9/seacrowd/sea_datasets/covost2/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/covost2/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10329 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/covost2/covost2.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.189034 seacrowd-0.0.9/seacrowd/sea_datasets/creole_rc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:45.000000 seacrowd-0.0.9/seacrowd/sea_datasets/creole_rc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9448 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/creole_rc/creole_rc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.228168 seacrowd-0.0.9/seacrowd/sea_datasets/crosssum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/crosssum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5467 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/crosssum/crosssum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.253272 seacrowd-0.0.9/seacrowd/sea_datasets/cub_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cub_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14495 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.280804 seacrowd-0.0.9/seacrowd/sea_datasets/culturax/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/culturax/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6383 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/culturax/culturax.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.319311 seacrowd-0.0.9/seacrowd/sea_datasets/cvss/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cvss/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11054 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/cvss/cvss.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.341406 seacrowd-0.0.9/seacrowd/sea_datasets/dengue_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/dengue_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4777 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.362956 seacrowd-0.0.9/seacrowd/sea_datasets/emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5522 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emot/emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.404784 seacrowd-0.0.9/seacrowd/sea_datasets/emotcmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emotcmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4484 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emotcmt/emotcmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.434301 seacrowd-0.0.9/seacrowd/sea_datasets/emotes_3k/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emotes_3k/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9257 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emotes_3k/emotes_3k.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.468795 seacrowd-0.0.9/seacrowd/sea_datasets/emotion_id_opinion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emotion_id_opinion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7315 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.491373 seacrowd-0.0.9/seacrowd/sea_datasets/etos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/etos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7041 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/etos/etos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.513605 seacrowd-0.0.9/seacrowd/sea_datasets/facqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/facqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5788 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/facqa/facqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.546012 seacrowd-0.0.9/seacrowd/sea_datasets/facqa/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/facqa/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      815 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/facqa/utils/facqa_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.576624 seacrowd-0.0.9/seacrowd/sea_datasets/fakenews_ph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fakenews_ph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4936 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.602447 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_gay_lang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_gay_lang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4808 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.628601 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_hatespeech_tiktok/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_hatespeech_tiktok/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4697 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.652577 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_slang_norm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_slang_norm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4967 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.674851 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_words_aoa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_words_aoa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4965 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.692704 seacrowd-0.0.9/seacrowd/sea_datasets/filwordnet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filwordnet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/filwordnet/filwordnet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.729399 seacrowd-0.0.9/seacrowd/sea_datasets/fleurs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fleurs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13115 2024-04-12 07:50:18.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fleurs/fleurs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      800 2024-04-12 07:46:55.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fleurs/lang_config.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.751363 seacrowd-0.0.9/seacrowd/sea_datasets/flores200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/flores200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13920 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/flores200/flores200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.770707 seacrowd-0.0.9/seacrowd/sea_datasets/fsl_105/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fsl_105/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6817 2024-04-12 07:57:15.000000 seacrowd-0.0.9/seacrowd/sea_datasets/fsl_105/fsl_105.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.793731 seacrowd-0.0.9/seacrowd/sea_datasets/gatitos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/gatitos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6624 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/gatitos/gatitos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.818176 seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_newsclass/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_newsclass/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6024 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.842298 seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5007 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.865423 seacrowd-0.0.9/seacrowd/sea_datasets/globalwoz/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/globalwoz/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10031 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/globalwoz/globalwoz.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.886727 seacrowd-0.0.9/seacrowd/sea_datasets/glotstorybook/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/glotstorybook/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5878 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/glotstorybook/glotstorybook.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.905727 seacrowd-0.0.9/seacrowd/sea_datasets/hoasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/hoasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6301 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/hoasa/hoasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.935717 seacrowd-0.0.9/seacrowd/sea_datasets/iapp_squad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/iapp_squad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5420 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/iapp_squad/iapp_squad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.955300 seacrowd-0.0.9/seacrowd/sea_datasets/iatf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/iatf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5870 2024-04-12 08:01:12.000000 seacrowd-0.0.9/seacrowd/sea_datasets/iatf/iatf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.981446 seacrowd-0.0.9/seacrowd/sea_datasets/icon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/icon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8351 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/icon/icon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:36.998861 seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6540 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive/id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.015795 seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive_news_comment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive_news_comment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4293 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.034585 seacrowd-0.0.9/seacrowd/sea_datasets/id_am2ico/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_am2ico/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7430 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_am2ico/id_am2ico.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.067051 seacrowd-0.0.9/seacrowd/sea_datasets/id_clickbait/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_clickbait/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5770 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_clickbait/id_clickbait.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.117409 seacrowd-0.0.9/seacrowd/sea_datasets/id_coreference_resolution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_coreference_resolution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7576 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.143025 seacrowd-0.0.9/seacrowd/sea_datasets/id_frog_story/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_frog_story/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4524 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_frog_story/id_frog_story.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.161516 seacrowd-0.0.9/seacrowd/sea_datasets/id_google_play_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_google_play_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6144 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.197122 seacrowd-0.0.9/seacrowd/sea_datasets/id_hatespeech/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_hatespeech/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4450 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.220883 seacrowd-0.0.9/seacrowd/sea_datasets/id_hoax_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_hoax_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.239781 seacrowd-0.0.9/seacrowd/sea_datasets/id_hsd_nofaaulia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_hsd_nofaaulia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7252 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.260649 seacrowd-0.0.9/seacrowd/sea_datasets/id_msvd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_msvd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5051 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_msvd/id_msvd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.286214 seacrowd-0.0.9/seacrowd/sea_datasets/id_multilabel_hs/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_multilabel_hs/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6021 2024-04-04 06:00:46.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.304830 seacrowd-0.0.9/seacrowd/sea_datasets/id_panl_bppt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_panl_bppt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5616 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.331858 seacrowd-0.0.9/seacrowd/sea_datasets/id_qqp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_qqp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4686 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_qqp/id_qqp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.353836 seacrowd-0.0.9/seacrowd/sea_datasets/id_sent_emo_mobile_apps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_sent_emo_mobile_apps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5395 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.380379 seacrowd-0.0.9/seacrowd/sea_datasets/id_sentiment_analysis/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_sentiment_analysis/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5538 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.409300 seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9107 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.447617 seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1826 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.472328 seacrowd-0.0.9/seacrowd/sea_datasets/id_stance/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_stance/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5114 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_stance/id_stance.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.491512 seacrowd-0.0.9/seacrowd/sea_datasets/id_sts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_sts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4308 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_sts/id_sts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.527030 seacrowd-0.0.9/seacrowd/sea_datasets/id_vaccines_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_vaccines_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4329 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.545102 seacrowd-0.0.9/seacrowd/sea_datasets/id_wiki_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_wiki_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6697 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.569487 seacrowd-0.0.9/seacrowd/sea_datasets/id_wsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_wsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6404 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/id_wsd/id_wsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.600589 seacrowd-0.0.9/seacrowd/sea_datasets/identic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/identic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13357 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/identic/identic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.647333 seacrowd-0.0.9/seacrowd/sea_datasets/identifikasi_bahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/identifikasi_bahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5177 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.671328 seacrowd-0.0.9/seacrowd/sea_datasets/idk_mrc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/idk_mrc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9530 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/idk_mrc/idk_mrc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.690472 seacrowd-0.0.9/seacrowd/sea_datasets/idn_tagged_corpus_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/idn_tagged_corpus_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6193 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.714686 seacrowd-0.0.9/seacrowd/sea_datasets/ijelid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ijelid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5403 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ijelid/ijelid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.735487 seacrowd-0.0.9/seacrowd/sea_datasets/imdb_jv/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/imdb_jv/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4894 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/imdb_jv/imdb_jv.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.760352 seacrowd-0.0.9/seacrowd/sea_datasets/indo4b/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo4b/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7236 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo4b/indo4b.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.779203 seacrowd-0.0.9/seacrowd/sea_datasets/indo4b_plus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo4b_plus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7417 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.826095 seacrowd-0.0.9/seacrowd/sea_datasets/indo_general_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_general_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6442 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.847585 seacrowd-0.0.9/seacrowd/sea_datasets/indo_law/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_law/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5445 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_law/indo_law.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.866945 seacrowd-0.0.9/seacrowd/sea_datasets/indo_puisi/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_puisi/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4018 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_puisi/indo_puisi.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.892421 seacrowd-0.0.9/seacrowd/sea_datasets/indo_religious_mt_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_religious_mt_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8507 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.916278 seacrowd-0.0.9/seacrowd/sea_datasets/indo_story_cloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_story_cloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6563 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.946132 seacrowd-0.0.9/seacrowd/sea_datasets/indocamrest/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocamrest/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6670 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocamrest/indocamrest.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:37.975309 seacrowd-0.0.9/seacrowd/sea_datasets/indocollex/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocollex/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6949 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocollex/indocollex.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.005412 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11610 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/indocoref.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.063115 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9072 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/feature_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2091 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/file_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4307 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.089210 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ner_ugm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ner_ugm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6402 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.127339 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_nerui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_nerui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8192 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.167850 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ntp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ntp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5885 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.193177 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12679 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.214130 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_tweet_ordering/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_tweet_ordering/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12454 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.238050 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_gsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_gsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8462 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.282210 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_pud/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_pud/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8825 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.332817 seacrowd-0.0.9/seacrowd/sea_datasets/indoler/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indoler/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9100 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indoler/indoler.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.354507 seacrowd-0.0.9/seacrowd/sea_datasets/indommlu/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indommlu/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10934 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indommlu/indommlu.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.386686 seacrowd-0.0.9/seacrowd/sea_datasets/indoner_tourism/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indoner_tourism/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8394 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.411472 seacrowd-0.0.9/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5250 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.451770 seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_madurese_bible_translation/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_madurese_bible_translation/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7932 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.474941 seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_news_dataset/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:47.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_news_dataset/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4581 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.509505 seacrowd-0.0.9/seacrowd/sea_datasets/indonesiannmt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesiannmt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9148 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.540942 seacrowd-0.0.9/seacrowd/sea_datasets/indonglish/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonglish/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8339 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonglish/indonglish.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.598626 seacrowd-0.0.9/seacrowd/sea_datasets/indonli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8050 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonli/indonli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.626150 seacrowd-0.0.9/seacrowd/sea_datasets/indonlu_nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonlu_nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5677 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.646145 seacrowd-0.0.9/seacrowd/sea_datasets/indoqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indoqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5422 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indoqa/indoqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.670391 seacrowd-0.0.9/seacrowd/sea_datasets/indosmd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indosmd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13550 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indosmd/indosmd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.692693 seacrowd-0.0.9/seacrowd/sea_datasets/indosum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indosum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6872 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indosum/indosum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.711099 seacrowd-0.0.9/seacrowd/sea_datasets/indotacos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indotacos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indotacos/indotacos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.728345 seacrowd-0.0.9/seacrowd/sea_datasets/indowiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indowiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7684 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indowiki/indowiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.749660 seacrowd-0.0.9/seacrowd/sea_datasets/indqner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indqner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6614 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indqner/indqner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.767224 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_digit_cdsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_digit_cdsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9856 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.784747 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8440 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.803775 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9432 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.834658 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8857 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.872567 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    11615 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.894230 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9932 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.931893 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_svcsr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_svcsr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9818 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.956717 seacrowd-0.0.9/seacrowd/sea_datasets/inset_lexicon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/inset_lexicon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4829 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:38.984762 seacrowd-0.0.9/seacrowd/sea_datasets/jadi_ide/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/jadi_ide/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4404 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/jadi_ide/jadi_ide.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.003635 seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6236 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.025542 seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7628 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.051977 seacrowd-0.0.9/seacrowd/sea_datasets/kamus_alay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kamus_alay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5286 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kamus_alay/kamus_alay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.077513 seacrowd-0.0.9/seacrowd/sea_datasets/karonese_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/karonese_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4533 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.098266 seacrowd-0.0.9/seacrowd/sea_datasets/kawat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kawat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5933 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kawat/kawat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.117354 seacrowd-0.0.9/seacrowd/sea_datasets/kde4/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kde4/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14408 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kde4/kde4.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.134112 seacrowd-0.0.9/seacrowd/sea_datasets/keps/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/keps/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5066 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/keps/keps.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.149941 seacrowd-0.0.9/seacrowd/sea_datasets/kheng_info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kheng_info/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3687 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kheng_info/kheng_info.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.189231 seacrowd-0.0.9/seacrowd/sea_datasets/khmer_alt_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/khmer_alt_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7442 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.225381 seacrowd-0.0.9/seacrowd/sea_datasets/khpos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/khpos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8756 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/khpos/khpos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.259488 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10035 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc/kopi_cc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.295086 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc_news/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc_news/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5088 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.314698 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_nllb/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_nllb/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5956 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.334001 seacrowd-0.0.9/seacrowd/sea_datasets/korpus_nusantara/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/korpus_nusantara/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8476 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.353940 seacrowd-0.0.9/seacrowd/sea_datasets/lazada_review_filipino/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/lazada_review_filipino/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4913 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.378263 seacrowd-0.0.9/seacrowd/sea_datasets/librivox_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/librivox_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8736 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.396459 seacrowd-0.0.9/seacrowd/sea_datasets/limesoda/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/limesoda/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6775 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/limesoda/limesoda.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.414698 seacrowd-0.0.9/seacrowd/sea_datasets/liputan6/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/liputan6/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7512 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/liputan6/liputan6.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.432515 seacrowd-0.0.9/seacrowd/sea_datasets/local_id_abusive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/local_id_abusive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7530 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.453744 seacrowd-0.0.9/seacrowd/sea_datasets/lr_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/lr_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6160 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/lr_sum/lr_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.472427 seacrowd-0.0.9/seacrowd/sea_datasets/m3exam/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/m3exam/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    14637 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/m3exam/m3exam.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.493868 seacrowd-0.0.9/seacrowd/sea_datasets/mabl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mabl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8609 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mabl/mabl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.513441 seacrowd-0.0.9/seacrowd/sea_datasets/malaysia_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/malaysia_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6432 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.529945 seacrowd-0.0.9/seacrowd/sea_datasets/malindo_morph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/malindo_morph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4617 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/malindo_morph/malindo_morph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.548740 seacrowd-0.0.9/seacrowd/sea_datasets/malindo_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/malindo_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6494 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.566918 seacrowd-0.0.9/seacrowd/sea_datasets/massive/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/massive/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    18420 2024-04-04 06:00:48.000000 seacrowd-0.0.9/seacrowd/sea_datasets/massive/massive.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.585384 seacrowd-0.0.9/seacrowd/sea_datasets/mc4_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mc4_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5510 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mc4_indo/mc4_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.607704 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_brunei/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_brunei/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10682 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.627972 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sabah/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sabah/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5561 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.645494 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sarawak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sarawak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6559 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.670497 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_standard_lisan/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_standard_lisan/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7594 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.689473 seacrowd-0.0.9/seacrowd/sea_datasets/memolon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/memolon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5589 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/memolon/memolon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.708591 seacrowd-0.0.9/seacrowd/sea_datasets/minangnlp_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/minangnlp_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6874 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.727579 seacrowd-0.0.9/seacrowd/sea_datasets/miracl/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/miracl/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    13119 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/miracl/miracl.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.745175 seacrowd-0.0.9/seacrowd/sea_datasets/mkqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mkqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8345 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mkqa/mkqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.773249 seacrowd-0.0.9/seacrowd/sea_datasets/mlqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mlqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9825 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mlqa/mlqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.793084 seacrowd-0.0.9/seacrowd/sea_datasets/mozilla_pontoon/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mozilla_pontoon/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6211 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.812370 seacrowd-0.0.9/seacrowd/sea_datasets/mswc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mswc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8048 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mswc/mswc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.839730 seacrowd-0.0.9/seacrowd/sea_datasets/mtop_intent_classification/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mtop_intent_classification/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2654 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mtop_intent_classification/labels.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5662 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.857683 seacrowd-0.0.9/seacrowd/sea_datasets/multilexnorm/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/multilexnorm/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6223 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/multilexnorm/multilexnorm.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.885593 seacrowd-0.0.9/seacrowd/sea_datasets/my_paraphrase/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/my_paraphrase/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8124 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.903315 seacrowd-0.0.9/seacrowd/sea_datasets/myanmar_rakhine_parallel/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/myanmar_rakhine_parallel/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7223 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.927941 seacrowd-0.0.9/seacrowd/sea_datasets/mypos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mypos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5116 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mypos/mypos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.946834 seacrowd-0.0.9/seacrowd/sea_datasets/mysentence/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mysentence/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7612 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/mysentence/mysentence.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.967610 seacrowd-0.0.9/seacrowd/sea_datasets/myxnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/myxnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5096 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/myxnli/myxnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:39.992689 seacrowd-0.0.9/seacrowd/sea_datasets/nergrit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nergrit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6322 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nergrit/nergrit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.012916 seacrowd-0.0.9/seacrowd/sea_datasets/nerp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nerp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4852 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nerp/nerp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.032231 seacrowd-0.0.9/seacrowd/sea_datasets/netifier/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/netifier/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4838 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/netifier/netifier.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.049934 seacrowd-0.0.9/seacrowd/sea_datasets/news_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/news_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5003 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/news_en_id/news_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.069346 seacrowd-0.0.9/seacrowd/sea_datasets/newsph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/newsph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3810 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/newsph/newsph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.096476 seacrowd-0.0.9/seacrowd/sea_datasets/nllb_seed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nllb_seed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15208 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nllb_seed/nllb_seed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.113983 seacrowd-0.0.9/seacrowd/sea_datasets/ntrex_128/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ntrex_128/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10971 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ntrex_128/ntrex_128.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.134490 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8785 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.150610 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_rhetoric/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_rhetoric/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8792 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.168575 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_topic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_topic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8845 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.196157 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.216292 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9156 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.235168 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8285 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.254241 seacrowd-0.0.9/seacrowd/sea_datasets/nusax_mt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusax_mt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7578 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusax_mt/nusax_mt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.275255 seacrowd-0.0.9/seacrowd/sea_datasets/nusax_senti/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusax_senti/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7250 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/nusax_senti/nusax_senti.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.293775 seacrowd-0.0.9/seacrowd/sea_datasets/oil/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/oil/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5477 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/oil/oil.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.311668 seacrowd-0.0.9/seacrowd/sea_datasets/ojw/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ojw/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5110 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ojw/ojw.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.333098 seacrowd-0.0.9/seacrowd/sea_datasets/openlid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/openlid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7915 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/openlid/openlid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.352731 seacrowd-0.0.9/seacrowd/sea_datasets/openslr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/openslr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10343 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/openslr/openslr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.382858 seacrowd-0.0.9/seacrowd/sea_datasets/orchid_pos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/orchid_pos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9625 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/orchid_pos/orchid_pos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.402811 seacrowd-0.0.9/seacrowd/sea_datasets/oscar_2201/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/oscar_2201/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    16270 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/oscar_2201/oscar_2201.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.436738 seacrowd-0.0.9/seacrowd/sea_datasets/palito/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/palito/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5930 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/palito/palito.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.467818 seacrowd-0.0.9/seacrowd/sea_datasets/paracotta_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/paracotta_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4768 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/paracotta_id/paracotta_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.489313 seacrowd-0.0.9/seacrowd/sea_datasets/parallel_id_nyo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/parallel_id_nyo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5471 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.510634 seacrowd-0.0.9/seacrowd/sea_datasets/parallel_su_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/parallel_su_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4782 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.529118 seacrowd-0.0.9/seacrowd/sea_datasets/ph_fake_news_corpus/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ph_fake_news_corpus/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4339 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.544303 seacrowd-0.0.9/seacrowd/sea_datasets/pho_ner_covid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/pho_ner_covid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6866 2024-04-04 06:00:49.000000 seacrowd-0.0.9/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.561481 seacrowd-0.0.9/seacrowd/sea_datasets/phomt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/phomt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5141 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/phomt/phomt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.592876 seacrowd-0.0.9/seacrowd/sea_datasets/phost/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/phost/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9498 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/phost/phost.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.612727 seacrowd-0.0.9/seacrowd/sea_datasets/posp/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/posp/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5990 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/posp/posp.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.641055 seacrowd-0.0.9/seacrowd/sea_datasets/postag_su/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/postag_su/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8033 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/postag_su/postag_su.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.667179 seacrowd-0.0.9/seacrowd/sea_datasets/prdect_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/prdect_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7572 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/prdect_id/prdect_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.701085 seacrowd-0.0.9/seacrowd/sea_datasets/qasina/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/qasina/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6424 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/qasina/qasina.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.728782 seacrowd-0.0.9/seacrowd/sea_datasets/roots_vi_ted/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/roots_vi_ted/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5065 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.749357 seacrowd-0.0.9/seacrowd/sea_datasets/sampiran/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sampiran/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5024 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sampiran/sampiran.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.768066 seacrowd-0.0.9/seacrowd/sea_datasets/sap_wat/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sap_wat/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7077 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sap_wat/sap_wat.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.794455 seacrowd-0.0.9/seacrowd/sea_datasets/sarawak_malay/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sarawak_malay/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7381 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.830782 seacrowd-0.0.9/seacrowd/sea_datasets/scb_mt_en_th/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/scb_mt_en_th/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7071 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.850682 seacrowd-0.0.9/seacrowd/sea_datasets/sea_bench/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_bench/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7206 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_bench/sea_bench.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.870954 seacrowd-0.0.9/seacrowd/sea_datasets/sea_madlad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_madlad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10051 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_madlad/sea_madlad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.903039 seacrowd-0.0.9/seacrowd/sea_datasets/sea_wiki/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_wiki/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1844 2024-04-12 07:50:53.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_wiki/lang_config.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9272 2024-04-12 07:52:13.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sea_wiki/sea_wiki.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.926216 seacrowd-0.0.9/seacrowd/sea_datasets/seaeval/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/seaeval/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9350 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/seaeval/seaeval.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.948782 seacrowd-0.0.9/seacrowd/sea_datasets/seahorse/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/seahorse/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6884 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/seahorse/seahorse.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.966471 seacrowd-0.0.9/seacrowd/sea_datasets/sentiment_nathasa_review/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sentiment_nathasa_review/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6002 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:40.986220 seacrowd-0.0.9/seacrowd/sea_datasets/shopee_reviews_tagalog/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/shopee_reviews_tagalog/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4597 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.006648 seacrowd-0.0.9/seacrowd/sea_datasets/singgalang/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/singgalang/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5430 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/singgalang/singgalang.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.036080 seacrowd-0.0.9/seacrowd/sea_datasets/smsa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/smsa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5575 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/smsa/smsa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.056470 seacrowd-0.0.9/seacrowd/sea_datasets/snli_indo/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/snli_indo/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6244 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/snli_indo/snli_indo.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.077016 seacrowd-0.0.9/seacrowd/sea_datasets/spamid_pair/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/spamid_pair/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5524 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/spamid_pair/spamid_pair.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.103227 seacrowd-0.0.9/seacrowd/sea_datasets/squad_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/squad_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5315 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/squad_id/squad_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.126489 seacrowd-0.0.9/seacrowd/sea_datasets/stb_ext/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/stb_ext/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9273 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/stb_ext/stb_ext.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.144499 seacrowd-0.0.9/seacrowd/sea_datasets/stif_indonesia/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/stif_indonesia/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5135 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.165124 seacrowd-0.0.9/seacrowd/sea_datasets/struct_amb_ind/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/struct_amb_ind/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7724 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.183342 seacrowd-0.0.9/seacrowd/sea_datasets/su_emot/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/su_emot/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4567 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/su_emot/su_emot.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.203215 seacrowd-0.0.9/seacrowd/sea_datasets/su_id_asr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/su_id_asr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5601 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/su_id_asr/su_id_asr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.230628 seacrowd-0.0.9/seacrowd/sea_datasets/su_id_tts/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/su_id_tts/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/su_id_tts/su_id_tts.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.248440 seacrowd-0.0.9/seacrowd/sea_datasets/talpco/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/talpco/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6870 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/talpco/talpco.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.264532 seacrowd-0.0.9/seacrowd/sea_datasets/tatabahasa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tatabahasa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5411 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tatabahasa/tatabahasa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.280352 seacrowd-0.0.9/seacrowd/sea_datasets/tatoeba/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tatoeba/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7636 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tatoeba/tatoeba.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.298520 seacrowd-0.0.9/seacrowd/sea_datasets/tcope/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tcope/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6693 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tcope/tcope.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.317137 seacrowd-0.0.9/seacrowd/sea_datasets/ted_en_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ted_en_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7105 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ted_en_id/ted_en_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.335985 seacrowd-0.0.9/seacrowd/sea_datasets/term_a/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/term_a/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5358 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/term_a/term_a.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.357127 seacrowd-0.0.9/seacrowd/sea_datasets/tgl_profanity/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tgl_profanity/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4351 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.375160 seacrowd-0.0.9/seacrowd/sea_datasets/tha_lao_embassy_parcor/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tha_lao_embassy_parcor/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4436 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.402490 seacrowd-0.0.9/seacrowd/sea_datasets/thai_alpaca/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_alpaca/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3943 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.424997 seacrowd-0.0.9/seacrowd/sea_datasets/thai_constitution/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_constitution/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10954 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_constitution/thai_constitution.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.444769 seacrowd-0.0.9/seacrowd/sea_datasets/thai_databricks_dolly/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_databricks_dolly/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4388 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.464460 seacrowd-0.0.9/seacrowd/sea_datasets/thai_depression/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_depression/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5739 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_depression/thai_depression.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.504418 seacrowd-0.0.9/seacrowd/sea_datasets/thai_gpteacher/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_gpteacher/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3960 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.522979 seacrowd-0.0.9/seacrowd/sea_datasets/thai_hh_rlhf/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_hh_rlhf/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5077 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.541490 seacrowd-0.0.9/seacrowd/sea_datasets/thai_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5683 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_sum/thai_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.559857 seacrowd-0.0.9/seacrowd/sea_datasets/thai_toxicity_tweet/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_toxicity_tweet/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4555 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.578119 seacrowd-0.0.9/seacrowd/sea_datasets/tico_19/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tico_19/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12192 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tico_19/tico_19.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.595879 seacrowd-0.0.9/seacrowd/sea_datasets/titml_idn/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/titml_idn/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/titml_idn/titml_idn.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.621433 seacrowd-0.0.9/seacrowd/sea_datasets/tlunified_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:50.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tlunified_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5800 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.639904 seacrowd-0.0.9/seacrowd/sea_datasets/toxicity_200/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/toxicity_200/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5975 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/toxicity_200/toxicity_200.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.665786 seacrowd-0.0.9/seacrowd/sea_datasets/tydiqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tydiqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23881 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/tydiqa/tydiqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.689695 seacrowd-0.0.9/seacrowd/sea_datasets/typhoon_yolanda_tweets/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/typhoon_yolanda_tweets/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5165 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.718324 seacrowd-0.0.9/seacrowd/sea_datasets/ucla_phonetic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ucla_phonetic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6531 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.741779 seacrowd-0.0.9/seacrowd/sea_datasets/ud_id_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ud_id_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9185 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.759938 seacrowd-0.0.9/seacrowd/sea_datasets/ud_jv_csui/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ud_jv_csui/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    10052 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.779304 seacrowd-0.0.9/seacrowd/sea_datasets/udhr/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/udhr/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6030 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/udhr/udhr.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.803050 seacrowd-0.0.9/seacrowd/sea_datasets/udhr_lid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/udhr_lid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5190 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/udhr_lid/udhr_lid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.837523 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vicov19qa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vicov19qa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7244 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.864712 seacrowd-0.0.9/seacrowd/sea_datasets/uit_victsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_victsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5311 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_victsd/uit_victsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.885171 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vihsd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vihsd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5721 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.910030 seacrowd-0.0.9/seacrowd/sea_datasets/uit_viic/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_viic/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6572 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_viic/uit_viic.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.928982 seacrowd-0.0.9/seacrowd/sea_datasets/uit_viocd/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_viocd/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_viocd/uit_viocd.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.947810 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vion/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vion/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5939 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vion/uit_vion.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.963325 seacrowd-0.0.9/seacrowd/sea_datasets/uit_visd4sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_visd4sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7034 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.980297 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsfc/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsfc/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8715 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:41.998724 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsmec/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsmec/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4802 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.016821 seacrowd-0.0.9/seacrowd/sea_datasets/unimorph/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/unimorph/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15492 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/unimorph/unimorph.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.037000 seacrowd-0.0.9/seacrowd/sea_datasets/unimorph_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/unimorph_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7445 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/unimorph_id/unimorph_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.057198 seacrowd-0.0.9/seacrowd/sea_datasets/vi_pubmed/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vi_pubmed/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    15136 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.081777 seacrowd-0.0.9/seacrowd/sea_datasets/vihealthqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vihealthqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5587 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vihealthqa/vihealthqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.112933 seacrowd-0.0.9/seacrowd/sea_datasets/visobert/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/visobert/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6265 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/visobert/visobert.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.134783 seacrowd-0.0.9/seacrowd/sea_datasets/vispamreviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vispamreviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7245 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vispamreviews/vispamreviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.168592 seacrowd-0.0.9/seacrowd/sea_datasets/vistec_tp_th_21/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vistec_tp_th_21/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6739 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.196369 seacrowd-0.0.9/seacrowd/sea_datasets/vitext2sql/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vitext2sql/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6893 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vitext2sql/vitext2sql.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.233699 seacrowd-0.0.9/seacrowd/sea_datasets/vivos/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vivos/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7832 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vivos/vivos.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.250084 seacrowd-0.0.9/seacrowd/sea_datasets/vivqa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vivqa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9080 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vivqa/vivqa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.266148 seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_ner/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_ner/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5857 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.282873 seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_sa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_sa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7134 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.331206 seacrowd-0.0.9/seacrowd/sea_datasets/vndt/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vndt/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2232 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vndt/utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7852 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/vndt/vndt.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.350189 seacrowd-0.0.9/seacrowd/sea_datasets/voxlingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/voxlingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7980 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/voxlingua/voxlingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.367501 seacrowd-0.0.9/seacrowd/sea_datasets/weathub/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/weathub/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7521 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/weathub/weathub.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.387417 seacrowd-0.0.9/seacrowd/sea_datasets/wikiann/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikiann/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8643 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikiann/wikiann.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.416602 seacrowd-0.0.9/seacrowd/sea_datasets/wikilingua/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikilingua/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4984 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikilingua/wikilingua.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.447221 seacrowd-0.0.9/seacrowd/sea_datasets/wikimatrix/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikimatrix/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8585 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikimatrix/wikimatrix.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.465168 seacrowd-0.0.9/seacrowd/sea_datasets/wikitext_tl_39/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikitext_tl_39/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3663 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.484369 seacrowd-0.0.9/seacrowd/sea_datasets/wili_2018/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wili_2018/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6699 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wili_2018/wili_2018.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.510447 seacrowd-0.0.9/seacrowd/sea_datasets/wisesight_thai_sentiment/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wisesight_thai_sentiment/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7027 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.536071 seacrowd-0.0.9/seacrowd/sea_datasets/wit/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wit/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12057 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wit/wit.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.556013 seacrowd-0.0.9/seacrowd/sea_datasets/wongnai_reviews/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wongnai_reviews/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4106 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.578437 seacrowd-0.0.9/seacrowd/sea_datasets/wrete/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wrete/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6113 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/wrete/wrete.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.597537 seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/__init__.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.652054 seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      473 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/utils/x_fact_utils.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5900 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/x_fact.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.671116 seacrowd-0.0.9/seacrowd/sea_datasets/xcopa/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xcopa/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     7024 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xcopa/xcopa.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.691396 seacrowd-0.0.9/seacrowd/sea_datasets/xl_jailbreak/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xl_jailbreak/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6317 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.716671 seacrowd-0.0.9/seacrowd/sea_datasets/xl_sum/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xl_sum/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6903 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xl_sum/xl_sum.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.743231 seacrowd-0.0.9/seacrowd/sea_datasets/xm3600/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xm3600/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8233 2024-04-11 08:39:41.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xm3600/xm3600.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.762373 seacrowd-0.0.9/seacrowd/sea_datasets/xnli/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xnli/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     8333 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xnli/xnli.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.783691 seacrowd-0.0.9/seacrowd/sea_datasets/xpersona_id/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xpersona_id/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6550 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xpersona_id/xpersona_id.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.804852 seacrowd-0.0.9/seacrowd/sea_datasets/xquad/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xquad/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     4819 2024-04-04 06:00:51.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xquad/xquad.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.829235 seacrowd-0.0.9/seacrowd/sea_datasets/xsid/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xsid/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     9510 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xsid/xsid.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.857095 seacrowd-0.0.9/seacrowd/sea_datasets/xstorycloze/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xstorycloze/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     6794 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/sea_datasets/xstorycloze/xstorycloze.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.876177 seacrowd-0.0.9/seacrowd/sea_datasets/yunshan_cup_2020/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/sea_datasets/yunshan_cup_2020/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5828 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:42.933982 seacrowd-0.0.9/seacrowd/utils/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     5493 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/common_parser.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      284 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/configs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    12786 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/constants.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:43.190276 seacrowd-0.0.9/seacrowd/utils/schemas/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1485 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      506 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/image_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1101 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/imqa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     2283 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/kb.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      626 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/pairs.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      371 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/pairs_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1007 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/qa.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      206 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/self_supervised_pretraining.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      525 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/seq_label.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      618 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      606 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/speech_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      454 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/speech_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      796 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/speech_to_speech.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      311 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      331 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/text_multilabel.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      444 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/text_to_text.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3046 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/tod.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     3068 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/tree.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      810 2024-04-04 06:00:52.000000 seacrowd-0.0.9/seacrowd/utils/schemas/video.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:43.271497 seacrowd-0.0.9/seacrowd.egg-info/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)     1071 2024-04-12 08:01:32.000000 seacrowd-0.0.9/seacrowd.egg-info/PKG-INFO
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    31367 2024-04-12 08:01:33.000000 seacrowd-0.0.9/seacrowd.egg-info/SOURCES.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        1 2024-04-12 08:01:32.000000 seacrowd-0.0.9/seacrowd.egg-info/dependency_links.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      409 2024-04-12 08:01:32.000000 seacrowd-0.0.9/seacrowd.egg-info/requires.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       15 2024-04-12 08:01:32.000000 seacrowd-0.0.9/seacrowd.egg-info/top_level.txt
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)      703 2024-04-12 08:01:43.305668 seacrowd-0.0.9/setup.cfg
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)       68 2024-04-12 07:28:29.000000 seacrowd-0.0.9/setup.py
+drwxr-xr-x   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-12 08:01:43.253785 seacrowd-0.0.9/tests/
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)        0 2024-04-04 06:00:52.000000 seacrowd-0.0.9/tests/__init__.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    23314 2024-04-04 06:00:52.000000 seacrowd-0.0.9/tests/test_seacrowd.py
+-rw-r--r--   0 holylovenia  (1006) holylovenia  (1007)    20714 2024-04-04 06:00:52.000000 seacrowd-0.0.9/tests/test_seacrowd_source_only.py
```

### Comparing `seacrowd-0.0.8/LICENSE` & `seacrowd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/PKG-INFO` & `seacrowd-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.8
+Version: 0.0.9
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.8/README.md` & `seacrowd-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/config_helper.py` & `seacrowd-0.0.9/seacrowd/config_helper.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/abui_wordnet/abui_wordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/alt_burmese_treebank.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/alt_burmese_treebank/utils/alt_burmese_treebank_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ara_close/ara_close.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ara_close/ara_close.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/asr_sindodusc/asr_sindodusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/asr_smaldusc/asr_smaldusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/asr_stidusc/asr_stidusc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/audio_keyword_spotting/audio_keyword_spotting.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/aya_dataset/aya_dataset.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/aya_dataset/aya_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/barasa/barasa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/barasa/barasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/beaye_lexicon/beaye_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/belebele/belebele.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/belebele/belebele.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bible_en_id/bible_en_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bible_en_id/bible_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bible_jv_id/bible_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bible_su_id/bible_su_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bible_su_id/bible_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bioner_id/bioner_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bioner_id/bioner_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bloom_captioning/bloom_captioning.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bloom_lm/bloom_lm.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bloom_lm/bloom_lm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bloom_speech/bloom_speech.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bloom_speech/bloom_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/bloom_vist/bloom_vist.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/bloom_vist/bloom_vist.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/burapha_th/burapha_th.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/burapha_th/burapha_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/burmese_romanize/burmese_romanize.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/casa/casa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/casa/casa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cc100/cc100.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cc100/cc100.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_doc/cc_aligned_doc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cc_aligned_sent/cc_aligned_sent.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cebuaner/cebuaner.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cebuaner/cebuaner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/coco_35l/coco_35l.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/coco_35l/coco_35l.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cod/cod.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cod/cod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/code_mixed_jv_id/code_mixed_jv_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/codeswitch_reddit/codeswitch_reddit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/commonvoice_120/commonvoice_120.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/copal/copal.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/copal/copal.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/covost2/covost2.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/covost2/covost2.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/creole_rc/creole_rc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/creole_rc/creole_rc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/crosssum/crosssum.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/crosssum/crosssum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cub_bahasa/cub_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/culturax/culturax.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/culturax/culturax.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/cvss/cvss.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/cvss/cvss.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/dengue_filipino/dengue_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/emot/emot.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/emot/emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/emotcmt/emotcmt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/emotcmt/emotcmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/emotes_3k/emotes_3k.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/emotes_3k/emotes_3k.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/emotion_id_opinion/emotion_id_opinion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/etos/etos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/etos/etos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/facqa/facqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/facqa/facqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/facqa/utils/facqa_utils.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/facqa/utils/facqa_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/fakenews_ph/fakenews_ph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/filipino_gay_lang/filipino_gay_lang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/filipino_hatespeech_tiktok/filipino_hatespeech_tiktok.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/filipino_slang_norm/filipino_slang_norm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/filipino_words_aoa/filipino_words_aoa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/filwordnet/filwordnet.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/filwordnet/filwordnet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/fleurs/fleurs.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/fleurs/fleurs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/fleurs/lang_config.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/fleurs/lang_config.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/flores200/flores200.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/flores200/flores200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/fsl_105/fsl_105.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/fsl_105/fsl_105.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/gatitos/gatitos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/gatitos/gatitos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_newsclass/gklmip_newsclass.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/gklmip_sentiment/gklmip_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/globalwoz/globalwoz.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/globalwoz/globalwoz.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/glotstorybook/glotstorybook.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/glotstorybook/glotstorybook.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/hoasa/hoasa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/hoasa/hoasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/iapp_squad/iapp_squad.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/iapp_squad/iapp_squad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/iatf/iatf.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/iatf/iatf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import datasets
-import pyreadr
+
+try:
+    import pyreadr
+except:
+    print("Install the `pyreadr` package to use.")
 
 from seacrowd.utils import schemas
 from seacrowd.utils.configs import SEACrowdConfig
 from seacrowd.utils.constants import (TASK_TO_SCHEMA, Licenses, Tasks)
 
 _DATASETNAME = "iatf"
```

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/icon/icon.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/icon/icon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive/id_abusive.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive/id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_abusive_news_comment/id_abusive_news_comment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_am2ico/id_am2ico.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_am2ico/id_am2ico.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_clickbait/id_clickbait.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_clickbait/id_clickbait.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_coreference_resolution/id_coreference_resolution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_frog_story/id_frog_story.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_frog_story/id_frog_story.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_google_play_review/id_google_play_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_hatespeech/id_hatespeech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_hoax_news/id_hoax_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_hsd_nofaaulia/id_hsd_nofaaulia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_msvd/id_msvd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_msvd/id_msvd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_multilabel_hs/id_multilabel_hs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_panl_bppt/id_panl_bppt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_qqp/id_qqp.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_qqp/id_qqp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_sent_emo_mobile_apps/id_sent_emo_mobile_apps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_sentiment_analysis/id_sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/id_short_answer_grading.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_short_answer_grading/utils/id_short_answer_grading_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_stance/id_stance.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_stance/id_stance.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_sts/id_sts.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_sts/id_sts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_vaccines_tweets/id_vaccines_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_wiki_parallel/id_wiki_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/id_wsd/id_wsd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/id_wsd/id_wsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/identic/identic.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/identic/identic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/identifikasi_bahasa/identifikasi_bahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/idk_mrc/idk_mrc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/idk_mrc/idk_mrc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/idn_tagged_corpus_csui/idn_tagged_corpus_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ijelid/ijelid.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ijelid/ijelid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/imdb_jv/imdb_jv.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/imdb_jv/imdb_jv.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo4b/indo4b.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo4b/indo4b.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo4b_plus/indo4b_plus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo_general_mt_en_id/indo_general_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo_law/indo_law.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo_law/indo_law.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo_puisi/indo_puisi.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo_puisi/indo_puisi.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo_religious_mt_en_id/indo_religious_mt_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indo_story_cloze/indo_story_cloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indocamrest/indocamrest.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indocamrest/indocamrest.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indocollex/indocollex.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indocollex/indocollex.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/indocoref.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/indocoref.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/feature_utils.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/feature_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/file_utils.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indocoref/utils/text_preprocess.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ner_ugm/indolem_ner_ugm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_nerui/indolem_nerui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ntp/indolem_ntp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_sentiment/indolem_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_tweet_ordering/indolem_tweet_ordering.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_gsd/indolem_ud_id_gsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indolem_ud_id_pud/indolem_ud_id_pud.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indoler/indoler.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indoler/indoler.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indommlu/indommlu.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indommlu/indommlu.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indoner_tourism/indoner_tourism.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonesia_chinese_mtrobusteval/indonesia_chinese_mtrobusteval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_madurese_bible_translation/indonesian_madurese_bible_translation.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonesian_news_dataset/indonesian_news_dataset.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonesiannmt/indonesiannmt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonglish/indonglish.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonglish/indonglish.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonli/indonli.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonli/indonli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indonlu_nergrit/indonlu_nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indoqa/indoqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indoqa/indoqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indosmd/indosmd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indosmd/indosmd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indosum/indosum.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indosum/indosum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indotacos/indotacos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indotacos/indotacos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indowiki/indowiki.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indowiki/indowiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indqner/indqner.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indqner/indqner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_digit_cdsr/indspeech_digit_cdsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_ethnicsr/indspeech_news_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_lvcsr/indspeech_news_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_news_tts/indspeech_news_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_newstra_ethnicsr/indspeech_newstra_ethnicsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_lvcsr/indspeech_teldialog_lvcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/indspeech_teldialog_svcsr/indspeech_teldialog_svcsr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/inset_lexicon/inset_lexicon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/jadi_ide/jadi_ide.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/jadi_ide/jadi_ide.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_asr/jv_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/jv_id_tts/jv_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kamus_alay/kamus_alay.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kamus_alay/kamus_alay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/karonese_sentiment/karonese_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kawat/kawat.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kawat/kawat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kde4/kde4.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kde4/kde4.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/keps/keps.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/keps/keps.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kheng_info/kheng_info.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kheng_info/kheng_info.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/khmer_alt_pos/khmer_alt_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/khpos/khpos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/khpos/khpos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc/kopi_cc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc/kopi_cc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kopi_cc_news/kopi_cc_news.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/kopi_nllb/kopi_nllb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/korpus_nusantara/korpus_nusantara.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/lazada_review_filipino/lazada_review_filipino.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/librivox_indonesia/librivox_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/limesoda/limesoda.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/limesoda/limesoda.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/liputan6/liputan6.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/liputan6/liputan6.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/local_id_abusive/local_id_abusive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/lr_sum/lr_sum.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/lr_sum/lr_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/m3exam/m3exam.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/m3exam/m3exam.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mabl/mabl.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mabl/mabl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/malaysia_tweets/malaysia_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/malindo_morph/malindo_morph.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/malindo_morph/malindo_morph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/malindo_parallel/malindo_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/massive/massive.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/massive/massive.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mc4_indo/mc4_indo.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mc4_indo/mc4_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/melayu_brunei/melayu_brunei.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sabah/melayu_sabah.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/melayu_sarawak/melayu_sarawak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/melayu_standard_lisan/melayu_standard_lisan.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/memolon/memolon.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/memolon/memolon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/minangnlp_mt/minangnlp_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/miracl/miracl.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/miracl/miracl.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mkqa/mkqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mkqa/mkqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mlqa/mlqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mlqa/mlqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mozilla_pontoon/mozilla_pontoon.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mswc/mswc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mswc/mswc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mtop_intent_classification/labels.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mtop_intent_classification/labels.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mtop_intent_classification/mtop_intent_classification.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/multilexnorm/multilexnorm.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/multilexnorm/multilexnorm.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/my_paraphrase/my_paraphrase.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/myanmar_rakhine_parallel/myanmar_rakhine_parallel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mypos/mypos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mypos/mypos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/mysentence/mysentence.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/mysentence/mysentence.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/myxnli/myxnli.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/myxnli/myxnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nergrit/nergrit.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nergrit/nergrit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nerp/nerp.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nerp/nerp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/netifier/netifier.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/netifier/netifier.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/news_en_id/news_en_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/news_en_id/news_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/newsph/newsph.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/newsph/newsph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nllb_seed/nllb_seed.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nllb_seed/nllb_seed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ntrex_128/ntrex_128.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ntrex_128/ntrex_128.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_emot/nusaparagraph_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_rhetoric/nusaparagraph_rhetoric.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusaparagraph_topic/nusaparagraph_topic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_emot/nusatranslation_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_mt/nusatranslation_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusatranslation_senti/nusatranslation_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusax_mt/nusax_mt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusax_mt/nusax_mt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/nusax_senti/nusax_senti.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/nusax_senti/nusax_senti.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/oil/oil.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/oil/oil.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ojw/ojw.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ojw/ojw.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/openlid/openlid.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/openlid/openlid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/openslr/openslr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/openslr/openslr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/orchid_pos/orchid_pos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/orchid_pos/orchid_pos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/oscar_2201/oscar_2201.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/oscar_2201/oscar_2201.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/palito/palito.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/palito/palito.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/paracotta_id/paracotta_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/paracotta_id/paracotta_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/parallel_id_nyo/parallel_id_nyo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/parallel_su_id/parallel_su_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ph_fake_news_corpus/ph_fake_news_corpus.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/pho_ner_covid/pho_ner_covid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/phomt/phomt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/phomt/phomt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/phost/phost.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/phost/phost.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/posp/posp.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/posp/posp.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/postag_su/postag_su.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/postag_su/postag_su.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/prdect_id/prdect_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/prdect_id/prdect_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/qasina/qasina.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/qasina/qasina.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/roots_vi_ted/roots_vi_ted.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sampiran/sampiran.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sampiran/sampiran.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sap_wat/sap_wat.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sap_wat/sap_wat.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sarawak_malay/sarawak_malay.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/scb_mt_en_th/scb_mt_en_th.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sea_bench/sea_bench.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sea_bench/sea_bench.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sea_madlad/sea_madlad.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sea_madlad/sea_madlad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sea_wiki/lang_config.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sea_wiki/lang_config.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sea_wiki/sea_wiki.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sea_wiki/sea_wiki.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/seaeval/seaeval.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/seaeval/seaeval.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/seahorse/seahorse.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/seahorse/seahorse.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/sentiment_nathasa_review/sentiment_nathasa_review.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/shopee_reviews_tagalog/shopee_reviews_tagalog.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/singgalang/singgalang.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/singgalang/singgalang.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/smsa/smsa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/smsa/smsa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/snli_indo/snli_indo.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/snli_indo/snli_indo.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/spamid_pair/spamid_pair.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/spamid_pair/spamid_pair.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/squad_id/squad_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/squad_id/squad_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/stb_ext/stb_ext.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/stb_ext/stb_ext.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/stif_indonesia/stif_indonesia.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/struct_amb_ind/struct_amb_ind.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/su_emot/su_emot.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/su_emot/su_emot.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/su_id_asr/su_id_asr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/su_id_asr/su_id_asr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/su_id_tts/su_id_tts.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/su_id_tts/su_id_tts.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/talpco/talpco.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/talpco/talpco.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tatabahasa/tatabahasa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tatabahasa/tatabahasa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tatoeba/tatoeba.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tatoeba/tatoeba.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tcope/tcope.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tcope/tcope.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ted_en_id/ted_en_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ted_en_id/ted_en_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/term_a/term_a.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/term_a/term_a.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tgl_profanity/tgl_profanity.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tha_lao_embassy_parcor/tha_lao_embassy_parcor.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_alpaca/thai_alpaca.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_constitution/thai_constitution.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_constitution/thai_constitution.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_databricks_dolly/thai_databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_depression/thai_depression.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_depression/thai_depression.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_gpteacher/thai_gpteacher.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_hh_rlhf/thai_hh_rlhf.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_sum/thai_sum.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_sum/thai_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/thai_toxicity_tweet/thai_toxicity_tweet.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tico_19/tico_19.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tico_19/tico_19.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/titml_idn/titml_idn.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/titml_idn/titml_idn.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tlunified_ner/tlunified_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/toxicity_200/toxicity_200.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/toxicity_200/toxicity_200.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/tydiqa/tydiqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/tydiqa/tydiqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/typhoon_yolanda_tweets/typhoon_yolanda_tweets.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ucla_phonetic/ucla_phonetic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ud_id_csui/ud_id_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/ud_jv_csui/ud_jv_csui.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/udhr/udhr.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/udhr/udhr.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/udhr_lid/udhr_lid.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/udhr_lid/udhr_lid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_vicov19qa/uit_vicov19qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_victsd/uit_victsd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_victsd/uit_victsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_vihsd/uit_vihsd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_viic/uit_viic.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_viic/uit_viic.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_viocd/uit_viocd.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_viocd/uit_viocd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_vion/uit_vion.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_vion/uit_vion.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_visd4sa/uit_visd4sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsfc/uit_vsfc.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/uit_vsmec/uit_vsmec.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/unimorph/unimorph.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/unimorph/unimorph.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/unimorph_id/unimorph_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/unimorph_id/unimorph_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vi_pubmed/vi_pubmed.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vihealthqa/vihealthqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vihealthqa/vihealthqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/visobert/visobert.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/visobert/visobert.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vispamreviews/vispamreviews.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vispamreviews/vispamreviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vistec_tp_th_21/vistec_tp_th_21.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vitext2sql/vitext2sql.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vitext2sql/vitext2sql.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vivos/vivos.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vivos/vivos.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vivqa/vivqa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vivqa/vivqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_ner/vlsp2016_ner.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vlsp2016_sa/vlsp2016_sa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vndt/utils.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vndt/utils.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/vndt/vndt.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/vndt/vndt.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/voxlingua/voxlingua.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/voxlingua/voxlingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/weathub/weathub.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/weathub/weathub.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wikiann/wikiann.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wikiann/wikiann.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wikilingua/wikilingua.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wikilingua/wikilingua.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wikimatrix/wikimatrix.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wikimatrix/wikimatrix.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wikitext_tl_39/wikitext_tl_39.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wili_2018/wili_2018.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wili_2018/wili_2018.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wisesight_thai_sentiment/wisesight_thai_sentiment.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wit/wit.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wit/wit.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wongnai_reviews/wongnai_reviews.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/wrete/wrete.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/wrete/wrete.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/x_fact/x_fact.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/x_fact/x_fact.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xcopa/xcopa.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xcopa/xcopa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xl_jailbreak/xl_jailbreak.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xl_sum/xl_sum.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xl_sum/xl_sum.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xm3600/xm3600.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xm3600/xm3600.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xnli/xnli.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xnli/xnli.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xpersona_id/xpersona_id.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xpersona_id/xpersona_id.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xquad/xquad.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xquad/xquad.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xsid/xsid.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xsid/xsid.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/xstorycloze/xstorycloze.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/xstorycloze/xstorycloze.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py` & `seacrowd-0.0.9/seacrowd/sea_datasets/yunshan_cup_2020/yunshan_cup_2020.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/common_parser.py` & `seacrowd-0.0.9/seacrowd/utils/common_parser.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/constants.py` & `seacrowd-0.0.9/seacrowd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/__init__.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/imqa.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/imqa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/kb.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/kb.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/pairs.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/pairs.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/qa.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/qa.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/seq_label.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/seq_label.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/speech.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/speech_multilabel.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/speech_multilabel.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/speech_to_speech.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/speech_to_speech.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/tod.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/tod.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/tree.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/tree.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd/utils/schemas/video.py` & `seacrowd-0.0.9/seacrowd/utils/schemas/video.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/seacrowd.egg-info/PKG-INFO` & `seacrowd-0.0.9/seacrowd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seacrowd
-Version: 0.0.8
+Version: 0.0.9
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: loguru>=0.5.3
 Requires-Dist: bioc>=1.3.7
 Requires-Dist: pandas>=1.3.3
 Requires-Dist: numpy>=1.20
 Requires-Dist: datasets>=2.2.0
```

### Comparing `seacrowd-0.0.8/seacrowd.egg-info/SOURCES.txt` & `seacrowd-0.0.9/seacrowd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/setup.cfg` & `seacrowd-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/tests/test_seacrowd.py` & `seacrowd-0.0.9/tests/test_seacrowd.py`

 * *Files identical despite different names*

### Comparing `seacrowd-0.0.8/tests/test_seacrowd_source_only.py` & `seacrowd-0.0.9/tests/test_seacrowd_source_only.py`

 * *Files identical despite different names*

