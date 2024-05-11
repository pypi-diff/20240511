# Comparing `tmp/mteb-1.8.7.tar.gz` & `tmp/mteb-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.8.7.tar", last modified: Thu May  9 16:47:02 2024, max compression
+gzip compressed data, was "mteb-1.8.8.tar", last modified: Sat May 11 09:52:28 2024, max compression
```

## Comparing `mteb-1.8.7.tar` & `mteb-1.8.8.tar`

### file list

```diff
@@ -1,1224 +1,1244 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.317839 mteb-1.8.7/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-09 16:46:57.000000 mteb-1.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)    24072 2024-05-09 16:47:02.317839 mteb-1.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9642 2024-05-09 16:46:57.000000 mteb-1.8.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.113839 mteb-1.8.7/docs/
--rw-r--r--   0 root         (0) root         (0)     2651 2024-05-09 16:46:57.000000 mteb-1.8.7/docs/create_tasks_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.113839 mteb-1.8.7/docs/mmteb/
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-09 16:46:57.000000 mteb-1.8.7/docs/mmteb/create_points_table.py
--rw-r--r--   0 root         (0) root         (0)     2108 2024-05-09 16:46:57.000000 mteb-1.8.7/docs/mmteb/validate_points.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.113839 mteb-1.8.7/mteb/
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.117839 mteb-1.8.7/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     6404 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5876 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2410 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     7433 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskClusteringFast.py
--rw-r--r--   0 root         (0) root         (0)    24968 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskInstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    13422 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1897 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/MultiSubsetLoader.py
--rw-r--r--   0 root         (0) root         (0)      653 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)    10404 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      465 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7082 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/iso_15924_to_script.json
--rw-r--r--   0 root         (0) root         (0)   193114 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/iso_639_3_to_language.json
--rw-r--r--   0 root         (0) root         (0)      541 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/abstasks/languages.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/benchmarks.py
--rw-r--r--   0 root         (0) root         (0)     5225 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/cmd.py
--rw-r--r--   0 root         (0) root         (0)     1702 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/encoder_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.117839 mteb-1.8.7/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13258 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.121839 mteb-1.8.7/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5840 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8927 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     7126 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9554 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    19805 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7965 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      820 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/logging.py
--rw-r--r--   0 root         (0) root         (0)     6530 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/overview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.093839 mteb-1.8.7/mteb/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.121839 mteb-1.8.7/mteb/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.121839 mteb-1.8.7/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.121839 mteb-1.8.7/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.121839 mteb-1.8.7/mteb/tasks/BitextMining/dan/
--rw-r--r--   0 root         (0) root         (0)     2246 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.121839 mteb-1.8.7/mteb/tasks/BitextMining/kat/
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/kat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.125839 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)    29308 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2263 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5951 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     4585 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     3552 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
--rw-r--r--   0 root         (0) root         (0)    13482 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1423 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1830 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5733 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1363 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.125839 mteb-1.8.7/mteb/tasks/BitextMining/srn/
--rw-r--r--   0 root         (0) root         (0)     2610 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/srn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.125839 mteb-1.8.7/mteb/tasks/BitextMining/vie/
--rw-r--r--   0 root         (0) root         (0)     2889 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/BitextMining/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.125839 mteb-1.8.7/mteb/tasks/CLSD/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.125839 mteb-1.8.7/mteb/tasks/CLSD/WMT1921/
--rw-r--r--   0 root         (0) root         (0)     4878 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py
--rw-r--r--   0 root         (0) root         (0)     4878 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/CLSD/WMT1921/__init__.py
--rw-r--r--   0 root         (0) root         (0)      162 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/CLSD/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.125839 mteb-1.8.7/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     5167 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.129839 mteb-1.8.7/mteb/tasks/Classification/ara/
--rw-r--r--   0 root         (0) root         (0)     1598 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ara/AJGT.py
--rw-r--r--   0 root         (0) root         (0)     1719 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1907 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ara/TweetEmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)     3161 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ara/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.129839 mteb-1.8.7/mteb/tasks/Classification/ben/
--rw-r--r--   0 root         (0) root         (0)     2122 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ben/BengaliDocumentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ben/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.129839 mteb-1.8.7/mteb/tasks/Classification/bul/
--rw-r--r--   0 root         (0) root         (0)     1947 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/bul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.129839 mteb-1.8.7/mteb/tasks/Classification/ces/
--rw-r--r--   0 root         (0) root         (0)     1704 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.129839 mteb-1.8.7/mteb/tasks/Classification/dan/
--rw-r--r--   0 root         (0) root         (0)     1750 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/dan/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     4348 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/dan/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2943 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     2435 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/dan/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/dan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.133839 mteb-1.8.7/mteb/tasks/Classification/deu/
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.133839 mteb-1.8.7/mteb/tasks/Classification/ell/
--rw-r--r--   0 root         (0) root         (0)     2172 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/eng/
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/ArxivClassification.py
--rw-r--r--   0 root         (0) root         (0)     1054 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     2072 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/DBpediaClassification.py
--rw-r--r--   0 root         (0) root         (0)     1374 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1735 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/FrenkEnClassification.py
--rw-r--r--   0 root         (0) root         (0)      990 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)   212918 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/LegalBenchClassification.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/NewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3186 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/PatentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2842 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/ToxicChatClassification.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1281 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)     2290 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/YelpReviewFullClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/est/
--rw-r--r--   0 root         (0) root         (0)     2407 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/est/estonian_valence.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/fas/
--rw-r--r--   0 root         (0) root         (0)     1714 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/fil/
--rw-r--r--   0 root         (0) root         (0)     1925 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
--rw-r--r--   0 root         (0) root         (0)     2040 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fil/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/fin/
--rw-r--r--   0 root         (0) root         (0)     2562 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fin/FinToxicityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/fra/
--rw-r--r--   0 root         (0) root         (0)     1468 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fra/FrenchBookReviews.py
--rw-r--r--   0 root         (0) root         (0)     1777 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/guj/
--rw-r--r--   0 root         (0) root         (0)     1285 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/guj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/hin/
--rw-r--r--   0 root         (0) root         (0)     2242 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/hin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.137839 mteb-1.8.7/mteb/tasks/Classification/hrv/
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/hrv/FrenkHrClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/hrv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/ind/
--rw-r--r--   0 root         (0) root         (0)     2928 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
--rw-r--r--   0 root         (0) root         (0)     3829 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ind/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/ita/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ita/ItaCaseholdClassification.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ita/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/jav/
--rw-r--r--   0 root         (0) root         (0)     1871 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/jav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/jpn/
--rw-r--r--   0 root         (0) root         (0)     3402 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/jpn/WRIMEClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/kan/
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kan/KannadaNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/kat/
--rw-r--r--   0 root         (0) root         (0)     3016 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/kor/
--rw-r--r--   0 root         (0) root         (0)     2428 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kor/KlueTC.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/kur/
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/kur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/mal/
--rw-r--r--   0 root         (0) root         (0)     1293 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/mal/MalayalamNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/mal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.141839 mteb-1.8.7/mteb/tasks/Classification/mkd/
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/mkd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.145839 mteb-1.8.7/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1377 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3360 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py
--rw-r--r--   0 root         (0) root         (0)     2638 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/HinDialectClassification.py
--rw-r--r--   0 root         (0) root         (0)     5163 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/IndicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     3286 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/LanguageClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1627 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     2537 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     6431 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MultiHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     3839 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1586 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     8376 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/SIB200Classification.py
--rw-r--r--   0 root         (0) root         (0)     2956 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py
--rw-r--r--   0 root         (0) root         (0)     3264 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/nep/
--rw-r--r--   0 root         (0) root         (0)     2770 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nep/NepaliNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nep/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/nld/
--rw-r--r--   0 root         (0) root         (0)     1751 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/nob/
--rw-r--r--   0 root         (0) root         (0)     1121 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nob/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1173 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/nob/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/ory/
--rw-r--r--   0 root         (0) root         (0)     1306 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ory/OdiaNewsClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/pan/
--rw-r--r--   0 root         (0) root         (0)     1336 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/pan/PunjabiNewsClassification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/pol/
--rw-r--r--   0 root         (0) root         (0)     4922 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/pol/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/por/
--rw-r--r--   0 root         (0) root         (0)     2307 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/por/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/ron/
--rw-r--r--   0 root         (0) root         (0)     1579 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ron/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/san/
--rw-r--r--   0 root         (0) root         (0)     2851 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/san/SanskritShlokasClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/san/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/sin/
--rw-r--r--   0 root         (0) root         (0)     2271 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/sin/SinhalaNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/sin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.149839 mteb-1.8.7/mteb/tasks/Classification/slv/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/slv/FrenkSlClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/slv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/spa/
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/spa/SpanishNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     2218 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/spa/SpanishSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/ssw/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ssw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/swe/
--rw-r--r--   0 root         (0) root         (0)     2834 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/swe/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/swe/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/swe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/tam/
--rw-r--r--   0 root         (0) root         (0)     1408 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tam/TamilNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/tel/
--rw-r--r--   0 root         (0) root         (0)     1382 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/tha/
--rw-r--r--   0 root         (0) root         (0)     2106 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tha/WisesightSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/tsn/
--rw-r--r--   0 root         (0) root         (0)     1760 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tsn/TswanaNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tsn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/tur/
--rw-r--r--   0 root         (0) root         (0)     1640 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1493 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/tur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.153839 mteb-1.8.7/mteb/tasks/Classification/ukr/
--rw-r--r--   0 root         (0) root         (0)     2485 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ukr/UkrFormalityClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/ukr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.157839 mteb-1.8.7/mteb/tasks/Classification/urd/
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/urd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.157839 mteb-1.8.7/mteb/tasks/Classification/vie/
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.157839 mteb-1.8.7/mteb/tasks/Classification/zho/
--rw-r--r--   0 root         (0) root         (0)     6571 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/zho/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)     1883 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.157839 mteb-1.8.7/mteb/tasks/Classification/zul/
--rw-r--r--   0 root         (0) root         (0)     1632 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Classification/zul/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.157839 mteb-1.8.7/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1644 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.157839 mteb-1.8.7/mteb/tasks/Clustering/deu/
--rw-r--r--   0 root         (0) root         (0)     1179 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1984 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1477 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1453 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.161839 mteb-1.8.7/mteb/tasks/Clustering/eng/
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1061 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1135 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.161839 mteb-1.8.7/mteb/tasks/Clustering/fra/
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1739 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1607 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/fra/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3055 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     3202 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     2687 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2701 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1676 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3442 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/nob/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/nob/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/pol/
--rw-r--r--   0 root         (0) root         (0)     3352 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/pol/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/rom/
--rw-r--r--   0 root         (0) root         (0)     1089 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/spa/
--rw-r--r--   0 root         (0) root         (0)     1042 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/swe/
--rw-r--r--   0 root         (0) root         (0)     4765 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/swe/SwednClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4094 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/swe/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/Clustering/zho/
--rw-r--r--   0 root         (0) root         (0)     3639 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/zho/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Clustering/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/InstructionRetrieval/
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/InstructionRetrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1547 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1547 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1556 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.165839 mteb-1.8.7/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/PairClassification/deu/
--rw-r--r--   0 root         (0) root         (0)     2862 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/PairClassification/eng/
--rw-r--r--   0 root         (0) root         (0)     4517 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/eng/LegalBenchPC.py
--rw-r--r--   0 root         (0) root         (0)     1152 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/PairClassification/hye/
--rw-r--r--   0 root         (0) root         (0)     1439 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/hye/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2780 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)     5117 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/multilingual/XNLI.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/PairClassification/pol/
--rw-r--r--   0 root         (0) root         (0)     3577 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/pol/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/PairClassification/zho/
--rw-r--r--   0 root         (0) root         (0)     1849 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/PairClassification/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.169839 mteb-1.8.7/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Reranking/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/eng/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     3054 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/eng/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1137 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Reranking/fra/
--rw-r--r--   0 root         (0) root         (0)     1195 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/fra/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/fra/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1269 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Reranking/zho/
--rw-r--r--   0 root         (0) root         (0)     3528 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/zho/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Reranking/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     3751 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Retrieval/code/
--rw-r--r--   0 root         (0) root         (0)     3275 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3377 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/code/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.173839 mteb-1.8.7/mteb/tasks/Retrieval/dan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/dan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/dan/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2574 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3139 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/dan/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.177839 mteb-1.8.7/mteb/tasks/Retrieval/deu/
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1228 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2891 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.177839 mteb-1.8.7/mteb/tasks/Retrieval/ell/
--rw-r--r--   0 root         (0) root         (0)     2683 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/ell/GreekCivicsQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/ell/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/eng/
--rw-r--r--   0 root         (0) root         (0)     1118 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1077 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1056 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1074 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1031 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1175 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      983 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3668 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1151 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3022 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3648 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3641 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2526 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1146 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1039 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     1650 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1991 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1114 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1046 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/est/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/est/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/est/estqa.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/fra/
--rw-r--r--   0 root         (0) root         (0)     2144 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3184 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2148 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/hun/
--rw-r--r--   0 root         (0) root         (0)     2589 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/hun/HunSum2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/jpn/
--rw-r--r--   0 root         (0) root         (0)     2853 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/kat/
--rw-r--r--   0 root         (0) root         (0)     2568 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/kat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.185839 mteb-1.8.7/mteb/tasks/Retrieval/kor/
--rw-r--r--   0 root         (0) root         (0)      906 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/kor/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/kor/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.189839 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3776 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3277 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     6239 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3432 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3731 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3771 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3145 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     4217 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.189839 mteb-1.8.7/mteb/tasks/Retrieval/nob/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/nob/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3943 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/nob/norquad.py
--rw-r--r--   0 root         (0) root         (0)     2699 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/nob/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/pol/
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      984 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1091 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/slk/
--rw-r--r--   0 root         (0) root         (0)     2891 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/slk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/spa/
--rw-r--r--   0 root         (0) root         (0)     2125 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2056 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/swe/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/swe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/swe/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     2610 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/tur/
--rw-r--r--   0 root         (0) root         (0)     3883 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/tur/TurHistQuad.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/tur/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/vie/
--rw-r--r--   0 root         (0) root         (0)     3798 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/vie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/Retrieval/zho/
--rw-r--r--   0 root         (0) root         (0)    10384 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Retrieval/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      787 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.193839 mteb-1.8.7/mteb/tasks/STS/deu/
--rw-r--r--   0 root         (0) root         (0)     1370 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/deu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/eng/
--rw-r--r--   0 root         (0) root         (0)     1184 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1184 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1148 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1208 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/fao/
--rw-r--r--   0 root         (0) root         (0)     2015 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/fao/FaroeseSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/fin/
--rw-r--r--   0 root         (0) root         (0)     3422 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/fin/FinParaSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/fin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/fra/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/fra/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/fra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/jpn/
--rw-r--r--   0 root         (0) root         (0)     3034 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/jpn/JSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/kor/
--rw-r--r--   0 root         (0) root         (0)     2504 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/kor/KlueSTS.py
--rw-r--r--   0 root         (0) root         (0)     1634 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/kor/KorSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/kor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.197839 mteb-1.8.7/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     4131 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1600 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2712 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/STS/pol/
--rw-r--r--   0 root         (0) root         (0)     2268 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/pol/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/pol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/STS/ron/
--rw-r--r--   0 root         (0) root         (0)     1896 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/ron/RonSTS.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/STS/spa/
--rw-r--r--   0 root         (0) root         (0)     1486 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/spa/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/spa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/STS/zho/
--rw-r--r--   0 root         (0) root         (0)     7122 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/zho/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/STS/zho/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/Summarization/eng/
--rw-r--r--   0 root         (0) root         (0)     1243 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Summarization/eng/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Summarization/eng/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/mteb/tasks/Summarization/fra/
--rw-r--r--   0 root         (0) root         (0)     1304 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/Summarization/fra/__init__.py
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-09 16:46:57.000000 mteb-1.8.7/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.317839 mteb-1.8.7/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    24072 2024-05-09 16:47:02.000000 mteb-1.8.7/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    71806 2024-05-09 16:47:02.000000 mteb-1.8.7/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 16:47:02.000000 mteb-1.8.7/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-05-09 16:47:02.000000 mteb-1.8.7/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      258 2024-05-09 16:47:02.000000 mteb-1.8.7/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-09 16:47:02.000000 mteb-1.8.7/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2752 2024-05-09 16:46:58.000000 mteb-1.8.7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.109839 mteb-1.8.7/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/results/GritLM__GritLM-7B/
--rw-r--r--   0 root         (0) root         (0)     2342 2024-05-09 16:46:57.000000 mteb-1.8.7/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.201839 mteb-1.8.7/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/
--rw-r--r--   0 root         (0) root         (0)     1154 2024-05-09 16:46:57.000000 mteb-1.8.7/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.109839 mteb-1.8.7/results/dangvantuan/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.205839 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      250 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      634 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      305 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
--rw-r--r--   0 root         (0) root         (0)      676 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
--rw-r--r--   0 root         (0) root         (0)      332 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      335 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
--rw-r--r--   0 root         (0) root         (0)      679 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2992 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)     2801 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      820 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/SICKFr.json
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/STS22.json
--rw-r--r--   0 root         (0) root         (0)      921 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
--rw-r--r--   0 root         (0) root         (0)      221 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
--rw-r--r--   0 root         (0) root         (0)     1099 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1245 2024-05-09 16:46:57.000000 mteb-1.8.7/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.109839 mteb-1.8.7/results/intfloat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.209839 mteb-1.8.7/results/intfloat/multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/HinDialectClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      366 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      367 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/TamilNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat/multilingual-e5-small/TswanaNewsClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.209839 mteb-1.8.7/results/intfloat__e5-small/
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__e5-small/TurkishProductSentimentClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.209839 mteb-1.8.7/results/intfloat__e5-small-v2/
--rw-r--r--   0 root         (0) root         (0)     2512 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2540 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     2550 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.213839 mteb-1.8.7/results/intfloat__multilingual-e5-base/
--rw-r--r--   0 root         (0) root         (0)      758 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     2281 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json
--rw-r--r--   0 root         (0) root         (0)     2293 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json
--rw-r--r--   0 root         (0) root         (0)      733 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      757 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-base/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.257839 mteb-1.8.7/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/AJGT.json
--rw-r--r--   0 root         (0) root         (0)      375 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/AfriSentiLangClassification.json
--rw-r--r--   0 root         (0) root         (0)     1422 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ArxivClassification.json
--rw-r--r--   0 root         (0) root         (0)      517 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json
--rw-r--r--   0 root         (0) root         (0)     1161 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BSARDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BengaliDocumentClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BengaliSentimentAnalysis.json
--rw-r--r--   0 root         (0) root         (0)   336719 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1081 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicensorLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADAntiAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADAuditRightsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADCapOnLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADChangeOfControlLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADCovenantNotToSueLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADEffectiveDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADExclusivityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADExpirationDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADGoverningLawLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADIPOwnershipAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      468 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADInsuranceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADJointIPOwnershipLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADLicenseGrantLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADLiquidatedDamagesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADMinimumCommitmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      396 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADMostFavoredNationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADNoSolicitOfCustomersLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADNoSolicitOfEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADNonCompeteLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      424 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADNonDisparagementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADNonTransferableLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADPostTerminationServicesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADPriceRestrictionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADRenewalTermLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      461 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADRevenueProfitSharingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADRofrRofoRofnLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADSourceCodeEscrowLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADTerminationForConvenienceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADThirdPartyBeneficiaryLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADUncappedLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADVolumeRestrictionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CUADWarrantyDurationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CanadaTaxCourtOutcomesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      616 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json
--rw-r--r--   0 root         (0) root         (0)    13681 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     5524 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIExplicitIdentificationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      483 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLILimitedUseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLINoLicensingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      492 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      422 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIPermissibleCopyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      461 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLISharingWithEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ContractNLISurvivalOfObligationsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CorporateLobbyingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     2305 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json
--rw-r--r--   0 root         (0) root         (0)     2309 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json
--rw-r--r--   0 root         (0) root         (0)      738 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/DBpediaClassification.json
--rw-r--r--   0 root         (0) root         (0)     1016 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      463 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2105 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FaroeseSTS.json
--rw-r--r--   0 root         (0) root         (0)      733 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      827 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FinParaSTS.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FinToxicityClassification.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FinancialPhrasebankClassification.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FrenchBookReviews.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FrenkEnClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FrenkHrClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/FrenkSlClassification.json
--rw-r--r--   0 root         (0) root         (0)     1168 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GeorgianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GermanDPR.json
--rw-r--r--   0 root         (0) root         (0)      401 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GermanPoliticiansTwitterSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GreekCivicsQA.json
--rw-r--r--   0 root         (0) root         (0)      606 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/HateSpeechPortugueseClassification.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1289 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      604 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     4319 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)    11798 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     4273 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     3924 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      644 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/InternationalCitizenshipQuestionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ItaCaseholdClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      429 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/JCrewBlockerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/JavaneseIMDBClassification.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/KLUE-TC.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/KannadaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1163 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7814 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7703 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1169 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LanguageClassification.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsBenefitsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsBusinessLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      437 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsConsumerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsCourtsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsCrimeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsDivorceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsDomesticViolenceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsEducationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsEmploymentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsEstatesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsFamilyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsHealthLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsHousingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsImmigrationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsTortsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LearnedHandsTrafficLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     1411 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LegalBenchPC.json
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/LegalReasoningCausalityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     2360 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MLQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     3894 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      749 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3151 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MultiHateClassification.json
--rw-r--r--   0 root         (0) root         (0)     8513 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)   417235 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NTREXBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NepaliNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     3386 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3392 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NordicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/PatentClassification.json
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      513 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/PunjabiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      403 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)    42700 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SIB200Classification.json
--rw-r--r--   0 root         (0) root         (0)      298 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      584 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      592 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SentimentAnalysisHindi.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SinhalaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SinhalaNewsSourceClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      453 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SlovakSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      375 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SpanishNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SpanishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1015 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      304 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)      893 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      524 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1023 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1062 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json
--rw-r--r--   0 root         (0) root         (0)     1116 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      629 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      522 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/ToxicConversationsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1166 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      459 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TurkishProductSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1827 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TweetTopicSingleClassification.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/UrduRomanSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1028 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      368 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)     2184 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/WisesightSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)    38759 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/XNLI.json
--rw-r--r--   0 root         (0) root         (0)    13972 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/XNLI2.json
--rw-r--r--   0 root         (0) root         (0)    12839 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/XQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-09 16:46:57.000000 mteb-1.8.7/results/intfloat__multilingual-e5-small/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.109839 mteb-1.8.7/results/sentence-transformers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.257839 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      364 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)    21290 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
--rw-r--r--   0 root         (0) root         (0)    21291 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TswanaNewsClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.261839 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
--rw-r--r--   0 root         (0) root         (0)      340 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)   387673 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1014 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      306 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      302 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/model.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.305839 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AJGT.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AfriSentiLangClassification.json
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json
--rw-r--r--   0 root         (0) root         (0)      355 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClassification.json
--rw-r--r--   0 root         (0) root         (0)      520 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json
--rw-r--r--   0 root         (0) root         (0)     1160 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1001 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliDocumentClassification.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliSentimentAnalysis.json
--rw-r--r--   0 root         (0) root         (0)   338028 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1086 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1088 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      344 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      398 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
--rw-r--r--   0 root         (0) root         (0)      462 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicensorLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAntiAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAuditRightsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCapOnLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADChangeOfControlLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCovenantNotToSueLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADEffectiveDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      431 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExclusivityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExpirationDateLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADGoverningLawLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIPOwnershipAssignmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADInsuranceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADJointIPOwnershipLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLicenseGrantLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLiquidatedDamagesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMinimumCommitmentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMostFavoredNationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      411 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfCustomersLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonCompeteLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonDisparagementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonTransferableLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      444 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPostTerminationServicesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPriceRestrictionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRenewalTermLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRevenueProfitSharingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRofrRofoRofnLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADSourceCodeEscrowLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      397 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADTerminationForConvenienceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADThirdPartyBeneficiaryLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUncappedLiabilityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADVolumeRestrictionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      398 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADWarrantyDurationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      387 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CanadaTaxCourtOutcomesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json
--rw-r--r--   0 root         (0) root         (0)    13663 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     5535 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      472 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIExplicitIdentificationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      414 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLILimitedUseLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      439 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoLicensingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleCopyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      426 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithEmployeesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISurvivalOfObligationsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CorporateLobbyingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     2340 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json
--rw-r--r--   0 root         (0) root         (0)     2295 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DBpediaClassification.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
--rw-r--r--   0 root         (0) root         (0)     2108 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FaroeseSTS.json
--rw-r--r--   0 root         (0) root         (0)      746 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      835 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinToxicityClassification.json
--rw-r--r--   0 root         (0) root         (0)      389 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinancialPhrasebankClassification.json
--rw-r--r--   0 root         (0) root         (0)      291 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenchBookReviews.json
--rw-r--r--   0 root         (0) root         (0)      443 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkEnClassification.json
--rw-r--r--   0 root         (0) root         (0)      445 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkHrClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkSlClassification.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
--rw-r--r--   0 root         (0) root         (0)      405 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GermanPoliticiansTwitterSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1157 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HateSpeechPortugueseClassification.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1317 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     4370 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)    11833 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     4276 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     3921 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      456 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InternationalCitizenshipQuestionsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      342 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaCaseholdClassification.json
--rw-r--r--   0 root         (0) root         (0)      430 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JCrewBlockerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JavaneseIMDBClassification.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
--rw-r--r--   0 root         (0) root         (0)      358 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-TC.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KannadaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      470 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1167 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7839 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     7915 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1153 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1152 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LanguageClassification.json
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBenefitsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      418 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBusinessLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsConsumerLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCourtsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCrimeLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDivorceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      425 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDomesticViolenceLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      412 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEducationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      419 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEmploymentLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      436 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEstatesLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsFamilyLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHealthLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHousingLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsImmigrationLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTortsLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTrafficLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)     1454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalReasoningCausalityLegalBenchClassification.json
--rw-r--r--   0 root         (0) root         (0)   104611 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)     3877 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)     3884 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      394 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
--rw-r--r--   0 root         (0) root         (0)      748 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     3151 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json
--rw-r--r--   0 root         (0) root         (0)     1332 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json
--rw-r--r--   0 root         (0) root         (0)     8537 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)   421556 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      365 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NepaliNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     3382 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
--rw-r--r--   0 root         (0) root         (0)     3376 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NordicLangClassification.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
--rw-r--r--   0 root         (0) root         (0)    16669 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PatentClassification.json
--rw-r--r--   0 root         (0) root         (0)    18247 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
--rw-r--r--   0 root         (0) root         (0)      741 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      517 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      448 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PunjabiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      452 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      308 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
--rw-r--r--   0 root         (0) root         (0)      441 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      471 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
--rw-r--r--   0 root         (0) root         (0)    42635 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
--rw-r--r--   0 root         (0) root         (0)     1011 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SentimentAnalysisHindi.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsSourceClassification.json
--rw-r--r--   0 root         (0) root         (0)      380 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1149 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishNewsClassification.json
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)     1021 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      303 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      523 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)     1022 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
--rw-r--r--   0 root         (0) root         (0)      637 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json
--rw-r--r--   0 root         (0) root         (0)      605 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json
--rw-r--r--   0 root         (0) root         (0)      523 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicChatClassification.json
--rw-r--r--   0 root         (0) root         (0)      447 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicConversationsClassification.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      451 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      440 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      373 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
--rw-r--r--   0 root         (0) root         (0)      450 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
--rw-r--r--   0 root         (0) root         (0)     1822 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetTopicSingleClassification.json
--rw-r--r--   0 root         (0) root         (0)     1035 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UrduRomanSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
--rw-r--r--   0 root         (0) root         (0)      351 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      370 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
--rw-r--r--   0 root         (0) root         (0)     2186 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
--rw-r--r--   0 root         (0) root         (0)      384 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WisesightSentimentClassification.json
--rw-r--r--   0 root         (0) root         (0)    38547 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json
--rw-r--r--   0 root         (0) root         (0)    13842 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI2.json
--rw-r--r--   0 root         (0) root         (0)    12890 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YahooAnswersTopicsClassification.json
--rw-r--r--   0 root         (0) root         (0)      378 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YelpReviewFullClassification.json
--rw-r--r--   0 root         (0) root         (0)      377 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
--rw-r--r--   0 root         (0) root         (0)      176 2024-05-09 16:46:57.000000 mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5924 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2133 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.309839 mteb-1.8.7/scripts/data/medicalqaretrieval/
--rw-r--r--   0 root         (0) root         (0)     1884 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/medicalqaretrieval/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/multilingual_sentiment_classification/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/multilingual_sentiment_classification/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/scala_classification/
--rw-r--r--   0 root         (0) root         (0)      475 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/scala_classification/create_multiling_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2435 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/toxic_conversations_50k/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/data/xnli2/
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/data/xnli2/create_multilang_ds.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/mteb_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.109839 mteb-1.8.7/scripts/results/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/results/intfloat__multilingual-e5-small/
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.313839 mteb-1.8.7/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
--rw-r--r--   0 root         (0) root         (0)      673 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1334 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1017 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_law.py
--rw-r--r--   0 root         (0) root         (0)     1141 2024-05-09 16:46:57.000000 mteb-1.8.7/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 16:47:02.317839 mteb-1.8.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 16:47:02.317839 mteb-1.8.7/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1418 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_InstructionRetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1129 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)     2602 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_all_abstasks.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_encoder_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     1390 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_mteb.py
--rw-r--r--   0 root         (0) root         (0)     7159 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_mteb_rerank.py
--rw-r--r--   0 root         (0) root         (0)     3013 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_overview.py
--rw-r--r--   0 root         (0) root         (0)      278 2024-05-09 16:46:57.000000 mteb-1.8.7/tests/test_retrieval_abstask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.042079 mteb-1.8.8/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-11 09:52:23.000000 mteb-1.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    24072 2024-05-11 09:52:28.042079 mteb-1.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9642 2024-05-11 09:52:23.000000 mteb-1.8.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.818077 mteb-1.8.8/docs/
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-05-11 09:52:23.000000 mteb-1.8.8/docs/create_tasks_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.818077 mteb-1.8.8/docs/mmteb/
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-11 09:52:23.000000 mteb-1.8.8/docs/mmteb/create_points_table.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-11 09:52:23.000000 mteb-1.8.8/docs/mmteb/validate_points.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.818077 mteb-1.8.8/mteb/
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.822077 mteb-1.8.8/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     6404 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5876 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     7433 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskClusteringFast.py
+-rw-r--r--   0 root         (0) root         (0)    24968 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskInstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    13422 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      562 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1897 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/MultiSubsetLoader.py
+-rw-r--r--   0 root         (0) root         (0)      653 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)    10404 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7082 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/iso_15924_to_script.json
+-rw-r--r--   0 root         (0) root         (0)   193114 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/iso_639_3_to_language.json
+-rw-r--r--   0 root         (0) root         (0)      541 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/abstasks/languages.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/benchmarks.py
+-rw-r--r--   0 root         (0) root         (0)     5225 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/cmd.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/encoder_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.822077 mteb-1.8.8/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13258 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8927 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7126 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    19805 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7965 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/logging.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/overview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/BitextMining/dan/
+-rw-r--r--   0 root         (0) root         (0)     2246 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.826077 mteb-1.8.8/mteb/tasks/BitextMining/kat/
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)    29308 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5951 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     4585 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)    13482 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/BitextMining/srn/
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/srn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/BitextMining/vie/
+-rw-r--r--   0 root         (0) root         (0)     2889 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/BitextMining/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/CLSD/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/
+-rw-r--r--   0 root         (0) root         (0)     4878 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py
+-rw-r--r--   0 root         (0) root         (0)     4878 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/WMT1921/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      162 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/CLSD/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.830077 mteb-1.8.8/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     5167 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ara/
+-rw-r--r--   0 root         (0) root         (0)     1598 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/AJGT.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1907 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/TweetEmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/TweetSarcasmClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ben/
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/BengaliDocumentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ben/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/bul/
+-rw-r--r--   0 root         (0) root         (0)     1947 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/bul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ces/
+-rw-r--r--   0 root         (0) root         (0)     1704 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/dan/
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/dan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.834077 mteb-1.8.8/mteb/tasks/Classification/ell/
+-rw-r--r--   0 root         (0) root         (0)     2172 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.838077 mteb-1.8.8/mteb/tasks/Classification/eng/
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ArxivClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/DBpediaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/FrenkEnClassification.py
+-rw-r--r--   0 root         (0) root         (0)      990 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)   241062 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/LegalBenchClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/NewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/PatentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ToxicChatClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/YelpReviewFullClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.838077 mteb-1.8.8/mteb/tasks/Classification/est/
+-rw-r--r--   0 root         (0) root         (0)     2407 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/est/estonian_valence.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.838077 mteb-1.8.8/mteb/tasks/Classification/fas/
+-rw-r--r--   0 root         (0) root         (0)     1714 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/fil/
+-rw-r--r--   0 root         (0) root         (0)     1925 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fil/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/fin/
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fin/FinToxicityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/fra/
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fra/FrenchBookReviews.py
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/guj/
+-rw-r--r--   0 root         (0) root         (0)     1285 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/guj/GujaratiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/guj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/hin/
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/hrv/
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hrv/FrenkHrClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/hrv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/ind/
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3829 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ind/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.842077 mteb-1.8.8/mteb/tasks/Classification/ita/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ita/ItaCaseholdClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ita/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/jav/
+-rw-r--r--   0 root         (0) root         (0)     1871 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/jav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3402 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/jpn/WRIMEClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kan/
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kan/KannadaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kat/
+-rw-r--r--   0 root         (0) root         (0)     3016 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kor/
+-rw-r--r--   0 root         (0) root         (0)     2428 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kor/KlueTC.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/kur/
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kur/KurdishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/kur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/mal/
+-rw-r--r--   0 root         (0) root         (0)     1293 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mal/MalayalamNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.846077 mteb-1.8.8/mteb/tasks/Classification/mkd/
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/mkd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.850077 mteb-1.8.8/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2638 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/HinDialectClassification.py
+-rw-r--r--   0 root         (0) root         (0)     5163 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/LanguageClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MultiHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3839 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     8376 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/SIB200Classification.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/nep/
+-rw-r--r--   0 root         (0) root         (0)     2770 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nep/NepaliNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nep/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/nld/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/nob/
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nob/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1173 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/nob/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/ory/
+-rw-r--r--   0 root         (0) root         (0)     1306 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ory/OdiaNewsClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/pan/
+-rw-r--r--   0 root         (0) root         (0)     1336 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/pan/PunjabiNewsClassification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/pol/
+-rw-r--r--   0 root         (0) root         (0)     4922 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/pol/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/por/
+-rw-r--r--   0 root         (0) root         (0)     2307 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/por/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/ron/
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ron/RomanianSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/san/
+-rw-r--r--   0 root         (0) root         (0)     2851 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/san/SanskritShlokasClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/san/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/sin/
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/sin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.854077 mteb-1.8.8/mteb/tasks/Classification/slv/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/slv/FrenkSlClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/slv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/spa/
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/spa/SpanishNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/spa/SpanishSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/ssw/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ssw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/swe/
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/swe/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/swe/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/swe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tam/
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tam/TamilNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tel/
+-rw-r--r--   0 root         (0) root         (0)     1382 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tha/
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tha/WisesightSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tsn/
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tsn/TswanaNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tsn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/tur/
+-rw-r--r--   0 root         (0) root         (0)     1640 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.858077 mteb-1.8.8/mteb/tasks/Classification/ukr/
+-rw-r--r--   0 root         (0) root         (0)     2485 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ukr/UkrFormalityClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/ukr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/urd/
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/urd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/vie/
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/zho/
+-rw-r--r--   0 root         (0) root         (0)     6571 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zho/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Classification/zul/
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Classification/zul/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1644 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.862077 mteb-1.8.8/mteb/tasks/Clustering/deu/
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.866078 mteb-1.8.8/mteb/tasks/Clustering/eng/
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.866078 mteb-1.8.8/mteb/tasks/Clustering/fra/
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3055 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     2687 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3442 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/nob/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/nob/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/pol/
+-rw-r--r--   0 root         (0) root         (0)     3352 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/pol/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/rom/
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/rom/RomaniBibleClustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/spa/
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/swe/
+-rw-r--r--   0 root         (0) root         (0)     4765 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/swe/SwednClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/swe/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/Clustering/zho/
+-rw-r--r--   0 root         (0) root         (0)     3639 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/zho/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Clustering/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.870077 mteb-1.8.8/mteb/tasks/InstructionRetrieval/
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1547 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/deu/
+-rw-r--r--   0 root         (0) root         (0)     2862 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/eng/
+-rw-r--r--   0 root         (0) root         (0)     4650 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/LegalBenchPC.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/hye/
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/hye/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2780 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/XNLI.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/pol/
+-rw-r--r--   0 root         (0) root         (0)     3577 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/pol/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/PairClassification/zho/
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/PairClassification/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.874077 mteb-1.8.8/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/fra/
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/fra/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/fra/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1269 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Reranking/zho/
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/zho/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Reranking/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     3751 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Retrieval/ara/
+-rw-r--r--   0 root         (0) root         (0)     2367 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ara/SadeemQuestionRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ara/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.878078 mteb-1.8.8/mteb/tasks/Retrieval/code/
+-rw-r--r--   0 root         (0) root         (0)     3275 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/code/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.882078 mteb-1.8.8/mteb/tasks/Retrieval/dan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2574 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/dan/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.882078 mteb-1.8.8/mteb/tasks/Retrieval/deu/
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.882078 mteb-1.8.8/mteb/tasks/Retrieval/ell/
+-rw-r--r--   0 root         (0) root         (0)     2683 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ell/GreekCivicsQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/ell/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.890078 mteb-1.8.8/mteb/tasks/Retrieval/eng/
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      983 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3668 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3022 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.890078 mteb-1.8.8/mteb/tasks/Retrieval/est/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/est/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/est/estqa.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/fra/
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/FQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/hun/
+-rw-r--r--   0 root         (0) root         (0)     2589 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/hun/HunSum2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/jpn/
+-rw-r--r--   0 root         (0) root         (0)     2853 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/kat/
+-rw-r--r--   0 root         (0) root         (0)     2568 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/kor/
+-rw-r--r--   0 root         (0) root         (0)      906 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kor/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.894078 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3776 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3277 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     6239 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3052 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/nob/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/nob/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3943 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/nob/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     2699 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/nob/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/pol/
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      984 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/slk/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/slk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.898078 mteb-1.8.8/mteb/tasks/Retrieval/spa/
+-rw-r--r--   0 root         (0) root         (0)     2125 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/swe/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/swe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/tur/
+-rw-r--r--   0 root         (0) root         (0)     3883 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/tur/TurHistQuad.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/tur/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/vie/
+-rw-r--r--   0 root         (0) root         (0)     3798 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/vie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/Retrieval/zho/
+-rw-r--r--   0 root         (0) root         (0)    10384 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Retrieval/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      787 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.902078 mteb-1.8.8/mteb/tasks/STS/deu/
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/deu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/eng/
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/fao/
+-rw-r--r--   0 root         (0) root         (0)     2015 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fao/FaroeseSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/fin/
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fin/FinParaSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/fra/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fra/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/fra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/jpn/
+-rw-r--r--   0 root         (0) root         (0)     3034 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/jpn/JSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/kor/
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/kor/KlueSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/kor/KorSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/kor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     4131 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/pol/
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/pol/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/pol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.906078 mteb-1.8.8/mteb/tasks/STS/ron/
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/ron/RonSTS.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/STS/spa/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/spa/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/spa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/STS/zho/
+-rw-r--r--   0 root         (0) root         (0)     7122 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/zho/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/STS/zho/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/Summarization/eng/
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/eng/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/mteb/tasks/Summarization/fra/
+-rw-r--r--   0 root         (0) root         (0)     1304 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/Summarization/fra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.042079 mteb-1.8.8/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24072 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    73769 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      258 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-11 09:52:27.000000 mteb-1.8.8/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2752 2024-05-11 09:52:24.000000 mteb-1.8.8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.814077 mteb-1.8.8/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/results/GritLM__GritLM-7B/
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-05-11 09:52:23.000000 mteb-1.8.8/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/GritLM__GritLM-7B/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.910078 mteb-1.8.8/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-11 09:52:23.000000 mteb-1.8.8/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.810077 mteb-1.8.8/results/dangvantuan/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.914078 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloProfClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloProfClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      250 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloprofReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      634 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/HALClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json
+-rw-r--r--   0 root         (0) root         (0)      676 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClassification.json
+-rw-r--r--   0 root         (0) root         (0)      332 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      335 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MasakhaNEWSClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      679 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2992 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)     2801 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      820 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SICKFr.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/STS22.json
+-rw-r--r--   0 root         (0) root         (0)      921 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SummEvalFr.json
+-rw-r--r--   0 root         (0) root         (0)      221 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SyntecReranking.json
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-05-11 09:52:23.000000 mteb-1.8.8/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.810077 mteb-1.8.8/results/intfloat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.918078 mteb-1.8.8/results/intfloat/multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/HinDialectClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      366 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1294 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/TamilNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat/multilingual-e5-small/TswanaNewsClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.918078 mteb-1.8.8/results/intfloat__e5-small/
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small/TurkishProductSentimentClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.918078 mteb-1.8.8/results/intfloat__e5-small-v2/
+-rw-r--r--   0 root         (0) root         (0)     2512 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small-v2/News21InstructionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     2550 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.922078 mteb-1.8.8/results/intfloat__multilingual-e5-base/
+-rw-r--r--   0 root         (0) root         (0)      758 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2281 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json
+-rw-r--r--   0 root         (0) root         (0)     2293 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      356 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/UyghurSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-base/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.970079 mteb-1.8.8/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/AJGT.json
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/AfriSentiLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ArxivClassification.json
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BengaliDocumentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BengaliSentimentAnalysis.json
+-rw-r--r--   0 root         (0) root         (0)   336719 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAffiliateLicenseLicensorLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAntiAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADAuditRightsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADCapOnLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADChangeOfControlLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADCovenantNotToSueLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADEffectiveDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADExclusivityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADExpirationDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADGoverningLawLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADIPOwnershipAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADInsuranceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADJointIPOwnershipLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADLicenseGrantLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADLiquidatedDamagesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADMinimumCommitmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      396 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADMostFavoredNationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNoSolicitOfCustomersLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNoSolicitOfEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNonCompeteLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      424 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNonDisparagementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNonTransferableLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADPostTerminationServicesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADPriceRestrictionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADRenewalTermLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADRevenueProfitSharingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADRofrRofoRofnLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADSourceCodeEscrowLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADTerminationForConvenienceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADThirdPartyBeneficiaryLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADUncappedLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADVolumeRestrictionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CUADWarrantyDurationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CanadaTaxCourtOutcomesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      616 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json
+-rw-r--r--   0 root         (0) root         (0)    13681 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIExplicitIdentificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      483 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLILimitedUseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLINoLicensingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      492 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      422 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissibleCopyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      461 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLISharingWithEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ContractNLISurvivalOfObligationsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CorporateLobbyingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json
+-rw-r--r--   0 root         (0) root         (0)     2309 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json
+-rw-r--r--   0 root         (0) root         (0)      738 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DBpediaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      458 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DefinitionClassificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity1LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity2LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      408 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity3LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity4LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity5LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Diversity6LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2105 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FaroeseSTS.json
+-rw-r--r--   0 root         (0) root         (0)      733 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      827 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FinToxicityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FinancialPhrasebankClassification.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenchBookReviews.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenkEnClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenkHrClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FrenkSlClassification.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/FunctionOfDecisionSectionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GeorgianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GermanDPR.json
+-rw-r--r--   0 root         (0) root         (0)      401 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GermanPoliticiansTwitterSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1150 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekCivicsQA.json
+-rw-r--r--   0 root         (0) root         (0)      606 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HateSpeechPortugueseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1289 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     4319 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)    11798 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     4273 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      644 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/InsurancePolicyInterpretationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/InternationalCitizenshipQuestionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ItaCaseholdClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      429 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JCrewBlockerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/JavaneseIMDBClassification.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KLUE-TC.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KannadaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7814 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7703 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1169 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LanguageClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsBenefitsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsBusinessLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsConsumerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsCourtsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsCrimeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsDivorceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsDomesticViolenceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsEducationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsEmploymentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsEstatesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsFamilyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsHealthLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsHousingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsImmigrationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsTortsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LearnedHandsTrafficLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LegalBenchPC.json
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/LegalReasoningCausalityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2360 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MLQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3894 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MultiHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)     8513 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)   417235 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NepaliNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3386 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NordicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PatentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      513 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/PunjabiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      403 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)    42700 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SIB200Classification.json
+-rw-r--r--   0 root         (0) root         (0)      298 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      584 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      592 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SentimentAnalysisHindi.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SinhalaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SinhalaNewsSourceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      453 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SlovakSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      375 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SpanishNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SpanishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      304 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      893 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1062 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/SyntecRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      629 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      597 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      522 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/ToxicConversationsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      459 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1827 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetTopicSingleClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      734 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/UrduRomanSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      368 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/WisesightSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    38759 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLI.json
+-rw-r--r--   0 root         (0) root         (0)    18115 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLIV2.json
+-rw-r--r--   0 root         (0) root         (0)    12839 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/XQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-11 09:52:23.000000 mteb-1.8.8/results/intfloat__multilingual-e5-small/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.814077 mteb-1.8.8/results/sentence-transformers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.974079 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      364 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)    21290 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
+-rw-r--r--   0 root         (0) root         (0)    21291 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TswanaNewsClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.978079 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
+-rw-r--r--   0 root         (0) root         (0)      340 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)   387673 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      306 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/model.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.030079 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AJGT.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/AfriSentiLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json
+-rw-r--r--   0 root         (0) root         (0)      355 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClassification.json
+-rw-r--r--   0 root         (0) root         (0)      520 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json
+-rw-r--r--   0 root         (0) root         (0)     1160 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BambaraSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliDocumentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BengaliSentimentAnalysis.json
+-rw-r--r--   0 root         (0) root         (0)   338028 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      344 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BornholmBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BulgarianStoreReviewSentimentClassfication.json
+-rw-r--r--   0 root         (0) root         (0)      462 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicenseeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAffiliateLicenseLicensorLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAntiAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADAuditRightsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCapOnLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADChangeOfControlLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCompetitiveRestrictionExceptionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADCovenantNotToSueLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADEffectiveDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      431 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExclusivityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADExpirationDateLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADGoverningLawLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIPOwnershipAssignmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADInsuranceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADIrrevocableOrPerpetualLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADJointIPOwnershipLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      415 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLicenseGrantLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADLiquidatedDamagesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMinimumCommitmentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADMostFavoredNationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfCustomersLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoSolicitOfEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonCompeteLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonDisparagementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNonTransferableLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADNoticePeriodToTerminateRenewalLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      444 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPostTerminationServicesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      438 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADPriceRestrictionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRenewalTermLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRevenueProfitSharingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADRofrRofoRofnLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADSourceCodeEscrowLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADTerminationForConvenienceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADThirdPartyBeneficiaryLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUncappedLiabilityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADUnlimitedAllYouCanEatLicenseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADVolumeRestrictionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CUADWarrantyDurationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      387 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CanadaTaxCourtOutcomesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json
+-rw-r--r--   0 root         (0) root         (0)    13663 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     5535 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      472 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIConfidentialityOfAgreementLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIExplicitIdentificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIInclusionOfVerballyConveyedInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      414 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLILimitedUseLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      439 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoLicensingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      474 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLINoticeOnCompelledDisclosureLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      469 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleAcquirementOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleCopyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissibleDevelopmentOfSimilarInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIPermissiblePostAgreementPossessionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLIReturnOfConfidentialInformationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithEmployeesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISharingWithThirdPartiesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISurvivalOfObligationsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CorporateLobbyingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2340 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json
+-rw-r--r--   0 root         (0) root         (0)     2295 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json
+-rw-r--r--   0 root         (0) root         (0)      758 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DBpediaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DefinitionClassificationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity1LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity2LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      426 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity3LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity4LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity5LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity6LegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
+-rw-r--r--   0 root         (0) root         (0)     2108 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FaroeseSTS.json
+-rw-r--r--   0 root         (0) root         (0)      746 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      835 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinToxicityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      389 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinancialPhrasebankClassification.json
+-rw-r--r--   0 root         (0) root         (0)      291 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenchBookReviews.json
+-rw-r--r--   0 root         (0) root         (0)      443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkEnClassification.json
+-rw-r--r--   0 root         (0) root         (0)      445 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkHrClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkSlClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FunctionOfDecisionSectionLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
+-rw-r--r--   0 root         (0) root         (0)      405 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GermanPoliticiansTwitterSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HateSpeechPortugueseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HotelReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1317 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     4370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)    11833 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     4276 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3921 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      456 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InsurancePolicyInterpretationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InternationalCitizenshipQuestionsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      342 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaCaseholdClassification.json
+-rw-r--r--   0 root         (0) root         (0)      430 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JCrewBlockerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JavaneseIMDBClassification.json
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-STS.json
+-rw-r--r--   0 root         (0) root         (0)      358 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KLUE-TC.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KannadaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      470 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KorSTS.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/KurdishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7839 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     7915 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1153 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LanguageClassification.json
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBenefitsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      418 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsBusinessLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsConsumerLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCourtsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsCrimeLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDivorceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      425 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsDomesticViolenceLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      412 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEducationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEmploymentLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsEstatesLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsFamilyLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHealthLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsHousingLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsImmigrationLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTortsLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LearnedHandsTrafficLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1443 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalReasoningCausalityLegalBenchClassification.json
+-rw-r--r--   0 root         (0) root         (0)   104611 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3877 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)     3884 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      394 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MacedonianTweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1332 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json
+-rw-r--r--   0 root         (0) root         (0)     8537 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)   421556 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      365 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NepaliNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     3382 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)     3376 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NordicLangClassification.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorwegianCourtsBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)    16669 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json
+-rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PatentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    18247 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json
+-rw-r--r--   0 root         (0) root         (0)      741 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      517 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      448 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PunjabiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RestaurantReviewSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaTalesBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      308 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomaniBibleClustering.json
+-rw-r--r--   0 root         (0) root         (0)      441 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RomanianSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      471 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/RonSTS.json
+-rw-r--r--   0 root         (0) root         (0)    42635 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLClustering.json
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SentimentAnalysisHindi.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SinhalaNewsSourceClassification.json
+-rw-r--r--   0 root         (0) root         (0)      380 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SiswatiNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishNewsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      454 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SpanishSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1021 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      303 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClustering.json
+-rw-r--r--   0 root         (0) root         (0)      898 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json
+-rw-r--r--   0 root         (0) root         (0)      637 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json
+-rw-r--r--   0 root         (0) root         (0)      523 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicChatClassification.json
+-rw-r--r--   0 root         (0) root         (0)      447 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ToxicConversationsClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      451 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishMovieSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      440 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurkishProductSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      373 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetEmotionClassification.json
+-rw-r--r--   0 root         (0) root         (0)      450 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSarcasmClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1822 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetTopicSingleClassification.json
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UrduRomanSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VGClustering.json
+-rw-r--r--   0 root         (0) root         (0)      351 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieMedEVBitextMining.json
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      370 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WisesightSentimentClassification.json
+-rw-r--r--   0 root         (0) root         (0)    38547 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json
+-rw-r--r--   0 root         (0) root         (0)    17971 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json
+-rw-r--r--   0 root         (0) root         (0)    12890 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YahooAnswersTopicsClassification.json
+-rw-r--r--   0 root         (0) root         (0)      378 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YelpReviewFullClassification.json
+-rw-r--r--   0 root         (0) root         (0)      377 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-11 09:52:23.000000 mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5924 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2133 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.034079 mteb-1.8.8/scripts/data/medicalqaretrieval/
+-rw-r--r--   0 root         (0) root         (0)     1884 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/medicalqaretrieval/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/multilingual_sentiment_classification/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/multilingual_sentiment_classification/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/scala_classification/
+-rw-r--r--   0 root         (0) root         (0)      475 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/scala_classification/create_multiling_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2435 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/toxic_conversations_50k/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/data/xnli2/
+-rw-r--r--   0 root         (0) root         (0)      688 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/data/xnli2/create_multilang_ds.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/mteb_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:27.814077 mteb-1.8.8/scripts/results/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/results/intfloat__multilingual-e5-small/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/results/intfloat__multilingual-e5-small/HindiDiscourseClassification.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.038079 mteb-1.8.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HindiDiscourseClassification.json
+-rw-r--r--   0 root         (0) root         (0)      673 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_law.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-05-11 09:52:23.000000 mteb-1.8.8/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 09:52:28.042079 mteb-1.8.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 09:52:28.042079 mteb-1.8.8/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_InstructionRetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_all_abstasks.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_encoder_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_mteb.py
+-rw-r--r--   0 root         (0) root         (0)     7159 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_mteb_rerank.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_overview.py
+-rw-r--r--   0 root         (0) root         (0)      278 2024-05-11 09:52:23.000000 mteb-1.8.8/tests/test_retrieval_abstask.py
```

### Comparing `mteb-1.8.7/LICENSE` & `mteb-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/PKG-INFO` & `mteb-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.8.7
+Version: 1.8.8
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.8.7/README.md` & `mteb-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/docs/create_tasks_table.py` & `mteb-1.8.8/docs/create_tasks_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/docs/mmteb/create_points_table.py` & `mteb-1.8.8/docs/mmteb/create_points_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/docs/mmteb/validate_points.py` & `mteb-1.8.8/docs/mmteb/validate_points.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTask.py` & `mteb-1.8.8/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskClusteringFast.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskClusteringFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskInstructionRetrieval.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskInstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.8.8/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/CrosslingualTask.py` & `mteb-1.8.8/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/LangMapping.py` & `mteb-1.8.8/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/MultiSubsetLoader.py` & `mteb-1.8.8/mteb/abstasks/MultiSubsetLoader.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/MultilingualTask.py` & `mteb-1.8.8/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/TaskMetadata.py` & `mteb-1.8.8/mteb/abstasks/TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/iso_15924_to_script.json` & `mteb-1.8.8/mteb/abstasks/iso_15924_to_script.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/iso_639_3_to_language.json` & `mteb-1.8.8/mteb/abstasks/iso_639_3_to_language.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/abstasks/languages.py` & `mteb-1.8.8/mteb/abstasks/languages.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/benchmarks.py` & `mteb-1.8.8/mteb/benchmarks.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/cmd.py` & `mteb-1.8.8/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/encoder_interface.py` & `mteb-1.8.8/mteb/encoder_interface.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/MTEB.py` & `mteb-1.8.8/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.8.8/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/evaluation/evaluators/utils.py` & `mteb-1.8.8/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/logging.py` & `mteb-1.8.8/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/overview.py` & `mteb-1.8.8/mteb/overview.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/__init__.py` & `mteb-1.8.8/mteb/tasks/BitextMining/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/dan/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/BibleNLPBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22ConvBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/IN22GenBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NTREXBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/RomaTalesBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/multilingual/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/srn/SRNCorpusBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py` & `mteb-1.8.8/mteb/tasks/BitextMining/vie/VieMedEVBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py` & `mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT19.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py` & `mteb-1.8.8/mteb/tasks/CLSD/WMT1921/CrossLingualSemanticDiscriminationWMT21.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/__init__.py` & `mteb-1.8.8/mteb/tasks/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ara/AJGT.py` & `mteb-1.8.8/mteb/tasks/Classification/ara/AJGT.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ara/HotelReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ara/RestaurantReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ara/TweetEmotionClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ara/TweetEmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ara/TweetSarcasmClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ara/TweetSarcasmClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ben/BengaliDocumentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ben/BengaliDocumentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ben/BengaliHateSpeechClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py` & `mteb-1.8.8/mteb/tasks/Classification/ben/BengaliSentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py` & `mteb-1.8.8/mteb/tasks/Classification/bul/BulgarianStoreReviewSentimentClassfication.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ces/CzechSubjectivityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/dan/AngryTweetsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/dan/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/dan/DKHateClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/dan/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/dan/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/dan/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/dan/LccSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/dan/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/deu/GermanPoliticiansTwitterSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ell/GreekLegalCodeClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/AmazonPolarityClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/ArxivClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/ArxivClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/Banking77Classification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/DBpediaClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/DBpediaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/EmotionClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/FinancialPhrasebankClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/FrenkEnClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/FrenkEnClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/ImdbClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/LegalBenchClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/LegalBenchClassification.py`

 * *Files 2% similar despite different names*

```diff
@@ -800,15 +800,15 @@
         )
         self.dataset = self.dataset.rename_column("answer", "label")
 
 
 class CorporateLobbyingLegalBenchClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="CorporateLobbyingLegalBenchClassification",
