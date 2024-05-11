# Comparing `tmp/vak-1.0.0a2.tar.gz` & `tmp/vak-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vak-1.0.0a2.tar", last modified: Mon Sep 11 16:01:21 2023, max compression
+gzip compressed data, was "vak-1.0.0a3.tar", last modified: Sat Sep 23 17:51:39 2023, max compression
```

## Comparing `vak-1.0.0a2.tar` & `vak-1.0.0a3.tar`

### file list

```diff
@@ -1,326 +1,326 @@
--rw-r--r--   0        0        0     5934 2023-09-11 01:47:52.504007 vak-1.0.0a2/.all-contributorsrc
--rw-r--r--   0        0        0     1843 2022-07-30 11:18:52.724175 vak-1.0.0a2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0     1267 2022-07-30 11:18:52.724175 vak-1.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2022-07-30 11:18:52.724175 vak-1.0.0a2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2022-07-30 11:18:52.724175 vak-1.0.0a2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      725 2023-09-11 15:26:44.475564 vak-1.0.0a2/.github/workflows/ci-linux.yml
--rw-r--r--   0        0        0      305 2023-06-05 14:33:25.498677 vak-1.0.0a2/.gitignore
--rw-r--r--   0        0        0      366 2022-07-30 11:18:52.724175 vak-1.0.0a2/.readthedocs.yaml
--rw-r--r--   0        0        0      982 2022-07-30 11:18:52.724175 vak-1.0.0a2/CITATION.cff
--rw-r--r--   0        0        0     5556 2022-07-30 11:18:52.724175 vak-1.0.0a2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1540 2021-03-20 03:21:29.941394 vak-1.0.0a2/LICENSE
--rw-r--r--   0        0        0    17457 2023-09-11 01:47:52.504007 vak-1.0.0a2/README.md
--rw-r--r--   0        0        0    61390 2023-08-15 01:14:02.957829 vak-1.0.0a2/doc/CHANGELOG.md
--rw-r--r--   0        0        0      580 2020-11-07 21:56:36.545662 vak-1.0.0a2/doc/Makefile
--rw-r--r--   0        0        0      612 2023-06-05 14:33:25.498677 vak-1.0.0a2/doc/_templates/class.rst
--rw-r--r--   0        0        0     1177 2023-06-05 14:33:25.498677 vak-1.0.0a2/doc/_templates/module.rst
--rw-r--r--   0        0        0     4875 2023-06-05 14:33:25.498677 vak-1.0.0a2/doc/api/index.rst
--rw-r--r--   0        0        0     7248 2023-09-11 15:58:37.015688 vak-1.0.0a2/doc/conf.py
--rw-r--r--   0        0        0      440 2022-07-30 11:18:52.728175 vak-1.0.0a2/doc/development/commit-abbreviations.rst
--rw-r--r--   0        0        0     9592 2023-01-15 00:38:08.515237 vak-1.0.0a2/doc/development/contributors.md
--rw-r--r--   0        0        0     1008 2023-01-15 00:38:08.515237 vak-1.0.0a2/doc/development/index.md
--rw-r--r--   0        0        0     1706 2022-08-18 00:25:51.168133 vak-1.0.0a2/doc/faq.md
--rw-r--r--   0        0        0    17488 2022-09-28 02:13:36.504024 vak-1.0.0a2/doc/get_started/autoannotate.md
--rw-r--r--   0        0        0      627 2022-07-30 11:18:52.728175 vak-1.0.0a2/doc/get_started/index.md
--rw-r--r--   0        0        0     7196 2022-10-12 01:04:43.860715 vak-1.0.0a2/doc/get_started/installation.md
--rw-r--r--   0        0        0     7727 2022-08-29 01:30:49.460626 vak-1.0.0a2/doc/howto/howto_prep_annotate.md
--rw-r--r--   0        0        0    11667 2023-01-15 00:38:08.515237 vak-1.0.0a2/doc/howto/howto_user_annot.md
--rw-r--r--   0        0        0     2518 2022-07-30 11:18:52.728175 vak-1.0.0a2/doc/howto/howto_user_spect.md
--rw-r--r--   0        0        0      316 2022-08-29 01:30:49.460626 vak-1.0.0a2/doc/howto/index.md
--rw-r--r--   0        0        0        0 2022-07-30 11:18:52.728175 vak-1.0.0a2/doc/howto/predict.md
--rw-r--r--   0        0        0        0 2022-07-30 11:18:52.728175 vak-1.0.0a2/doc/howto/train.md
--rw-r--r--   0        0        0   227036 2022-07-30 11:18:52.728175 vak-1.0.0a2/doc/images/annotation-example.png
--rw-r--r--   0        0        0   148869 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/images/annotation_example_for_tutorial.png
--rw-r--r--   0        0        0   132467 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/images/logo/vak-logo-primary.png
--rw-r--r--   0        0        0   125419 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/images/logo/vak-logo-secondary.png
--rw-r--r--   0        0        0    77914 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/images/logo/vak-logomark.png
--rw-r--r--   0        0        0    90177 2020-11-07 21:56:36.545662 vak-1.0.0a2/doc/images/song_with_colored_segments.png
--rw-r--r--   0        0        0   107387 2020-11-07 21:56:36.545662 vak-1.0.0a2/doc/images/terminalizer/vak-help.gif
--rw-r--r--   0        0        0     3712 2020-11-07 21:56:36.545662 vak-1.0.0a2/doc/images/terminalizer/vak-help.yml
--rw-r--r--   0        0        0     2085 2023-06-05 14:33:25.502677 vak-1.0.0a2/doc/index.md
--rw-r--r--   0        0        0      787 2020-11-07 21:56:36.545662 vak-1.0.0a2/doc/make.bat
--rw-r--r--   0        0        0       96 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/poems/index.md
--rw-r--r--   0        0        0      488 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/poems/the-bird-may-die.rst
--rw-r--r--   0        0        0     1305 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/poems/unknown-bird.rst
--rw-r--r--   0        0        0      836 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/poems/what-does-the-bird-care.rst
--rw-r--r--   0        0        0     6535 2023-09-11 01:54:21.637744 vak-1.0.0a2/doc/reference/about.md
--rw-r--r--   0        0        0     2356 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/reference/cli.md
--rw-r--r--   0        0        0     2052 2022-07-30 11:18:52.732175 vak-1.0.0a2/doc/reference/config.md
--rw-r--r--   0        0        0     4610 2022-08-29 01:30:49.460626 vak-1.0.0a2/doc/reference/filenames.md
--rw-r--r--   0        0        0      125 2022-08-18 00:25:51.168133 vak-1.0.0a2/doc/reference/index.md
--rw-r--r--   0        0        0     1099 2023-06-05 14:33:25.502677 vak-1.0.0a2/doc/reference/models.md
--rw-r--r--   0        0        0     4070 2022-08-29 01:30:49.460626 vak-1.0.0a2/doc/reference/spect_file_format.md
--rw-r--r--   0        0        0   130300 2020-11-07 21:56:36.545662 vak-1.0.0a2/doc/sample_phrase_annotation.png
--rw-r--r--   0        0        0      774 2023-09-11 15:58:37.027687 vak-1.0.0a2/doc/toml/gy6or6_predict.toml
--rw-r--r--   0        0        0      647 2023-09-11 15:58:37.035688 vak-1.0.0a2/doc/toml/gy6or6_train.toml
--rw-r--r--   0        0        0     8924 2023-09-11 01:47:52.504007 vak-1.0.0a2/noxfile.py
--rw-r--r--   0        0        0     2320 2023-09-11 15:29:38.266489 vak-1.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     4258 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/scripts/download_autoannotate_data.py
--rw-r--r--   0        0        0      845 2023-09-11 15:29:38.282489 vak-1.0.0a2/src/vak/__about__.py
--rw-r--r--   0        0        0      780 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/__init__.py
--rw-r--r--   0        0        0     1401 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/__main__.py
--rw-r--r--   0        0        0      239 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/cli/__init__.py
--rw-r--r--   0        0        0     1097 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/cli/cli.py
--rw-r--r--   0        0        0     2070 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/cli/eval.py
--rw-r--r--   0        0        0     3131 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/cli/learncurve.py
--rw-r--r--   0        0        0     2311 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/cli/predict.py
--rw-r--r--   0        0        0     6312 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/cli/prep.py
--rw-r--r--   0        0        0     2935 2023-08-21 14:21:20.822816 vak-1.0.0a2/src/vak/cli/train.py
--rw-r--r--   0        0        0      845 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/__init__.py
--rw-r--r--   0        0        0    27813 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/annotation.py
--rw-r--r--   0        0        0     1147 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/constants.py
--rw-r--r--   0        0        0     5087 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/converters.py
--rw-r--r--   0        0        0      298 2023-06-06 21:30:23.974424 vak-1.0.0a2/src/vak/common/device.py
--rw-r--r--   0        0        0      123 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/files/__init__.py
--rw-r--r--   0        0        0     3418 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/files/files.py
--rw-r--r--   0        0        0     8084 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/files/spect.py
--rw-r--r--   0        0        0     5365 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/labels.py
--rw-r--r--   0        0        0      432 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/learncurve.py
--rw-r--r--   0        0        0     2620 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/logging.py
--rw-r--r--   0        0        0     1371 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/paths.py
--rw-r--r--   0        0        0     5248 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/common/tensorboard.py
--rw-r--r--   0        0        0     1255 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/timebins.py
--rw-r--r--   0        0        0      270 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/common/timenow.py
--rw-r--r--   0        0        0     1968 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/common/trainer.py
--rw-r--r--   0        0        0       77 2023-06-06 21:30:23.974424 vak-1.0.0a2/src/vak/common/typing.py
--rw-r--r--   0        0        0     1989 2023-06-06 21:30:23.974424 vak-1.0.0a2/src/vak/common/validators.py
--rw-r--r--   0        0        0      384 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/__init__.py
--rw-r--r--   0        0        0     1577 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/config.py
--rw-r--r--   0        0        0     6339 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/eval.py
--rw-r--r--   0        0        0     2544 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/learncurve.py
--rw-r--r--   0        0        0     2693 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/model.py
--rw-r--r--   0        0        0     6322 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/parse.py
--rw-r--r--   0        0        0     5203 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/predict.py
--rw-r--r--   0        0        0     8091 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/config/prep.py
--rw-r--r--   0        0        0     3126 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/spect_params.py
--rw-r--r--   0        0        0     5468 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/train.py
--rw-r--r--   0        0        0     3521 2023-08-14 01:30:57.912904 vak-1.0.0a2/src/vak/config/valid.toml
--rw-r--r--   0        0        0     4568 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/config/validators.py
--rw-r--r--   0        0        0      118 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/__init__.py
--rw-r--r--   0        0        0      210 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/frame_classification/__init__.py
--rw-r--r--   0        0        0      353 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/frame_classification/constants.py
--rw-r--r--   0        0        0     4036 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/frame_classification/frames_dataset.py
--rw-r--r--   0        0        0     6275 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/datasets/frame_classification/metadata.py
--rw-r--r--   0        0        0     8543 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/frame_classification/window_dataset.py
--rw-r--r--   0        0        0      131 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/parametric_umap/__init__.py
--rw-r--r--   0        0        0     5411 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/parametric_umap/metadata.py
--rw-r--r--   0        0        0    11175 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/datasets/parametric_umap/parametric_umap.py
--rw-r--r--   0        0        0      175 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/eval/__init__.py
--rw-r--r--   0        0        0     5899 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/eval/eval_.py
--rw-r--r--   0        0        0     9223 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/eval/frame_classification.py
--rw-r--r--   0        0        0     6226 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/eval/parametric_umap.py
--rw-r--r--   0        0        0      241 2023-09-11 01:47:52.504007 vak-1.0.0a2/src/vak/learncurve/__init__.py
--rw-r--r--   0        0        0     5682 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/learncurve/curvefit.py
--rw-r--r--   0        0        0      538 2023-06-27 18:57:19.764652 vak-1.0.0a2/src/vak/learncurve/dirname.py
--rw-r--r--   0        0        0    13170 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/learncurve/frame_classification.py
--rw-r--r--   0        0        0     6455 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/learncurve/learncurve.py
--rw-r--r--   0        0        0       94 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/metrics/__init__.py
--rw-r--r--   0        0        0       69 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/metrics/classification/__init__.py
--rw-r--r--   0        0        0      509 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/metrics/classification/classification.py
--rw-r--r--   0        0        0      538 2020-11-07 21:56:36.549662 vak-1.0.0a2/src/vak/metrics/classification/functional.py
--rw-r--r--   0        0        0       99 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/metrics/distance/__init__.py
--rw-r--r--   0        0        0     1191 2021-04-13 02:29:39.812554 vak-1.0.0a2/src/vak/metrics/distance/distance.py
--rw-r--r--   0        0        0     2812 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/metrics/distance/functional.py
--rw-r--r--   0        0        0      810 2021-04-13 02:29:39.812554 vak-1.0.0a2/src/vak/metrics/util.py
--rw-r--r--   0        0        0      635 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/models/__init__.py
--rw-r--r--   0        0        0    16272 2023-08-14 13:35:41.524081 vak-1.0.0a2/src/vak/models/base.py
--rw-r--r--   0        0        0     2068 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/models/convencoder_umap.py
--rw-r--r--   0        0        0     2992 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/models/decorator.py
--rw-r--r--   0        0        0    18905 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/models/definition.py
--rw-r--r--   0        0        0     1571 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/models/ed_tcn.py
--rw-r--r--   0        0        0    13791 2023-08-15 21:25:45.395609 vak-1.0.0a2/src/vak/models/frame_classification_model.py
--rw-r--r--   0        0        0     3721 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/models/get.py
--rw-r--r--   0        0        0     6453 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/models/parametric_umap_model.py
--rw-r--r--   0        0        0     3506 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/models/registry.py
--rw-r--r--   0        0        0     2389 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/models/tweetynet.py
--rw-r--r--   0        0        0      260 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/nets/__init__.py
--rw-r--r--   0        0        0     3018 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/nets/conv_encoder.py
--rw-r--r--   0        0        0     4929 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nets/ed_tcn.py
--rw-r--r--   0        0        0     7301 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/nets/tweetynet.py
--rw-r--r--   0        0        0      128 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/__init__.py
--rw-r--r--   0        0        0     2315 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/functional.py
--rw-r--r--   0        0        0      158 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/loss/__init__.py
--rw-r--r--   0        0        0     4672 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/loss/dice.py
--rw-r--r--   0        0        0     4521 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/loss/umap.py
--rw-r--r--   0        0        0      107 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/modules/__init__.py
--rw-r--r--   0        0        0      850 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/modules/activation.py
--rw-r--r--   0        0        0     3237 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/nn/modules/conv.py
--rw-r--r--   0        0        0      244 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/plot/__init__.py
--rw-r--r--   0        0        0     4455 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/plot/annot.py
--rw-r--r--   0        0        0     4299 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/plot/learncurve.py
--rw-r--r--   0        0        0     3997 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/plot/spect.py
--rw-r--r--   0        0        0      190 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/predict/__init__.py
--rw-r--r--   0        0        0    12523 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/predict/frame_classification.py
--rw-r--r--   0        0        0     6341 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/predict/parametric_umap.py
--rw-r--r--   0        0        0     6487 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/predict/predict_.py
--rw-r--r--   0        0        0      448 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/__init__.py
--rw-r--r--   0        0        0     7395 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/audio_dataset.py
--rw-r--r--   0        0        0      548 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/constants.py
--rw-r--r--   0        0        0     2770 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/dataset_df_helper.py
--rw-r--r--   0        0        0      285 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/frame_classification/__init__.py
--rw-r--r--   0        0        0    13744 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/frame_classification/dataset_arrays.py
--rw-r--r--   0        0        0    17398 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/frame_classification/frame_classification.py
--rw-r--r--   0        0        0     6709 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/frame_classification/learncurve.py
--rw-r--r--   0        0        0     1595 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/frame_classification/validators.py
--rw-r--r--   0        0        0      161 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/parametric_umap/__init__.py
--rw-r--r--   0        0        0     4537 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/parametric_umap/dataset_arrays.py
--rw-r--r--   0        0        0    13964 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/parametric_umap/parametric_umap.py
--rw-r--r--   0        0        0     9661 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/prep_.py
--rw-r--r--   0        0        0     2353 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/sequence_dataset.py
--rw-r--r--   0        0        0      189 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/spectrogram_dataset/__init__.py
--rw-r--r--   0        0        0     9857 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/spectrogram_dataset/audio_helper.py
--rw-r--r--   0        0        0     8073 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/spectrogram_dataset/prep.py
--rw-r--r--   0        0        0     3150 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/spectrogram_dataset/spect.py
--rw-r--r--   0        0        0    11377 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/spectrogram_dataset/spect_helper.py
--rw-r--r--   0        0        0      185 2023-08-24 14:39:59.417577 vak-1.0.0a2/src/vak/prep/split/__init__.py
--rw-r--r--   0        0        0       70 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/split/algorithms/__init__.py
--rw-r--r--   0        0        0    12457 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/split/algorithms/bruteforce.py
--rw-r--r--   0        0        0     3918 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/split/algorithms/validate.py
--rw-r--r--   0        0        0     9088 2023-09-11 01:47:52.508007 vak-1.0.0a2/src/vak/prep/split/split.py
--rw-r--r--   0        0        0      130 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/prep/unit_dataset/__init__.py
--rw-r--r--   0        0        0    12476 2023-08-18 14:49:44.247942 vak-1.0.0a2/src/vak/prep/unit_dataset/unit_dataset.py
--rw-r--r--   0        0        0      180 2023-09-11 01:47:52.512007 vak-1.0.0a2/src/vak/train/__init__.py
--rw-r--r--   0        0        0    14305 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/train/frame_classification.py
--rw-r--r--   0        0        0    11393 2023-09-11 01:47:52.512007 vak-1.0.0a2/src/vak/train/parametric_umap.py
--rw-r--r--   0        0        0     8819 2023-09-11 01:47:52.512007 vak-1.0.0a2/src/vak/train/train_.py
--rw-r--r--   0        0        0       93 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/__init__.py
--rw-r--r--   0        0        0      171 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/defaults/__init__.py
--rw-r--r--   0        0        0     9714 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/defaults/frame_classification.py
--rw-r--r--   0        0        0     1471 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/defaults/get.py
--rw-r--r--   0        0        0      602 2023-09-11 01:47:52.512007 vak-1.0.0a2/src/vak/transforms/defaults/parametric_umap.py
--rw-r--r--   0        0        0      128 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/frame_labels/__init__.py
--rw-r--r--   0        0        0    17855 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/frame_labels/functional.py
--rw-r--r--   0        0        0     9877 2023-08-14 13:35:41.528081 vak-1.0.0a2/src/vak/transforms/frame_labels/transforms.py
--rw-r--r--   0        0        0     6788 2023-08-14 13:35:41.532081 vak-1.0.0a2/src/vak/transforms/functional.py
--rw-r--r--   0        0        0    13478 2023-09-11 01:47:52.512007 vak-1.0.0a2/src/vak/transforms/transforms.py
--rw-r--r--   0        0        0        0 2021-03-20 03:21:29.953394 vak-1.0.0a2/tests/__init__.py
--rw-r--r--   0        0        0      900 2023-09-11 01:47:52.512007 vak-1.0.0a2/tests/conftest.py
--rw-r--r--   0        0        0      328 2023-06-25 20:47:16.590134 vak-1.0.0a2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     5811 2023-09-11 01:47:52.512007 vak-1.0.0a2/tests/fixtures/annot.py
--rw-r--r--   0        0        0     3897 2023-09-11 01:47:52.512007 vak-1.0.0a2/tests/fixtures/audio.py
--rw-r--r--   0        0        0    12598 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/fixtures/config.py
--rw-r--r--   0        0        0     1416 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/fixtures/csv.py
--rw-r--r--   0        0        0     3412 2023-06-25 20:47:16.590134 vak-1.0.0a2/tests/fixtures/das.py
--rw-r--r--   0        0        0     1157 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/fixtures/dataframe.py
--rw-r--r--   0        0        0      810 2023-06-06 21:30:23.978424 vak-1.0.0a2/tests/fixtures/dataset.py
--rw-r--r--   0        0        0      470 2021-04-13 02:29:39.816553 vak-1.0.0a2/tests/fixtures/device.py
--rw-r--r--   0        0        0      541 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/fixtures/model.py
--rw-r--r--   0        0        0      869 2023-06-06 21:30:23.978424 vak-1.0.0a2/tests/fixtures/path.py
--rw-r--r--   0        0        0      745 2023-06-06 21:30:23.978424 vak-1.0.0a2/tests/fixtures/results.py
--rw-r--r--   0        0        0     4310 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/fixtures/spect.py
--rw-r--r--   0        0        0     1509 2023-06-06 21:30:23.978424 vak-1.0.0a2/tests/fixtures/split.py
--rw-r--r--   0        0        0      245 2022-07-30 11:18:52.744175 vak-1.0.0a2/tests/fixtures/tensorboard.py
--rw-r--r--   0        0        0     1235 2023-06-25 20:47:16.590134 vak-1.0.0a2/tests/fixtures/test_data.py
--rw-r--r--   0        0        0      736 2023-02-18 03:07:26.485344 vak-1.0.0a2/tests/fixtures/torch.py
--rw-r--r--   0        0        0    33574 2023-06-25 20:47:16.590134 vak-1.0.0a2/tests/scripts/das-test-data-env.txt
--rw-r--r--   0        0        0    13491 2023-06-25 20:47:16.590134 vak-1.0.0a2/tests/scripts/das-test-data-env.yml
--rw-r--r--   0        0        0     5387 2023-06-27 18:57:10.080703 vak-1.0.0a2/tests/scripts/generate_das_test_data.py
--rw-r--r--   0        0        0     6969 2023-08-31 17:23:19.388619 vak-1.0.0a2/tests/scripts/generate_data_for_tests.py
--rw-r--r--   0        0        0     2661 2021-04-13 02:29:39.816553 vak-1.0.0a2/tests/scripts/move_csv.py
--rw-r--r--   0        0        0       99 2023-08-14 01:30:57.920904 vak-1.0.0a2/tests/scripts/vaktestdata/__init__.py
--rw-r--r--   0        0        0      378 2023-08-14 01:30:57.920904 vak-1.0.0a2/tests/scripts/vaktestdata/config_metadata.py
--rw-r--r--   0        0        0     7256 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/scripts/vaktestdata/configs.py
--rw-r--r--   0        0        0     1595 2023-08-14 01:30:57.920904 vak-1.0.0a2/tests/scripts/vaktestdata/constants.py
--rw-r--r--   0        0        0     2301 2023-08-14 01:30:57.920904 vak-1.0.0a2/tests/scripts/vaktestdata/dirs.py
--rw-r--r--   0        0        0     1093 2023-08-14 01:30:57.920904 vak-1.0.0a2/tests/scripts/vaktestdata/parser.py
--rw-r--r--   0        0        0     1231 2023-08-14 01:30:57.920904 vak-1.0.0a2/tests/scripts/vaktestdata/prep.py
--rw-r--r--   0        0        0     1858 2022-07-30 11:18:52.744175 vak-1.0.0a2/tests/test___main__.py
--rw-r--r--   0        0        0        0 2021-03-20 03:21:29.957394 vak-1.0.0a2/tests/test_cli/__init__.py
--rw-r--r--   0        0        0      684 2023-05-30 01:19:26.147042 vak-1.0.0a2/tests/test_cli/cli_asserts.py
--rw-r--r--   0        0        0     1949 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_cli/test_eval.py
--rw-r--r--   0        0        0     2415 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_cli/test_learncurve.py
--rw-r--r--   0        0        0     2043 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_cli/test_predict.py
--rw-r--r--   0        0        0     3878 2023-06-06 21:30:23.978424 vak-1.0.0a2/tests/test_cli/test_prep.py
--rw-r--r--   0        0        0     2562 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_cli/test_train.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/__init__.py
--rw-r--r--   0        0        0    11367 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_annotation.py
--rw-r--r--   0        0        0      535 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_console_script.py
--rw-r--r--   0        0        0      853 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_converters.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_files/__init__.py
--rw-r--r--   0        0        0     2865 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_files/test_files.py
--rw-r--r--   0        0        0     2645 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_files/test_spect.py
--rw-r--r--   0        0        0     3175 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_common/test_labels.py
--rw-r--r--   0        0        0     2207 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_paths.py
--rw-r--r--   0        0        0      510 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_tensorboard.py
--rw-r--r--   0        0        0      317 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_timebins.py
--rw-r--r--   0        0        0      595 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_common/test_timenow.py
--rw-r--r--   0        0        0      163 2021-03-20 03:21:29.957394 vak-1.0.0a2/tests/test_config/__init__.py
--rw-r--r--   0        0        0      704 2021-03-20 03:21:29.957394 vak-1.0.0a2/tests/test_config/attr_helpers.py
--rw-r--r--   0        0        0     1088 2021-04-13 02:29:39.816553 vak-1.0.0a2/tests/test_config/test_config.py
--rw-r--r--   0        0        0      417 2022-08-17 14:02:21.758688 vak-1.0.0a2/tests/test_config/test_eval.py
--rw-r--r--   0        0        0      492 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_config/test_learncurve.py
--rw-r--r--   0        0        0     1865 2023-06-05 14:33:25.510677 vak-1.0.0a2/tests/test_config/test_model.py
--rw-r--r--   0        0        0     9648 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_config/test_parse.py
--rw-r--r--   0        0        0      453 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_config/test_predict.py
--rw-r--r--   0        0        0      479 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_config/test_prep.py
--rw-r--r--   0        0        0     2127 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_config/test_spect_params.py
--rw-r--r--   0        0        0      480 2021-04-13 02:29:39.816553 vak-1.0.0a2/tests/test_config/test_train.py
--rw-r--r--   0        0        0      856 2021-04-13 02:29:39.816553 vak-1.0.0a2/tests/test_config/test_validators.py
--rw-r--r--   0        0        0        0 2022-08-17 14:02:21.762688 vak-1.0.0a2/tests/test_datasets/__init__.py
--rw-r--r--   0        0        0        0 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_datasets/test_frame_classification/__init__.py
--rw-r--r--   0        0        0     1395 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_datasets/test_frame_classification/test_frames_dataset.py
--rw-r--r--   0        0        0     3299 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_datasets/test_frame_classification/test_metadata.py
--rw-r--r--   0        0        0     1623 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_datasets/test_frame_classification/test_window_dataset.py
--rw-r--r--   0        0        0        0 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_datasets/test_parametric_umap/__init__.py
--rw-r--r--   0        0        0     1428 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_datasets/test_parametric_umap/test_parametric_umap.py
--rw-r--r--   0        0        0        0 2022-08-17 14:02:21.762688 vak-1.0.0a2/tests/test_datasets/test_seq/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_eval/__init__.py
--rw-r--r--   0        0        0     2284 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_eval/test_eval.py
--rw-r--r--   0        0        0     6973 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_eval/test_frame_classification.py
--rw-r--r--   0        0        0     5674 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_eval/test_parametric_umap.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_learncurve/__init__.py
--rw-r--r--   0        0        0     6017 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_learncurve/test_frame_classification.py
--rw-r--r--   0        0        0        0 2021-04-25 00:42:45.347480 vak-1.0.0a2/tests/test_metrics/__init__.py
--rw-r--r--   0        0        0        0 2021-04-25 00:42:45.347480 vak-1.0.0a2/tests/test_metrics/test_distance/__init__.py
--rw-r--r--   0        0        0     1613 2021-04-25 00:42:45.347480 vak-1.0.0a2/tests/test_metrics/test_distance/test_functional.py
--rw-r--r--   0        0        0        0 2021-04-04 15:40:00.958474 vak-1.0.0a2/tests/test_models/__init__.py
--rw-r--r--   0        0        0     5175 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_models/conftest.py
--rw-r--r--   0        0        0    11862 2023-09-11 01:47:52.516007 vak-1.0.0a2/tests/test_models/test_base.py
--rw-r--r--   0        0        0     1564 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_convencoder_umap.py
--rw-r--r--   0        0        0     2045 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_decorator.py
--rw-r--r--   0        0        0    10934 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_definition.py
--rw-r--r--   0        0        0     1139 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_ed_tcn.py
--rw-r--r--   0        0        0     5770 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_frame_classification_model.py
--rw-r--r--   0        0        0     5088 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_parametric_umap_model.py
--rw-r--r--   0        0        0     4232 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_registry.py
--rw-r--r--   0        0        0     1966 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_models/test_tweetynet.py
--rw-r--r--   0        0        0        0 2023-06-05 14:33:25.514677 vak-1.0.0a2/tests/test_nets/__init__.py
--rw-r--r--   0        0        0     1413 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_nets/test_convencoder.py
--rw-r--r--   0        0        0     2944 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_nets/test_ed_tcn.py
--rw-r--r--   0        0        0     2957 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_nets/test_tweetynet.py
--rw-r--r--   0        0        0        0 2021-04-25 22:29:23.560050 vak-1.0.0a2/tests/test_nn/__init__.py
--rw-r--r--   0        0        0      726 2022-07-30 11:18:52.748175 vak-1.0.0a2/tests/test_nn/test_functional.py
--rw-r--r--   0        0        0        0 2021-04-25 22:29:23.560050 vak-1.0.0a2/tests/test_nn/test_loss/__init__.py
--rw-r--r--   0        0        0     2512 2021-04-25 22:29:23.560050 vak-1.0.0a2/tests/test_nn/test_loss/test_dice.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_predict/__init__.py
--rw-r--r--   0        0        0     8097 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_predict/test_frame_classification.py
--rw-r--r--   0        0        0     2419 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_predict/test_predict.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/__init__.py
--rw-r--r--   0        0        0     4191 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_audio_dataset.py
--rw-r--r--   0        0        0        0 2023-06-25 20:47:16.590134 vak-1.0.0a2/tests/test_prep/test_frame_classification/__init__.py
--rw-r--r--   0        0        0     6377 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_frame_classification/test_dataset_arrays.py
--rw-r--r--   0        0        0    13143 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_frame_classification/test_frame_classification.py
--rw-r--r--   0        0        0     3896 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_frame_classification/test_learncurve.py
--rw-r--r--   0        0        0       67 2023-06-27 18:57:19.764652 vak-1.0.0a2/tests/test_prep/test_frame_classification/test_validators.py
--rw-r--r--   0        0        0     2777 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_prep.py
--rw-r--r--   0        0        0     1259 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_sequence_dataset.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/__init__.py
--rw-r--r--   0        0        0    15324 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/test_audio_helper.py
--rw-r--r--   0        0        0     9300 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/test_prep.py
--rw-r--r--   0        0        0     7275 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/test_spect_helper.py
--rw-r--r--   0        0        0       55 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/test_split/__init__.py
--rw-r--r--   0        0        0       58 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/test_split/test_algorithms/__init__.py
--rw-r--r--   0        0        0     9531 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/test_split/test_algorithms/test_bruteforce.py
--rw-r--r--   0        0        0     2330 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_prep/test_split/test_algorithms/test_validate.py
--rw-r--r--   0        0        0    10892 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_prep/test_split/test_split.py
--rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a2/tests/test_train/__init__.py
--rw-r--r--   0        0        0     9778 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_train/test_frame_classification.py
--rw-r--r--   0        0        0     6730 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_train/test_parametric_umap.py
--rw-r--r--   0        0        0     2892 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_train/test_train.py
--rw-r--r--   0        0        0        0 2023-02-11 00:18:57.767185 vak-1.0.0a2/tests/test_transforms/__init__.py
--rw-r--r--   0        0        0        0 2023-09-11 01:47:52.520007 vak-1.0.0a2/tests/test_transforms/test_frame_labels/__init__.py
--rw-r--r--   0        0        0    17206 2023-09-11 01:47:52.524007 vak-1.0.0a2/tests/test_transforms/test_frame_labels/test_functional.py
--rw-r--r--   0        0        0     9096 2023-09-11 01:47:52.524007 vak-1.0.0a2/tests/test_transforms/test_frame_labels/test_transforms.py
--rw-r--r--   0        0        0     4789 2023-09-11 01:47:52.524007 vak-1.0.0a2/tests/test_transforms/test_transforms.py
--rw-r--r--   0        0        0       61 2023-09-11 01:47:52.524007 vak-1.0.0a2/tests/vak.tests.config.json
--rw-r--r--   0        0        0    19645 1970-01-01 00:00:00.000000 vak-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     6185 2023-09-23 17:41:02.407718 vak-1.0.0a3/.all-contributorsrc
+-rw-r--r--   0        0        0     1843 2022-07-30 11:18:52.724175 vak-1.0.0a3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1267 2022-07-30 11:18:52.724175 vak-1.0.0a3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2022-07-30 11:18:52.724175 vak-1.0.0a3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2022-07-30 11:18:52.724175 vak-1.0.0a3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      725 2023-09-11 15:26:44.475564 vak-1.0.0a3/.github/workflows/ci-linux.yml
+-rw-r--r--   0        0        0      305 2023-06-05 14:33:25.498677 vak-1.0.0a3/.gitignore
+-rw-r--r--   0        0        0      367 2023-09-11 16:20:24.635288 vak-1.0.0a3/.readthedocs.yaml
+-rw-r--r--   0        0        0      982 2022-07-30 11:18:52.724175 vak-1.0.0a3/CITATION.cff
+-rw-r--r--   0        0        0     5556 2022-07-30 11:18:52.724175 vak-1.0.0a3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1540 2021-03-20 03:21:29.941394 vak-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0    18642 2023-09-23 17:41:02.407718 vak-1.0.0a3/README.md
+-rw-r--r--   0        0        0    61723 2023-09-23 17:44:24.990467 vak-1.0.0a3/doc/CHANGELOG.md
+-rw-r--r--   0        0        0      580 2020-11-07 21:56:36.545662 vak-1.0.0a3/doc/Makefile
+-rw-r--r--   0        0        0      612 2023-06-05 14:33:25.498677 vak-1.0.0a3/doc/_templates/class.rst
+-rw-r--r--   0        0        0     1177 2023-06-05 14:33:25.498677 vak-1.0.0a3/doc/_templates/module.rst
+-rw-r--r--   0        0        0     5450 2023-09-11 17:01:35.019813 vak-1.0.0a3/doc/api/index.rst
+-rw-r--r--   0        0        0     7248 2023-09-11 15:58:37.015688 vak-1.0.0a3/doc/conf.py
+-rw-r--r--   0        0        0      440 2022-07-30 11:18:52.728175 vak-1.0.0a3/doc/development/commit-abbreviations.rst
+-rw-r--r--   0        0        0     9592 2023-01-15 00:38:08.515237 vak-1.0.0a3/doc/development/contributors.md
+-rw-r--r--   0        0        0     1008 2023-01-15 00:38:08.515237 vak-1.0.0a3/doc/development/index.md
+-rw-r--r--   0        0        0     1706 2022-08-18 00:25:51.168133 vak-1.0.0a3/doc/faq.md
+-rw-r--r--   0        0        0    17488 2022-09-28 02:13:36.504024 vak-1.0.0a3/doc/get_started/autoannotate.md
+-rw-r--r--   0        0        0      627 2022-07-30 11:18:52.728175 vak-1.0.0a3/doc/get_started/index.md
+-rw-r--r--   0        0        0     7196 2022-10-12 01:04:43.860715 vak-1.0.0a3/doc/get_started/installation.md
+-rw-r--r--   0        0        0     7727 2022-08-29 01:30:49.460626 vak-1.0.0a3/doc/howto/howto_prep_annotate.md
+-rw-r--r--   0        0        0    11667 2023-01-15 00:38:08.515237 vak-1.0.0a3/doc/howto/howto_user_annot.md
+-rw-r--r--   0        0        0     2518 2022-07-30 11:18:52.728175 vak-1.0.0a3/doc/howto/howto_user_spect.md
+-rw-r--r--   0        0        0      316 2022-08-29 01:30:49.460626 vak-1.0.0a3/doc/howto/index.md
+-rw-r--r--   0        0        0        0 2022-07-30 11:18:52.728175 vak-1.0.0a3/doc/howto/predict.md
+-rw-r--r--   0        0        0        0 2022-07-30 11:18:52.728175 vak-1.0.0a3/doc/howto/train.md
+-rw-r--r--   0        0        0   227036 2022-07-30 11:18:52.728175 vak-1.0.0a3/doc/images/annotation-example.png
+-rw-r--r--   0        0        0   148869 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/images/annotation_example_for_tutorial.png
+-rw-r--r--   0        0        0   132467 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/images/logo/vak-logo-primary.png
+-rw-r--r--   0        0        0   125419 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/images/logo/vak-logo-secondary.png
+-rw-r--r--   0        0        0    77914 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/images/logo/vak-logomark.png
+-rw-r--r--   0        0        0    90177 2020-11-07 21:56:36.545662 vak-1.0.0a3/doc/images/song_with_colored_segments.png
+-rw-r--r--   0        0        0   107387 2020-11-07 21:56:36.545662 vak-1.0.0a3/doc/images/terminalizer/vak-help.gif
+-rw-r--r--   0        0        0     3712 2020-11-07 21:56:36.545662 vak-1.0.0a3/doc/images/terminalizer/vak-help.yml
+-rw-r--r--   0        0        0     2428 2023-09-21 01:05:40.835897 vak-1.0.0a3/doc/index.md
+-rw-r--r--   0        0        0      787 2020-11-07 21:56:36.545662 vak-1.0.0a3/doc/make.bat
+-rw-r--r--   0        0        0       96 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/poems/index.md
+-rw-r--r--   0        0        0      488 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/poems/the-bird-may-die.rst
+-rw-r--r--   0        0        0     1305 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/poems/unknown-bird.rst
+-rw-r--r--   0        0        0      836 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/poems/what-does-the-bird-care.rst
+-rw-r--r--   0        0        0     6535 2023-09-11 01:54:21.637744 vak-1.0.0a3/doc/reference/about.md
+-rw-r--r--   0        0        0     2356 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/reference/cli.md
+-rw-r--r--   0        0        0     2052 2022-07-30 11:18:52.732175 vak-1.0.0a3/doc/reference/config.md
+-rw-r--r--   0        0        0     4610 2022-08-29 01:30:49.460626 vak-1.0.0a3/doc/reference/filenames.md
+-rw-r--r--   0        0        0      125 2022-08-18 00:25:51.168133 vak-1.0.0a3/doc/reference/index.md
+-rw-r--r--   0        0        0     1099 2023-06-05 14:33:25.502677 vak-1.0.0a3/doc/reference/models.md
+-rw-r--r--   0        0        0     4070 2022-08-29 01:30:49.460626 vak-1.0.0a3/doc/reference/spect_file_format.md
+-rw-r--r--   0        0        0   130300 2020-11-07 21:56:36.545662 vak-1.0.0a3/doc/sample_phrase_annotation.png
+-rw-r--r--   0        0        0      774 2023-09-11 15:58:37.027687 vak-1.0.0a3/doc/toml/gy6or6_predict.toml
+-rw-r--r--   0        0        0      647 2023-09-11 15:58:37.035688 vak-1.0.0a3/doc/toml/gy6or6_train.toml
+-rw-r--r--   0        0        0     8924 2023-09-11 01:47:52.504007 vak-1.0.0a3/noxfile.py
+-rw-r--r--   0        0        0     2320 2023-09-23 17:51:06.103989 vak-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     4258 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/scripts/download_autoannotate_data.py
+-rw-r--r--   0        0        0      845 2023-09-23 17:51:06.107989 vak-1.0.0a3/src/vak/__about__.py
+-rw-r--r--   0        0        0      780 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/__init__.py
+-rw-r--r--   0        0        0     1401 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/__main__.py
+-rw-r--r--   0        0        0      239 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/cli/__init__.py
+-rw-r--r--   0        0        0     1097 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/cli/cli.py
+-rw-r--r--   0        0        0     2070 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/cli/eval.py
+-rw-r--r--   0        0        0     3131 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/cli/learncurve.py
+-rw-r--r--   0        0        0     2311 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/cli/predict.py
+-rw-r--r--   0        0        0     6312 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/cli/prep.py
+-rw-r--r--   0        0        0     2935 2023-08-21 14:21:20.822816 vak-1.0.0a3/src/vak/cli/train.py
+-rw-r--r--   0        0        0      845 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/__init__.py
+-rw-r--r--   0        0        0    27813 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/annotation.py
+-rw-r--r--   0        0        0     1147 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/constants.py
+-rw-r--r--   0        0        0     5087 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/converters.py
+-rw-r--r--   0        0        0      298 2023-06-06 21:30:23.974424 vak-1.0.0a3/src/vak/common/device.py
+-rw-r--r--   0        0        0      123 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/files/__init__.py
+-rw-r--r--   0        0        0     3418 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/files/files.py
+-rw-r--r--   0        0        0     8084 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/files/spect.py
+-rw-r--r--   0        0        0     5365 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/labels.py
+-rw-r--r--   0        0        0      432 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/learncurve.py
+-rw-r--r--   0        0        0     2620 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/logging.py
+-rw-r--r--   0        0        0     1371 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/paths.py
+-rw-r--r--   0        0        0     5248 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/common/tensorboard.py
+-rw-r--r--   0        0        0     1255 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/timebins.py
+-rw-r--r--   0        0        0      270 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/common/timenow.py
+-rw-r--r--   0        0        0     1968 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/common/trainer.py
+-rw-r--r--   0        0        0       77 2023-06-06 21:30:23.974424 vak-1.0.0a3/src/vak/common/typing.py
+-rw-r--r--   0        0        0     1989 2023-06-06 21:30:23.974424 vak-1.0.0a3/src/vak/common/validators.py
+-rw-r--r--   0        0        0      384 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/__init__.py
+-rw-r--r--   0        0        0     1577 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/config.py
+-rw-r--r--   0        0        0     6339 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/eval.py
+-rw-r--r--   0        0        0     2544 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/learncurve.py
+-rw-r--r--   0        0        0     2693 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/model.py
+-rw-r--r--   0        0        0     6322 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/parse.py
+-rw-r--r--   0        0        0     5203 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/predict.py
+-rw-r--r--   0        0        0     8091 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/config/prep.py
+-rw-r--r--   0        0        0     3126 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/spect_params.py
+-rw-r--r--   0        0        0     5468 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/train.py
+-rw-r--r--   0        0        0     3521 2023-08-14 01:30:57.912904 vak-1.0.0a3/src/vak/config/valid.toml
+-rw-r--r--   0        0        0     4568 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/config/validators.py
+-rw-r--r--   0        0        0      118 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/__init__.py
+-rw-r--r--   0        0        0      210 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/frame_classification/__init__.py
+-rw-r--r--   0        0        0      353 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/frame_classification/constants.py
+-rw-r--r--   0        0        0     4036 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/frame_classification/frames_dataset.py
+-rw-r--r--   0        0        0     6275 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/datasets/frame_classification/metadata.py
+-rw-r--r--   0        0        0     8543 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/frame_classification/window_dataset.py
+-rw-r--r--   0        0        0      131 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/parametric_umap/__init__.py
+-rw-r--r--   0        0        0     5411 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/parametric_umap/metadata.py
+-rw-r--r--   0        0        0    11175 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/datasets/parametric_umap/parametric_umap.py
+-rw-r--r--   0        0        0      175 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/eval/__init__.py
+-rw-r--r--   0        0        0     5899 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/eval/eval_.py
+-rw-r--r--   0        0        0     9223 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/eval/frame_classification.py
+-rw-r--r--   0        0        0     6226 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/eval/parametric_umap.py
+-rw-r--r--   0        0        0      241 2023-09-11 01:47:52.504007 vak-1.0.0a3/src/vak/learncurve/__init__.py
+-rw-r--r--   0        0        0     5682 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/learncurve/curvefit.py
+-rw-r--r--   0        0        0      538 2023-06-27 18:57:19.764652 vak-1.0.0a3/src/vak/learncurve/dirname.py
+-rw-r--r--   0        0        0    13170 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/learncurve/frame_classification.py
+-rw-r--r--   0        0        0     6455 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/learncurve/learncurve.py
+-rw-r--r--   0        0        0       94 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/metrics/__init__.py
+-rw-r--r--   0        0        0       69 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/metrics/classification/__init__.py
+-rw-r--r--   0        0        0      509 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/metrics/classification/classification.py
+-rw-r--r--   0        0        0      538 2020-11-07 21:56:36.549662 vak-1.0.0a3/src/vak/metrics/classification/functional.py
+-rw-r--r--   0        0        0       99 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/metrics/distance/__init__.py
+-rw-r--r--   0        0        0     1191 2021-04-13 02:29:39.812554 vak-1.0.0a3/src/vak/metrics/distance/distance.py
+-rw-r--r--   0        0        0     2909 2023-09-23 17:41:02.407718 vak-1.0.0a3/src/vak/metrics/distance/functional.py
+-rw-r--r--   0        0        0      810 2021-04-13 02:29:39.812554 vak-1.0.0a3/src/vak/metrics/util.py
+-rw-r--r--   0        0        0      635 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/models/__init__.py
+-rw-r--r--   0        0        0    16272 2023-08-14 13:35:41.524081 vak-1.0.0a3/src/vak/models/base.py
+-rw-r--r--   0        0        0     2068 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/models/convencoder_umap.py
+-rw-r--r--   0        0        0     2992 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/models/decorator.py
+-rw-r--r--   0        0        0    18905 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/models/definition.py
+-rw-r--r--   0        0        0     1571 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/models/ed_tcn.py
+-rw-r--r--   0        0        0    13791 2023-09-21 00:50:30.394719 vak-1.0.0a3/src/vak/models/frame_classification_model.py
+-rw-r--r--   0        0        0     3721 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/models/get.py
+-rw-r--r--   0        0        0     6453 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/models/parametric_umap_model.py
+-rw-r--r--   0        0        0     3506 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/models/registry.py
+-rw-r--r--   0        0        0     2389 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/models/tweetynet.py
+-rw-r--r--   0        0        0      260 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/nets/__init__.py
+-rw-r--r--   0        0        0     3018 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/nets/conv_encoder.py
+-rw-r--r--   0        0        0     4929 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nets/ed_tcn.py
+-rw-r--r--   0        0        0     7301 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/nets/tweetynet.py
+-rw-r--r--   0        0        0      128 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/__init__.py
+-rw-r--r--   0        0        0     2315 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/functional.py
+-rw-r--r--   0        0        0      158 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/loss/__init__.py
+-rw-r--r--   0        0        0     4672 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/loss/dice.py
+-rw-r--r--   0        0        0     4521 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/loss/umap.py
+-rw-r--r--   0        0        0      107 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/modules/__init__.py
+-rw-r--r--   0        0        0      850 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/modules/activation.py
+-rw-r--r--   0        0        0     3237 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/nn/modules/conv.py
+-rw-r--r--   0        0        0      244 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/plot/__init__.py
+-rw-r--r--   0        0        0     4455 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/plot/annot.py
+-rw-r--r--   0        0        0     4299 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/plot/learncurve.py
+-rw-r--r--   0        0        0     3997 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/plot/spect.py
+-rw-r--r--   0        0        0      190 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/predict/__init__.py
+-rw-r--r--   0        0        0    12523 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/predict/frame_classification.py
+-rw-r--r--   0        0        0     6341 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/predict/parametric_umap.py
+-rw-r--r--   0        0        0     6487 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/predict/predict_.py
+-rw-r--r--   0        0        0      448 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/__init__.py
+-rw-r--r--   0        0        0     7395 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/audio_dataset.py
+-rw-r--r--   0        0        0      548 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/constants.py
+-rw-r--r--   0        0        0     2770 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/dataset_df_helper.py
+-rw-r--r--   0        0        0      285 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/frame_classification/__init__.py
+-rw-r--r--   0        0        0    13744 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/frame_classification/dataset_arrays.py
+-rw-r--r--   0        0        0    17398 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/frame_classification/frame_classification.py
+-rw-r--r--   0        0        0     6709 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/frame_classification/learncurve.py
+-rw-r--r--   0        0        0     1595 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/frame_classification/validators.py
+-rw-r--r--   0        0        0      161 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/parametric_umap/__init__.py
+-rw-r--r--   0        0        0     4537 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/parametric_umap/dataset_arrays.py
+-rw-r--r--   0        0        0    13964 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/parametric_umap/parametric_umap.py
+-rw-r--r--   0        0        0     9661 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/prep_.py
+-rw-r--r--   0        0        0     2353 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/sequence_dataset.py
+-rw-r--r--   0        0        0      189 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/spectrogram_dataset/__init__.py
+-rw-r--r--   0        0        0     9857 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/spectrogram_dataset/audio_helper.py
+-rw-r--r--   0        0        0     8073 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/spectrogram_dataset/prep.py
+-rw-r--r--   0        0        0     3150 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/spectrogram_dataset/spect.py
+-rw-r--r--   0        0        0    11377 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/spectrogram_dataset/spect_helper.py
+-rw-r--r--   0        0        0      185 2023-08-24 14:39:59.417577 vak-1.0.0a3/src/vak/prep/split/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/split/algorithms/__init__.py
+-rw-r--r--   0        0        0    12457 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/split/algorithms/bruteforce.py
+-rw-r--r--   0        0        0     3918 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/split/algorithms/validate.py
+-rw-r--r--   0        0        0     9088 2023-09-11 01:47:52.508007 vak-1.0.0a3/src/vak/prep/split/split.py
+-rw-r--r--   0        0        0      130 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/prep/unit_dataset/__init__.py
+-rw-r--r--   0        0        0    12476 2023-08-18 14:49:44.247942 vak-1.0.0a3/src/vak/prep/unit_dataset/unit_dataset.py
+-rw-r--r--   0        0        0      180 2023-09-11 01:47:52.512007 vak-1.0.0a3/src/vak/train/__init__.py
+-rw-r--r--   0        0        0    14305 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/train/frame_classification.py
+-rw-r--r--   0        0        0    11393 2023-09-11 01:47:52.512007 vak-1.0.0a3/src/vak/train/parametric_umap.py
+-rw-r--r--   0        0        0     8819 2023-09-11 01:47:52.512007 vak-1.0.0a3/src/vak/train/train_.py
+-rw-r--r--   0        0        0       93 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/__init__.py
+-rw-r--r--   0        0        0      171 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/defaults/__init__.py
+-rw-r--r--   0        0        0     9714 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/defaults/frame_classification.py
+-rw-r--r--   0        0        0     1471 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/defaults/get.py
+-rw-r--r--   0        0        0      602 2023-09-11 01:47:52.512007 vak-1.0.0a3/src/vak/transforms/defaults/parametric_umap.py
+-rw-r--r--   0        0        0      128 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/frame_labels/__init__.py
+-rw-r--r--   0        0        0    17855 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/frame_labels/functional.py
+-rw-r--r--   0        0        0     9877 2023-08-14 13:35:41.528081 vak-1.0.0a3/src/vak/transforms/frame_labels/transforms.py
+-rw-r--r--   0        0        0     6788 2023-08-14 13:35:41.532081 vak-1.0.0a3/src/vak/transforms/functional.py
+-rw-r--r--   0        0        0    13478 2023-09-11 01:47:52.512007 vak-1.0.0a3/src/vak/transforms/transforms.py
+-rw-r--r--   0        0        0        0 2021-03-20 03:21:29.953394 vak-1.0.0a3/tests/__init__.py
+-rw-r--r--   0        0        0      900 2023-09-11 01:47:52.512007 vak-1.0.0a3/tests/conftest.py
+-rw-r--r--   0        0        0      328 2023-06-25 20:47:16.590134 vak-1.0.0a3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     5811 2023-09-11 01:47:52.512007 vak-1.0.0a3/tests/fixtures/annot.py
+-rw-r--r--   0        0        0     3897 2023-09-11 01:47:52.512007 vak-1.0.0a3/tests/fixtures/audio.py
+-rw-r--r--   0        0        0    12598 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/fixtures/config.py
+-rw-r--r--   0        0        0     1416 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/fixtures/csv.py
+-rw-r--r--   0        0        0     3412 2023-06-25 20:47:16.590134 vak-1.0.0a3/tests/fixtures/das.py
+-rw-r--r--   0        0        0     1157 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/fixtures/dataframe.py
+-rw-r--r--   0        0        0      810 2023-06-06 21:30:23.978424 vak-1.0.0a3/tests/fixtures/dataset.py
+-rw-r--r--   0        0        0      470 2021-04-13 02:29:39.816553 vak-1.0.0a3/tests/fixtures/device.py
+-rw-r--r--   0        0        0      541 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/fixtures/model.py
+-rw-r--r--   0        0        0      869 2023-06-06 21:30:23.978424 vak-1.0.0a3/tests/fixtures/path.py
+-rw-r--r--   0        0        0      745 2023-06-06 21:30:23.978424 vak-1.0.0a3/tests/fixtures/results.py
+-rw-r--r--   0        0        0     4310 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/fixtures/spect.py
+-rw-r--r--   0        0        0     1509 2023-06-06 21:30:23.978424 vak-1.0.0a3/tests/fixtures/split.py
+-rw-r--r--   0        0        0      245 2022-07-30 11:18:52.744175 vak-1.0.0a3/tests/fixtures/tensorboard.py
+-rw-r--r--   0        0        0     1235 2023-06-25 20:47:16.590134 vak-1.0.0a3/tests/fixtures/test_data.py
+-rw-r--r--   0        0        0      736 2023-02-18 03:07:26.485344 vak-1.0.0a3/tests/fixtures/torch.py
+-rw-r--r--   0        0        0    33574 2023-06-25 20:47:16.590134 vak-1.0.0a3/tests/scripts/das-test-data-env.txt
+-rw-r--r--   0        0        0    13491 2023-06-25 20:47:16.590134 vak-1.0.0a3/tests/scripts/das-test-data-env.yml
+-rw-r--r--   0        0        0     5387 2023-06-27 18:57:10.080703 vak-1.0.0a3/tests/scripts/generate_das_test_data.py
+-rw-r--r--   0        0        0     6969 2023-08-31 17:23:19.388619 vak-1.0.0a3/tests/scripts/generate_data_for_tests.py
+-rw-r--r--   0        0        0     2661 2021-04-13 02:29:39.816553 vak-1.0.0a3/tests/scripts/move_csv.py
+-rw-r--r--   0        0        0       99 2023-08-14 01:30:57.920904 vak-1.0.0a3/tests/scripts/vaktestdata/__init__.py
+-rw-r--r--   0        0        0      378 2023-08-14 01:30:57.920904 vak-1.0.0a3/tests/scripts/vaktestdata/config_metadata.py
+-rw-r--r--   0        0        0     7256 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/scripts/vaktestdata/configs.py
+-rw-r--r--   0        0        0     1595 2023-08-14 01:30:57.920904 vak-1.0.0a3/tests/scripts/vaktestdata/constants.py
+-rw-r--r--   0        0        0     2301 2023-08-14 01:30:57.920904 vak-1.0.0a3/tests/scripts/vaktestdata/dirs.py
+-rw-r--r--   0        0        0     1093 2023-08-14 01:30:57.920904 vak-1.0.0a3/tests/scripts/vaktestdata/parser.py
+-rw-r--r--   0        0        0     1231 2023-08-14 01:30:57.920904 vak-1.0.0a3/tests/scripts/vaktestdata/prep.py
+-rw-r--r--   0        0        0     1858 2022-07-30 11:18:52.744175 vak-1.0.0a3/tests/test___main__.py
+-rw-r--r--   0        0        0        0 2021-03-20 03:21:29.957394 vak-1.0.0a3/tests/test_cli/__init__.py
+-rw-r--r--   0        0        0      684 2023-05-30 01:19:26.147042 vak-1.0.0a3/tests/test_cli/cli_asserts.py
+-rw-r--r--   0        0        0     1949 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_cli/test_eval.py
+-rw-r--r--   0        0        0     2415 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_cli/test_learncurve.py
+-rw-r--r--   0        0        0     2043 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_cli/test_predict.py
+-rw-r--r--   0        0        0     3878 2023-06-06 21:30:23.978424 vak-1.0.0a3/tests/test_cli/test_prep.py
+-rw-r--r--   0        0        0     2562 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_cli/test_train.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/__init__.py
+-rw-r--r--   0        0        0    11367 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_annotation.py
+-rw-r--r--   0        0        0      535 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_console_script.py
+-rw-r--r--   0        0        0      853 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_converters.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_files/__init__.py
+-rw-r--r--   0        0        0     2865 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_files/test_files.py
+-rw-r--r--   0        0        0     2645 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_files/test_spect.py
+-rw-r--r--   0        0        0     3175 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_common/test_labels.py
+-rw-r--r--   0        0        0     2207 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_paths.py
+-rw-r--r--   0        0        0      510 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_tensorboard.py
+-rw-r--r--   0        0        0      317 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_timebins.py
+-rw-r--r--   0        0        0      595 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_common/test_timenow.py
+-rw-r--r--   0        0        0      163 2021-03-20 03:21:29.957394 vak-1.0.0a3/tests/test_config/__init__.py
+-rw-r--r--   0        0        0      704 2021-03-20 03:21:29.957394 vak-1.0.0a3/tests/test_config/attr_helpers.py
+-rw-r--r--   0        0        0     1088 2021-04-13 02:29:39.816553 vak-1.0.0a3/tests/test_config/test_config.py
+-rw-r--r--   0        0        0      417 2022-08-17 14:02:21.758688 vak-1.0.0a3/tests/test_config/test_eval.py
+-rw-r--r--   0        0        0      492 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_config/test_learncurve.py
+-rw-r--r--   0        0        0     1865 2023-06-05 14:33:25.510677 vak-1.0.0a3/tests/test_config/test_model.py
+-rw-r--r--   0        0        0     9648 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_config/test_parse.py
+-rw-r--r--   0        0        0      453 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_config/test_predict.py
+-rw-r--r--   0        0        0      479 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_config/test_prep.py
+-rw-r--r--   0        0        0     2127 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_config/test_spect_params.py
+-rw-r--r--   0        0        0      480 2021-04-13 02:29:39.816553 vak-1.0.0a3/tests/test_config/test_train.py
+-rw-r--r--   0        0        0      856 2021-04-13 02:29:39.816553 vak-1.0.0a3/tests/test_config/test_validators.py
+-rw-r--r--   0        0        0        0 2022-08-17 14:02:21.762688 vak-1.0.0a3/tests/test_datasets/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_datasets/test_frame_classification/__init__.py
+-rw-r--r--   0        0        0     1395 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_datasets/test_frame_classification/test_frames_dataset.py
+-rw-r--r--   0        0        0     3299 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_datasets/test_frame_classification/test_metadata.py
+-rw-r--r--   0        0        0     1623 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_datasets/test_frame_classification/test_window_dataset.py
+-rw-r--r--   0        0        0        0 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_datasets/test_parametric_umap/__init__.py
+-rw-r--r--   0        0        0     1428 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_datasets/test_parametric_umap/test_parametric_umap.py
+-rw-r--r--   0        0        0        0 2022-08-17 14:02:21.762688 vak-1.0.0a3/tests/test_datasets/test_seq/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_eval/__init__.py
+-rw-r--r--   0        0        0     2284 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_eval/test_eval.py
+-rw-r--r--   0        0        0     6973 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_eval/test_frame_classification.py
+-rw-r--r--   0        0        0     5674 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_eval/test_parametric_umap.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_learncurve/__init__.py
+-rw-r--r--   0        0        0     6017 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_learncurve/test_frame_classification.py
+-rw-r--r--   0        0        0        0 2021-04-25 00:42:45.347480 vak-1.0.0a3/tests/test_metrics/__init__.py
+-rw-r--r--   0        0        0        0 2021-04-25 00:42:45.347480 vak-1.0.0a3/tests/test_metrics/test_distance/__init__.py
+-rw-r--r--   0        0        0     1613 2021-04-25 00:42:45.347480 vak-1.0.0a3/tests/test_metrics/test_distance/test_functional.py
+-rw-r--r--   0        0        0        0 2021-04-04 15:40:00.958474 vak-1.0.0a3/tests/test_models/__init__.py
+-rw-r--r--   0        0        0     5175 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_models/conftest.py
+-rw-r--r--   0        0        0    11862 2023-09-11 01:47:52.516007 vak-1.0.0a3/tests/test_models/test_base.py
+-rw-r--r--   0        0        0     1564 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_convencoder_umap.py
+-rw-r--r--   0        0        0     2045 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_decorator.py
+-rw-r--r--   0        0        0    10934 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_definition.py
+-rw-r--r--   0        0        0     1139 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_ed_tcn.py
+-rw-r--r--   0        0        0     5770 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_frame_classification_model.py
+-rw-r--r--   0        0        0     5088 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_parametric_umap_model.py
+-rw-r--r--   0        0        0     4232 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_registry.py
+-rw-r--r--   0        0        0     1966 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_models/test_tweetynet.py
+-rw-r--r--   0        0        0        0 2023-06-05 14:33:25.514677 vak-1.0.0a3/tests/test_nets/__init__.py
+-rw-r--r--   0        0        0     1413 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_nets/test_convencoder.py
+-rw-r--r--   0        0        0     2944 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_nets/test_ed_tcn.py
+-rw-r--r--   0        0        0     2957 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_nets/test_tweetynet.py
+-rw-r--r--   0        0        0        0 2021-04-25 22:29:23.560050 vak-1.0.0a3/tests/test_nn/__init__.py
+-rw-r--r--   0        0        0      726 2022-07-30 11:18:52.748175 vak-1.0.0a3/tests/test_nn/test_functional.py
+-rw-r--r--   0        0        0        0 2021-04-25 22:29:23.560050 vak-1.0.0a3/tests/test_nn/test_loss/__init__.py
+-rw-r--r--   0        0        0     2512 2021-04-25 22:29:23.560050 vak-1.0.0a3/tests/test_nn/test_loss/test_dice.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_predict/__init__.py
+-rw-r--r--   0        0        0     8097 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_predict/test_frame_classification.py
+-rw-r--r--   0        0        0     2419 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_predict/test_predict.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/__init__.py
+-rw-r--r--   0        0        0     4191 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_audio_dataset.py
+-rw-r--r--   0        0        0        0 2023-06-25 20:47:16.590134 vak-1.0.0a3/tests/test_prep/test_frame_classification/__init__.py
+-rw-r--r--   0        0        0     6377 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_frame_classification/test_dataset_arrays.py
+-rw-r--r--   0        0        0    13143 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_frame_classification/test_frame_classification.py
+-rw-r--r--   0        0        0     3896 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_frame_classification/test_learncurve.py
+-rw-r--r--   0        0        0       67 2023-06-27 18:57:19.764652 vak-1.0.0a3/tests/test_prep/test_frame_classification/test_validators.py
+-rw-r--r--   0        0        0     2777 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_prep.py
+-rw-r--r--   0        0        0     1259 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_sequence_dataset.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/__init__.py
+-rw-r--r--   0        0        0    15324 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/test_audio_helper.py
+-rw-r--r--   0        0        0     9300 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/test_prep.py
+-rw-r--r--   0        0        0     7275 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/test_spect_helper.py
+-rw-r--r--   0        0        0       55 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/test_split/__init__.py
+-rw-r--r--   0        0        0       58 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/test_split/test_algorithms/__init__.py
+-rw-r--r--   0        0        0     9531 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/test_split/test_algorithms/test_bruteforce.py
+-rw-r--r--   0        0        0     2330 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_prep/test_split/test_algorithms/test_validate.py
+-rw-r--r--   0        0        0    10892 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_prep/test_split/test_split.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:30:23.982424 vak-1.0.0a3/tests/test_train/__init__.py
+-rw-r--r--   0        0        0     9778 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_train/test_frame_classification.py
+-rw-r--r--   0        0        0     6730 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_train/test_parametric_umap.py
+-rw-r--r--   0        0        0     2892 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_train/test_train.py
+-rw-r--r--   0        0        0        0 2023-02-11 00:18:57.767185 vak-1.0.0a3/tests/test_transforms/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-11 01:47:52.520007 vak-1.0.0a3/tests/test_transforms/test_frame_labels/__init__.py
+-rw-r--r--   0        0        0    17206 2023-09-11 01:47:52.524007 vak-1.0.0a3/tests/test_transforms/test_frame_labels/test_functional.py
+-rw-r--r--   0        0        0     9096 2023-09-11 01:47:52.524007 vak-1.0.0a3/tests/test_transforms/test_frame_labels/test_transforms.py
+-rw-r--r--   0        0        0     4789 2023-09-11 01:47:52.524007 vak-1.0.0a3/tests/test_transforms/test_transforms.py
+-rw-r--r--   0        0        0       61 2023-09-11 01:47:52.524007 vak-1.0.0a3/tests/vak.tests.config.json
+-rw-r--r--   0        0        0    20830 1970-01-01 00:00:00.000000 vak-1.0.0a3/PKG-INFO
```

### Comparing `vak-1.0.0a2/.all-contributorsrc` & `vak-1.0.0a3/.all-contributorsrc`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060606%*

 * *Differences: {"'contributors'": "{insert: [(21, OrderedDict([('login', 'VenetianRed'), ('name', 'Mark "*

 * *                   "Muldoon'), ('avatar_url', "*

 * *                   "'https://avatars.githubusercontent.com/u/5350159?v=4'), ('profile', "*

 * *                   "'http://maths.manchester.ac.uk/~mrm/'), ('contributions', ['bug'])]))]}"}*

```diff
@@ -214,14 +214,23 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/52127436?v=4",
             "contributions": [
                 "bug"
             ],
             "login": "JacquelineGoe",
             "name": "Jacqueline",
             "profile": "https://github.com/JacquelineGoe"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/5350159?v=4",