-        description="The Corporate Lobbying task cosists of determining whether a proposed Congressional bill may be relevant to a company based on a company's self-description in its SEC 10K filing.",
+        description="The Corporate Lobbying task consists of determining whether a proposed Congressional bill may be relevant to a company based on a company's self-description in its SEC 10K filing.",
         reference="https://huggingface.co/datasets/nguha/legalbench",
         dataset={
             "path": "nguha/legalbench",
             "name": "corporate_lobbying",
             "revision": "12ca3b695563788fead87a982ad1a068284413f4",
         },
         type="Classification",
@@ -2914,14 +2914,601 @@
             lambda example: {
                 "answer": mapping.get(example["answer"].lower(), example["answer"])
             }
         )
         self.dataset = self.dataset.rename_column("answer", "label")
 
 
+class DefinitionClassificationLegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="DefinitionClassificationLegalBenchClassification",
+        description="This task consists of determining whether or not a sentence from a Supreme Court opinion offers a definition of a term.",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "definition_classification",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-sa-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 1337},
+        avg_character_length={"test": 253.72},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+
+class Diversity1LegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="Diversity1LegalBenchClassification",
+        description="Given a set of facts about the citizenships of plaintiffs and defendants and the amounts associated with claims, determine if the criteria for diversity jurisdiction have been met (variant 1).",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "diversity_1",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 300},
+        avg_character_length={"test": 103.21},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        # Map the boolean columns to readable plaintext
+        _diverse_parties_map = {
+            "True": "The parties are diverse.",
+            "False": "The parties are not diverse.",
+        }
+
+        _amount_in_controversy_map = {
+            "True": "The Amount-in-controversy was met.",
+            "False": "The Amount-in-controversy was not met.",
+        }
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["text"]
+                + " "
+                + _diverse_parties_map[example["parties_are_diverse"]]
+                + " "
+                + _amount_in_controversy_map[example["aic_is_met"]]
+            }
+        )
+        self.dataset = self.dataset.remove_columns(
+            ["parties_are_diverse", "aic_is_met"]
+        )
+
+
+class Diversity2LegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="Diversity2LegalBenchClassification",
+        description="Given a set of facts about the citizenships of plaintiffs and defendants and the amounts associated with claims, determine if the criteria for diversity jurisdiction have been met (variant 2).",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "diversity_2",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 300},
+        avg_character_length={"test": 0},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        # Map the boolean columns to readable plaintext
+        _diverse_parties_map = {
+            "True": "The parties are diverse.",
+            "False": "The parties are not diverse.",
+        }
+
+        _amount_in_controversy_map = {
+            "True": "The Amount-in-controversy was met.",
+            "False": "The Amount-in-controversy was not met.",
+        }
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["text"]
+                + " "
+                + _diverse_parties_map[example["parties_are_diverse"]]
+                + " "
+                + _amount_in_controversy_map[example["aic_is_met"]]
+            }
+        )
+        self.dataset = self.dataset.remove_columns(
+            ["parties_are_diverse", "aic_is_met"]
+        )
+
+
+class Diversity3LegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="Diversity3LegalBenchClassification",
+        description="Given a set of facts about the citizenships of plaintiffs and defendants and the amounts associated with claims, determine if the criteria for diversity jurisdiction have been met (variant 3).",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "diversity_3",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 300},
+        avg_character_length={"test": 135.46},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        # Map the boolean columns to readable plaintext
+        _diverse_parties_map = {
+            "True": "The parties are diverse.",
+            "False": "The parties are not diverse.",
+        }
+
+        _amount_in_controversy_map = {
+            "True": "The Amount-in-controversy was met.",
+            "False": "The Amount-in-controversy was not met.",
+        }
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["text"]
+                + " "
+                + _diverse_parties_map[example["parties_are_diverse"]]
+                + " "
+                + _amount_in_controversy_map[example["aic_is_met"]]
+            }
+        )
+        self.dataset = self.dataset.remove_columns(
+            ["parties_are_diverse", "aic_is_met"]
+        )
+
+
+class Diversity4LegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="Diversity4LegalBenchClassification",
+        description="Given a set of facts about the citizenships of plaintiffs and defendants and the amounts associated with claims, determine if the criteria for diversity jurisdiction have been met (variant 4).",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "diversity_4",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 300},
+        avg_character_length={"test": 144.52},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        # Map the boolean columns to readable plaintext
+        _diverse_parties_map = {
+            "True": "The parties are diverse.",
+            "False": "The parties are not diverse.",
+        }
+
+        _amount_in_controversy_map = {
+            "True": "The Amount-in-controversy was met.",
+            "False": "The Amount-in-controversy was not met.",
+        }
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["text"]
+                + " "
+                + _diverse_parties_map[example["parties_are_diverse"]]
+                + " "
+                + _amount_in_controversy_map[example["aic_is_met"]]
+            }
+        )
+        self.dataset = self.dataset.remove_columns(
+            ["parties_are_diverse", "aic_is_met"]
+        )
+
+
+class Diversity5LegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="Diversity5LegalBenchClassification",
+        description="Given a set of facts about the citizenships of plaintiffs and defendants and the amounts associated with claims, determine if the criteria for diversity jurisdiction have been met (variant 5).",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "diversity_5",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 300},
+        avg_character_length={"test": 174.77},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        # Map the boolean columns to readable plaintext
+        _diverse_parties_map = {
+            "True": "The parties are diverse.",
+            "False": "The parties are not diverse.",
+        }
+
+        _amount_in_controversy_map = {
+            "True": "The Amount-in-controversy was met.",
+            "False": "The Amount-in-controversy was not met.",
+        }
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["text"]
+                + " "
+                + _diverse_parties_map[example["parties_are_diverse"]]
+                + " "
+                + _amount_in_controversy_map[example["aic_is_met"]]
+            }
+        )
+        self.dataset = self.dataset.remove_columns(
+            ["parties_are_diverse", "aic_is_met"]
+        )
+
+
+class Diversity6LegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="Diversity6LegalBenchClassification",
+        description="Given a set of facts about the citizenships of plaintiffs and defendants and the amounts associated with claims, determine if the criteria for diversity jurisdiction have been met (variant 6).",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "diversity_6",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 300},
+        avg_character_length={"test": 301.01},
+    )
+
+    def dataset_transform(self):
+        mapping = {"yes": 1, "no": 0}
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "answer": mapping.get(example["answer"].lower(), example["answer"])
+            }
+        )
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        # Map the boolean columns to readable plaintext
+        _diverse_parties_map = {
+            "True": "The parties are diverse.",
+            "False": "The parties are not diverse.",
+        }
+
+        _amount_in_controversy_map = {
+            "True": "The Amount-in-controversy was met.",
+            "False": "The Amount-in-controversy was not met.",
+        }
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["text"]
+                + " "
+                + _diverse_parties_map[example["parties_are_diverse"]]
+                + " "
+                + _amount_in_controversy_map[example["aic_is_met"]]
+            }
+        )
+        self.dataset = self.dataset.remove_columns(
+            ["parties_are_diverse", "aic_is_met"]
+        )
+
+
+class FunctionOfDecisionSectionLegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="FunctionOfDecisionSectionLegalBenchClassification",
+        description="""The task is to classify a paragraph extracted from a written court decision into one of seven possible categories:
+            1. Facts - The paragraph describes the faction background that led up to the present lawsuit.
+            2. Procedural History - The paragraph describes the course of litigation that led to the current proceeding before the court.
+            3. Issue - The paragraph describes the legal or factual issue that must be resolved by the court.
+            4. Rule - The paragraph describes a rule of law relevant to resolving the issue.
+            5. Analysis - The paragraph analyzes the legal issue by applying the relevant legal principles to the facts of the present dispute.
+            6. Conclusion - The paragraph presents a conclusion of the court.
+            7. Decree - The paragraph constitutes a decree resolving the dispute.
+        """,
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "function_of_decision_section",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 367},
+        avg_character_length={"test": 551.07},
+    )
+
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["Paragraph"]
+                + "\n\n"
+                + "Citation: "
+                + example["Citation"]
+            }
+        )
+
+
+class InsurancePolicyInterpretationLegalBenchClassification(AbsTaskClassification):
+    metadata = TaskMetadata(
+        name="InsurancePolicyInterpretationLegalBenchClassification",
+        description="Given an insurance claim and policy, determine whether the claim is covered by the policy.",
+        reference="https://huggingface.co/datasets/nguha/legalbench",
+        dataset={
+            "path": "nguha/legalbench",
+            "name": "insurance_policy_interpretation",
+            "revision": "12ca3b695563788fead87a982ad1a068284413f4",
+        },
+        type="Classification",
+        category="s2s",
+        eval_splits=["test"],
+        eval_langs=["eng-Latn"],
+        main_score="accuracy",
+        date=("2000-01-01", "2023-08-23"),  # best guess
+        form=["written"],
+        domains=["Legal"],
+        task_subtypes=[],
+        license="cc-by-4.0",
+        socioeconomic_status="high",
+        annotations_creators="expert-annotated",
+        dialect=[],
+        text_creation="found",
+        bibtex_citation="""
+        @misc{guha2023legalbench,
+            title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
+            author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
+            year={2023},
+            eprint={2308.11462},
+            archivePrefix={arXiv},
+            primaryClass={cs.CL}
+        },
+        """,
+        n_samples={"test": 133},
+        avg_character_length={"test": 521.88},
+    )
+
+    def dataset_transform(self):
+        self.dataset = self.dataset.rename_column("answer", "label")
+
+        self.dataset = self.dataset.map(
+            lambda example: {
+                "text": example["policy"] + "\n\n" + "Claim: " + example["claim"]
+            }
+        )
+
+
 class InternationalCitizenshipQuestionsLegalBenchClassification(AbsTaskClassification):
     metadata = TaskMetadata(
         name="InternationalCitizenshipQuestionsLegalBenchClassification",
         description="Answer questions about citizenship law from across the world. Dataset was made using the GLOBALCIT citizenship law dataset, by constructing questions about citizenship law as Yes or No questions.",
         reference="https://huggingface.co/datasets/nguha/legalbench",
         dataset={
             "path": "nguha/legalbench",
```

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/NewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/NewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/PatentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/PatentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/ToxicChatClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/ToxicChatClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/ToxicConversationsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/TweetTopicSingleClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/YahooAnswersTopicsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/eng/YelpReviewFullClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/eng/YelpReviewFullClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/est/estonian_valence.py` & `mteb-1.8.8/mteb/tasks/Classification/est/estonian_valence.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/fas/PersianFoodSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoHateSpeechClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/fil/FilipinoShopeeReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/fin/FinToxicityClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/fin/FinToxicityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/fra/FrenchBookReviews.py` & `mteb-1.8.8/mteb/tasks/Classification/fra/FrenchBookReviews.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/fra/MovieReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/guj/GujaratiNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/guj/GujaratiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/hin/HindiDiscourseClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/hin/HindiDiscourseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py` & `mteb-1.8.8/mteb/tasks/Classification/hin/SentimentAnalysisHindi.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/hrv/FrenkHrClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/hrv/FrenkHrClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianIdClickbaitClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ind/IndonesianMongabayConservationClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ita/ItaCaseholdClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ita/ItaCaseholdClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ita/ItalianLinguistAcceptabilityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/jav/JavaneseIMDBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/jpn/WRIMEClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/jpn/WRIMEClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/kan/KannadaNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/kan/KannadaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/kat/GeorgianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/kor/KlueTC.py` & `mteb-1.8.8/mteb/tasks/Classification/kor/KlueTC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/kur/KurdishSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/kur/KurdishSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/mal/MalayalamNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/mal/MalayalamNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/mkd/MacedonianTweetSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/AfriSentiLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/CataloniaTweetClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/HinDialectClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/HinDialectClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/IndicLangClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/IndicSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/LanguageClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/LanguageClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MultiHateClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MultiHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/MultilingualSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/SIB200Classification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/SIB200Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/SouthAfricanLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/SwissJudgementClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/multilingual/TweetSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/nep/NepaliNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/nep/NepaliNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/nld/DutchBookReviewSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/nob/NoRecClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/nob/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/nob/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ory/OdiaNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ory/OdiaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/pan/PunjabiNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/pan/PunjabiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/pol/PolishClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/pol/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/por/HateSpeechPortugueseClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ron/RomanianSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ron/RomanianSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/san/SanskritShlokasClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/san/SanskritShlokasClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/sin/SinhalaNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/sin/SinhalaNewsSourceClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/slv/FrenkSlClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/slv/FrenkSlClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/spa/SpanishNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/spa/SpanishNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/spa/SpanishSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/spa/SpanishSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ssw/SiswatiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/swe/DalajClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/swe/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/swe/SweRecClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/swe/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/tam/TamilNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/tam/TamilNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/tel/TeluguAndhraJyotiNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/tha/WisesightSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/tha/WisesightSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/tsn/TswanaNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/tsn/TswanaNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/tur/TurkishMovieSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/tur/TurkishProductSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/ukr/UkrFormalityClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/ukr/UkrFormalityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/urd/UrduRomanSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/vie/VieStudentFeedbackClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/zho/CMTEBClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/zho/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/zho/YueOpenriceReviewClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py` & `mteb-1.8.8/mteb/tasks/Classification/zul/IsiZuluNewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/__init__.py` & `mteb-1.8.8/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringP2PFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/BlurbsClusteringS2SFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringP2PFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py` & `mteb-1.8.8/mteb/tasks/Clustering/deu/TenKGnadClusteringS2SFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringP2PFast.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/BigPatentClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/RedditClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/RedditClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/StackExchangeClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/eng/WikiCitiesClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/eng/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/fra/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/fra/HALClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/fra/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/multilingual/IndicReviewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/multilingual/WikiClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/nob/snl_clustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/nob/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/nob/vg_clustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/nob/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/pol/PolishClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/pol/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/rom/RomaniBibleClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/rom/RomaniBibleClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/spa/FloresClusteringS2S.py` & `mteb-1.8.8/mteb/tasks/Clustering/spa/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py` & `mteb-1.8.8/mteb/tasks/Clustering/spa/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/swe/SwednClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/swe/SwednClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/swe/swedn_clustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/swe/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Clustering/zho/CMTEBClustering.py` & `mteb-1.8.8/mteb/tasks/Clustering/zho/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py` & `mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Core17InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py` & `mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/News21InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py` & `mteb-1.8.8/mteb/tasks/InstructionRetrieval/eng/Robust04InstructionRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/deu/FalseFriendsDeEnPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/eng/LegalBenchPC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/eng/LegalBenchPC.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,20 @@
     },
     {
         "name": "consumer_contracts_qa",
         "sent1": "question",
         "sent2": "contract",
         "labels": "answer",
     },
+    {
+        "name": "hearsay",
+        "sent1": "text",
+        "sent2": "slice",
+        "labels": "answer",
+    },
 ]
 
 
 class LegalBenchPC(AbsTaskPairClassification):
     metadata = TaskMetadata(
         name="LegalBenchPC",
         description="LegalBench Dataset",
@@ -34,15 +40,15 @@
             "revision": "12ca3b695563788fead87a982ad1a068284413f4",
         },
         type="PairClassification",
         category="s2s",
         eval_splits=["test"],
         eval_langs=["eng-Latn"],
         main_score="accuracy",
-        date=("2023-08-23", "2023-08-23"),
+        date=("2000-01-01", "2023-08-23"),  # best guess
         form=["written"],
         domains=["Legal"],
         task_subtypes=[],
         license="cc-by-4.0",
         socioeconomic_status="high",
         annotations_creators="expert-annotated",
         dialect=[],
@@ -52,16 +58,16 @@
             title={LegalBench: A Collaboratively Built Benchmark for Measuring Legal Reasoning in Large Language Models}, 
             author={Neel Guha and Julian Nyarko and Daniel E. Ho and Christopher Ré and Adam Chilton and Aditya Narayana and Alex Chohlas-Wood and Austin Peters and Brandon Waldon and Daniel N. Rockmore and Diego Zambrano and Dmitry Talisman and Enam Hoque and Faiz Surani and Frank Fagan and Galit Sarfaty and Gregory M. Dickinson and Haggai Porat and Jason Hegland and Jessica Wu and Joe Nudell and Joel Niklaus and John Nay and Jonathan H. Choi and Kevin Tobia and Margaret Hagan and Megan Ma and Michael Livermore and Nikon Rasumov-Rahe and Nils Holzenberger and Noam Kolt and Peter Henderson and Sean Rehaag and Sharad Goel and Shang Gao and Spencer Williams and Sunny Gandhi and Tom Zur and Varun Iyer and Zehua Li},
             year={2023},
             eprint={2308.11462},
             archivePrefix={arXiv},
             primaryClass={cs.CL}
             }""",
-        n_samples={"test": 584},
-        avg_character_length={"test": 74.75},
+        n_samples={"test": 678},
+        avg_character_length={"test": 83.94},
     )
 
     def load_data(self, **kwargs: Any) -> None:
         """Load dataset from HuggingFace hub"""
         if self.data_loaded:
             return
```

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/eng/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/eng/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/hye/ArmenianParaphrasePC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.8.8/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/multilingual/XNLI.py` & `mteb-1.8.8/mteb/tasks/PairClassification/multilingual/XNLI.py`

 * *Files 15% similar despite different names*

```diff
@@ -99,27 +99,30 @@
     "assamese": ["asm-Beng"],
     "bengali": ["ben-Beng"],
     "marathi": ["mar-Deva"],
     "bhojpuri": ["bho-Deva"],
     "odiya": ["ory-Orya"],
     "sanskrit": ["san-Deva"],
     "tamil": ["tam-Taml"],
+    "turkish": ["tur-Latn"],
+    "greek": ["ell-Grek"],
+    "russian": ["rus-Cyrl"],
 }
 
 
-class XNLI2(XNLI):
+class XNLIV2(MultilingualTask, AbsTaskPairClassification):
     metadata = TaskMetadata(
-        name="XNLI2",
+        name="XNLIV2",
         dataset={
             "path": "mteb/xnli2.0-multi-pair",
-            "revision": "1a3794e88c74db2a13aebc5e8abc3dc4312a7543",
+            "revision": "5b7d477a8c62cdd18e2fed7e015497c20b4371ad",
         },
         description="""
         This is subset of 'XNLI 2.0: Improving XNLI dataset and performance on Cross Lingual Understanding'
-        with languages that were not part of the original XNLI.
+        with languages that were not part of the original XNLI plus three (verified) languages that are not strongly covered in MTEB
         """,
         reference="https://arxiv.org/pdf/2301.06527",
         category="s2s",
         type="PairClassification",
         eval_splits=["test"],
         eval_langs=_LANGS_2,
         main_score="ap",
@@ -127,20 +130,45 @@
         form=["written"],
         domains=["Non-fiction", "Fiction", "Government"],
         task_subtypes=[],
         license="Not specified",
         socioeconomic_status="mixed",
         annotations_creators="expert-annotated",
         dialect=[],
-        text_creation="created",
+        text_creation="machine-translated and verified",
         bibtex_citation="""@inproceedings{upadhyay2023xnli,
             title={XNLI 2.0: Improving XNLI dataset and performance on Cross Lingual Understanding (XLU)},
             author={Upadhyay, Ankit Kumar and Upadhya, Harsit Kumar},
             booktitle={2023 IEEE 8th International Conference for Convergence in Technology (I2CT)},
             pages={1--6},
             year={2023},
             organization={IEEE}
             }
         """,
         n_samples={"test": 5010},
-        avg_character_length={"test": 105.72},  # average of premise and hypothesis
+        avg_character_length={"test": 80.06},  # average of premise and hypothesis
     )
+
+    def dataset_transform(self):
+        _dataset = {}
+        for lang in self.langs:
+            _dataset[lang] = {}
+            self.dataset[lang] = self.stratified_subsampling(
+                self.dataset[lang], seed=self.seed, splits=self.metadata.eval_splits
+            )
+            for split in self.metadata.eval_splits:
+                # 0=entailment, 2=contradiction. Filter out neutral to match the task.
+                # Then map entailment as positive (1) and contradiction as negative (0).
+                hf_dataset = self.dataset[lang][split].filter(
+                    lambda x: x["label"] in [0, 2]
+                )
+                hf_dataset = hf_dataset.map(
+                    lambda example: {"label": 0 if example["label"] == 2 else 1}
+                )
+                _dataset[lang][split] = [
+                    {
+                        "sent1": hf_dataset["premise"],
+                        "sent2": hf_dataset["hypothesis"],
+                        "labels": hf_dataset["label"],
+                    }
+                ]
+        self.dataset = _dataset
```

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/pol/PolishPC.py` & `mteb-1.8.8/mteb/tasks/PairClassification/pol/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py` & `mteb-1.8.8/mteb/tasks/PairClassification/zho/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py` & `mteb-1.8.8/mteb/tasks/Reranking/eng/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/eng/MindSmallReranking.py` & `mteb-1.8.8/mteb/tasks/Reranking/eng/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/eng/SciDocsReranking.py` & `mteb-1.8.8/mteb/tasks/Reranking/eng/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py` & `mteb-1.8.8/mteb/tasks/Reranking/eng/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/fra/AlloprofReranking.py` & `mteb-1.8.8/mteb/tasks/Reranking/fra/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/fra/SyntecReranking.py` & `mteb-1.8.8/mteb/tasks/Reranking/fra/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.8.8/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Reranking/zho/CMTEBReranking.py` & `mteb-1.8.8/mteb/tasks/Reranking/zho/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/__init__.py` & `mteb-1.8.8/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/dan/dan_fever.py` & `mteb-1.8.8/mteb/tasks/Retrieval/dan/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/dan/t2nord_retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/dan/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/dan/twitterhjerne.py` & `mteb-1.8.8/mteb/tasks/Retrieval/dan/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/deu/GerDaLIRSmallRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/deu/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/deu/LegalQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/ell/GreekCivicsQA.py` & `mteb-1.8.8/mteb/tasks/Retrieval/ell/GreekCivicsQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/AILACasedocsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/AILAStatutesRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/FEVERRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/HagridRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBNeedleRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBPasskeyRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBQMSumRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBSummScreenFDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LEMBWikimQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchConsumerContractsQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalBenchCorporateLobbyingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/LegalSummarizationRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/MedicalQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/NQRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/QuoraRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/SciFactRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/eng/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/est/estqa.py` & `mteb-1.8.8/mteb/tasks/Retrieval/est/estqa.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/fra/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/fra/BSARDRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/fra/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/fra/FQuADRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/fra/FQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/fra/SyntecRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/fra/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/hun/HunSum2.py` & `mteb-1.8.8/mteb/tasks/Retrieval/hun/HunSum2.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/jpn/JaQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/kat/GeorgianFAQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/kor/KoMiracl.py` & `mteb-1.8.8/mteb/tasks/Retrieval/kor/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/kor/KoStrategyQA.py` & `mteb-1.8.8/mteb/tasks/Retrieval/kor/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/IndicQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MLQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2022Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/NeuCLIR2023Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/multilingual/XQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/nob/norquad.py` & `mteb-1.8.8/mteb/tasks/Retrieval/nob/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/nob/snl_retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/nob/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/NQPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/pol/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/slk/SlovakSumRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py` & `mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py` & `mteb-1.8.8/mteb/tasks/Retrieval/spa/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/swe/swedn_retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/swe/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/swe/swefaq_retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/swe/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/tur/TurHistQuad.py` & `mteb-1.8.8/mteb/tasks/Retrieval/tur/TurHistQuad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/vie/VieQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/zho/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py` & `mteb-1.8.8/mteb/tasks/Retrieval/zho/LeCaRDv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/__init__.py` & `mteb-1.8.8/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py` & `mteb-1.8.8/mteb/tasks/STS/deu/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/BiossesSTS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/STS12STS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/STS13STS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/STS14STS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/STS15STS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/STS16STS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/STSBenchmarkSTS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/eng/SickrSTS.py` & `mteb-1.8.8/mteb/tasks/STS/eng/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/fao/FaroeseSTS.py` & `mteb-1.8.8/mteb/tasks/STS/fao/FaroeseSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/fin/FinParaSTS.py` & `mteb-1.8.8/mteb/tasks/STS/fin/FinParaSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/fra/SickFrSTS.py` & `mteb-1.8.8/mteb/tasks/STS/fra/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/jpn/JSTS.py` & `mteb-1.8.8/mteb/tasks/STS/jpn/JSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/kor/KlueSTS.py` & `mteb-1.8.8/mteb/tasks/STS/kor/KlueSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/kor/KorSTS.py` & `mteb-1.8.8/mteb/tasks/STS/kor/KorSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py` & `mteb-1.8.8/mteb/tasks/STS/multilingual/IndicCrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.8.8/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.8.8/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.8.8/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/pol/PolishSTS.py` & `mteb-1.8.8/mteb/tasks/STS/pol/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/ron/RonSTS.py` & `mteb-1.8.8/mteb/tasks/STS/ron/RonSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/spa/STSES.py` & `mteb-1.8.8/mteb/tasks/STS/spa/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/STS/zho/CMTEBSTS.py` & `mteb-1.8.8/mteb/tasks/STS/zho/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Summarization/eng/SummEvalSummarization.py` & `mteb-1.8.8/mteb/tasks/Summarization/eng/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py` & `mteb-1.8.8/mteb/tasks/Summarization/fra/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/mteb.egg-info/PKG-INFO` & `mteb-1.8.8/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.8.7
+Version: 1.8.8
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mteb-1.8.7/mteb.egg-info/SOURCES.txt` & `mteb-1.8.8/mteb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 mteb/evaluation/evaluators/PairClassificationEvaluator.py
 mteb/evaluation/evaluators/RerankingEvaluator.py
 mteb/evaluation/evaluators/RetrievalEvaluator.py
 mteb/evaluation/evaluators/STSEvaluator.py
 mteb/evaluation/evaluators/SummarizationEvaluator.py
 mteb/evaluation/evaluators/__init__.py
 mteb/evaluation/evaluators/utils.py
-mteb/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
 mteb/tasks/__init__.py
 mteb/tasks/BitextMining/__init__.py
 mteb/tasks/BitextMining/dan/BornholmskBitextMining.py
 mteb/tasks/BitextMining/dan/__init__.py
 mteb/tasks/BitextMining/kat/TbilisiCityHallBitextMining.py
 mteb/tasks/BitextMining/kat/__init__.py
 mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
@@ -315,14 +314,16 @@
 mteb/tasks/Reranking/fra/SyntecReranking.py
 mteb/tasks/Reranking/fra/__init__.py
 mteb/tasks/Reranking/multilingual/MIRACLReranking.py
 mteb/tasks/Reranking/multilingual/__init__.py
 mteb/tasks/Reranking/zho/CMTEBReranking.py
 mteb/tasks/Reranking/zho/__init__.py
 mteb/tasks/Retrieval/__init__.py
+mteb/tasks/Retrieval/ara/SadeemQuestionRetrieval.py
+mteb/tasks/Retrieval/ara/__init__.py
 mteb/tasks/Retrieval/code/CodeEditSearchRetrieval.py
 mteb/tasks/Retrieval/code/CodeSearchNetRetrieval.py
 mteb/tasks/Retrieval/code/__init__.py
 mteb/tasks/Retrieval/dan/__init__.py
 mteb/tasks/Retrieval/dan/dan_fever.py
 mteb/tasks/Retrieval/dan/t2nord_retrieval.py
 mteb/tasks/Retrieval/dan/twitterhjerne.py
@@ -497,14 +498,15 @@
 results/dangvantuan/sentence-camembert-base/SummEvalFr.json
 results/dangvantuan/sentence-camembert-base/SyntecReranking.json
 results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json
 results/dangvantuan/sentence-camembert-base/XPQARetrieval.json
 results/intfloat/multilingual-e5-small/HinDialectClassification.json
 results/intfloat/multilingual-e5-small/MalayalamNewsClassification.json
 results/intfloat/multilingual-e5-small/OdiaNewsClassification.json
+results/intfloat/multilingual-e5-small/SadeemQuestionRetrieval.json
 results/intfloat/multilingual-e5-small/SouthAfricanLangClassification.json
 results/intfloat/multilingual-e5-small/TamilNewsClassification.json
 results/intfloat/multilingual-e5-small/TeluguAndhraJyotiNewsClassification.json
 results/intfloat/multilingual-e5-small/TswanaNewsClassification.json
 results/intfloat__e5-small/TurkishProductSentimentClassification.json
 results/intfloat__e5-small-v2/Core17InstructionRetrieval.json
 results/intfloat__e5-small-v2/News21InstructionRetrieval.json
@@ -595,28 +597,36 @@
 results/intfloat__multilingual-e5-small/ContractNLISurvivalOfObligationsLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/CorporateLobbyingLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json
 results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json
 results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json
 results/intfloat__multilingual-e5-small/DBpediaClassification.json
 results/intfloat__multilingual-e5-small/DanFEVER.json
+results/intfloat__multilingual-e5-small/DefinitionClassificationLegalBenchClassification.json
+results/intfloat__multilingual-e5-small/Diversity1LegalBenchClassification.json
+results/intfloat__multilingual-e5-small/Diversity2LegalBenchClassification.json
+results/intfloat__multilingual-e5-small/Diversity3LegalBenchClassification.json
+results/intfloat__multilingual-e5-small/Diversity4LegalBenchClassification.json
+results/intfloat__multilingual-e5-small/Diversity5LegalBenchClassification.json
+results/intfloat__multilingual-e5-small/Diversity6LegalBenchClassification.json
 results/intfloat__multilingual-e5-small/DutchBookReviewSentimentClassification.json
 results/intfloat__multilingual-e5-small/EstQA.json
 results/intfloat__multilingual-e5-small/EstonianValenceClassification.json
 results/intfloat__multilingual-e5-small/FQuADRetrieval.json
 results/intfloat__multilingual-e5-small/FaroeseSTS.json
 results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json
 results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json
 results/intfloat__multilingual-e5-small/FinParaSTS.json
 results/intfloat__multilingual-e5-small/FinToxicityClassification.json
 results/intfloat__multilingual-e5-small/FinancialPhrasebankClassification.json
 results/intfloat__multilingual-e5-small/FrenchBookReviews.json
 results/intfloat__multilingual-e5-small/FrenkEnClassification.json
 results/intfloat__multilingual-e5-small/FrenkHrClassification.json
 results/intfloat__multilingual-e5-small/FrenkSlClassification.json
+results/intfloat__multilingual-e5-small/FunctionOfDecisionSectionLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json
 results/intfloat__multilingual-e5-small/GeorgianSentimentClassification.json
 results/intfloat__multilingual-e5-small/GermanDPR.json
 results/intfloat__multilingual-e5-small/GermanPoliticiansTwitterSentimentClassification.json
 results/intfloat__multilingual-e5-small/GreekCivicsQA.json
 results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json
 results/intfloat__multilingual-e5-small/GujaratiNewsClassification.json
@@ -629,14 +639,15 @@
 results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json
 results/intfloat__multilingual-e5-small/IndicLangClassification.json
 results/intfloat__multilingual-e5-small/IndicQARetrieval.json
 results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json
 results/intfloat__multilingual-e5-small/IndicSentimentClassification.json
 results/intfloat__multilingual-e5-small/IndonesianIdClickbaitClassification.json
 results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json
+results/intfloat__multilingual-e5-small/InsurancePolicyInterpretationLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/InternationalCitizenshipQuestionsLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/IsiZuluNewsClassification.json
 results/intfloat__multilingual-e5-small/ItaCaseholdClassification.json
 results/intfloat__multilingual-e5-small/Itacola.json
 results/intfloat__multilingual-e5-small/JCrewBlockerLegalBenchClassification.json
 results/intfloat__multilingual-e5-small/JSTS.json
 results/intfloat__multilingual-e5-small/JaQuADRetrieval.json
@@ -737,23 +748,24 @@
 results/intfloat__multilingual-e5-small/VieMedEVBitextMining.json
 results/intfloat__multilingual-e5-small/VieQuADRetrieval.json
 results/intfloat__multilingual-e5-small/VieStudentFeedbackClassification.json
 results/intfloat__multilingual-e5-small/WRIMEClassification.json
 results/intfloat__multilingual-e5-small/WikiClusteringP2P.json
 results/intfloat__multilingual-e5-small/WisesightSentimentClassification.json
 results/intfloat__multilingual-e5-small/XNLI.json
-results/intfloat__multilingual-e5-small/XNLI2.json
+results/intfloat__multilingual-e5-small/XNLIV2.json
 results/intfloat__multilingual-e5-small/XQuADRetrieval.json
 results/intfloat__multilingual-e5-small/YahooAnswersTopicsClassification.json
 results/intfloat__multilingual-e5-small/YelpReviewFullClassification.json
 results/intfloat__multilingual-e5-small/YueOpenriceReviewClassification.json
 results/intfloat__multilingual-e5-small/model_meta.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/HinDialectClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/MalayalamNewsClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/OdiaNewsClassification.json
+results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SadeemQuestionRetrieval.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/SouthAfricanLangClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TamilNewsClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TeluguAndhraJyotiNewsClassification.json
 results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/TswanaNewsClassification.json
 results/sentence-transformers__all-MiniLM-L6-v2/Banking77Classification.json
@@ -845,15 +857,22 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ContractNLISurvivalOfObligationsLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CorporateLobbyingLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DBpediaClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DefinitionClassificationLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity1LegalBenchClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity2LegalBenchClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity3LegalBenchClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity4LegalBenchClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity5LegalBenchClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Diversity6LegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DutchBookReviewSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstonianValenceClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FaroeseSTS.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json
@@ -861,14 +880,15 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinToxicityClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinancialPhrasebankClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FloresClusteringS2S.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenchBookReviews.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkEnClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkHrClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FrenkSlClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FunctionOfDecisionSectionLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GermanPoliticiansTwitterSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GujaratiNewsClassification.json
@@ -881,14 +901,15 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicLangClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianIdClickbaitClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InsurancePolicyInterpretationLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/InternationalCitizenshipQuestionsLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IsiZuluNewsClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ItaCaseholdClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/Itacola.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JCrewBlockerLegalBenchClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JSTS.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json
@@ -991,15 +1012,15 @@
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieStudentFeedbackClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WRIMEClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiCitiesClustering.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WisesightSentimentClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json
-results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI2.json
+results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YahooAnswersTopicsClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YelpReviewFullClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/YueOpenriceReviewClassification.json
 results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/model_meta.json
 scripts/merge_cqadupstack.py
 scripts/mteb_meta.py
```

### Comparing `mteb-1.8.7/pyproject.toml` & `mteb-1.8.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.8.7"
+version = "1.8.8"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
```

### Comparing `mteb-1.8.7/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json` & `mteb-1.8.8/results/GritLM__GritLM-7B/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/GritLM__GritLM-7B/News21InstructionRetrieval.json` & `mteb-1.8.8/results/GritLM__GritLM-7B/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json` & `mteb-1.8.8/results/GritLM__GritLM-7B/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json` & `mteb-1.8.8/results/cross_encoder__ms-marco-TinyBERT-L-2-v2/NFCorpus.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AlloprofRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/AmazonReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPDomainClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MTOPIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveIntentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MassiveScenarioClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/MintakaRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/PawsX.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/SICKFr.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SICKFr.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/STSBenchmarkMultilingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json` & `mteb-1.8.8/results/dangvantuan/sentence-camembert-base/XPQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json` & `mteb-1.8.8/results/intfloat__e5-small-v2/Core17InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__e5-small-v2/News21InstructionRetrieval.json` & `mteb-1.8.8/results/intfloat__e5-small-v2/News21InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json` & `mteb-1.8.8/results/intfloat__e5-small-v2/Robust04InstructionRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-base/CroatianSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT19.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-base/CrossLingualSemanticDiscriminationWMT21.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-base/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-base/MalteseSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/ArmenianParaphrasePC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/ArxivClusteringP2P.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/BSARDRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/BSARDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/BibleNLPBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/BlurbsClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/CataloniaTweetClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeEditSearchRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT19.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/CrossLingualSemanticDiscriminationWMT21.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/DanFEVER.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/EstQA.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/FQuADRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoHateSpeechClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/FilipinoShopeeReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/FinParaSTS.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/FinParaSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/GeorgianFAQRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/GermanDPR.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/GermanDPR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/GreekCivicsQA.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekCivicsQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicCrosslingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicQARetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicReviewsClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndicSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/IndonesianMongabayConservationClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/LegalBenchPC.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/LegalBenchPC.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9665178571428572%*

 * *Differences: {"'test'": "{'cos_sim': {'accuracy': 0.5722713864306784, 'ap': 0.5233200465732908, 'f1': "*

 * *           "0.6295546558704453, 'f1_threshold': 0.7433135509490967, 'precision': "*

 * *           "0.46005917159763315, 'recall': 0.9967948717948718}, 'dot': {'accuracy': "*

 * *           "0.5722713864306784, 'ap': 0.5233224857880587, 'f1': 0.6295546558704453, "*

 * *           "'f1_threshold': 0.7433135509490967, 'precision': 0.46005917159763315, 'recall': "*

 * *           "0.9967948717948718}, 'euclidean': {'accuracy': 0.57227138643 […]*

```diff
@@ -1,49 +1,49 @@
 {
     "dataset_revision": "12ca3b695563788fead87a982ad1a068284413f4",
     "mteb_dataset_name": "LegalBenchPC",
     "mteb_version": "1.7.7",
     "test": {
         "cos_sim": {
-            "accuracy": 0.5736301369863014,
+            "accuracy": 0.5722713864306784,
             "accuracy_threshold": 0.872885525226593,
-            "ap": 0.5402842739866689,
-            "f1": 0.6346604215456675,
-            "f1_threshold": 0.751397430896759,
-            "precision": 0.4648370497427101,
-            "recall": 1.0
+            "ap": 0.5233200465732908,
+            "f1": 0.6295546558704453,
+            "f1_threshold": 0.7433135509490967,
+            "precision": 0.46005917159763315,
+            "recall": 0.9967948717948718
         },
         "dot": {
-            "accuracy": 0.5736301369863014,
+            "accuracy": 0.5722713864306784,
             "accuracy_threshold": 0.8728854656219482,
-            "ap": 0.5402842739866689,
-            "f1": 0.6346604215456675,
-            "f1_threshold": 0.7513974905014038,
-            "precision": 0.4648370497427101,
-            "recall": 1.0
+            "ap": 0.5233224857880587,
+            "f1": 0.6295546558704453,
+            "f1_threshold": 0.7433135509490967,
+            "precision": 0.46005917159763315,
+            "recall": 0.9967948717948718
         },
         "euclidean": {
-            "accuracy": 0.5736301369863014,
+            "accuracy": 0.5722713864306784,
             "accuracy_threshold": 0.5042111873626709,
-            "ap": 0.5402842739866689,
-            "f1": 0.6346604215456675,
-            "f1_threshold": 0.7051099538803101,
-            "precision": 0.4648370497427101,
-            "recall": 1.0
+            "ap": 0.5233200465732908,
+            "f1": 0.6295546558704453,
+            "f1_threshold": 0.7164959907531738,
+            "precision": 0.46005917159763315,
+            "recall": 0.9967948717948718
         },
-        "evaluation_time": 80.01,
+        "evaluation_time": 85.28,
         "manhattan": {
-            "accuracy": 0.5804794520547946,
+            "accuracy": 0.5781710914454278,
             "accuracy_threshold": 8.489166259765625,
-            "ap": 0.5412059665799563,
-            "f1": 0.6349206349206349,
-            "f1_threshold": 10.36783218383789,
-            "precision": 0.4744525547445255,
-            "recall": 0.959409594095941
+            "ap": 0.5241034805085035,
+            "f1": 0.6309403437815976,
+            "f1_threshold": 11.268424034118652,
+            "precision": 0.4608567208271787,
+            "recall": 1.0
         },
         "max": {
-            "accuracy": 0.5804794520547946,
-            "ap": 0.5412059665799563,
-            "f1": 0.6349206349206349
+            "accuracy": 0.5781710914454278,
+            "ap": 0.5241034805085035,
+            "f1": 0.6309403437815976
         }
     }
 }
```

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MLQARetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MLQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MLSUMClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MovieReviewSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MultiHateClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MultiHateClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/MultilingualSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/NTREXBitextMining.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/NTREXBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/PersianFoodSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/PlscClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SIB200Classification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SIB200Classification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SNLRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SRNCorpusBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SanskritShlokasClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SlovakSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SwednRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SwissJudgementClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/SyntecRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/SyntecRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TbilisiCityHallBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TenKGnadClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TurHistQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TweetSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/UkrFormalityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/XNLI.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLI.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/XNLI2.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/XNLIV2.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.591656037414966%*

 * *Differences: {"'dataset_revision'": "'c3a8ffbc19ab5d22b0958961490b4a5654b19d89'",*

 * * "'mteb_dataset_name'": "'XNLIV2'",*

 * * "'mteb_version'": "'1.8.0'",*

 * * "'test'": "{'assamese': {'cos_sim': {'ap': 0.6730718675189772, 'f1_threshold': "*

 * *           "0.8353620767593384}, 'dot': {'accuracy_threshold': 0.8617695569992065, 'f1_threshold': "*

 * *           "0.8353620171546936}, 'euclidean': {'accuracy_threshold': 0.5257953405380249, 'ap': "*

 * *           "0.6730718675189772, 'f1_threshold': 0.5738255977630615}, 'manhattan': "*

 * *           "{ […]*

```diff
@@ -1,46 +1,46 @@
 {
-    "dataset_revision": "1a3794e88c74db2a13aebc5e8abc3dc4312a7543",
-    "mteb_dataset_name": "XNLI2",
-    "mteb_version": "1.6.37",
+    "dataset_revision": "c3a8ffbc19ab5d22b0958961490b4a5654b19d89",
+    "mteb_dataset_name": "XNLIV2",
+    "mteb_version": "1.8.0",
     "test": {
         "assamese": {
             "cos_sim": {
                 "accuracy": 0.638095238095238,
                 "accuracy_threshold": 0.8617695569992065,
-                "ap": 0.6730718675189771,
+                "ap": 0.6730718675189772,
                 "f1": 0.7026713124274101,
-                "f1_threshold": 0.8353620171546936,
+                "f1_threshold": 0.8353620767593384,
                 "precision": 0.5817307692307693,
                 "recall": 0.8870967741935484
             },
             "dot": {
                 "accuracy": 0.638095238095238,
-                "accuracy_threshold": 0.8617696166038513,
+                "accuracy_threshold": 0.8617695569992065,
                 "ap": 0.6730718675189771,
                 "f1": 0.7026713124274101,
-                "f1_threshold": 0.8353620767593384,
+                "f1_threshold": 0.8353620171546936,
                 "precision": 0.5817307692307693,
                 "recall": 0.8870967741935484
             },
             "euclidean": {
                 "accuracy": 0.638095238095238,
-                "accuracy_threshold": 0.5257954597473145,
-                "ap": 0.6730718675189771,
+                "accuracy_threshold": 0.5257953405380249,
+                "ap": 0.6730718675189772,
                 "f1": 0.7026713124274101,
-                "f1_threshold": 0.5738257169723511,
+                "f1_threshold": 0.5738255977630615,
                 "precision": 0.5817307692307693,
                 "recall": 0.8870967741935484
             },
             "manhattan": {
                 "accuracy": 0.6366300366300366,
-                "accuracy_threshold": 8.027642250061035,
+                "accuracy_threshold": 8.027643203735352,
                 "ap": 0.6744995915704297,
                 "f1": 0.7005193306405079,
-                "f1_threshold": 8.922069549560547,
+                "f1_threshold": 8.922067642211914,
                 "precision": 0.5775451950523312,
                 "recall": 0.8900293255131965
             },
             "max": {
                 "accuracy": 0.638095238095238,
                 "ap": 0.6744995915704297,
                 "f1": 0.7026713124274101
@@ -54,123 +54,166 @@
                 "f1": 0.7117437722419928,
                 "f1_threshold": 0.8309766054153442,
                 "precision": 0.5976095617529881,
                 "recall": 0.8797653958944281
             },
             "dot": {
                 "accuracy": 0.6798534798534799,
-                "accuracy_threshold": 0.8565397262573242,
-                "ap": 0.7093293669269711,
+                "accuracy_threshold": 0.856539785861969,
+                "ap": 0.7093293669269709,
                 "f1": 0.7117437722419928,
                 "f1_threshold": 0.8309766054153442,
                 "precision": 0.5976095617529881,
                 "recall": 0.8797653958944281
             },
             "euclidean": {
                 "accuracy": 0.6798534798534799,
-                "accuracy_threshold": 0.5356496572494507,
+                "accuracy_threshold": 0.5356495380401611,
                 "ap": 0.7093293669269711,
                 "f1": 0.7117437722419928,
-                "f1_threshold": 0.581417977809906,
+                "f1_threshold": 0.5814179182052612,
                 "precision": 0.5976095617529881,
                 "recall": 0.8797653958944281
             },
             "manhattan": {
                 "accuracy": 0.6717948717948717,
-                "accuracy_threshold": 8.257460594177246,
+                "accuracy_threshold": 8.257458686828613,
                 "ap": 0.7075658858542314,
                 "f1": 0.7097844112769485,
-                "f1_threshold": 9.383186340332031,
+                "f1_threshold": 9.383184432983398,
                 "precision": 0.5696539485359361,
                 "recall": 0.9413489736070382
             },
             "max": {
                 "accuracy": 0.6798534798534799,
                 "ap": 0.7093293669269711,
                 "f1": 0.7117437722419928
             }
         },
         "bhojpuri": {
             "cos_sim": {
                 "accuracy": 0.6512820512820513,
                 "accuracy_threshold": 0.8608050346374512,
-                "ap": 0.7013897157128592,
+                "ap": 0.7013870459470882,
                 "f1": 0.7062857142857142,
-                "f1_threshold": 0.8388409614562988,
+                "f1_threshold": 0.8388410806655884,
                 "precision": 0.5786516853932584,
                 "recall": 0.906158357771261
             },
             "dot": {
                 "accuracy": 0.6512820512820513,
-                "accuracy_threshold": 0.8608050346374512,
+                "accuracy_threshold": 0.8608049750328064,
                 "ap": 0.701386259818611,
                 "f1": 0.7062857142857142,
                 "f1_threshold": 0.8388410210609436,
                 "precision": 0.5786516853932584,
                 "recall": 0.906158357771261
             },
             "euclidean": {
                 "accuracy": 0.6512820512820513,
-                "accuracy_threshold": 0.5276266932487488,
-                "ap": 0.701388929584382,
+                "accuracy_threshold": 0.527626633644104,
+                "ap": 0.7013870459470883,
                 "f1": 0.7062857142857142,
-                "f1_threshold": 0.5677306652069092,
+                "f1_threshold": 0.5677304863929749,
                 "precision": 0.5786516853932584,
                 "recall": 0.906158357771261
             },
             "manhattan": {
                 "accuracy": 0.6512820512820513,
                 "accuracy_threshold": 8.120187759399414,
                 "ap": 0.7000978943249034,
                 "f1": 0.7037457434733257,
-                "f1_threshold": 8.81391716003418,
+                "f1_threshold": 8.813915252685547,
                 "precision": 0.5740740740740741,
                 "recall": 0.9090909090909091
             },
             "max": {
                 "accuracy": 0.6512820512820513,
-                "ap": 0.7013897157128592,
+                "ap": 0.7013870459470883,
                 "f1": 0.7062857142857142
             }
         },
-        "evaluation_time": 74.54,
+        "evaluation_time": 174.31,
+        "greek": {
+            "cos_sim": {
+                "accuracy": 0.6490842490842491,
+                "accuracy_threshold": 0.9039740562438965,
+                "ap": 0.6865683319774634,
+                "f1": 0.6957494407158837,
+                "f1_threshold": 0.8623661994934082,
+                "precision": 0.5623869801084991,
+                "recall": 0.9120234604105572
+            },
+            "dot": {
+                "accuracy": 0.6490842490842491,
+                "accuracy_threshold": 0.9039740562438965,
+                "ap": 0.6865693171306013,
+                "f1": 0.6957494407158837,
+                "f1_threshold": 0.8623661994934082,
+                "precision": 0.5623869801084991,
+                "recall": 0.9120234604105572
+            },
+            "euclidean": {
+                "accuracy": 0.6490842490842491,
+                "accuracy_threshold": 0.43823719024658203,
+                "ap": 0.6865683319774634,
+                "f1": 0.6957494407158837,
+                "f1_threshold": 0.5246594548225403,
+                "precision": 0.5623869801084991,
+                "recall": 0.9120234604105572
+            },
+            "manhattan": {
+                "accuracy": 0.6461538461538462,
+                "accuracy_threshold": 6.934526443481445,
+                "ap": 0.6835689070233777,
+                "f1": 0.690450054884742,
+                "f1_threshold": 8.24932861328125,
+                "precision": 0.5517543859649123,
+                "recall": 0.9222873900293255
+            },
+            "max": {
+                "accuracy": 0.6490842490842491,
+                "ap": 0.6865693171306013,
+                "f1": 0.6957494407158837
+            }
+        },
         "gujrati": {
             "cos_sim": {
                 "accuracy": 0.6534798534798535,
                 "accuracy_threshold": 0.858397364616394,
                 "ap": 0.7037232662082877,
                 "f1": 0.7114942528735633,
                 "f1_threshold": 0.8226242065429688,
                 "precision": 0.5850661625708885,
                 "recall": 0.907624633431085
             },
             "dot": {
                 "accuracy": 0.6534798534798535,
                 "accuracy_threshold": 0.858397364616394,
-                "ap": 0.7037232662082875,
+                "ap": 0.7037232662082877,
                 "f1": 0.7114942528735633,
-                "f1_threshold": 0.822624146938324,
+                "f1_threshold": 0.8226242065429688,
                 "precision": 0.5850661625708885,
                 "recall": 0.907624633431085
             },
             "euclidean": {
                 "accuracy": 0.6534798534798535,
-                "accuracy_threshold": 0.532170295715332,
+                "accuracy_threshold": 0.5321701765060425,
                 "ap": 0.7037232662082877,
                 "f1": 0.7114942528735633,
                 "f1_threshold": 0.5956101417541504,
                 "precision": 0.5850661625708885,
                 "recall": 0.907624633431085
             },
             "manhattan": {
                 "accuracy": 0.652014652014652,
-                "accuracy_threshold": 8.676247596740723,
+                "accuracy_threshold": 8.676246643066406,
                 "ap": 0.7016562101100351,
                 "f1": 0.7071057192374349,
-                "f1_threshold": 9.18206787109375,
+                "f1_threshold": 9.182065963745117,
                 "precision": 0.5834127740705434,
                 "recall": 0.8973607038123167
             },
             "max": {
                 "accuracy": 0.6534798534798535,
                 "ap": 0.7037232662082877,
                 "f1": 0.7114942528735633
@@ -187,76 +230,76 @@
                 "recall": 0.906158357771261
             },
             "dot": {
                 "accuracy": 0.6673992673992674,
                 "accuracy_threshold": 0.8478111028671265,
                 "ap": 0.7148418788384423,
                 "f1": 0.7169373549883992,
-                "f1_threshold": 0.8258670568466187,
+                "f1_threshold": 0.8258669376373291,
                 "precision": 0.5930902111324377,
                 "recall": 0.906158357771261
             },
             "euclidean": {
                 "accuracy": 0.6673992673992674,
                 "accuracy_threshold": 0.5517044067382812,
                 "ap": 0.7148418788384423,
                 "f1": 0.7169373549883992,
-                "f1_threshold": 0.5901405215263367,
+                "f1_threshold": 0.5901404619216919,
                 "precision": 0.5930902111324377,
                 "recall": 0.906158357771261
             },
             "manhattan": {
                 "accuracy": 0.6615384615384615,
                 "accuracy_threshold": 8.537461280822754,
                 "ap": 0.7129574804232354,
                 "f1": 0.7105561861520999,
-                "f1_threshold": 9.28622817993164,
+                "f1_threshold": 9.286229133605957,
                 "precision": 0.5796296296296296,
                 "recall": 0.9178885630498533
             },
             "max": {
                 "accuracy": 0.6673992673992674,
                 "ap": 0.7148418788384423,
                 "f1": 0.7169373549883992
             }
         },
         "marathi": {
             "cos_sim": {
                 "accuracy": 0.6666666666666666,
-                "accuracy_threshold": 0.8576674461364746,
+                "accuracy_threshold": 0.8576675653457642,
                 "ap": 0.7210534315211277,
                 "f1": 0.7147766323024055,
                 "f1_threshold": 0.8252026438713074,
                 "precision": 0.5864661654135338,
                 "recall": 0.9149560117302052
             },
             "dot": {
                 "accuracy": 0.6666666666666666,
-                "accuracy_threshold": 0.8576675057411194,
+                "accuracy_threshold": 0.8576675653457642,
                 "ap": 0.7210534315211277,
                 "f1": 0.7147766323024055,
-                "f1_threshold": 0.8252027034759521,
+                "f1_threshold": 0.8252025842666626,
                 "precision": 0.5864661654135338,
                 "recall": 0.9149560117302052
             },
             "euclidean": {
                 "accuracy": 0.6666666666666666,
-                "accuracy_threshold": 0.5335400104522705,
+                "accuracy_threshold": 0.533539891242981,
                 "ap": 0.7210534315211277,
                 "f1": 0.7147766323024055,
                 "f1_threshold": 0.5912652015686035,
                 "precision": 0.5864661654135338,
                 "recall": 0.9149560117302052
             },
             "manhattan": {
                 "accuracy": 0.6622710622710622,
-                "accuracy_threshold": 8.451714515686035,
-                "ap": 0.7195599322365811,
+                "accuracy_threshold": 8.451715469360352,
+                "ap": 0.7195605634001658,
                 "f1": 0.717626925270964,
-                "f1_threshold": 9.201488494873047,
+                "f1_threshold": 9.201489448547363,
                 "precision": 0.5873015873015873,
                 "recall": 0.9222873900293255
             },
             "max": {
                 "accuracy": 0.6666666666666666,
                 "ap": 0.7210534315211277,
                 "f1": 0.717626925270964
@@ -270,169 +313,255 @@
                 "f1": 0.701098901098901,
                 "f1_threshold": 0.8265218138694763,
                 "precision": 0.5606326889279437,
                 "recall": 0.9354838709677419
             },
             "dot": {
                 "accuracy": 0.638095238095238,
-                "accuracy_threshold": 0.8649595379829407,
+                "accuracy_threshold": 0.8649595975875854,
                 "ap": 0.6871482867115513,
                 "f1": 0.701098901098901,
-                "f1_threshold": 0.8265218138694763,
+                "f1_threshold": 0.8265218734741211,
                 "precision": 0.5606326889279437,
                 "recall": 0.9354838709677419
             },
             "euclidean": {
                 "accuracy": 0.638095238095238,
                 "accuracy_threshold": 0.5196930170059204,
                 "ap": 0.6871482867115513,
                 "f1": 0.701098901098901,
                 "f1_threshold": 0.5890300273895264,
                 "precision": 0.5606326889279437,
                 "recall": 0.9354838709677419
             },
             "manhattan": {
                 "accuracy": 0.6336996336996337,
-                "accuracy_threshold": 8.162399291992188,
-                "ap": 0.6875816583031257,
+                "accuracy_threshold": 8.162397384643555,
+                "ap": 0.6875816583031258,
                 "f1": 0.7000550357732526,
                 "f1_threshold": 9.133846282958984,
                 "precision": 0.560352422907489,
                 "recall": 0.9325513196480938
             },
             "max": {
                 "accuracy": 0.638095238095238,
-                "ap": 0.6875816583031257,
+                "ap": 0.6875816583031258,
                 "f1": 0.701098901098901
             }
         },
         "punjabi": {
             "cos_sim": {
                 "accuracy": 0.6586080586080586,
                 "accuracy_threshold": 0.8369609117507935,
-                "ap": 0.7124114890058897,
+                "ap": 0.7124114890058898,
                 "f1": 0.7171411265899456,
-                "f1_threshold": 0.8335449695587158,
+                "f1_threshold": 0.8335450887680054,
                 "precision": 0.6109391124871001,
                 "recall": 0.8680351906158358
             },
             "dot": {
                 "accuracy": 0.6586080586080586,
                 "accuracy_threshold": 0.8369609117507935,
                 "ap": 0.7124123874325822,
                 "f1": 0.7171411265899456,
-                "f1_threshold": 0.8335450291633606,
+                "f1_threshold": 0.8335451483726501,
                 "precision": 0.6109391124871001,
                 "recall": 0.8680351906158358
             },
             "euclidean": {
                 "accuracy": 0.6586080586080586,
-                "accuracy_threshold": 0.5710324048995972,
+                "accuracy_threshold": 0.5710324645042419,
                 "ap": 0.7124114890058897,
                 "f1": 0.7171411265899456,
-                "f1_threshold": 0.5769834518432617,
+                "f1_threshold": 0.5769832730293274,
                 "precision": 0.6109391124871001,
                 "recall": 0.8680351906158358
             },
             "manhattan": {
                 "accuracy": 0.6512820512820513,
-                "accuracy_threshold": 7.766175270080566,
+                "accuracy_threshold": 7.766173362731934,
                 "ap": 0.7105645757339836,
                 "f1": 0.7086330935251799,
-                "f1_threshold": 8.973298072814941,
+                "f1_threshold": 8.973297119140625,
                 "precision": 0.5993914807302231,
                 "recall": 0.8665689149560117
             },
             "max": {
                 "accuracy": 0.6586080586080586,
                 "ap": 0.7124123874325822,
                 "f1": 0.7171411265899456
             }
         },
+        "russian": {
+            "cos_sim": {
+                "accuracy": 0.6981684981684981,
+                "accuracy_threshold": 0.8810277581214905,
+                "ap": 0.7476236112991022,
+                "f1": 0.7207207207207208,
+                "f1_threshold": 0.8686713576316833,
+                "precision": 0.6422018348623854,
+                "recall": 0.8211143695014663
+            },
+            "dot": {
+                "accuracy": 0.6981684981684981,
+                "accuracy_threshold": 0.8810278177261353,
+                "ap": 0.7476236112991022,
+                "f1": 0.7207207207207208,
+                "f1_threshold": 0.8686714172363281,
+                "precision": 0.6422018348623854,
+                "recall": 0.8211143695014663
+            },
+            "euclidean": {
+                "accuracy": 0.6981684981684981,
+                "accuracy_threshold": 0.48779553174972534,
+                "ap": 0.7476236112991022,
+                "f1": 0.7207207207207208,
+                "f1_threshold": 0.5125008821487427,
+                "precision": 0.6422018348623854,
+                "recall": 0.8211143695014663
+            },
+            "manhattan": {
+                "accuracy": 0.6959706959706959,
+                "accuracy_threshold": 7.493196487426758,
+                "ap": 0.7446821075264964,
+                "f1": 0.71875,
+                "f1_threshold": 8.217985153198242,
+                "precision": 0.6089613034623218,
+                "recall": 0.8768328445747801
+            },
+            "max": {
+                "accuracy": 0.6981684981684981,
+                "ap": 0.7476236112991022,
+                "f1": 0.7207207207207208
+            }
+        },
         "sanskrit": {
             "cos_sim": {
                 "accuracy": 0.6410256410256411,
                 "accuracy_threshold": 0.8779851198196411,
-                "ap": 0.665944784062027,
+                "ap": 0.6659461391167943,
                 "f1": 0.7052023121387284,
                 "f1_threshold": 0.8529165983200073,
                 "precision": 0.5820610687022901,
                 "recall": 0.8944281524926686
             },
             "dot": {
                 "accuracy": 0.6410256410256411,
-                "accuracy_threshold": 0.8779852390289307,
-                "ap": 0.6659461391167943,
+                "accuracy_threshold": 0.8779851794242859,
+                "ap": 0.6659439513339602,
                 "f1": 0.7052023121387284,
-                "f1_threshold": 0.8529165387153625,
+                "f1_threshold": 0.8529164791107178,
                 "precision": 0.5820610687022901,
                 "recall": 0.8944281524926686
             },
             "euclidean": {
                 "accuracy": 0.6410256410256411,
                 "accuracy_threshold": 0.4939935803413391,
-                "ap": 0.6659437149180529,
+                "ap": 0.6659461391167943,
                 "f1": 0.7052023121387284,
                 "f1_threshold": 0.5423715114593506,
                 "precision": 0.5820610687022901,
                 "recall": 0.8944281524926686
             },
             "manhattan": {
                 "accuracy": 0.638095238095238,
-                "accuracy_threshold": 7.559727668762207,
+                "accuracy_threshold": 7.559725284576416,
                 "ap": 0.666890440556938,
                 "f1": 0.7060869565217391,
-                "f1_threshold": 8.41229248046875,
+                "f1_threshold": 8.412291526794434,
                 "precision": 0.5838926174496645,
                 "recall": 0.8929618768328446
             },
             "max": {
                 "accuracy": 0.6410256410256411,
                 "ap": 0.666890440556938,
                 "f1": 0.7060869565217391
             }
         },
         "tamil": {
             "cos_sim": {
                 "accuracy": 0.6754578754578755,
-                "accuracy_threshold": 0.8529529571533203,
+                "accuracy_threshold": 0.8529530167579651,
                 "ap": 0.7217046279510617,
                 "f1": 0.7148548662492885,
                 "f1_threshold": 0.8228673338890076,
                 "precision": 0.5841860465116279,
                 "recall": 0.9208211143695014
             },
             "dot": {
                 "accuracy": 0.6754578754578755,
                 "accuracy_threshold": 0.8529529571533203,
                 "ap": 0.7217046279510617,
                 "f1": 0.7148548662492885,
-                "f1_threshold": 0.8228673934936523,
+                "f1_threshold": 0.8228672742843628,
                 "precision": 0.5841860465116279,
                 "recall": 0.9208211143695014
             },
             "euclidean": {
                 "accuracy": 0.6754578754578755,
-                "accuracy_threshold": 0.5423041582107544,
+                "accuracy_threshold": 0.5423040390014648,
                 "ap": 0.7217046279510617,
                 "f1": 0.7148548662492885,
-                "f1_threshold": 0.595201849937439,
+                "f1_threshold": 0.5952019095420837,
                 "precision": 0.5841860465116279,
                 "recall": 0.9208211143695014
             },
             "manhattan": {
                 "accuracy": 0.6725274725274726,
-                "accuracy_threshold": 8.458455085754395,
+                "accuracy_threshold": 8.458454132080078,
                 "ap": 0.7205209069368703,
                 "f1": 0.7115264797507789,
-                "f1_threshold": 8.803674697875977,
+                "f1_threshold": 8.80367374420166,
                 "precision": 0.6186348862405201,
                 "recall": 0.8372434017595308
             },
             "max": {
                 "accuracy": 0.6754578754578755,
                 "ap": 0.7217046279510617,
                 "f1": 0.7148548662492885
             }
+        },
+        "turkish": {
+            "cos_sim": {
+                "accuracy": 0.643956043956044,
+                "accuracy_threshold": 0.8897090554237366,
+                "ap": 0.6882866877028895,
+                "f1": 0.7060830017055145,
+                "f1_threshold": 0.8627848625183105,
+                "precision": 0.5766016713091922,
+                "recall": 0.9105571847507331
+            },
+            "dot": {
+                "accuracy": 0.643956043956044,
+                "accuracy_threshold": 0.8897090554237366,
+                "ap": 0.6882866877028895,
+                "f1": 0.7060830017055145,
+                "f1_threshold": 0.8627848625183105,
+                "precision": 0.5766016713091922,
+                "recall": 0.9105571847507331
+            },
+            "euclidean": {
+                "accuracy": 0.643956043956044,
+                "accuracy_threshold": 0.46966150403022766,
+                "ap": 0.6882866877028895,
+                "f1": 0.7060830017055145,
+                "f1_threshold": 0.5238609910011292,
+                "precision": 0.5766016713091922,
+                "recall": 0.9105571847507331
+            },
+            "manhattan": {
+                "accuracy": 0.6417582417582418,
+                "accuracy_threshold": 7.348048210144043,
+                "ap": 0.6832081694870337,
+                "f1": 0.7034242600116076,
+                "f1_threshold": 8.027097702026367,
+                "precision": 0.5821325648414986,
+                "recall": 0.8885630498533724
+            },
+            "max": {
+                "accuracy": 0.643956043956044,
+                "ap": 0.6882866877028895,
+                "f1": 0.7060830017055145
+            }
         }
     }
 }
```

### Comparing `mteb-1.8.7/results/intfloat__multilingual-e5-small/XQuADRetrieval.json` & `mteb-1.8.8/results/intfloat__multilingual-e5-small/XQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json` & `mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_fast.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json` & `mteb-1.8.8/results/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2/Tatoeba_slow.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NTREXBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__all-MiniLM-L6-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArmenianParaphrasePC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/ArxivClusteringP2P.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BSARDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BUCC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BibleNLPBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/BlurbsClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CataloniaTweetClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeEditSearchRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CodeSearchNetRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT19.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CrossLingualSemanticDiscriminationWMT21.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/CzechSubjectivityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DanFEVER.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/DiaBlaBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/EstQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoHateSpeechClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FilipinoShopeeReviewsClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/FinParaSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GeorgianFAQRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GerDaLIR.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekCivicsQA.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/GreekLegalCodeClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/HunSum2AbstractiveRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22ConvBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IN22GenBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicCrosslingualSTS.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicReviewsClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndicSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/IndonesianMongabayConservationClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/JaQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNarrativeQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBNeedleRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBPasskeyRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBQMSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBSummScreenFDRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LEMBWikimQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/LegalBenchPC.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TweetSentimentClassification.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5044642857142857%*

 * *Differences: {"'dataset_revision'": "'14b13edfbc4046892f6011d114c29c0f83170589'",*

 * * "'mteb_dataset_name'": "'TweetSentimentClassification'",*

 * * "'mteb_version'": "'1.7.40'",*

 * * "'test'": "{'evaluation_time': 9.35, 'arabic': OrderedDict([('accuracy', 0.428125), "*

 * *           "('accuracy_stderr', 0.03644344934278313), ('f1', 0.4150515354479289), ('f1_stderr', "*

 * *           "0.042044791973811474), ('main_score', 0.428125)]), 'english': "*

 * *           "OrderedDict([('accuracy', 0.4640625), ('accuracy_stderr', 0.03897646776020757), ( […]*

```diff
@@ -1,49 +1,64 @@
 {
-    "dataset_revision": "12ca3b695563788fead87a982ad1a068284413f4",
-    "mteb_dataset_name": "LegalBenchPC",
-    "mteb_version": "1.7.7",
+    "dataset_revision": "14b13edfbc4046892f6011d114c29c0f83170589",
+    "mteb_dataset_name": "TweetSentimentClassification",
+    "mteb_version": "1.7.40",
     "test": {
-        "cos_sim": {
-            "accuracy": 0.5787671232876712,
-            "accuracy_threshold": 0.5056948065757751,
-            "ap": 0.5402065162027007,
-            "f1": 0.6338028169014085,
-            "f1_threshold": -0.04414784908294678,
-            "precision": 0.46471600688468157,
-            "recall": 0.996309963099631
-        },
-        "dot": {
-            "accuracy": 0.5873287671232876,
-            "accuracy_threshold": 9.095282554626465,
-            "ap": 0.5542338305178248,
-            "f1": 0.6330597889800704,
-            "f1_threshold": -1.3291501998901367,
-            "precision": 0.4639175257731959,
-            "recall": 0.996309963099631
-        },
-        "euclidean": {
-            "accuracy": 0.5616438356164384,
-            "accuracy_threshold": 3.218596935272217,
-            "ap": 0.5370663976538543,
-            "f1": 0.6323185011709602,
-            "f1_threshold": 6.803489685058594,
-            "precision": 0.4631217838765009,
-            "recall": 0.996309963099631
-        },
-        "evaluation_time": 32.4,
-        "manhattan": {
-            "accuracy": 0.559931506849315,
-            "accuracy_threshold": 49.70074462890625,
-            "ap": 0.534497153521956,
-            "f1": 0.6323185011709602,
-            "f1_threshold": 106.46473693847656,
-            "precision": 0.4631217838765009,
-            "recall": 0.996309963099631
-        },
-        "max": {
-            "accuracy": 0.5873287671232876,
-            "ap": 0.5542338305178248,
-            "f1": 0.6338028169014085
+        "arabic": {
+            "accuracy": 0.428125,
+            "accuracy_stderr": 0.03644344934278313,
+            "f1": 0.4150515354479289,
+            "f1_stderr": 0.042044791973811474,
+            "main_score": 0.428125
+        },
+        "english": {
+            "accuracy": 0.4640625,
+            "accuracy_stderr": 0.03897646776020757,
+            "f1": 0.4526982107712719,
+            "f1_stderr": 0.03476162212189228,
+            "main_score": 0.4640625
+        },
+        "evaluation_time": 9.35,
+        "french": {
+            "accuracy": 0.44765625,
+            "accuracy_stderr": 0.03278458634118326,
+            "f1": 0.4435231069614679,
+            "f1_stderr": 0.034001046922440895,
+            "main_score": 0.44765625
+        },
+        "german": {
+            "accuracy": 0.496875,
+            "accuracy_stderr": 0.04677071733467427,
+            "f1": 0.49158929944119245,
+            "f1_stderr": 0.04940566081017425,
+            "main_score": 0.496875
+        },
+        "hindi": {
+            "accuracy": 0.348828125,
+            "accuracy_stderr": 0.035071512461371336,
+            "f1": 0.3405460869610343,
+            "f1_stderr": 0.03555657925349932,
+            "main_score": 0.348828125
+        },
+        "italian": {
+            "accuracy": 0.47734375,
+            "accuracy_stderr": 0.06163463413536256,
+            "f1": 0.47508665894167024,
+            "f1_stderr": 0.06221424083081577,
+            "main_score": 0.47734375
+        },
+        "portuguese": {
+            "accuracy": 0.433984375,
+            "accuracy_stderr": 0.034958209565359964,
+            "f1": 0.42976637947800683,
+            "f1_stderr": 0.03371352482544993,
+            "main_score": 0.433984375
+        },
+        "spanish": {
+            "accuracy": 0.448828125,
+            "accuracy_stderr": 0.04046128369831616,
+            "f1": 0.44069230613856447,
+            "f1_stderr": 0.04471458030498882,
+            "main_score": 0.448828125
         }
     }
 }
```

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MLSUMClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MedicalQARetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MovieReviewSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiHateClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultiScalaClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/MultilingualSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NTREXBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2022Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NeuCLIR2023Retrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/NorQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/OpusparcusPC.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PawsX.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PersianFoodSentimentClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/PlscClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SIB200Classification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SNLRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SRNCorpusBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SanskritShlokasClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SlovakSumRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SweFaqRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwednRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/SwissJudgementClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TV2Nordretrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TbilisiCityHallBitextMining.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TenKGnadClusteringS2S.v2.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TurHistQuadRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/TwitterHjerneRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/UkrFormalityClassification.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/VieQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/WikiClusteringP2P.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLI2.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XNLIV2.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.591454081632653%*

 * *Differences: {"'dataset_revision'": "'c3a8ffbc19ab5d22b0958961490b4a5654b19d89'",*

 * * "'mteb_dataset_name'": "'XNLIV2'",*

 * * "'mteb_version'": "'1.8.0'",*

 * * "'test'": "{'assamese': {'cos_sim': {'accuracy_threshold': 0.7693372368812561, 'f1_threshold': "*

 * *           "0.05036741495132446}, 'dot': {'accuracy_threshold': 2.2226834297180176, "*

 * *           "'f1_threshold': 1.3805371522903442}, 'euclidean': {'accuracy_threshold': "*

 * *           "1.7874953746795654, 'f1_threshold': 6.081642150878906}, 'manhattan': "*

 * *           "{'accuracy_ […]*

```diff
@@ -1,86 +1,86 @@
 {
-    "dataset_revision": "1a3794e88c74db2a13aebc5e8abc3dc4312a7543",
-    "mteb_dataset_name": "XNLI2",
-    "mteb_version": "1.6.37",
+    "dataset_revision": "c3a8ffbc19ab5d22b0958961490b4a5654b19d89",
+    "mteb_dataset_name": "XNLIV2",
+    "mteb_version": "1.8.0",
     "test": {
         "assamese": {
             "cos_sim": {
                 "accuracy": 0.5472527472527473,
-                "accuracy_threshold": 0.7693371772766113,
+                "accuracy_threshold": 0.7693372368812561,
                 "ap": 0.5445644825866423,
                 "f1": 0.6669926650366748,
-                "f1_threshold": 0.050367385149002075,
+                "f1_threshold": 0.05036741495132446,
                 "precision": 0.5003668378576669,
                 "recall": 1.0
             },
             "dot": {
                 "accuracy": 0.536996336996337,
-                "accuracy_threshold": 2.2226829528808594,
+                "accuracy_threshold": 2.2226834297180176,
                 "ap": 0.5245164005991778,
                 "f1": 0.6699751861042185,
-                "f1_threshold": 1.3805397748947144,
+                "f1_threshold": 1.3805371522903442,
                 "precision": 0.5063765941485371,
                 "recall": 0.9897360703812317
             },
             "euclidean": {
                 "accuracy": 0.5428571428571428,
-                "accuracy_threshold": 1.7874946594238281,
+                "accuracy_threshold": 1.7874953746795654,
                 "ap": 0.5504693581663612,
                 "f1": 0.6660146699266504,
-                "f1_threshold": 6.081643581390381,
+                "f1_threshold": 6.081642150878906,
                 "precision": 0.4996331621423331,
                 "recall": 0.998533724340176
             },
             "manhattan": {
                 "accuracy": 0.5435897435897435,
-                "accuracy_threshold": 26.327974319458008,
+                "accuracy_threshold": 26.32797622680664,
                 "ap": 0.551091667607061,
                 "f1": 0.6660146699266504,
-                "f1_threshold": 93.4553451538086,
+                "f1_threshold": 93.455322265625,
                 "precision": 0.4996331621423331,
                 "recall": 0.998533724340176
             },
             "max": {
                 "accuracy": 0.5472527472527473,
                 "ap": 0.551091667607061,
                 "f1": 0.6699751861042185
             }
         },
         "bengali": {
             "cos_sim": {
                 "accuracy": 0.5663003663003663,
-                "accuracy_threshold": 0.48992347717285156,
+                "accuracy_threshold": 0.4899238049983978,
                 "ap": 0.5635239433141879,
                 "f1": 0.6706290242694403,
-                "f1_threshold": 0.0879027247428894,
+                "f1_threshold": 0.08790278434753418,
                 "precision": 0.506357516828721,
                 "recall": 0.9926686217008798
             },
             "dot": {
                 "accuracy": 0.5699633699633699,
-                "accuracy_threshold": 2.366478443145752,
+                "accuracy_threshold": 2.3664767742156982,
                 "ap": 0.5445077899345492,
                 "f1": 0.6740623349181193,
-                "f1_threshold": 1.4896223545074463,
+                "f1_threshold": 1.4896219968795776,
                 "precision": 0.5268373245251858,
                 "recall": 0.9354838709677419
             },
             "euclidean": {
                 "accuracy": 0.5435897435897435,
-                "accuracy_threshold": 1.8956698179244995,
+                "accuracy_threshold": 1.8956701755523682,
                 "ap": 0.5458683601104932,
                 "f1": 0.6660137120470128,
-                "f1_threshold": 6.415295124053955,
+                "f1_threshold": 6.415295600891113,
                 "precision": 0.5,
                 "recall": 0.9970674486803519
             },
             "manhattan": {
                 "accuracy": 0.5413919413919414,
-                "accuracy_threshold": 26.73360824584961,
+                "accuracy_threshold": 26.733631134033203,
                 "ap": 0.5461459810463395,
                 "f1": 0.6660137120470128,
                 "f1_threshold": 98.31781005859375,
                 "precision": 0.5,
                 "recall": 0.9970674486803519
             },
             "max": {
@@ -88,175 +88,218 @@
                 "ap": 0.5635239433141879,
                 "f1": 0.6740623349181193
             }
         },
         "bhojpuri": {
             "cos_sim": {
                 "accuracy": 0.6476190476190476,
-                "accuracy_threshold": 0.571101725101471,
+                "accuracy_threshold": 0.5711019039154053,
                 "ap": 0.6691262376054212,
                 "f1": 0.6823821339950372,
-                "f1_threshold": 0.4622383415699005,
+                "f1_threshold": 0.4622385501861572,
                 "precision": 0.5913978494623656,
                 "recall": 0.8064516129032258
             },
             "dot": {
                 "accuracy": 0.6161172161172161,
-                "accuracy_threshold": 5.594806671142578,
+                "accuracy_threshold": 5.594807147979736,
                 "ap": 0.6195101641149054,
                 "f1": 0.6768138001014713,
-                "f1_threshold": 1.6663808822631836,
+                "f1_threshold": 1.6663817167282104,
                 "precision": 0.517455391776571,
                 "recall": 0.9780058651026393
             },
             "euclidean": {
                 "accuracy": 0.5970695970695971,
-                "accuracy_threshold": 3.145210027694702,
-                "ap": 0.6321895885541609,
+                "accuracy_threshold": 3.1452102661132812,
+                "ap": 0.6321875603051037,
                 "f1": 0.6816932380428807,
-                "f1_threshold": 3.669229030609131,
+                "f1_threshold": 3.66922926902771,
                 "precision": 0.5452946350043976,
                 "recall": 0.9090909090909091
             },
             "manhattan": {
                 "accuracy": 0.5978021978021978,
-                "accuracy_threshold": 47.76917266845703,
+                "accuracy_threshold": 47.76918029785156,
                 "ap": 0.6318463271798119,
                 "f1": 0.6807359307359307,
-                "f1_threshold": 58.23374938964844,
+                "f1_threshold": 58.23375701904297,
                 "precision": 0.5394511149228131,
                 "recall": 0.9222873900293255
             },
             "max": {
                 "accuracy": 0.6476190476190476,
                 "ap": 0.6691262376054212,
                 "f1": 0.6823821339950372
             }
         },
-        "evaluation_time": 72.0,
+        "evaluation_time": 169.31,
+        "greek": {
+            "cos_sim": {
+                "accuracy": 0.7553113553113553,
+                "accuracy_threshold": 0.5415382385253906,
+                "ap": 0.809763134795446,
+                "f1": 0.7775577557755774,
+                "f1_threshold": 0.516772985458374,
+                "precision": 0.7070828331332533,
+                "recall": 0.8636363636363636
+            },
+            "dot": {
+                "accuracy": 0.7120879120879121,
+                "accuracy_threshold": 8.467190742492676,
+                "ap": 0.7488327533282937,
+                "f1": 0.7473487211478477,
+                "f1_threshold": 6.983940124511719,
+                "precision": 0.6503800217155266,
+                "recall": 0.8782991202346041
+            },
+            "euclidean": {
+                "accuracy": 0.7450549450549451,
+                "accuracy_threshold": 3.8312158584594727,
+                "ap": 0.7911813338826728,
+                "f1": 0.7644683714670256,
+                "f1_threshold": 3.850269317626953,
+                "precision": 0.7064676616915423,
+                "recall": 0.8328445747800587
+            },
+            "manhattan": {
+                "accuracy": 0.7435897435897436,
+                "accuracy_threshold": 56.99772262573242,
+                "ap": 0.7898787764422444,
+                "f1": 0.7645536869340233,
+                "f1_threshold": 61.499656677246094,
+                "precision": 0.6840277777777778,
+                "recall": 0.8665689149560117
+            },
+            "max": {
+                "accuracy": 0.7553113553113553,
+                "ap": 0.809763134795446,
+                "f1": 0.7775577557755774
+            }
+        },
         "gujrati": {
             "cos_sim": {
                 "accuracy": 0.676923076923077,
-                "accuracy_threshold": 0.5593810081481934,
+                "accuracy_threshold": 0.5593808889389038,
                 "ap": 0.7161662651788183,
                 "f1": 0.7121771217712177,
-                "f1_threshold": 0.3808695375919342,
+                "f1_threshold": 0.38086968660354614,
                 "precision": 0.6133474576271186,
                 "recall": 0.8489736070381232
             },
             "dot": {
                 "accuracy": 0.6278388278388278,
                 "accuracy_threshold": 5.026564598083496,
-                "ap": 0.6670597222971537,
+                "ap": 0.6670603254183737,
                 "f1": 0.6912642430819316,
-                "f1_threshold": 2.5369977951049805,
+                "f1_threshold": 2.5369999408721924,
                 "precision": 0.5486649440137812,
                 "recall": 0.9340175953079178
             },
             "euclidean": {
                 "accuracy": 0.6681318681318681,
-                "accuracy_threshold": 3.4943923950195312,
-                "ap": 0.6785630031998113,
+                "accuracy_threshold": 3.494391441345215,
+                "ap": 0.6785638807029948,
                 "f1": 0.6924882629107981,
-                "f1_threshold": 4.235073566436768,
+                "f1_threshold": 4.235074043273926,
                 "precision": 0.5772994129158513,
                 "recall": 0.8651026392961877
             },
             "manhattan": {
                 "accuracy": 0.6659340659340659,
-                "accuracy_threshold": 54.415802001953125,
+                "accuracy_threshold": 54.415809631347656,
                 "ap": 0.6769154756045737,
                 "f1": 0.692992213570634,
-                "f1_threshold": 69.65553283691406,
+                "f1_threshold": 69.65550231933594,
                 "precision": 0.5582437275985663,
                 "recall": 0.9134897360703812
             },
             "max": {
                 "accuracy": 0.676923076923077,
                 "ap": 0.7161662651788183,
                 "f1": 0.7121771217712177
             }
         },
         "kannada": {
             "cos_sim": {
                 "accuracy": 0.5230769230769231,
-                "accuracy_threshold": 0.6138522624969482,
+                "accuracy_threshold": 0.6138523817062378,
                 "ap": 0.5042982302588335,
                 "f1": 0.6673257538309442,
-                "f1_threshold": 0.2575363516807556,
+                "f1_threshold": 0.25753629207611084,
                 "precision": 0.5033557046979866,
                 "recall": 0.9897360703812317
             },
             "dot": {
                 "accuracy": 0.5062271062271062,
                 "accuracy_threshold": 32.45844268798828,
                 "ap": 0.48819366741455483,
                 "f1": 0.6669926650366748,
-                "f1_threshold": 0.5589466094970703,
+                "f1_threshold": 0.5589467287063599,
                 "precision": 0.5003668378576669,
                 "recall": 1.0
             },
             "euclidean": {
                 "accuracy": 0.5172161172161173,
-                "accuracy_threshold": 2.4965827465057373,
+                "accuracy_threshold": 2.496582508087158,
                 "ap": 0.5125625690057163,
                 "f1": 0.6673238048299656,
-                "f1_threshold": 5.243943214416504,
+                "f1_threshold": 5.243943691253662,
                 "precision": 0.5025983667409057,
                 "recall": 0.9926686217008798
             },
             "manhattan": {
                 "accuracy": 0.5186813186813187,
-                "accuracy_threshold": 40.778953552246094,
+                "accuracy_threshold": 40.77893829345703,
                 "ap": 0.5128804622935561,
                 "f1": 0.6676499508357914,
-                "f1_threshold": 84.32908630371094,
+                "f1_threshold": 84.32909393310547,
                 "precision": 0.5022189349112426,
                 "recall": 0.9956011730205279
             },
             "max": {
                 "accuracy": 0.5230769230769231,
                 "ap": 0.5128804622935561,
                 "f1": 0.6676499508357914
             }
         },
         "marathi": {
             "cos_sim": {
                 "accuracy": 0.7054945054945055,
-                "accuracy_threshold": 0.5290974378585815,
+                "accuracy_threshold": 0.529097318649292,
                 "ap": 0.7687114735850316,
                 "f1": 0.7277486910994764,
-                "f1_threshold": 0.44833582639694214,
+                "f1_threshold": 0.4483357071876526,
                 "precision": 0.6572104018912529,
                 "recall": 0.8152492668621701
             },
             "dot": {
                 "accuracy": 0.6454212454212455,
-                "accuracy_threshold": 6.3349199295043945,
+                "accuracy_threshold": 6.334921836853027,
                 "ap": 0.6840399057545968,
                 "f1": 0.6903835464146748,
-                "f1_threshold": 2.933309555053711,
+                "f1_threshold": 2.9333088397979736,
                 "precision": 0.5559534467323187,
                 "recall": 0.9105571847507331
             },
             "euclidean": {
                 "accuracy": 0.706959706959707,
-                "accuracy_threshold": 3.4942715167999268,
-                "ap": 0.7370709259382664,
+                "accuracy_threshold": 3.4942712783813477,
+                "ap": 0.7370715106002214,
                 "f1": 0.7163798597833015,
-                "f1_threshold": 3.8744213581085205,
+                "f1_threshold": 3.874422073364258,
                 "precision": 0.6335963923337091,
                 "recall": 0.8240469208211144
             },
             "manhattan": {
                 "accuracy": 0.7018315018315018,
-                "accuracy_threshold": 54.511260986328125,
+                "accuracy_threshold": 54.511253356933594,
                 "ap": 0.7362211388483443,
                 "f1": 0.7142857142857144,
-                "f1_threshold": 56.44367980957031,
+                "f1_threshold": 56.44368362426758,
                 "precision": 0.6776315789473685,
                 "recall": 0.7551319648093842
             },
             "max": {
                 "accuracy": 0.706959706959707,
                 "ap": 0.7687114735850316,
                 "f1": 0.7277486910994764
@@ -270,27 +313,27 @@
                 "f1": 0.6731875719217492,
                 "f1_threshold": 0.3742383122444153,
                 "precision": 0.5539772727272727,
                 "recall": 0.8577712609970675
             },
             "dot": {
                 "accuracy": 0.6146520146520147,
-                "accuracy_threshold": 3.77984619140625,
+                "accuracy_threshold": 3.7798449993133545,
                 "ap": 0.5905332630219975,
                 "f1": 0.6798927613941018,
-                "f1_threshold": 2.2372069358825684,
+                "f1_threshold": 2.2372066974639893,
                 "precision": 0.5359256128486898,
                 "recall": 0.9296187683284457
             },
             "euclidean": {
                 "accuracy": 0.6131868131868132,
                 "accuracy_threshold": 2.6283605098724365,
                 "ap": 0.6165891889083529,
                 "f1": 0.6660146699266504,
-                "f1_threshold": 6.748752117156982,
+                "f1_threshold": 6.748752593994141,
                 "precision": 0.4996331621423331,
                 "recall": 0.998533724340176
             },
             "manhattan": {
                 "accuracy": 0.613919413919414,
                 "accuracy_threshold": 35.878814697265625,
                 "ap": 0.6163234160760352,
@@ -304,135 +347,221 @@
                 "ap": 0.6186211912945951,
                 "f1": 0.6798927613941018
             }
         },
         "punjabi": {
             "cos_sim": {
                 "accuracy": 0.550915750915751,
-                "accuracy_threshold": 0.47661083936691284,
+                "accuracy_threshold": 0.4766108989715576,
                 "ap": 0.5116763111650886,
                 "f1": 0.6748216106014272,
-                "f1_threshold": 0.24432814121246338,
+                "f1_threshold": 0.24432802200317383,
                 "precision": 0.5171875,
                 "recall": 0.9706744868035191
             },
             "dot": {
                 "accuracy": 0.5597069597069597,
-                "accuracy_threshold": 1.9611485004425049,
+                "accuracy_threshold": 1.9611477851867676,
                 "ap": 0.5019350242608148,
                 "f1": 0.6814204837879568,
-                "f1_threshold": 1.6902294158935547,
+                "f1_threshold": 1.6902297735214233,
                 "precision": 0.5249801744647106,
                 "recall": 0.9706744868035191
             },
             "euclidean": {
                 "accuracy": 0.5435897435897435,
-                "accuracy_threshold": 2.4475417137145996,
+                "accuracy_threshold": 2.4475414752960205,
                 "ap": 0.5333796303716746,
                 "f1": 0.6683119447186575,
                 "f1_threshold": 5.828757286071777,
                 "precision": 0.5037202380952381,
                 "recall": 0.9926686217008798
             },
             "manhattan": {
                 "accuracy": 0.5428571428571428,
-                "accuracy_threshold": 38.26271438598633,
+                "accuracy_threshold": 38.26274108886719,
                 "ap": 0.5327764115191864,
                 "f1": 0.6686537506209637,
-                "f1_threshold": 85.60132598876953,
+                "f1_threshold": 85.6013412475586,
                 "precision": 0.5056348610067618,
                 "recall": 0.9868035190615836
             },
             "max": {
                 "accuracy": 0.5597069597069597,
                 "ap": 0.5333796303716746,
                 "f1": 0.6814204837879568
             }
         },
+        "russian": {
+            "cos_sim": {
+                "accuracy": 0.7589743589743589,
+                "accuracy_threshold": 0.6166112422943115,
+                "ap": 0.8314514501860153,
+                "f1": 0.7680412371134021,
+                "f1_threshold": 0.5059094429016113,
+                "precision": 0.6850574712643678,
+                "recall": 0.873900293255132
+            },
+            "dot": {
+                "accuracy": 0.7098901098901099,
+                "accuracy_threshold": 8.012662887573242,
+                "ap": 0.762361506444045,
+                "f1": 0.7417956656346749,
+                "f1_threshold": 6.508602142333984,
+                "precision": 0.6420150053590568,
+                "recall": 0.8782991202346041
+            },
+            "euclidean": {
+                "accuracy": 0.7457875457875458,
+                "accuracy_threshold": 3.4959919452667236,
+                "ap": 0.8117728760401746,
+                "f1": 0.7606727037516171,
+                "f1_threshold": 3.7834253311157227,
+                "precision": 0.6805555555555556,
+                "recall": 0.8621700879765396
+            },
+            "manhattan": {
+                "accuracy": 0.7457875457875458,
+                "accuracy_threshold": 53.98133850097656,
+                "ap": 0.8117760839286252,
+                "f1": 0.7616613418530351,
+                "f1_threshold": 59.450931549072266,
+                "precision": 0.6749716874292185,
+                "recall": 0.873900293255132
+            },
+            "max": {
+                "accuracy": 0.7589743589743589,
+                "ap": 0.8314514501860153,
+                "f1": 0.7680412371134021
+            }
+        },
         "sanskrit": {
             "cos_sim": {
                 "accuracy": 0.5970695970695971,
                 "accuracy_threshold": 0.498678594827652,
                 "ap": 0.5881658900272513,
                 "f1": 0.6700100300902708,
-                "f1_threshold": 0.1445103883743286,
+                "f1_threshold": 0.14451023936271667,
                 "precision": 0.5091463414634146,
                 "recall": 0.9794721407624634
             },
             "dot": {
                 "accuracy": 0.5633699633699634,
                 "accuracy_threshold": 2.68283748626709,
                 "ap": 0.5547350327099301,
                 "f1": 0.6743215031315241,
-                "f1_threshold": 1.6816132068634033,
+                "f1_threshold": 1.6816134452819824,
                 "precision": 0.5235008103727715,
                 "recall": 0.9472140762463344
             },
             "euclidean": {
                 "accuracy": 0.589010989010989,
-                "accuracy_threshold": 2.4787545204162598,
+                "accuracy_threshold": 2.478755474090576,
                 "ap": 0.5751010592711443,
                 "f1": 0.6686274509803921,
-                "f1_threshold": 5.892199516296387,
+                "f1_threshold": 5.892199993133545,
                 "precision": 0.5022091310751104,
                 "recall": 1.0
             },
             "manhattan": {
                 "accuracy": 0.5816849816849817,
-                "accuracy_threshold": 38.17951202392578,
+                "accuracy_threshold": 38.17951965332031,
                 "ap": 0.5745488269646966,
                 "f1": 0.6686274509803921,
-                "f1_threshold": 88.86477661132812,
+                "f1_threshold": 88.86478424072266,
                 "precision": 0.5022091310751104,
                 "recall": 1.0
             },
             "max": {
                 "accuracy": 0.5970695970695971,
                 "ap": 0.5881658900272513,
                 "f1": 0.6743215031315241
             }
         },
         "tamil": {
             "cos_sim": {
                 "accuracy": 0.5355311355311355,
                 "accuracy_threshold": 0.7952712178230286,
-                "ap": 0.5145258007454051,
+                "ap": 0.5145245568467282,
                 "f1": 0.6697015680323724,
-                "f1_threshold": 0.31247392296791077,
+                "f1_threshold": 0.3124740421772003,
                 "precision": 0.5111969111969112,
                 "recall": 0.9706744868035191
             },
             "dot": {
                 "accuracy": 0.5230769230769231,
-                "accuracy_threshold": 3.2145144939422607,
+                "accuracy_threshold": 3.2145142555236816,
                 "ap": 0.4926278025365225,
                 "f1": 0.6719367588932806,
-                "f1_threshold": 1.7679429054260254,
+                "f1_threshold": 1.767941951751709,
                 "precision": 0.5067064083457526,
                 "recall": 0.9970674486803519
             },
             "euclidean": {
                 "accuracy": 0.5413919413919414,
-                "accuracy_threshold": 2.2082271575927734,
+                "accuracy_threshold": 2.2082276344299316,
                 "ap": 0.531486263648674,
                 "f1": 0.6669926650366748,
                 "f1_threshold": 6.154478073120117,
                 "precision": 0.5003668378576669,
                 "recall": 1.0
             },
             "manhattan": {
                 "accuracy": 0.5391941391941392,
-                "accuracy_threshold": 31.274255752563477,
+                "accuracy_threshold": 31.274248123168945,
                 "ap": 0.5324475879580712,
                 "f1": 0.6669926650366748,
-                "f1_threshold": 96.16970825195312,
+                "f1_threshold": 96.16972351074219,
                 "precision": 0.5003668378576669,
                 "recall": 1.0
             },
             "max": {
                 "accuracy": 0.5413919413919414,
                 "ap": 0.5324475879580712,
                 "f1": 0.6719367588932806
             }
+        },
+        "turkish": {
+            "cos_sim": {
+                "accuracy": 0.7311355311355311,
+                "accuracy_threshold": 0.5297951102256775,
+                "ap": 0.7992955752693494,
+                "f1": 0.7628865979381444,
+                "f1_threshold": 0.4986806809902191,
+                "precision": 0.6804597701149425,
+                "recall": 0.8680351906158358
+            },
+            "dot": {
+                "accuracy": 0.6886446886446886,
+                "accuracy_threshold": 8.365798950195312,
+                "ap": 0.7377809304884222,
+                "f1": 0.7194513715710723,
+                "f1_threshold": 6.619801044464111,
+                "precision": 0.6258134490238612,
+                "recall": 0.8460410557184751
+            },
+            "euclidean": {
+                "accuracy": 0.7347985347985349,
+                "accuracy_threshold": 3.477938175201416,
+                "ap": 0.7933361570309152,
+                "f1": 0.7571337983513,
+                "f1_threshold": 3.9908242225646973,
+                "precision": 0.6670391061452514,
+                "recall": 0.875366568914956
+            },
+            "manhattan": {
+                "accuracy": 0.7377289377289378,
+                "accuracy_threshold": 56.21800994873047,
+                "ap": 0.792577455338066,
+                "f1": 0.7524875621890548,
+                "f1_threshold": 62.92649459838867,
+                "precision": 0.6533477321814255,
+                "recall": 0.8870967741935484
+            },
+            "max": {
+                "accuracy": 0.7377289377289378,
+                "ap": 0.7992955752693494,
+                "f1": 0.7628865979381444
+            }
         }
     }
 }
```

### Comparing `mteb-1.8.7/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json` & `mteb-1.8.8/results/sentence-transformers__paraphrase-multilingual-MiniLM-L12-v2/XQuADRetrieval.json`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/amazon_polarity/create_data.py` & `mteb-1.8.8/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.8.8/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/arxiv/script_clustering.py` & `mteb-1.8.8/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/arxiv/script_raw.py` & `mteb-1.8.8/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/biorxiv/script_clustering.py` & `mteb-1.8.8/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/biorxiv/script_raw.py` & `mteb-1.8.8/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/bucc/create_data.py` & `mteb-1.8.8/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/create_task_table.py` & `mteb-1.8.8/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/germanquad/process_data.py` & `mteb-1.8.8/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/hal/create_data.py` & `mteb-1.8.8/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/imdb/create_data.py` & `mteb-1.8.8/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/medicalqaretrieval/create_data.py` & `mteb-1.8.8/scripts/data/medicalqaretrieval/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/medrxiv/script_clustering.py` & `mteb-1.8.8/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/medrxiv/script_raw.py` & `mteb-1.8.8/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/mind/prepare_data.py` & `mteb-1.8.8/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/multilingual_sentiment_classification/create_data.py` & `mteb-1.8.8/scripts/data/multilingual_sentiment_classification/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/redditp2p/script_clustering.py` & `mteb-1.8.8/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.8.8/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.8.8/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/summeval_fr/create_data.py` & `mteb-1.8.8/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.8.8/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/data/xnli2/create_multilang_ds.py` & `mteb-1.8.8/scripts/data/xnli2/create_multilang_ds.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,15 @@
     "assamese": ["asm-Beng"],
     "bengali": ["ben-Beng"],
     "marathi": ["mar-Deva"],
     "bhojpuri": ["bho-Deva"],
     "odiya": ["ory-Orya"],
     "sanskrit": ["san-Deva"],
     "tamil": ["tam-Taml"],
+    "turkish": ["tur-Latn"],
+    "greek": ["ell-Grek"],
+    "russian": ["rus-Cyrl"],
 }
 
 for lang in _LANGS.keys():
     raw_ds = load_dataset(f"Harsit/xnli2.0_{lang}")
     raw_ds.push_to_hub(repo_id=repo_id, config_name=lang)
```

### Comparing `mteb-1.8.7/scripts/merge_cqadupstack.py` & `mteb-1.8.8/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/mteb_meta.py` & `mteb-1.8.8/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_chinese.py` & `mteb-1.8.8/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_english.py` & `mteb-1.8.8/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_french.py` & `mteb-1.8.8/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_german.py` & `mteb-1.8.8/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_korean.py` & `mteb-1.8.8/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_law.py` & `mteb-1.8.8/scripts/run_mteb_law.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/scripts/run_mteb_polish.py` & `mteb-1.8.8/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_ClusteringEvaluator.py` & `mteb-1.8.8/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_InstructionRetrievalEvaluator.py` & `mteb-1.8.8/tests/test_InstructionRetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_PairClassificationEvaluator.py` & `mteb-1.8.8/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_RerankingEvaluator.py` & `mteb-1.8.8/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_RetrievalEvaluator.py` & `mteb-1.8.8/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_TaskMetadata.py` & `mteb-1.8.8/tests/test_TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_all_abstasks.py` & `mteb-1.8.8/tests/test_all_abstasks.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_encoder_interfaces.py` & `mteb-1.8.8/tests/test_encoder_interfaces.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_mteb.py` & `mteb-1.8.8/tests/test_mteb.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_mteb_rerank.py` & `mteb-1.8.8/tests/test_mteb_rerank.py`

 * *Files identical despite different names*

### Comparing `mteb-1.8.7/tests/test_overview.py` & `mteb-1.8.8/tests/test_overview.py`

 * *Files identical despite different names*