+            "contributions": [
+                "bug"
+            ],
+            "login": "VenetianRed",
+            "name": "Mark Muldoon",
+            "profile": "http://maths.manchester.ac.uk/~mrm/"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `vak-1.0.0a2/.github/CONTRIBUTING.md` & `vak-1.0.0a3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md` & `vak-1.0.0a3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/.github/ISSUE_TEMPLATE/feature_request.md` & `vak-1.0.0a3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/.github/workflows/ci-linux.yml` & `vak-1.0.0a3/.github/workflows/ci-linux.yml`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/CITATION.cff` & `vak-1.0.0a3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/CODE_OF_CONDUCT.md` & `vak-1.0.0a3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/LICENSE` & `vak-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/README.md` & `vak-1.0.0a3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 <hr>
 
 ## A neural network framework for animal acoustic communication and bioacoustics
 
 [![DOI](https://zenodo.org/badge/173566541.svg)](https://zenodo.org/badge/latestdoi/173566541)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-21-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-22-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 [![PyPI version](https://badge.fury.io/py/vak.svg)](https://badge.fury.io/py/vak)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Build Status](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/badge.svg)](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/badge.svg)
 [![codecov](https://codecov.io/gh/vocalpy/vak/branch/main/graph/badge.svg?token=9Y4XXB2ELA)](https://codecov.io/gh/vocalpy/vak)
 
-<h3>🚧 vak version 1.0.0 is in development! 🚧 📣 Test out the alpha release: <code>pip install vak==1.0.0a1</code>. 📣 For more info, please see <a href="https://forum.vocalpy.org/t/vak-1-0-0a1-released/55"> this forum post<a>.</h3>
+<h3>🚧 vak version 1.0.0 is in development! 🚧 📣 Test out the alpha release: <code>pip install vak==1.0.0a2</code>. 📣 For more info, please see <a href="https://forum.vocalpy.org/t/vak-1-0-0a1-released/55"> this forum post<a>.</h3>
 
 
 `vak` is a Python framework for neural network models, 
 designed for researchers studying animal acoustic communication and bioacoustics.
 Many people will be familiar with work in this area on 
 animal vocalizations such as birdsong, bat calls, and even human speech.
 Neural network models have provided a powerful new tool for researchers in this area, 
@@ -42,14 +42,25 @@
 You give `vak` training data in the form of audio or spectrogram files with annotations, 
 and then `vak` helps you train neural network models 
 and use the trained models to predict annotations for new files.
 
 We developed `vak` to benchmark a neural network model we call [`tweetynet`](https://github.com/yardencsGitHub/tweetynet).  
 Please see the eLife article here: https://elifesciences.org/articles/63853  
 
+To learn more about the goals and design of vak, 
+please see this talk from the SciPy 2023 conference, 
+and the associated Proceedings paper 
+[here](https://conference.scipy.org/proceedings/scipy2023/pdfs/david_nicholson.pdf).
+
+<p align="center">
+<a href="https://www.youtube.com/watch?v=tpL0m5UwpZM" target="_blank">
+ <img src="https://img.youtube.com/vi/tpL0m5UwpZM/mqdefault.jpg" alt="Thumbnail of SciPy 2023 talk on vak" width="400" border="10" />
+</a>
+</p>
+
 For more background on animal acoustic communication and deep learning, 
 and how these intersect with related fields like 
 computational ethology and neuroscience,
 please see the ["About"](#About) section below.
 
 ### Installation
 Short version:
@@ -108,15 +119,31 @@
 please use the issue tracker on GitHub:  
 <https://github.com/vocalpy/vak/issues>
 
 For a guide on how you can contribute to `vak`, please see:
 https://vak.readthedocs.io/en/latest/development/index.html
 
 ### Citation
-If you use vak for a publication, please cite its DOI:  
+If you use vak for a publication, please cite both the Proceedings paper and the software.
+
+#### Proceedings paper (BiBTex)
+
+```
+@inproceedings{nicholson2023vak,
+  title={vak: a neural network framework for researchers studying animal acoustic communication},
+  author={Nicholson, David and Cohen, Yarden},
+  booktitle={Python in Science Conference},
+  pages={59--67},
+  year={2023}
+}
+
+```
+
+#### Software
+
 [![DOI](https://zenodo.org/badge/173566541.svg)](https://zenodo.org/badge/latestdoi/173566541)
 
 ### License
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)  
 is [here](./LICENSE).
 
 ### About
@@ -190,14 +217,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lmpascual"><img src="https://avatars.githubusercontent.com/u/62260534?v=4?s=100" width="100px;" alt="lmpascual"/><br /><sub><b>lmpascual</b></sub></a><br /><a href="https://github.com/vocalpy/vak/commits?author=lmpascual" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ItamarFruchter"><img src="https://avatars.githubusercontent.com/u/19908942?v=4?s=100" width="100px;" alt="ItamarFruchter"/><br /><sub><b>ItamarFruchter</b></sub></a><br /><a href="https://github.com/vocalpy/vak/commits?author=ItamarFruchter" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kalleknast"><img src="https://avatars.githubusercontent.com/u/12412777?v=4?s=100" width="100px;" alt="Hjalmar K. Turesson"/><br /><sub><b>Hjalmar K. Turesson</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3Akalleknast" title="Bug reports">🐛</a> <a href="#ideas-kalleknast" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nhoglen"><img src="https://avatars.githubusercontent.com/u/13972140?v=4?s=100" width="100px;" alt="nhoglen"/><br /><sub><b>nhoglen</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3Anhoglen" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://test0.zip"><img src="https://avatars.githubusercontent.com/u/46551097?v=4?s=100" width="100px;" alt="Ja-sonYun"/><br /><sub><b>Ja-sonYun</b></sub></a><br /><a href="https://github.com/vocalpy/vak/commits?author=Ja-sonYun" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/JacquelineGoe"><img src="https://avatars.githubusercontent.com/u/52127436?v=4?s=100" width="100px;" alt="Jacqueline"/><br /><sub><b>Jacqueline</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3AJacquelineGoe" title="Bug reports">🐛</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://maths.manchester.ac.uk/~mrm/"><img src="https://avatars.githubusercontent.com/u/5350159?v=4?s=100" width="100px;" alt="Mark Muldoon"/><br /><sub><b>Mark Muldoon</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3AVenetianRed" title="Bug reports">🐛</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 
       [https://github.com/vocalpy/vak/blob/main/doc/images/logo/vak-logo-
                              primary.png?raw=True]
 ===============================================================================
 ## A neural network framework for animal acoustic communication and
 bioacoustics [![DOI](https://zenodo.org/badge/173566541.svg)](https://
 zenodo.org/badge/latestdoi/173566541) [![All Contributors](https://
-img.shields.io/badge/all_contributors-21-orange.svg?style=flat-square)]
+img.shields.io/badge/all_contributors-22-orange.svg?style=flat-square)]
 (#contributors-) [![PyPI version](https://badge.fury.io/py/vak.svg)](https://
 badge.fury.io/py/vak) [![License](https://img.shields.io/badge/License-BSD%203-
 -Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Build
 Status](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/
 badge.svg)](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/
 badge.svg) [![codecov](https://codecov.io/gh/vocalpy/vak/branch/main/graph/
 badge.svg?token=9Y4XXB2ELA)](https://codecov.io/gh/vocalpy/vak)
 ******** ?ð???§ vvaakk vveerrssiioonn 11..00..00 iiss iinn ddeevveellooppmmeenntt!! ?ð???§ ?ð???£ TTeesstt oouutt tthhee aallpphhaa
-rreelleeaassee:: ppiipp iinnssttaallll vvaakk====11..00..00aa11.. ?ð???£ FFoorr mmoorree iinnffoo,, pplleeaassee sseeee _tt_hh_ii_ss_ _ff_oo_rr_uu_mm
+rreelleeaassee:: ppiipp iinnssttaallll vvaakk====11..00..00aa22.. ?ð???£ FFoorr mmoorree iinnffoo,, pplleeaassee sseeee _tt_hh_ii_ss_ _ff_oo_rr_uu_mm
 _pp_oo_ss_tt_.. ********
 `vak` is a Python framework for neural network models, designed for researchers
 studying animal acoustic communication and bioacoustics. Many people will be
 familiar with work in this area on animal vocalizations such as birdsong, bat
 calls, and even human speech. Neural network models have provided a powerful
 new tool for researchers in this area, as in many other fields. The library has
 two main goals: 1. Make it easier for researchers studying animal vocalizations
@@ -29,71 +29,81 @@
 the example of annotated birdsong shown below:
               [spectrogram of birdsong with syllables annotated]
 You give `vak` training data in the form of audio or spectrogram files with
 annotations, and then `vak` helps you train neural network models and use the
 trained models to predict annotations for new files. We developed `vak` to
 benchmark a neural network model we call [`tweetynet`](https://github.com/
 yardencsGitHub/tweetynet). Please see the eLife article here: https://
-elifesciences.org/articles/63853 For more background on animal acoustic
-communication and deep learning, and how these intersect with related fields
-like computational ethology and neuroscience, please see the ["About"](#About)
-section below. ### Installation Short version: #### with `pip` ```console $ pip
-install vak ``` #### with `conda` ```console $ conda install vak -c pytorch -
-c conda-forge $ # ^ notice additional channel! ``` Notice that for `conda` you
-specify two channels, and that the `pytorch` channel should come first, so it
-takes priority when installing the dependencies `pytorch` and `torchvision`.
-For more details, please see: https://vak.readthedocs.io/en/latest/get_started/
-installation.html We test `vak` on Ubuntu and MacOS. We have run on Windows and
-know of other users successfully running `vak` on that operating system, but
-installation on Windows may require some troubleshooting. A good place to start
-is by searching the [issues](https://github.com/vocalpy/vak/issues). ### Usage
-#### Tutorial Currently the easiest way to work with `vak` is through the
-command line. ![terminal showing vak help command output](https://github.com/
-vocalpy/vak/blob/main/doc/images/terminalizer/vak-help.gif?raw=True) You run it
-with configuration files, using one of a handful of commands. For more details,
+elifesciences.org/articles/63853 To learn more about the goals and design of
+vak, please see this talk from the SciPy 2023 conference, and the associated
+Proceedings paper [here](https://conference.scipy.org/proceedings/scipy2023/
+pdfs/david_nicholson.pdf).
+                     _[_T_h_u_m_b_n_a_i_l_ _o_f_ _S_c_i_P_y_ _2_0_2_3_ _t_a_l_k_ _o_n_ _v_a_k_]
+For more background on animal acoustic communication and deep learning, and how
+these intersect with related fields like computational ethology and
+neuroscience, please see the ["About"](#About) section below. ### Installation
+Short version: #### with `pip` ```console $ pip install vak ``` #### with
+`conda` ```console $ conda install vak -c pytorch -c conda-forge $ # ^ notice
+additional channel! ``` Notice that for `conda` you specify two channels, and
+that the `pytorch` channel should come first, so it takes priority when
+installing the dependencies `pytorch` and `torchvision`. For more details,
+please see: https://vak.readthedocs.io/en/latest/get_started/installation.html
+We test `vak` on Ubuntu and MacOS. We have run on Windows and know of other
+users successfully running `vak` on that operating system, but installation on
+Windows may require some troubleshooting. A good place to start is by searching
+the [issues](https://github.com/vocalpy/vak/issues). ### Usage #### Tutorial
+Currently the easiest way to work with `vak` is through the command line. !
+[terminal showing vak help command output](https://github.com/vocalpy/vak/blob/
+main/doc/images/terminalizer/vak-help.gif?raw=True) You run it with
+configuration files, using one of a handful of commands. For more details,
 please see the "autoannotate" tutorial here: https://vak.readthedocs.io/en/
 latest/get_started/autoannotate.html #### How can I use my data with `vak`?
 Please see the How-To Guides in the documentation here: https://
 vak.readthedocs.io/en/latest/howto/index.html ### Support / Contributing For
 help, please begin by checking out the Frequently Asked Questions: https://
 vak.readthedocs.io/en/latest/faq.html. To ask a question about vak, discuss its
 development, or share how you are using it, please start a new "Q&A" topic on
 the VocalPy forum with the vak tag:
 forum.vocalpy.org/> To report a bug, or to request a feature, please use the
 issue tracker on GitHub:
 github.com/vocalpy/vak/issues> For a guide on how you can contribute to `vak`,
 please see: https://vak.readthedocs.io/en/latest/development/index.html ###
-Citation If you use vak for a publication, please cite its DOI: [![DOI](https:/
-/zenodo.org/badge/173566541.svg)](https://zenodo.org/badge/latestdoi/173566541)
-### License [![License](https://img.shields.io/badge/License-BSD%203--Clause-
-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) is [here](./LICENSE).
-### About Are humans unique among animals? We speak languages, but is speech
-somehow like other animal behaviors, such as birdsong? Questions like these are
-answered by studying how animals communicate with sound. This research requires
-cutting edge computational methods and big team science across a wide range of
-disciplines, including ecology, ethology, bioacoustics, psychology,
-neuroscience, linguistics, and genomics [^1][^2][^3]. As in many other domains,
-this research is being revolutionized by deep learning algorithms [^1][^2][^3].
-Deep neural network models enable answering questions that were previously
-impossible to address, in part because these models automate analysis of very
-large datasets. Within the study of animal acoustic communication, multiple
-models have been proposed for similar tasks, often implemented as research code
-with different libraries, such as Keras and Pytorch. This situation has created
-a real need for a framework that allows researchers to easily benchmark models
-and apply trained models to their own data. To address this need, we developed
-vak. We originally developed vak to benchmark a neural network model, TweetyNet
-[^4][^5], that automates annotation of birdsong by segmenting spectrograms.
-TweetyNet and vak have been used in both neuroscience [^6][^7][^8] and
-bioacoustics [^9]. For additional background and papers that have used `vak`,
-please see: https://vak.readthedocs.io/en/latest/reference/about.html [^1]:
-https://www.frontiersin.org/articles/10.3389/fnbeh.2021.811737/full [^2]:
-https://peerj.com/articles/13152/ [^3]: https://www.jneurosci.org/content/42/
-45/8514 [^4]: https://elifesciences.org/articles/63853 [^5]: https://
-github.com/yardencsGitHub/tweetynet [^6]: https://www.nature.com/articles/
-s41586-020-2397-3 [^7]: https://elifesciences.org/articles/67855 [^8]: https://
+Citation If you use vak for a publication, please cite both the Proceedings
+paper and the software. #### Proceedings paper (BiBTex) ``` @inproceedings
+{nicholson2023vak, title={vak: a neural network framework for researchers
+studying animal acoustic communication}, author={Nicholson, David and Cohen,
+Yarden}, booktitle={Python in Science Conference}, pages={59--67}, year={2023}
+} ``` #### Software [![DOI](https://zenodo.org/badge/173566541.svg)](https://
+zenodo.org/badge/latestdoi/173566541) ### License [![License](https://
+img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/
+licenses/BSD-3-Clause) is [here](./LICENSE). ### About Are humans unique among
+animals? We speak languages, but is speech somehow like other animal behaviors,
+such as birdsong? Questions like these are answered by studying how animals
+communicate with sound. This research requires cutting edge computational
+methods and big team science across a wide range of disciplines, including
+ecology, ethology, bioacoustics, psychology, neuroscience, linguistics, and
+genomics [^1][^2][^3]. As in many other domains, this research is being
+revolutionized by deep learning algorithms [^1][^2][^3]. Deep neural network
+models enable answering questions that were previously impossible to address,
+in part because these models automate analysis of very large datasets. Within
+the study of animal acoustic communication, multiple models have been proposed
+for similar tasks, often implemented as research code with different libraries,
+such as Keras and Pytorch. This situation has created a real need for a
+framework that allows researchers to easily benchmark models and apply trained
+models to their own data. To address this need, we developed vak. We originally
+developed vak to benchmark a neural network model, TweetyNet [^4][^5], that
+automates annotation of birdsong by segmenting spectrograms. TweetyNet and vak
+have been used in both neuroscience [^6][^7][^8] and bioacoustics [^9]. For
+additional background and papers that have used `vak`, please see: https://
+vak.readthedocs.io/en/latest/reference/about.html [^1]: https://
+www.frontiersin.org/articles/10.3389/fnbeh.2021.811737/full [^2]: https://
+peerj.com/articles/13152/ [^3]: https://www.jneurosci.org/content/42/45/8514
+[^4]: https://elifesciences.org/articles/63853 [^5]: https://github.com/
+yardencsGitHub/tweetynet [^6]: https://www.nature.com/articles/s41586-020-2397-
+3 [^7]: https://elifesciences.org/articles/67855 [^8]: https://
 elifesciences.org/articles/75691 [^9]: https://journals.plos.org/plosone/
 article?id=10.1371/journal.pone.0278522 #### "Why this name, vak?" It has only
 three letters, so it is quick to type, and it wasn't taken on [pypi](https://
 pypi.org/) yet. Also I guess it has [something to do with speech](https://
 en.wikipedia.org/wiki/V%C4%81c). "vak" rhymes with "squawk" and "talk". ####
 Does your library have any poems? [Yes.](https://vak.readthedocs.io/en/latest/
 poems/index.html) ## Contributors â¨ Thanks goes to these wonderful people (
@@ -115,10 +125,13 @@
      _ð___        _ð___ _ð___      _ð___» _ð__¤_      _ð___ _ð___     _ð___ _ð___     _ð___     _ð___ _ð___
                                                                                        _ð__¤_
  _[_y_a_n_g_z_h_e_n_g_-    _[_l_m_p_a_s_c_u_a_l_]  _[_I_t_a_m_a_r_F_r_u_c_h_t_e_r_] _[_H_j_a_l_m_a_r_ _K_.    _[_n_h_o_g_l_e_n_]     _[_J_a_-   _[_J_a_c_q_u_e_l_i_n_e_]
      _1_2_1_]        _ll_mm_pp_aa_ss_cc_uu_aa_ll    _II_tt_aa_mm_aa_rr_FF_rr_uu_cc_hh_tt_ee_rr   _T_u_r_e_s_s_o_n_]      _nn_hh_oo_gg_ll_ee_nn    _s_o_n_Y_u_n_]   _JJ_aa_cc_qq_uu_ee_ll_ii_nn_ee
 _yy_aa_nn_gg_zz_hh_ee_nn_gg_--_11_22_11      _ð___            _ð___       _HH_jj_aa_ll_mm_aa_rr_ _KK_..        _ð___       _JJ_aa_--        _ð___
   _ð___ _ð__¤_                                    _TT_uu_rr_ee_ss_ss_oo_nn                   _ss_oo_nn_YY_uu_nn
                                                _ð___ _ð__¤_                   _ð___»
+_[_M_a_r_k_ _M_u_l_d_o_o_n_]
+ _MM_aa_rr_kk_ _MM_uu_ll_dd_oo_oo_nn
+     _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `vak-1.0.0a2/doc/CHANGELOG.md` & `vak-1.0.0a3/doc/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,17 @@
   and to clean up spaghetti code that slows down adding new functionality. 
   Move functions from core up to top-level: eval, learncurve, predict, prep, train.
   Move `vak.io` into prep, rename `prep_spectrogram_dataset`. Also move `vak.spect` in there.
   Move `vak.split` into `vak.prep` since that's the only place it's used.
   Make various other minor clean-ups.
   [#666](https://github.com/NickleDave/vak/pull/666).
   Fixes [#663](https://github.com/NickleDave/vak/issues/663).
+- Have distance metrics return tensors
+  [#702](https://github.com/NickleDave/vak/pull/702).
+  Fixes [#701](https://github.com/NickleDave/vak/issues/701).
 
 ### Removed
 - Remove entry points since they are not being used
   outside the project but require maintenance and testing
   [#621](https://github.com/NickleDave/vak/pull/621).
   Fixes [#601](https://github.com/NickleDave/vak/issues/601).
 - Remove unused/incomplete functionality for training multiple models
@@ -99,14 +102,17 @@
 - Change label mapping to use single characters
   for the validation step of WindowedFrameClassificationModel *only*,
   to avoid affecting the edit distance metric, 
   instead of modifying the mapping inside the top-level eval function,
   which can cause a crash because the mapping is used in other places 
   [#665](https://github.com/NickleDave/vak/pull/665).
   Fixed in [#664](https://github.com/NickleDave/vak/pull/664).
+- Fix bug that caused crash on Apple M1 / MPS accelerator 
+  [#700](https://github.com/NickleDave/vak/issues/700).
+  Fixed in [#702](https://github.com/NickleDave/vak/pull/702).
 
 ## 0.8.1 -- 2023-03-02
 ### Fixed
 - Fix transform that converts labeled timebins to segments
   so that it returns all `None`s when there are no segments 
   in the vector, either before or after applying any 
   post-processing transforms
```

### Comparing `vak-1.0.0a2/doc/Makefile` & `vak-1.0.0a3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/_templates/class.rst` & `vak-1.0.0a3/doc/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/_templates/module.rst` & `vak-1.0.0a3/doc/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/api/index.rst` & `vak-1.0.0a3/doc/api/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -20,46 +20,120 @@
    cli.cli
    cli.eval
    cli.learncurve
    cli.predict
    cli.prep
    cli.train
 
-Core
-----
+Commands
+--------
+
+These high-level functions correspond to commands in the
+commmand-line interface. The commands are to prepare datasets,
+train and evaluate models, and generate predictions from trained models.
+
+Prep
+~~~~
+
+.. autosummary::
+   :toctree: generated
+   :template: module.rst
+   :recursive:
+
+   prep
+   prep.frame_classification
+   prep.parametric_umap
+   prep.spectrogram_dataset
+   prep.unit_dataset
+   prep.audio_dataset
+   prep.constants
+   prep.dataset_df_helper
+   prep.prep_
+   prep.sequence_dataset
+
+Train-test-validation splits of datasets
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The :mod:`vak.split` module contains functionality
+for generating train-validation-test splits from
+datasets. It is called by the :mod:`vak.prep` function
+when running ``vak prep`` through the command line interface.
+
+.. autosummary::
+   :toctree: generated
+   :template: module.rst
+   :recursive:
+
+   prep.split.algorithms.bruteforce
+   prep.split.algorithms.validate
+   prep.split.split
+
+
+Train
+~~~~~
+
+.. autosummary::
+   :toctree: generated
+   :template: module.rst
+   :recursive:
+
+   train.train_
+   train.frame_classification
+   train.parametric_umap
+
+Eval
+~~~~
+
+.. autosummary::
+   :toctree: generated
+   :template: module.rst
+   :recursive:
 
-The :mod:`vak.core` module contains high-level functions called by the
-commmand-line interface to prepare datasets, train and evaluate
-models, and generate predictions from trained models.
+   eval.eval_
+   eval.frame_classification
+   eval.parametric_umap
+
+Predict
+~~~~~~~
+
+.. autosummary::
+   :toctree: generated
+   :template: module.rst
+   :recursive:
+
+   predict.predict_
+   predict.frame_classification
+   predict.parametric_umap
+
+Learning Curve
+~~~~~~~~~~~~~~
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
-   core.learncurve
-   core.eval
-   core.predict
-   core.prep
-   core.train
+   learncurve.curvefit
+   learncurve.dirname
+   learncurve.frame_classification
+   learncurve.learncurve
 
 Configuration files
 -------------------
 
 The :mod:`vak.config` module contains functions to parse
 the TOML configuration files used with vak,
 and dataclasses that represent tables from those files.
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
    config.config
-   config.dataloader
    config.eval
    config.learncurve
    config.model
    config.parse
    config.predict
    config.prep
    config.spect_params
@@ -71,43 +145,16 @@
 The :mod:`vak.datasets` module contains datasets built into vak.
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
-   datasets.seq.validators
-   datasets.vocal_dataset
-   datasets.window_dataset
-
-Files
---------
-The :mod:`vak.files` module contains helper functions for working with files.
-
-.. autosummary::
-   :toctree: generated
-   :template: module.rst
-   :recursive:
-
-   files.files
-   files.spect
-
-Input-Output
-------------
-The :mod:`vak.io` module contains functions for generating datasets used by vak
-from input files: audio files, spectograms, and/or annotation files.
-
-.. autosummary::
-   :toctree: generated
-   :template: module.rst
-   :recursive:
-
-   io.audio
-   io.dataframe
-   io.spect
+   datasets.frame_classification
+   datasets.parametric_umap
 
 Metrics
 -------
 The :mod:`vak.metrics` module contains metrics used
 when evaluating neural network model performance.
 
 .. autosummary::
@@ -129,36 +176,39 @@
 for training, predicting, etc.
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
-   models._api
    models.base
+   models.convencoder_umap
    models.decorator
    models.definition
+   models.ed_tcn
+   models.frame_classification_model
    models.get
-   models.teenytweetynet
+   models.parametric_umap_model
+   models.registry
    models.tweetynet
-   models.windowed_frame_classification_model
 
 Nets
 ----
 The :mod:`vak.nets` module contains
 neural network architectures built into vak.
 All models include a neural network architecture
 (along with an optimizer, loss function, and metrics).
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
-   nets.teenytweetynet
+   nets.conv_encoder
+   nets.ed_tcn
    nets.tweetynet
 
 Neural Network Layers and Operations
 ------------------------------------
 The :mod:`vak.nn` module contains
 operations, layers, and other graph components
 used in neural network architectures.
@@ -182,65 +232,51 @@
    :template: module.rst
    :recursive:
 
    plot.annot
    plot.learncurve
    plot.spect
 
-Train-test-validation splits of datasets
-----------------------------------------
-
-The :mod:`vak.split` module contains functionality
-for generating train-validation-test splits from
-datasets. It is called by the :mod:`vak.prep` function
-when running ``vak prep`` through the command line interface.
-
-.. autosummary::
-   :toctree: generated
-   :template: module.rst
-   :recursive:
-
-   split.algorithms.bruteforce
-   split.algorithms.validate
-   split.split
-
 Transforms
 ----------
 
 The :mod:`vak.transforms` module contains transforms
 that can be applied to input or output of neural networks,
 i.e., for pre-processing or post-processing.
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
-   transforms.labeled_timebins.functional
-   transforms.labeled_timebins.transforms
+   transforms.defaults
+   transforms.frame_labels.functional
+   transforms.frame_labels.transforms
    transforms.functional
    transforms.transforms
 
-Miscellaneous
--------------
+Common
+------
+
+This module contains helper functions
+used by multiple other modules.
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
 
-   annotation
-   constants
-   converters
-   curvefit
-   device
-   labeled_timebins
-   labels
-   logging
-   paths
-   spect
-   tensorboard
-   timebins
-   timenow
-   trainer
-   typing
-   validators
+   common.annotation
+   common.constants
+   common.converters
+   common.device
+   common.files
+   common.labels
+   common.learncurve
+   common.logging
+   common.paths
+   common.tensorboard
+   common.timebins
+   common.timenow
+   common.trainer
+   common.typing
+   common.validators
```

### Comparing `vak-1.0.0a2/doc/conf.py` & `vak-1.0.0a3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/development/contributors.md` & `vak-1.0.0a3/doc/development/contributors.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/development/index.md` & `vak-1.0.0a3/doc/development/index.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/faq.md` & `vak-1.0.0a3/doc/faq.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/get_started/autoannotate.md` & `vak-1.0.0a3/doc/get_started/autoannotate.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/get_started/index.md` & `vak-1.0.0a3/doc/get_started/index.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/get_started/installation.md` & `vak-1.0.0a3/doc/get_started/installation.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/howto/howto_prep_annotate.md` & `vak-1.0.0a3/doc/howto/howto_prep_annotate.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/howto/howto_user_annot.md` & `vak-1.0.0a3/doc/howto/howto_user_annot.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/howto/howto_user_spect.md` & `vak-1.0.0a3/doc/howto/howto_user_spect.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/annotation-example.png` & `vak-1.0.0a3/doc/images/annotation-example.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/annotation_example_for_tutorial.png` & `vak-1.0.0a3/doc/images/annotation_example_for_tutorial.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/logo/vak-logo-primary.png` & `vak-1.0.0a3/doc/images/logo/vak-logo-primary.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/logo/vak-logo-secondary.png` & `vak-1.0.0a3/doc/images/logo/vak-logo-secondary.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/logo/vak-logomark.png` & `vak-1.0.0a3/doc/images/logo/vak-logomark.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/song_with_colored_segments.png` & `vak-1.0.0a3/doc/images/song_with_colored_segments.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/terminalizer/vak-help.gif` & `vak-1.0.0a3/doc/images/terminalizer/vak-help.gif`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/images/terminalizer/vak-help.yml` & `vak-1.0.0a3/doc/images/terminalizer/vak-help.yml`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/index.md` & `vak-1.0.0a3/doc/index.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 
 `vak` is a library that makes it easier
 for researchers studying animal
 vocalizations---such as birdsong, bat calls,
 and even human speech---to work with
 neural network algorithms.
 
+To learn more about the goals and design of vak, 
+please see this talk from the SciPy 2023 conference, 
+and the associated Proceedings paper 
+[here](https://conference.scipy.org/proceedings/scipy2023/pdfs/david_nicholson.pdf).
+
+```{iframe} https://www.youtube.com/embed/tpL0m5UwpZM?si=YSoCpS_Upa7h9hyw
+:width: 100%
+SciPy 2023 talk on vak
+```
+
 Currently, the main use is automated **annotation** of animal vocalizations.
 By **annotation**, we mean something like this example of annotated birdsong:
 
 ```{image} images/annotation_example_for_tutorial.png
 ```
 
 Please see links below for information on how to get started and how to use `vak` to
```

### Comparing `vak-1.0.0a2/doc/make.bat` & `vak-1.0.0a3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/poems/unknown-bird.rst` & `vak-1.0.0a3/doc/poems/unknown-bird.rst`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/poems/what-does-the-bird-care.rst` & `vak-1.0.0a3/doc/poems/what-does-the-bird-care.rst`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/reference/about.md` & `vak-1.0.0a3/doc/reference/about.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/reference/cli.md` & `vak-1.0.0a3/doc/reference/cli.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/reference/config.md` & `vak-1.0.0a3/doc/reference/config.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/reference/filenames.md` & `vak-1.0.0a3/doc/reference/filenames.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/reference/models.md` & `vak-1.0.0a3/doc/reference/models.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/reference/spect_file_format.md` & `vak-1.0.0a3/doc/reference/spect_file_format.md`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/sample_phrase_annotation.png` & `vak-1.0.0a3/doc/sample_phrase_annotation.png`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/toml/gy6or6_predict.toml` & `vak-1.0.0a3/doc/toml/gy6or6_predict.toml`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/doc/toml/gy6or6_train.toml` & `vak-1.0.0a3/doc/toml/gy6or6_train.toml`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/noxfile.py` & `vak-1.0.0a3/noxfile.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/pyproject.toml` & `vak-1.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vak"
 description = "a neural network toolbox for animal vocalizations and bioacoustics"
-version = "1.0.0a2"
+version = "1.0.0a3"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
 classifiers = [
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
```

### Comparing `vak-1.0.0a2/src/scripts/download_autoannotate_data.py` & `vak-1.0.0a3/src/scripts/download_autoannotate_data.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/__about__.py` & `vak-1.0.0a3/src/vak/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 __title__ = "vak"
 __summary__ = (
     "a neural network toolbox for animal vocalizations and bioacoustics"
 )
 __uri__ = "https://github.com/NickleDave/vak"
 
-__version__ = "1.0.0a2"
+__version__ = "1.0.0a3"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `vak-1.0.0a2/src/vak/__init__.py` & `vak-1.0.0a3/src/vak/__init__.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/__main__.py` & `vak-1.0.0a3/src/vak/__main__.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/cli/cli.py` & `vak-1.0.0a3/src/vak/cli/cli.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/cli/eval.py` & `vak-1.0.0a3/src/vak/cli/eval.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/cli/learncurve.py` & `vak-1.0.0a3/src/vak/cli/learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/cli/predict.py` & `vak-1.0.0a3/src/vak/cli/predict.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/cli/prep.py` & `vak-1.0.0a3/src/vak/cli/prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/cli/train.py` & `vak-1.0.0a3/src/vak/cli/train.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/__init__.py` & `vak-1.0.0a3/src/vak/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/annotation.py` & `vak-1.0.0a3/src/vak/common/annotation.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/constants.py` & `vak-1.0.0a3/src/vak/common/constants.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/converters.py` & `vak-1.0.0a3/src/vak/common/converters.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/files/files.py` & `vak-1.0.0a3/src/vak/common/files/files.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/files/spect.py` & `vak-1.0.0a3/src/vak/common/files/spect.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/labels.py` & `vak-1.0.0a3/src/vak/common/labels.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/logging.py` & `vak-1.0.0a3/src/vak/common/logging.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/paths.py` & `vak-1.0.0a3/src/vak/common/paths.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/tensorboard.py` & `vak-1.0.0a3/src/vak/common/tensorboard.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/timebins.py` & `vak-1.0.0a3/src/vak/common/timebins.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/trainer.py` & `vak-1.0.0a3/src/vak/common/trainer.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/common/validators.py` & `vak-1.0.0a3/src/vak/common/validators.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/config.py` & `vak-1.0.0a3/src/vak/config/config.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/eval.py` & `vak-1.0.0a3/src/vak/config/eval.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/learncurve.py` & `vak-1.0.0a3/src/vak/config/learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/model.py` & `vak-1.0.0a3/src/vak/config/model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/parse.py` & `vak-1.0.0a3/src/vak/config/parse.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/predict.py` & `vak-1.0.0a3/src/vak/config/predict.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/prep.py` & `vak-1.0.0a3/src/vak/config/prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/spect_params.py` & `vak-1.0.0a3/src/vak/config/spect_params.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/train.py` & `vak-1.0.0a3/src/vak/config/train.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/valid.toml` & `vak-1.0.0a3/src/vak/config/valid.toml`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/config/validators.py` & `vak-1.0.0a3/src/vak/config/validators.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/datasets/frame_classification/frames_dataset.py` & `vak-1.0.0a3/src/vak/datasets/frame_classification/frames_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/datasets/frame_classification/metadata.py` & `vak-1.0.0a3/src/vak/datasets/frame_classification/metadata.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/datasets/frame_classification/window_dataset.py` & `vak-1.0.0a3/src/vak/datasets/frame_classification/window_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/datasets/parametric_umap/metadata.py` & `vak-1.0.0a3/src/vak/datasets/parametric_umap/metadata.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/datasets/parametric_umap/parametric_umap.py` & `vak-1.0.0a3/src/vak/datasets/parametric_umap/parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/eval/eval_.py` & `vak-1.0.0a3/src/vak/eval/eval_.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/eval/frame_classification.py` & `vak-1.0.0a3/src/vak/eval/frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/eval/parametric_umap.py` & `vak-1.0.0a3/src/vak/eval/parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/learncurve/curvefit.py` & `vak-1.0.0a3/src/vak/learncurve/curvefit.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/learncurve/dirname.py` & `vak-1.0.0a3/src/vak/learncurve/dirname.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/learncurve/frame_classification.py` & `vak-1.0.0a3/src/vak/learncurve/frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/learncurve/learncurve.py` & `vak-1.0.0a3/src/vak/learncurve/learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/metrics/classification/functional.py` & `vak-1.0.0a3/src/vak/metrics/classification/functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/metrics/distance/distance.py` & `vak-1.0.0a3/src/vak/metrics/distance/distance.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/metrics/distance/functional.py` & `vak-1.0.0a3/src/vak/metrics/distance/functional.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import torch
 
 
 def levenshtein(source, target):
     """Levenshtein distance: number of deletions, insertions,
     or substitutions required to convert source string
     into target string.
 
@@ -61,15 +62,15 @@
                 if y_cost < cost:
                     cost = y_cost
 
             d1[j + 1] = cost
 
         d0, d1 = d1, d0
 
-    return d0[-1]
+    return torch.tensor(d0[-1], dtype=torch.int32)
 
 
 def segment_error_rate(y_pred, y_true):
     """Levenshtein edit distance normalized by length of true sequence.
     Also known as word error distance; here applied to other vocalizations
     in addition to speech.
 
@@ -91,8 +92,9 @@
     if len(y_true) == 0 and len(y_pred) == 0:
         return 0.0
     elif len(y_true) == 0 and len(y_pred) != 0:
         raise ValueError(
             "segment error rate is undefined when length of y_true is zero"
         )
 
-    return levenshtein(y_pred, y_true) / len(y_true)
+    rate = levenshtein(y_pred, y_true) / len(y_true)
+    return torch.tensor(rate, dtype=torch.float32)
```

### Comparing `vak-1.0.0a2/src/vak/metrics/util.py` & `vak-1.0.0a3/src/vak/metrics/util.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/__init__.py` & `vak-1.0.0a3/src/vak/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/base.py` & `vak-1.0.0a3/src/vak/models/base.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/convencoder_umap.py` & `vak-1.0.0a3/src/vak/models/convencoder_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/decorator.py` & `vak-1.0.0a3/src/vak/models/decorator.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/definition.py` & `vak-1.0.0a3/src/vak/models/definition.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/ed_tcn.py` & `vak-1.0.0a3/src/vak/models/ed_tcn.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/frame_classification_model.py` & `vak-1.0.0a3/src/vak/models/frame_classification_model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/get.py` & `vak-1.0.0a3/src/vak/models/get.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/parametric_umap_model.py` & `vak-1.0.0a3/src/vak/models/parametric_umap_model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/registry.py` & `vak-1.0.0a3/src/vak/models/registry.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/models/tweetynet.py` & `vak-1.0.0a3/src/vak/models/tweetynet.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nets/conv_encoder.py` & `vak-1.0.0a3/src/vak/nets/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nets/ed_tcn.py` & `vak-1.0.0a3/src/vak/nets/ed_tcn.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nets/tweetynet.py` & `vak-1.0.0a3/src/vak/nets/tweetynet.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nn/functional.py` & `vak-1.0.0a3/src/vak/nn/functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nn/loss/dice.py` & `vak-1.0.0a3/src/vak/nn/loss/dice.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nn/loss/umap.py` & `vak-1.0.0a3/src/vak/nn/loss/umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nn/modules/activation.py` & `vak-1.0.0a3/src/vak/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/nn/modules/conv.py` & `vak-1.0.0a3/src/vak/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/plot/annot.py` & `vak-1.0.0a3/src/vak/plot/annot.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/plot/learncurve.py` & `vak-1.0.0a3/src/vak/plot/learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/plot/spect.py` & `vak-1.0.0a3/src/vak/plot/spect.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/predict/frame_classification.py` & `vak-1.0.0a3/src/vak/predict/frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/predict/parametric_umap.py` & `vak-1.0.0a3/src/vak/predict/parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/predict/predict_.py` & `vak-1.0.0a3/src/vak/predict/predict_.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/audio_dataset.py` & `vak-1.0.0a3/src/vak/prep/audio_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/constants.py` & `vak-1.0.0a3/src/vak/prep/constants.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/dataset_df_helper.py` & `vak-1.0.0a3/src/vak/prep/dataset_df_helper.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/frame_classification/dataset_arrays.py` & `vak-1.0.0a3/src/vak/prep/frame_classification/dataset_arrays.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/frame_classification/frame_classification.py` & `vak-1.0.0a3/src/vak/prep/frame_classification/frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/frame_classification/learncurve.py` & `vak-1.0.0a3/src/vak/prep/frame_classification/learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/frame_classification/validators.py` & `vak-1.0.0a3/src/vak/prep/frame_classification/validators.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/parametric_umap/dataset_arrays.py` & `vak-1.0.0a3/src/vak/prep/parametric_umap/dataset_arrays.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/parametric_umap/parametric_umap.py` & `vak-1.0.0a3/src/vak/prep/parametric_umap/parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/prep_.py` & `vak-1.0.0a3/src/vak/prep/prep_.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/sequence_dataset.py` & `vak-1.0.0a3/src/vak/prep/sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/spectrogram_dataset/audio_helper.py` & `vak-1.0.0a3/src/vak/prep/spectrogram_dataset/audio_helper.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/spectrogram_dataset/prep.py` & `vak-1.0.0a3/src/vak/prep/spectrogram_dataset/prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/spectrogram_dataset/spect.py` & `vak-1.0.0a3/src/vak/prep/spectrogram_dataset/spect.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/spectrogram_dataset/spect_helper.py` & `vak-1.0.0a3/src/vak/prep/spectrogram_dataset/spect_helper.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/split/algorithms/bruteforce.py` & `vak-1.0.0a3/src/vak/prep/split/algorithms/bruteforce.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/split/algorithms/validate.py` & `vak-1.0.0a3/src/vak/prep/split/algorithms/validate.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/split/split.py` & `vak-1.0.0a3/src/vak/prep/split/split.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/prep/unit_dataset/unit_dataset.py` & `vak-1.0.0a3/src/vak/prep/unit_dataset/unit_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/train/frame_classification.py` & `vak-1.0.0a3/src/vak/train/frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/train/parametric_umap.py` & `vak-1.0.0a3/src/vak/train/parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/train/train_.py` & `vak-1.0.0a3/src/vak/train/train_.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/defaults/frame_classification.py` & `vak-1.0.0a3/src/vak/transforms/defaults/frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/defaults/get.py` & `vak-1.0.0a3/src/vak/transforms/defaults/get.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/defaults/parametric_umap.py` & `vak-1.0.0a3/src/vak/transforms/defaults/parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/frame_labels/functional.py` & `vak-1.0.0a3/src/vak/transforms/frame_labels/functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/frame_labels/transforms.py` & `vak-1.0.0a3/src/vak/transforms/frame_labels/transforms.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/functional.py` & `vak-1.0.0a3/src/vak/transforms/functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/src/vak/transforms/transforms.py` & `vak-1.0.0a3/src/vak/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/conftest.py` & `vak-1.0.0a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/annot.py` & `vak-1.0.0a3/tests/fixtures/annot.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/audio.py` & `vak-1.0.0a3/tests/fixtures/audio.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/config.py` & `vak-1.0.0a3/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/csv.py` & `vak-1.0.0a3/tests/fixtures/csv.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/das.py` & `vak-1.0.0a3/tests/fixtures/das.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/dataframe.py` & `vak-1.0.0a3/tests/fixtures/dataframe.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/dataset.py` & `vak-1.0.0a3/tests/fixtures/dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/model.py` & `vak-1.0.0a3/tests/fixtures/model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/path.py` & `vak-1.0.0a3/tests/fixtures/path.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/results.py` & `vak-1.0.0a3/tests/fixtures/results.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/spect.py` & `vak-1.0.0a3/tests/fixtures/spect.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/split.py` & `vak-1.0.0a3/tests/fixtures/split.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/test_data.py` & `vak-1.0.0a3/tests/fixtures/test_data.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/fixtures/torch.py` & `vak-1.0.0a3/tests/fixtures/torch.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/das-test-data-env.txt` & `vak-1.0.0a3/tests/scripts/das-test-data-env.txt`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/das-test-data-env.yml` & `vak-1.0.0a3/tests/scripts/das-test-data-env.yml`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/generate_das_test_data.py` & `vak-1.0.0a3/tests/scripts/generate_das_test_data.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/generate_data_for_tests.py` & `vak-1.0.0a3/tests/scripts/generate_data_for_tests.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/move_csv.py` & `vak-1.0.0a3/tests/scripts/move_csv.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/vaktestdata/configs.py` & `vak-1.0.0a3/tests/scripts/vaktestdata/configs.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/vaktestdata/constants.py` & `vak-1.0.0a3/tests/scripts/vaktestdata/constants.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/vaktestdata/dirs.py` & `vak-1.0.0a3/tests/scripts/vaktestdata/dirs.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/vaktestdata/parser.py` & `vak-1.0.0a3/tests/scripts/vaktestdata/parser.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/scripts/vaktestdata/prep.py` & `vak-1.0.0a3/tests/scripts/vaktestdata/prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test___main__.py` & `vak-1.0.0a3/tests/test___main__.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_cli/cli_asserts.py` & `vak-1.0.0a3/tests/test_cli/cli_asserts.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_cli/test_eval.py` & `vak-1.0.0a3/tests/test_cli/test_eval.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_cli/test_learncurve.py` & `vak-1.0.0a3/tests/test_cli/test_learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_cli/test_predict.py` & `vak-1.0.0a3/tests/test_cli/test_predict.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_cli/test_prep.py` & `vak-1.0.0a3/tests/test_cli/test_prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_cli/test_train.py` & `vak-1.0.0a3/tests/test_cli/test_train.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_annotation.py` & `vak-1.0.0a3/tests/test_common/test_annotation.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_console_script.py` & `vak-1.0.0a3/tests/test_common/test_console_script.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_converters.py` & `vak-1.0.0a3/tests/test_common/test_converters.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_files/test_files.py` & `vak-1.0.0a3/tests/test_common/test_files/test_files.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_files/test_spect.py` & `vak-1.0.0a3/tests/test_common/test_files/test_spect.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_labels.py` & `vak-1.0.0a3/tests/test_common/test_labels.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_paths.py` & `vak-1.0.0a3/tests/test_common/test_paths.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_common/test_timenow.py` & `vak-1.0.0a3/tests/test_common/test_timenow.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_config/attr_helpers.py` & `vak-1.0.0a3/tests/test_config/attr_helpers.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_config/test_config.py` & `vak-1.0.0a3/tests/test_config/test_config.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_config/test_model.py` & `vak-1.0.0a3/tests/test_config/test_model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_config/test_parse.py` & `vak-1.0.0a3/tests/test_config/test_parse.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_config/test_spect_params.py` & `vak-1.0.0a3/tests/test_config/test_spect_params.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_config/test_validators.py` & `vak-1.0.0a3/tests/test_config/test_validators.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_datasets/test_frame_classification/test_frames_dataset.py` & `vak-1.0.0a3/tests/test_datasets/test_frame_classification/test_frames_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_datasets/test_frame_classification/test_metadata.py` & `vak-1.0.0a3/tests/test_datasets/test_frame_classification/test_metadata.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_datasets/test_frame_classification/test_window_dataset.py` & `vak-1.0.0a3/tests/test_datasets/test_frame_classification/test_window_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_datasets/test_parametric_umap/test_parametric_umap.py` & `vak-1.0.0a3/tests/test_datasets/test_parametric_umap/test_parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_eval/test_eval.py` & `vak-1.0.0a3/tests/test_eval/test_eval.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_eval/test_frame_classification.py` & `vak-1.0.0a3/tests/test_eval/test_frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_eval/test_parametric_umap.py` & `vak-1.0.0a3/tests/test_eval/test_parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_learncurve/test_frame_classification.py` & `vak-1.0.0a3/tests/test_learncurve/test_frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_metrics/test_distance/test_functional.py` & `vak-1.0.0a3/tests/test_metrics/test_distance/test_functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/conftest.py` & `vak-1.0.0a3/tests/test_models/conftest.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_base.py` & `vak-1.0.0a3/tests/test_models/test_base.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_convencoder_umap.py` & `vak-1.0.0a3/tests/test_models/test_convencoder_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_decorator.py` & `vak-1.0.0a3/tests/test_models/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_definition.py` & `vak-1.0.0a3/tests/test_models/test_definition.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_ed_tcn.py` & `vak-1.0.0a3/tests/test_models/test_ed_tcn.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_frame_classification_model.py` & `vak-1.0.0a3/tests/test_models/test_frame_classification_model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_parametric_umap_model.py` & `vak-1.0.0a3/tests/test_models/test_parametric_umap_model.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_registry.py` & `vak-1.0.0a3/tests/test_models/test_registry.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_models/test_tweetynet.py` & `vak-1.0.0a3/tests/test_models/test_tweetynet.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_nets/test_convencoder.py` & `vak-1.0.0a3/tests/test_nets/test_convencoder.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_nets/test_ed_tcn.py` & `vak-1.0.0a3/tests/test_nets/test_ed_tcn.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_nets/test_tweetynet.py` & `vak-1.0.0a3/tests/test_nets/test_tweetynet.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_nn/test_functional.py` & `vak-1.0.0a3/tests/test_nn/test_functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_nn/test_loss/test_dice.py` & `vak-1.0.0a3/tests/test_nn/test_loss/test_dice.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_predict/test_frame_classification.py` & `vak-1.0.0a3/tests/test_predict/test_frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_predict/test_predict.py` & `vak-1.0.0a3/tests/test_predict/test_predict.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_audio_dataset.py` & `vak-1.0.0a3/tests/test_prep/test_audio_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_frame_classification/test_dataset_arrays.py` & `vak-1.0.0a3/tests/test_prep/test_frame_classification/test_dataset_arrays.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_frame_classification/test_frame_classification.py` & `vak-1.0.0a3/tests/test_prep/test_frame_classification/test_frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_frame_classification/test_learncurve.py` & `vak-1.0.0a3/tests/test_prep/test_frame_classification/test_learncurve.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_prep.py` & `vak-1.0.0a3/tests/test_prep/test_prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_sequence_dataset.py` & `vak-1.0.0a3/tests/test_prep/test_sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/test_audio_helper.py` & `vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/test_audio_helper.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/test_prep.py` & `vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/test_prep.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_spectrogram_dataset/test_spect_helper.py` & `vak-1.0.0a3/tests/test_prep/test_spectrogram_dataset/test_spect_helper.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_split/test_algorithms/test_bruteforce.py` & `vak-1.0.0a3/tests/test_prep/test_split/test_algorithms/test_bruteforce.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_split/test_algorithms/test_validate.py` & `vak-1.0.0a3/tests/test_prep/test_split/test_algorithms/test_validate.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_prep/test_split/test_split.py` & `vak-1.0.0a3/tests/test_prep/test_split/test_split.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_train/test_frame_classification.py` & `vak-1.0.0a3/tests/test_train/test_frame_classification.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_train/test_parametric_umap.py` & `vak-1.0.0a3/tests/test_train/test_parametric_umap.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_train/test_train.py` & `vak-1.0.0a3/tests/test_train/test_train.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_transforms/test_frame_labels/test_functional.py` & `vak-1.0.0a3/tests/test_transforms/test_frame_labels/test_functional.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_transforms/test_frame_labels/test_transforms.py` & `vak-1.0.0a3/tests/test_transforms/test_frame_labels/test_transforms.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/tests/test_transforms/test_transforms.py` & `vak-1.0.0a3/tests/test_transforms/test_transforms.py`

 * *Files identical despite different names*

### Comparing `vak-1.0.0a2/PKG-INFO` & `vak-1.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vak
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: a neural network toolbox for animal vocalizations and bioacoustics
 Author-email: David Nicholson <nickledave@users.noreply.github.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -59,22 +59,22 @@
 
 <hr>
 
 ## A neural network framework for animal acoustic communication and bioacoustics
 
 [![DOI](https://zenodo.org/badge/173566541.svg)](https://zenodo.org/badge/latestdoi/173566541)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-21-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-22-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 [![PyPI version](https://badge.fury.io/py/vak.svg)](https://badge.fury.io/py/vak)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Build Status](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/badge.svg)](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/badge.svg)
 [![codecov](https://codecov.io/gh/vocalpy/vak/branch/main/graph/badge.svg?token=9Y4XXB2ELA)](https://codecov.io/gh/vocalpy/vak)
 
-<h3>🚧 vak version 1.0.0 is in development! 🚧 📣 Test out the alpha release: <code>pip install vak==1.0.0a1</code>. 📣 For more info, please see <a href="https://forum.vocalpy.org/t/vak-1-0-0a1-released/55"> this forum post<a>.</h3>
+<h3>🚧 vak version 1.0.0 is in development! 🚧 📣 Test out the alpha release: <code>pip install vak==1.0.0a2</code>. 📣 For more info, please see <a href="https://forum.vocalpy.org/t/vak-1-0-0a1-released/55"> this forum post<a>.</h3>
 
 
 `vak` is a Python framework for neural network models, 
 designed for researchers studying animal acoustic communication and bioacoustics.
 Many people will be familiar with work in this area on 
 animal vocalizations such as birdsong, bat calls, and even human speech.
 Neural network models have provided a powerful new tool for researchers in this area, 
@@ -96,14 +96,25 @@
 You give `vak` training data in the form of audio or spectrogram files with annotations, 
 and then `vak` helps you train neural network models 
 and use the trained models to predict annotations for new files.
 
 We developed `vak` to benchmark a neural network model we call [`tweetynet`](https://github.com/yardencsGitHub/tweetynet).  
 Please see the eLife article here: https://elifesciences.org/articles/63853  
 
+To learn more about the goals and design of vak, 
+please see this talk from the SciPy 2023 conference, 
+and the associated Proceedings paper 
+[here](https://conference.scipy.org/proceedings/scipy2023/pdfs/david_nicholson.pdf).
+
+<p align="center">
+<a href="https://www.youtube.com/watch?v=tpL0m5UwpZM" target="_blank">
+ <img src="https://img.youtube.com/vi/tpL0m5UwpZM/mqdefault.jpg" alt="Thumbnail of SciPy 2023 talk on vak" width="400" border="10" />
+</a>
+</p>
+
 For more background on animal acoustic communication and deep learning, 
 and how these intersect with related fields like 
 computational ethology and neuroscience,
 please see the ["About"](#About) section below.
 
 ### Installation
 Short version:
@@ -162,15 +173,31 @@
 please use the issue tracker on GitHub:  
 <https://github.com/vocalpy/vak/issues>
 
 For a guide on how you can contribute to `vak`, please see:
 https://vak.readthedocs.io/en/latest/development/index.html
 
 ### Citation
-If you use vak for a publication, please cite its DOI:  
+If you use vak for a publication, please cite both the Proceedings paper and the software.
+
+#### Proceedings paper (BiBTex)
+
+```
+@inproceedings{nicholson2023vak,
+  title={vak: a neural network framework for researchers studying animal acoustic communication},
+  author={Nicholson, David and Cohen, Yarden},
+  booktitle={Python in Science Conference},
+  pages={59--67},
+  year={2023}
+}
+
+```
+
+#### Software
+
 [![DOI](https://zenodo.org/badge/173566541.svg)](https://zenodo.org/badge/latestdoi/173566541)
 
 ### License
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)  
 is [here](./LICENSE).
 
 ### About
@@ -244,14 +271,17 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lmpascual"><img src="https://avatars.githubusercontent.com/u/62260534?v=4?s=100" width="100px;" alt="lmpascual"/><br /><sub><b>lmpascual</b></sub></a><br /><a href="https://github.com/vocalpy/vak/commits?author=lmpascual" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ItamarFruchter"><img src="https://avatars.githubusercontent.com/u/19908942?v=4?s=100" width="100px;" alt="ItamarFruchter"/><br /><sub><b>ItamarFruchter</b></sub></a><br /><a href="https://github.com/vocalpy/vak/commits?author=ItamarFruchter" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kalleknast"><img src="https://avatars.githubusercontent.com/u/12412777?v=4?s=100" width="100px;" alt="Hjalmar K. Turesson"/><br /><sub><b>Hjalmar K. Turesson</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3Akalleknast" title="Bug reports">🐛</a> <a href="#ideas-kalleknast" title="Ideas, Planning, & Feedback">🤔</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/nhoglen"><img src="https://avatars.githubusercontent.com/u/13972140?v=4?s=100" width="100px;" alt="nhoglen"/><br /><sub><b>nhoglen</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3Anhoglen" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://test0.zip"><img src="https://avatars.githubusercontent.com/u/46551097?v=4?s=100" width="100px;" alt="Ja-sonYun"/><br /><sub><b>Ja-sonYun</b></sub></a><br /><a href="https://github.com/vocalpy/vak/commits?author=Ja-sonYun" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/JacquelineGoe"><img src="https://avatars.githubusercontent.com/u/52127436?v=4?s=100" width="100px;" alt="Jacqueline"/><br /><sub><b>Jacqueline</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3AJacquelineGoe" title="Bug reports">🐛</a></td>
     </tr>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="http://maths.manchester.ac.uk/~mrm/"><img src="https://avatars.githubusercontent.com/u/5350159?v=4?s=100" width="100px;" alt="Mark Muldoon"/><br /><sub><b>Mark Muldoon</b></sub></a><br /><a href="https://github.com/vocalpy/vak/issues?q=author%3AVenetianRed" title="Bug reports">🐛</a></td>
+    </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vak Version: 1.0.0a2 Summary: a neural network
+Metadata-Version: 2.1 Name: vak Version: 1.0.0a3 Summary: a neural network
 toolbox for animal vocalizations and bioacoustics Author-email: David Nicholson
 users.noreply.github.com> Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Classifier: License :: OSI Approved :: BSD License Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
@@ -29,24 +29,24 @@
 Provides-Extra: test
       [https://github.com/vocalpy/vak/blob/main/doc/images/logo/vak-logo-
                              primary.png?raw=True]
 ===============================================================================
 ## A neural network framework for animal acoustic communication and
 bioacoustics [![DOI](https://zenodo.org/badge/173566541.svg)](https://
 zenodo.org/badge/latestdoi/173566541) [![All Contributors](https://
-img.shields.io/badge/all_contributors-21-orange.svg?style=flat-square)]
+img.shields.io/badge/all_contributors-22-orange.svg?style=flat-square)]
 (#contributors-) [![PyPI version](https://badge.fury.io/py/vak.svg)](https://
 badge.fury.io/py/vak) [![License](https://img.shields.io/badge/License-BSD%203-
 -Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Build
 Status](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/
 badge.svg)](https://github.com/vocalpy/vak/actions/workflows/ci-linux.yml/
 badge.svg) [![codecov](https://codecov.io/gh/vocalpy/vak/branch/main/graph/
 badge.svg?token=9Y4XXB2ELA)](https://codecov.io/gh/vocalpy/vak)
 ******** ?ð???§ vvaakk vveerrssiioonn 11..00..00 iiss iinn ddeevveellooppmmeenntt!! ?ð???§ ?ð???£ TTeesstt oouutt tthhee aallpphhaa
-rreelleeaassee:: ppiipp iinnssttaallll vvaakk====11..00..00aa11.. ?ð???£ FFoorr mmoorree iinnffoo,, pplleeaassee sseeee _tt_hh_ii_ss_ _ff_oo_rr_uu_mm
+rreelleeaassee:: ppiipp iinnssttaallll vvaakk====11..00..00aa22.. ?ð???£ FFoorr mmoorree iinnffoo,, pplleeaassee sseeee _tt_hh_ii_ss_ _ff_oo_rr_uu_mm
 _pp_oo_ss_tt_.. ********
 `vak` is a Python framework for neural network models, designed for researchers
 studying animal acoustic communication and bioacoustics. Many people will be
 familiar with work in this area on animal vocalizations such as birdsong, bat
 calls, and even human speech. Neural network models have provided a powerful
 new tool for researchers in this area, as in many other fields. The library has
 two main goals: 1. Make it easier for researchers studying animal vocalizations
@@ -57,71 +57,81 @@
 the example of annotated birdsong shown below:
               [spectrogram of birdsong with syllables annotated]
 You give `vak` training data in the form of audio or spectrogram files with
 annotations, and then `vak` helps you train neural network models and use the
 trained models to predict annotations for new files. We developed `vak` to
 benchmark a neural network model we call [`tweetynet`](https://github.com/
 yardencsGitHub/tweetynet). Please see the eLife article here: https://
-elifesciences.org/articles/63853 For more background on animal acoustic
-communication and deep learning, and how these intersect with related fields
-like computational ethology and neuroscience, please see the ["About"](#About)
-section below. ### Installation Short version: #### with `pip` ```console $ pip
-install vak ``` #### with `conda` ```console $ conda install vak -c pytorch -
-c conda-forge $ # ^ notice additional channel! ``` Notice that for `conda` you
-specify two channels, and that the `pytorch` channel should come first, so it
-takes priority when installing the dependencies `pytorch` and `torchvision`.
-For more details, please see: https://vak.readthedocs.io/en/latest/get_started/
-installation.html We test `vak` on Ubuntu and MacOS. We have run on Windows and
-know of other users successfully running `vak` on that operating system, but
-installation on Windows may require some troubleshooting. A good place to start
-is by searching the [issues](https://github.com/vocalpy/vak/issues). ### Usage
-#### Tutorial Currently the easiest way to work with `vak` is through the
-command line. ![terminal showing vak help command output](https://github.com/
-vocalpy/vak/blob/main/doc/images/terminalizer/vak-help.gif?raw=True) You run it
-with configuration files, using one of a handful of commands. For more details,
+elifesciences.org/articles/63853 To learn more about the goals and design of
+vak, please see this talk from the SciPy 2023 conference, and the associated
+Proceedings paper [here](https://conference.scipy.org/proceedings/scipy2023/
+pdfs/david_nicholson.pdf).
+                     _[_T_h_u_m_b_n_a_i_l_ _o_f_ _S_c_i_P_y_ _2_0_2_3_ _t_a_l_k_ _o_n_ _v_a_k_]
+For more background on animal acoustic communication and deep learning, and how
+these intersect with related fields like computational ethology and
+neuroscience, please see the ["About"](#About) section below. ### Installation
+Short version: #### with `pip` ```console $ pip install vak ``` #### with
+`conda` ```console $ conda install vak -c pytorch -c conda-forge $ # ^ notice
+additional channel! ``` Notice that for `conda` you specify two channels, and
+that the `pytorch` channel should come first, so it takes priority when
+installing the dependencies `pytorch` and `torchvision`. For more details,
+please see: https://vak.readthedocs.io/en/latest/get_started/installation.html
+We test `vak` on Ubuntu and MacOS. We have run on Windows and know of other
+users successfully running `vak` on that operating system, but installation on
+Windows may require some troubleshooting. A good place to start is by searching
+the [issues](https://github.com/vocalpy/vak/issues). ### Usage #### Tutorial
+Currently the easiest way to work with `vak` is through the command line. !
+[terminal showing vak help command output](https://github.com/vocalpy/vak/blob/
+main/doc/images/terminalizer/vak-help.gif?raw=True) You run it with
+configuration files, using one of a handful of commands. For more details,
 please see the "autoannotate" tutorial here: https://vak.readthedocs.io/en/
 latest/get_started/autoannotate.html #### How can I use my data with `vak`?
 Please see the How-To Guides in the documentation here: https://
 vak.readthedocs.io/en/latest/howto/index.html ### Support / Contributing For
 help, please begin by checking out the Frequently Asked Questions: https://
 vak.readthedocs.io/en/latest/faq.html. To ask a question about vak, discuss its
 development, or share how you are using it, please start a new "Q&A" topic on
 the VocalPy forum with the vak tag:
 forum.vocalpy.org/> To report a bug, or to request a feature, please use the
 issue tracker on GitHub:
 github.com/vocalpy/vak/issues> For a guide on how you can contribute to `vak`,
 please see: https://vak.readthedocs.io/en/latest/development/index.html ###
-Citation If you use vak for a publication, please cite its DOI: [![DOI](https:/
-/zenodo.org/badge/173566541.svg)](https://zenodo.org/badge/latestdoi/173566541)
-### License [![License](https://img.shields.io/badge/License-BSD%203--Clause-
-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) is [here](./LICENSE).
-### About Are humans unique among animals? We speak languages, but is speech
-somehow like other animal behaviors, such as birdsong? Questions like these are
-answered by studying how animals communicate with sound. This research requires
-cutting edge computational methods and big team science across a wide range of
-disciplines, including ecology, ethology, bioacoustics, psychology,
-neuroscience, linguistics, and genomics [^1][^2][^3]. As in many other domains,
-this research is being revolutionized by deep learning algorithms [^1][^2][^3].
-Deep neural network models enable answering questions that were previously
-impossible to address, in part because these models automate analysis of very
-large datasets. Within the study of animal acoustic communication, multiple
-models have been proposed for similar tasks, often implemented as research code
-with different libraries, such as Keras and Pytorch. This situation has created
-a real need for a framework that allows researchers to easily benchmark models
-and apply trained models to their own data. To address this need, we developed
-vak. We originally developed vak to benchmark a neural network model, TweetyNet
-[^4][^5], that automates annotation of birdsong by segmenting spectrograms.
-TweetyNet and vak have been used in both neuroscience [^6][^7][^8] and
-bioacoustics [^9]. For additional background and papers that have used `vak`,
-please see: https://vak.readthedocs.io/en/latest/reference/about.html [^1]:
-https://www.frontiersin.org/articles/10.3389/fnbeh.2021.811737/full [^2]:
-https://peerj.com/articles/13152/ [^3]: https://www.jneurosci.org/content/42/
-45/8514 [^4]: https://elifesciences.org/articles/63853 [^5]: https://
-github.com/yardencsGitHub/tweetynet [^6]: https://www.nature.com/articles/
-s41586-020-2397-3 [^7]: https://elifesciences.org/articles/67855 [^8]: https://
+Citation If you use vak for a publication, please cite both the Proceedings
+paper and the software. #### Proceedings paper (BiBTex) ``` @inproceedings
+{nicholson2023vak, title={vak: a neural network framework for researchers
+studying animal acoustic communication}, author={Nicholson, David and Cohen,
+Yarden}, booktitle={Python in Science Conference}, pages={59--67}, year={2023}
+} ``` #### Software [![DOI](https://zenodo.org/badge/173566541.svg)](https://
+zenodo.org/badge/latestdoi/173566541) ### License [![License](https://
+img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/
+licenses/BSD-3-Clause) is [here](./LICENSE). ### About Are humans unique among
+animals? We speak languages, but is speech somehow like other animal behaviors,
+such as birdsong? Questions like these are answered by studying how animals
+communicate with sound. This research requires cutting edge computational
+methods and big team science across a wide range of disciplines, including
+ecology, ethology, bioacoustics, psychology, neuroscience, linguistics, and
+genomics [^1][^2][^3]. As in many other domains, this research is being
+revolutionized by deep learning algorithms [^1][^2][^3]. Deep neural network
+models enable answering questions that were previously impossible to address,
+in part because these models automate analysis of very large datasets. Within
+the study of animal acoustic communication, multiple models have been proposed
+for similar tasks, often implemented as research code with different libraries,
+such as Keras and Pytorch. This situation has created a real need for a
+framework that allows researchers to easily benchmark models and apply trained
+models to their own data. To address this need, we developed vak. We originally
+developed vak to benchmark a neural network model, TweetyNet [^4][^5], that
+automates annotation of birdsong by segmenting spectrograms. TweetyNet and vak
+have been used in both neuroscience [^6][^7][^8] and bioacoustics [^9]. For
+additional background and papers that have used `vak`, please see: https://
+vak.readthedocs.io/en/latest/reference/about.html [^1]: https://
+www.frontiersin.org/articles/10.3389/fnbeh.2021.811737/full [^2]: https://
+peerj.com/articles/13152/ [^3]: https://www.jneurosci.org/content/42/45/8514
+[^4]: https://elifesciences.org/articles/63853 [^5]: https://github.com/
+yardencsGitHub/tweetynet [^6]: https://www.nature.com/articles/s41586-020-2397-
+3 [^7]: https://elifesciences.org/articles/67855 [^8]: https://
 elifesciences.org/articles/75691 [^9]: https://journals.plos.org/plosone/
 article?id=10.1371/journal.pone.0278522 #### "Why this name, vak?" It has only
 three letters, so it is quick to type, and it wasn't taken on [pypi](https://
 pypi.org/) yet. Also I guess it has [something to do with speech](https://
 en.wikipedia.org/wiki/V%C4%81c). "vak" rhymes with "squawk" and "talk". ####
 Does your library have any poems? [Yes.](https://vak.readthedocs.io/en/latest/
 poems/index.html) ## Contributors â¨ Thanks goes to these wonderful people (
@@ -143,10 +153,13 @@
      _ð___        _ð___ _ð___      _ð___» _ð__¤_      _ð___ _ð___     _ð___ _ð___     _ð___     _ð___ _ð___
                                                                                        _ð__¤_
  _[_y_a_n_g_z_h_e_n_g_-    _[_l_m_p_a_s_c_u_a_l_]  _[_I_t_a_m_a_r_F_r_u_c_h_t_e_r_] _[_H_j_a_l_m_a_r_ _K_.    _[_n_h_o_g_l_e_n_]     _[_J_a_-   _[_J_a_c_q_u_e_l_i_n_e_]
      _1_2_1_]        _ll_mm_pp_aa_ss_cc_uu_aa_ll    _II_tt_aa_mm_aa_rr_FF_rr_uu_cc_hh_tt_ee_rr   _T_u_r_e_s_s_o_n_]      _nn_hh_oo_gg_ll_ee_nn    _s_o_n_Y_u_n_]   _JJ_aa_cc_qq_uu_ee_ll_ii_nn_ee
 _yy_aa_nn_gg_zz_hh_ee_nn_gg_--_11_22_11      _ð___            _ð___       _HH_jj_aa_ll_mm_aa_rr_ _KK_..        _ð___       _JJ_aa_--        _ð___
   _ð___ _ð__¤_                                    _TT_uu_rr_ee_ss_ss_oo_nn                   _ss_oo_nn_YY_uu_nn
                                                _ð___ _ð__¤_                   _ð___»
+_[_M_a_r_k_ _M_u_l_d_o_o_n_]
+ _MM_aa_rr_kk_ _MM_uu_ll_dd_oo_oo_nn
+     _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

