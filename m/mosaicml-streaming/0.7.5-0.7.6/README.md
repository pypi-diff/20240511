# Comparing `tmp/mosaicml-streaming-0.7.5.tar.gz` & `tmp/mosaicml-streaming-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-streaming-0.7.5.tar", last modified: Mon Apr  8 23:51:41 2024, max compression
+gzip compressed data, was "mosaicml-streaming-0.7.6.tar", last modified: Fri May 10 22:11:13 2024, max compression
```

## Comparing `mosaicml-streaming-0.7.5.tar` & `mosaicml-streaming-0.7.6.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.839965 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 23:51:41.000000 mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.839965 mosaicml-streaming-0.7.5/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.843965 mosaicml-streaming-0.7.5/simulation/core/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/last_used_ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/node_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/shard_downloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/shuffle_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_spanner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/sim_world.py
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/core/yaml_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.843965 mosaicml-streaming-0.7.5/simulation/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/interface_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/sim_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/sim_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/sim_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/interfaces/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/simulation/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.843965 mosaicml-streaming-0.7.5/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/batching/
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/per_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/batching/stratified.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/constant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/converters/dataframe_to_mds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    68222 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.847965 mosaicml-streaming-0.7.5/streaming/base/format/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/base/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/base/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    23447 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/base/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/json/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/json/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/mds/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/mds/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/format/xsv/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/format/xsv/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/partition/
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/partition/orig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/partition/relaxed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.851965 mosaicml-streaming-0.7.5/streaming/base/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shared/scalar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/base/shuffle/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1b.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1br.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py1s.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/shuffle/py2s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/spanner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/base/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    45219 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/storage/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/base/world.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/extract_webvid_videos.py
--rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/multimodal/webvid.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.855965 mosaicml-streaming-0.7.5/streaming/text/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/merge_shard_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/count_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/enwiki_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/convert/pile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/enwiki.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/text/pile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.859965 mosaicml-streaming-0.7.5/streaming/vision/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.863965 mosaicml-streaming-0.7.5/streaming/vision/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/coco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/fake_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/convert/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/streaming/vision/imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 23:51:41.867965 mosaicml-streaming-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_eviction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_laziness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_spanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    39855 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_streaming_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_unsafe_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26288 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    12359 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-04-08 23:51:21.000000 mosaicml-streaming-0.7.5/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.744713 mosaicml-streaming-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16221 2024-05-10 22:11:13.744713 mosaicml-streaming-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.720713 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16221 2024-05-10 22:11:13.000000 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-05-10 22:11:13.000000 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:11:13.000000 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 22:11:13.000000 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-10 22:11:13.000000 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-10 22:11:13.000000 mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16016 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:11:13.744713 mosaicml-streaming-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.720713 mosaicml-streaming-0.7.6/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.720713 mosaicml-streaming-0.7.6/simulation/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/last_used_ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/node_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/shard_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/shuffle_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/sim_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/sim_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/sim_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/sim_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/core/yaml_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.720713 mosaicml-streaming-0.7.6/simulation/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/interfaces/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/interfaces/sim_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/interfaces/sim_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21816 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/interfaces/sim_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23561 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/interfaces/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/simulation/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.724713 mosaicml-streaming-0.7.6/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.724713 mosaicml-streaming-0.7.6/streaming/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.724713 mosaicml-streaming-0.7.6/streaming/base/batching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/batching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/batching/device_per_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/batching/per_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/batching/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/batching/stratified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/constant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.724713 mosaicml-streaming-0.7.6/streaming/base/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/converters/dataframe_to_mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68309 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.728713 mosaicml-streaming-0.7.6/streaming/base/format/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.728713 mosaicml-streaming-0.7.6/streaming/base/format/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23447 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/base/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.728713 mosaicml-streaming-0.7.6/streaming/base/format/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/json/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/json/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/json/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.728713 mosaicml-streaming-0.7.6/streaming/base/format/mds/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/mds/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/mds/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/mds/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.728713 mosaicml-streaming-0.7.6/streaming/base/format/xsv/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/xsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/xsv/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10411 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/xsv/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/format/xsv/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.728713 mosaicml-streaming-0.7.6/streaming/base/partition/
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/partition/orig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/partition/relaxed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/base/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shared/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shared/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shared/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shared/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shared/scalar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/base/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/py1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/py1br.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/py1e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/py1s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/shuffle/py2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/spanner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/base/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20817 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51190 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/storage/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/base/world.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/multimodal/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/multimodal/convert/laion/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/laion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/multimodal/convert/laion/laion400m/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/laion/laion400m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.732713 mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/crawl_webvid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/extract_webvid_videos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/multimodal/webvid.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.736713 mosaicml-streaming-0.7.6/streaming/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.736713 mosaicml-streaming-0.7.6/streaming/text/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.736713 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.736713 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/merge_shard_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.736713 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/count_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/enwiki_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/convert/pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/enwiki.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/text/pile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.740713 mosaicml-streaming-0.7.6/streaming/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.740713 mosaicml-streaming-0.7.6/streaming/vision/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/coco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/fake_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/convert/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/streaming/vision/imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:11:13.744713 mosaicml-streaming-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9258 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_eviction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_laziness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12813 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_spanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43360 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_streaming_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_unsafe_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28011 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-05-10 22:11:04.000000 mosaicml-streaming-0.7.6/tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.7.5/LICENSE` & `mosaicml-streaming-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/PKG-INFO` & `mosaicml-streaming-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.7.5
+Version: 0.7.6
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: simulator
 Provides-Extra: spark
 Provides-Extra: databricks
+Provides-Extra: alipan
 Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/streaming#gh-light-mode-only" class="only-light">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.5 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.6 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.9 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
 Extra: simulator Provides-Extra: spark Provides-Extra: databricks Provides-
-Extra: testing Provides-Extra: all License-File: LICENSE
+Extra: alipan Provides-Extra: testing Provides-Extra: all License-File: LICENSE
 _[_h_t_t_p_s_:_/_/_s_t_o_r_a_g_e_._g_o_o_g_l_e_a_p_i_s_._c_o_m_/_d_o_c_s_._m_o_s_a_i_c_m_l_._c_o_m_/_i_m_a_g_e_s_/_s_t_r_e_a_m_i_n_g_-_l_o_g_o_-_l_i_g_h_t_-
                                    _m_o_d_e_._p_n_g_]
 ********** FFaasstt,, aaccccuurraattee ssttrreeaammiinngg ooff ttrraaiinniinngg ddaattaa ffrroomm cclloouudd ssttoorraaggee **********
 ****** _[[_WW_ee_bb_ss_ii_tt_ee_]] -- _[[_GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd_]] -- _[[_DD_oo_cc_ss_]]_ _--_ _[[_WW_ee_''_rr_ee_ _HH_ii_rr_ii_nn_gg_!!_]] ******
 _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_U_n_i_t_ _t_e_s_t_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
                             _[_C_h_a_t_ _@_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
```

### Comparing `mosaicml-streaming-0.7.5/README.md` & `mosaicml-streaming-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/PKG-INFO` & `mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.7.5
+Version: 0.7.6
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: simulator
 Provides-Extra: spark
 Provides-Extra: databricks
+Provides-Extra: alipan
 Provides-Extra: testing
 Provides-Extra: all
 License-File: LICENSE
 
 <br />
 <p align="center">
     <a href="https://github.com/mosaicml/streaming#gh-light-mode-only" class="only-light">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.5 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.7.6 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.9 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
 Extra: simulator Provides-Extra: spark Provides-Extra: databricks Provides-
-Extra: testing Provides-Extra: all License-File: LICENSE
+Extra: alipan Provides-Extra: testing Provides-Extra: all License-File: LICENSE
 _[_h_t_t_p_s_:_/_/_s_t_o_r_a_g_e_._g_o_o_g_l_e_a_p_i_s_._c_o_m_/_d_o_c_s_._m_o_s_a_i_c_m_l_._c_o_m_/_i_m_a_g_e_s_/_s_t_r_e_a_m_i_n_g_-_l_o_g_o_-_l_i_g_h_t_-
                                    _m_o_d_e_._p_n_g_]
 ********** FFaasstt,, aaccccuurraattee ssttrreeaammiinngg ooff ttrraaiinniinngg ddaattaa ffrroomm cclloouudd ssttoorraaggee **********
 ****** _[[_WW_ee_bb_ss_ii_tt_ee_]] -- _[[_GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd_]] -- _[[_DD_oo_cc_ss_]]_ _--_ _[[_WW_ee_''_rr_ee_ _HH_ii_rr_ii_nn_gg_!!_]] ******
 _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_U_n_i_t_ _t_e_s_t_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
                             _[_C_h_a_t_ _@_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
```

### Comparing `mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/SOURCES.txt` & `mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 streaming/base/local.py
 streaming/base/sampling.py
 streaming/base/spanner.py
 streaming/base/stream.py
 streaming/base/util.py
 streaming/base/world.py
 streaming/base/batching/__init__.py
+streaming/base/batching/device_per_stream.py
 streaming/base/batching/per_stream.py
 streaming/base/batching/random.py
 streaming/base/batching/stratified.py
 streaming/base/converters/__init__.py
 streaming/base/converters/dataframe_to_mds.py
 streaming/base/format/__init__.py
 streaming/base/format/index.py
```

### Comparing `mosaicml-streaming-0.7.5/mosaicml_streaming.egg-info/requires.txt` & `mosaicml-streaming-0.7.6/mosaicml_streaming.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,45 @@
 xxhash<4,>=3.0.0
 zstd<2,>=1.5.2.5
 oci<3,>=2.88
 azure-storage-blob<13,>=12.0.0
 azure-storage-file-datalake<13,>=12.11.0
 azure-identity>=1.13.0
 
+[alipan]
+AliPCS-Py<1,>=0.8
+
 [all]
+AliPCS-Py<1,>=0.8
 GitPython==3.1.42
 PyYAML<7,>=6.0
 altair<6,>=5.1.1
-databricks-sdk==0.23.0
+databricks-sdk==0.27.0
 datasets<3,>=2.4.0
 docformatter>=1.4
 docutils==0.17.1
-fastapi==0.110.0
+fastapi==0.110.2
 furo==2022.9.29
 humanize<5,>=4.7.0
 jupyter==1.0.0
 mosaicml-cli<0.7,>=0.5.25
 moto<6,>=4.0
 myst-parser==0.16.1
 nbsphinx==0.9.1
 omegaconf<3,>=2.3.0
 pandas<3,>=2.0.3
 pandoc==2.3
 pre-commit<4,>=2.18.1
 pyarrow>14.0.0
-pydantic==2.6.4
+pydantic==2.7.1
 pypandoc==1.13
 pyspark<4,>=3
 pytest-cov<6,>=4
 pytest-split==0.8.2
-pytest==8.1.1
+pytest==8.2.0
 pytest_codeblocks==0.17.0
 sortedcollections<3,>=2.1.0
 sphinx-argparse==0.4.0
 sphinx-copybutton==0.5.2
 sphinx-tabs==3.4.5
 sphinx==4.4.0
 sphinxcontrib-applehelp==1.0.0
@@ -57,30 +61,30 @@
 streamlit<2,>=1.26.0
 toml==0.10.2
 uvicorn==0.29.0
 wandb<1,>=0.15.5
 yamllint==1.35.1
 
 [databricks]
-databricks-sdk==0.23.0
+databricks-sdk==0.27.0
 
 [dev]
 datasets<3,>=2.4.0
 pyarrow>14.0.0
 docformatter>=1.4
 jupyter==1.0.0
 pre-commit<4,>=2.18.1
-pytest==8.1.1
+pytest==8.2.0
 pytest_codeblocks==0.17.0
 pytest-cov<6,>=4
 toml==0.10.2
 yamllint==1.35.1
 moto<6,>=4.0
-fastapi==0.110.0
-pydantic==2.6.4
+fastapi==0.110.2
+pydantic==2.7.1
 uvicorn==0.29.0
 pytest-split==0.8.2
 
 [docs]
 GitPython==3.1.42
 docutils==0.17.1
 furo==2022.9.29
```

### Comparing `mosaicml-streaming-0.7.5/pyproject.toml` & `mosaicml-streaming-0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/setup.py` & `mosaicml-streaming-0.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,22 +64,22 @@
 
 extra_deps['dev'] = [
     'datasets>=2.4.0,<3',
     'pyarrow>14.0.0',
     'docformatter>=1.4',
     'jupyter==1.0.0',
     'pre-commit>=2.18.1,<4',
-    'pytest==8.1.1',
+    'pytest==8.2.0',
     'pytest_codeblocks==0.17.0',
     'pytest-cov>=4,<6',
     'toml==0.10.2',
     'yamllint==1.35.1',
     'moto>=4.0,<6',
-    'fastapi==0.110.0',
-    'pydantic==2.6.4',
+    'fastapi==0.110.2',
+    'pydantic==2.7.1',
     'uvicorn==0.29.0',
     'pytest-split==0.8.2',
 ]
 
 extra_deps['docs'] = [
     'GitPython==3.1.42',
     'docutils==0.17.1',
@@ -112,15 +112,19 @@
 ]
 
 extra_deps['spark'] = [
     'pyspark>=3,<4',
 ]
 
 extra_deps['databricks'] = [
-    'databricks-sdk==0.23.0',
+    'databricks-sdk==0.27.0',
+]
+
+extra_deps['alipan'] = [
+    'AliPCS-Py>=0.8,<1',
 ]
 
 extra_deps['testing'] = [
     'mosaicml-cli>=0.5.25,<0.7',
 ]
 
 extra_deps['all'] = sorted({dep for deps in extra_deps.values() for dep in deps})
```

### Comparing `mosaicml-streaming-0.7.5/simulation/core/create_index.py` & `mosaicml-streaming-0.7.6/simulation/core/create_index.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/last_used_ordered_set.py` & `mosaicml-streaming-0.7.6/simulation/core/last_used_ordered_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/main.py` & `mosaicml-streaming-0.7.6/simulation/core/main.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/node_tracker.py` & `mosaicml-streaming-0.7.6/simulation/core/node_tracker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/shard_downloads.py` & `mosaicml-streaming-0.7.6/simulation/core/shard_downloads.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/shuffle_quality.py` & `mosaicml-streaming-0.7.6/simulation/core/shuffle_quality.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/sim_dataset.py` & `mosaicml-streaming-0.7.6/simulation/core/sim_dataset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/sim_spanner.py` & `mosaicml-streaming-0.7.6/simulation/core/sim_spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/sim_time.py` & `mosaicml-streaming-0.7.6/simulation/core/sim_time.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/sim_world.py` & `mosaicml-streaming-0.7.6/simulation/core/sim_world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/utils.py` & `mosaicml-streaming-0.7.6/simulation/core/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/core/yaml_processing.py` & `mosaicml-streaming-0.7.6/simulation/core/yaml_processing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/interfaces/interface_utils.py` & `mosaicml-streaming-0.7.6/simulation/interfaces/interface_utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/interfaces/sim_cli.py` & `mosaicml-streaming-0.7.6/simulation/interfaces/sim_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/interfaces/sim_script.py` & `mosaicml-streaming-0.7.6/simulation/interfaces/sim_script.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/interfaces/sim_ui.py` & `mosaicml-streaming-0.7.6/simulation/interfaces/sim_ui.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/simulation/interfaces/widgets.py` & `mosaicml-streaming-0.7.6/simulation/interfaces/widgets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/__init__.py` & `mosaicml-streaming-0.7.6/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/array.py` & `mosaicml-streaming-0.7.6/streaming/base/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/batching/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/batching/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 from numpy.typing import NDArray
 
+from streaming.base.batching.device_per_stream import generate_work_device_per_stream_batching
 from streaming.base.batching.per_stream import generate_work_per_stream_batching
 from streaming.base.batching.random import generate_work_random_batching
 from streaming.base.batching.stratified import generate_work_stratified_batching
 from streaming.base.world import World
 
 if TYPE_CHECKING:
     from streaming.base.dataset import StreamingDataset
 
 batching_methods = {
     'random': generate_work_random_batching,
     'stratified': generate_work_stratified_batching,
     'per_stream': generate_work_per_stream_batching,
+    'device_per_stream': generate_work_device_per_stream_batching,
 }
 
 
 def generate_work(batching_method: str, dataset: StreamingDataset, world: World, epoch: int,
                   sample_in_epoch: int) -> NDArray[np.int64]:
     """Apportion shards/samples to nodes/ranks/workers for elastically deterministic sample order.
```

### Comparing `mosaicml-streaming-0.7.5/streaming/base/batching/per_stream.py` & `mosaicml-streaming-0.7.6/streaming/base/batching/per_stream.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/batching/random.py` & `mosaicml-streaming-0.7.6/streaming/base/batching/random.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/batching/stratified.py` & `mosaicml-streaming-0.7.6/streaming/base/batching/stratified.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/compression.py` & `mosaicml-streaming-0.7.6/streaming/base/compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/constant.py` & `mosaicml-streaming-0.7.6/streaming/base/constant.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/converters/dataframe_to_mds.py` & `mosaicml-streaming-0.7.6/streaming/base/converters/dataframe_to_mds.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,111 +15,148 @@
 from streaming.base.util import merge_index as do_merge_index
 
 try:
     from pyspark import TaskContext
     from pyspark.sql.dataframe import DataFrame
     from pyspark.sql.types import (ArrayType, BinaryType, BooleanType, ByteType, DateType,
                                    DayTimeIntervalType, DecimalType, DoubleType, FloatType,
-                                   IntegerType, LongType, MapType, ShortType, StringType,
+                                   IntegerType, LongType, NullType, ShortType, StringType,
                                    StructField, StructType, TimestampNTZType, TimestampType)
 except ImportError as e:
     e.msg = get_import_exception_message(e.name, extra_deps='spark')  # pyright: ignore
     raise e
 
 from streaming import MDSWriter
 from streaming.base.format.index import get_index_basename
 from streaming.base.format.mds.encodings import _encodings
 from streaming.base.storage.upload import CloudUploader
 
 logger = logging.getLogger(__name__)
 
-MAPPING_SPARK_TO_MDS = {
-    ByteType: 'uint8',
-    ShortType: 'uint16',
-    IntegerType: 'int',
-    LongType: 'int64',
-    FloatType: 'float32',
-    DoubleType: 'float64',
-    DecimalType: 'str_decimal',
-    StringType: 'str',
-    BinaryType: 'bytes',
-    BooleanType: None,
-    TimestampType: None,
-    TimestampNTZType: None,
-    DateType: None,
-    DayTimeIntervalType: None,
-    ArrayType: None,
-    MapType: None,
-    StructType: None,
-    StructField: None
+SPARK_TO_MDS = {
+    ByteType(): 'uint8',
+    ShortType(): 'uint16',
+    IntegerType(): 'int32',
+    LongType(): 'int64',
+    FloatType(): 'float32',
+    DoubleType(): 'float64',
+    DecimalType(): 'str_decimal',
+    StringType(): 'str',
+    BinaryType(): 'bytes',
+    BooleanType(): None,
+    TimestampType(): None,
+    TimestampNTZType(): None,
+    DateType(): None,
+    DayTimeIntervalType(): None,
+    ArrayType(IntegerType()): 'ndarray:int32',
+    ArrayType(ShortType()): 'ndarray:int16',
+    ArrayType(LongType()): 'ndarray:int64',
+    ArrayType(FloatType()): 'ndarray:float32',
+    ArrayType(DoubleType()): 'ndarray:float64',
 }
 
 
+def is_json_compatible(data_type: Any):
+    """Recursively check if a given PySpark DataType is JSON compatible.
+
+    JSON = Union[Dict[str, 'JSON'], List['JSON'], str, float, int, bool, None]
+
+    Args:
+        data_type (Any): A pyspark schema for a column of the input spark dataframe.
+
+    Returns:
+        (bool): True if data_type is JSON compatible.
+    """
+    if isinstance(data_type, StructType):
+        return all(is_json_compatible(field.dataType) for field in data_type.fields)
+    elif isinstance(data_type, ArrayType):
+        return is_json_compatible(data_type.elementType)
+    elif isinstance(data_type, (StringType, IntegerType, FloatType, BooleanType, NullType)):
+        return True
+    else:
+        return False
+
+
 def infer_dataframe_schema(dataframe: DataFrame,
                            user_defined_cols: Optional[Dict[str, Any]] = None) -> Optional[Dict]:
-    """Retrieve schema to construct a dictionary or do sanity check for MDSWriter.
+    """Retrieve schema to construct a dictionary or do sanity check for dataframe_to_mds.
 
     Args:
         dataframe (spark dataframe): dataframe to inspect schema
-        user_defined_cols (Optional[Dict[str, Any]]): user specified schema for MDSWriter
+        user_defined_cols (Optional[Dict[str, Any]]): user specified schema for dataframe_to_mds
 
     Returns:
         If user_defined_cols is None, return schema_dict (dict): column name and dtypes that are
         supported by MDSWriter, else None
 
     Raises:
-        ValueError if any of the datatypes are unsupported by MDSWriter.
+        ValueError if any of the datatypes are unsupported by dataframe_to_mds.
     """
 
     def map_spark_dtype(spark_data_type: Any) -> str:
         """Map spark data type to mds supported types.
 
         Args:
             spark_data_type: https://spark.apache.org/docs/latest/sql-ref-datatypes.html
 
         Returns:
             str: corresponding mds datatype for input.
 
         Raises:
             raise ValueError if no mds datatype is found for input type
         """
-        mds_type = MAPPING_SPARK_TO_MDS.get(type(spark_data_type), None)
+        if issubclass(type(spark_data_type), DecimalType):
+            mds_type = SPARK_TO_MDS.get(DecimalType(), None)
+        else:
+            mds_type = SPARK_TO_MDS.get(spark_data_type, None)
+
         if mds_type is None:
-            raise ValueError(f'{spark_data_type} is not supported by MDSWriter')
+            raise ValueError(f'{spark_data_type} is not supported by dataframe_to_mds')
         return mds_type
 
     # user has provided schema, we just check if mds supports the dtype
     if user_defined_cols is not None:
-        mds_supported_dtypes = {
-            mds_type for mds_type in MAPPING_SPARK_TO_MDS.values() if mds_type is not None
-        }
+        mds_supported_dtypes = set(filter(bool, SPARK_TO_MDS.values()))
+
         for col_name, user_dtype in user_defined_cols.items():
             if col_name not in dataframe.columns:
                 raise ValueError(
                     f'{col_name} is not a column of input dataframe: {dataframe.columns}')
-            if user_dtype not in mds_supported_dtypes:
-                raise ValueError(f'{user_dtype} is not supported by MDSWriter')
+
+            if user_dtype.startswith('ndarray:'):
+                parts = user_dtype.split(':')
+                if len(parts) == 3:
+                    user_dtype = ':'.join(parts[:-1])
 
             actual_spark_dtype = dataframe.schema[col_name].dataType
+
+            if user_dtype not in mds_supported_dtypes:
+                if user_dtype == 'json':
+                    if is_json_compatible(actual_spark_dtype):
+                        continue
+                    else:
+                        raise ValueError(f'{col_name} can not be encoded by MDS JSON.')
+                raise ValueError(f'{user_dtype} is not supported by dataframe_to_mds')
+
             mapped_mds_dtype = map_spark_dtype(actual_spark_dtype)
             if user_dtype != mapped_mds_dtype:
                 raise ValueError(
                     f'Mismatched types: column name `{col_name}` is `{mapped_mds_dtype}` in ' +
                     f'DataFrame but `{user_dtype}` in user_defined_cols')
         return None
 
     schema = dataframe.schema
     schema_dict = {}
 
     for field in schema:
         dtype = map_spark_dtype(field.dataType)
-        if dtype in _encodings:
+        if dtype.split(':')[0] in _encodings:
             schema_dict[field.name] = dtype
         else:
-            raise ValueError(f'{dtype} is not supported by MDSWriter')
+            raise ValueError(f'{dtype} is not supported by dataframe_to_mds')
     return schema_dict
 
 
 def dataframeToMDS(dataframe: DataFrame,
                    merge_index: bool = True,
                    mds_kwargs: Optional[Dict[str, Any]] = None,
                    udf_iterable: Optional[Callable] = None,
```

### Comparing `mosaicml-streaming-0.7.5/streaming/base/dataloader.py` & `mosaicml-streaming-0.7.6/streaming/base/dataloader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/dataset.py` & `mosaicml-streaming-0.7.6/streaming/base/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,16 +293,16 @@
             ``False``.
         shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1e``.
         shuffle_seed (int): Seed for deterministic data shuffling. Defaults to ``9176``.
         shuffle_block_size (int, optional): Unit of shuffle. A canonical node's samples are split
             into blocks of this size, and samples within each block are shuffled. If ``None``, its
             value is calculated as ``max(4_000_000 // num_canonical_nodes), 1 << 18)``. Defaults to
             ``None``.
-        batching_method (str): Which batching method to use, either ``random``, ``stratified``, or
-            ``per_stream``. Defaults to ``random``.
+        batching_method (str): Which batching method to use, either ``random``, ``stratified``,
+            ``per_stream``, or ``device_per_stream``. Defaults to ``random``.
         allow_unsafe_types (bool): If a shard contains Pickle, which allows arbitrary code
             execution during deserialization, whether to keep going if ``True`` or raise an error
             if ``False``. Defaults to ``False``.
         replication (int, optional): Determines how many consecutive devices will receive the same
             samples. Useful for training with tensor or sequence parallelism, where multiple
             devices need to see the same partition of the dataset. Defaults to ``None``.
     """
@@ -384,19 +384,19 @@
             )
 
         # Check sampling granularity.
         if self.sampling_granularity <= 0:
             raise ValueError(f'`sampling_granularity` must be a positive integer, but got: ' +
                              f'{self.sampling_granularity}.')
 
-        # Check batching method is one of "random", "stratified", or "per_stream".
-        if self.batching_method not in ['random', 'stratified', 'per_stream']:
+        # Check batching method is one of "random", "stratified", "per_stream", or "device_per_stream".
+        if self.batching_method not in ['random', 'stratified', 'per_stream', 'device_per_stream']:
             raise ValueError(
                 f'Invalid batching method: {batching_method}. ' + \
-                f'Must be one of `random`, `stratified`, or `per_stream.'
+                f'Must be one of `random`, `stratified`, `per_stream`, or `device_per_stream`.'
             )
 
         # issue deprecation warning for py1b shuffle algorithm.
         if self.shuffle_algo == 'py1b':
             warnings.warn('The \'py1b\' shuffle algorithm will soon be deprecated. \
                 Please use the more performant \'py1br\' algorithm instead.',
                           DeprecationWarning,
```

### Comparing `mosaicml-streaming-0.7.5/streaming/base/distributed.py` & `mosaicml-streaming-0.7.6/streaming/base/distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/base/reader.py` & `mosaicml-streaming-0.7.6/streaming/base/format/base/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/base/writer.py` & `mosaicml-streaming-0.7.6/streaming/base/format/base/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/json/encodings.py` & `mosaicml-streaming-0.7.6/streaming/base/format/json/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/json/reader.py` & `mosaicml-streaming-0.7.6/streaming/base/format/json/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/json/writer.py` & `mosaicml-streaming-0.7.6/streaming/base/format/json/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/mds/encodings.py` & `mosaicml-streaming-0.7.6/streaming/base/format/mds/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/mds/reader.py` & `mosaicml-streaming-0.7.6/streaming/base/format/mds/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/mds/writer.py` & `mosaicml-streaming-0.7.6/streaming/base/format/mds/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/xsv/encodings.py` & `mosaicml-streaming-0.7.6/streaming/base/format/xsv/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/xsv/reader.py` & `mosaicml-streaming-0.7.6/streaming/base/format/xsv/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/format/xsv/writer.py` & `mosaicml-streaming-0.7.6/streaming/base/format/xsv/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/hashing.py` & `mosaicml-streaming-0.7.6/streaming/base/hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/local.py` & `mosaicml-streaming-0.7.6/streaming/base/local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/partition/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/partition/orig.py` & `mosaicml-streaming-0.7.6/streaming/base/partition/orig.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/partition/relaxed.py` & `mosaicml-streaming-0.7.6/streaming/base/partition/relaxed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/sampling.py` & `mosaicml-streaming-0.7.6/streaming/base/sampling.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shared/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shared/array.py` & `mosaicml-streaming-0.7.6/streaming/base/shared/array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shared/barrier.py` & `mosaicml-streaming-0.7.6/streaming/base/shared/barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shared/memory.py` & `mosaicml-streaming-0.7.6/streaming/base/shared/memory.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shared/prefix.py` & `mosaicml-streaming-0.7.6/streaming/base/shared/prefix.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shared/scalar.py` & `mosaicml-streaming-0.7.6/streaming/base/shared/scalar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/naive.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/naive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1b.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/py1b.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1br.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/py1br.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1e.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/py1e.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/py1s.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/py1s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/shuffle/py2s.py` & `mosaicml-streaming-0.7.6/streaming/base/shuffle/py2s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/spanner.py` & `mosaicml-streaming-0.7.6/streaming/base/spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/storage/__init__.py` & `mosaicml-streaming-0.7.6/streaming/base/storage/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2022-2024 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 """Base module for downloading/uploading files from/to cloud storage."""
 
-from streaming.base.storage.download import (download_file, download_from_azure,
-                                             download_from_azure_datalake,
+from streaming.base.storage.download import (download_file, download_from_alipan,
+                                             download_from_azure, download_from_azure_datalake,
                                              download_from_databricks_unity_catalog,
                                              download_from_dbfs, download_from_gcs,
                                              download_from_local, download_from_oci,
                                              download_from_s3, download_from_sftp)
 from streaming.base.storage.upload import (AzureDataLakeUploader, AzureUploader, CloudUploader,
                                            GCSUploader, LocalUploader, OCIUploader, S3Uploader)
 
@@ -25,9 +25,10 @@
     'download_from_sftp',
     'download_from_gcs',
     'download_from_oci',
     'download_from_azure',
     'download_from_azure_datalake',
     'download_from_databricks_unity_catalog',
     'download_from_dbfs',
+    'download_from_alipan',
     'download_from_local',
 ]
```

### Comparing `mosaicml-streaming-0.7.5/streaming/base/storage/download.py` & `mosaicml-streaming-0.7.6/streaming/base/storage/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'download_from_sftp',
     'download_from_gcs',
     'download_from_oci',
     'download_from_azure',
     'download_from_azure_datalake',
     'download_from_databricks_unity_catalog',
     'download_from_dbfs',
+    'download_from_alipan',
     'download_from_local',
 ]
 
 BOTOCORE_CLIENT_ERROR_CODES = {'403', '404', 'NoSuchKey'}
 
 GCS_ERROR_NO_AUTHENTICATION = """\
 Either set the environment variables `GCS_KEY` and `GCS_SECRET` or use any of the methods in \
@@ -418,14 +419,58 @@
                       f'Databricks Unity Catalog, file path must starts with `dbfs:/Volumes` ' +
                       f'and for Databricks File System, file path must starts with `dbfs`. ' +
                       e.args[0],)
         raise e
     os.rename(local_tmp, local)
 
 
+def download_from_alipan(remote: str, local: str) -> None:
+    """Download a file from remote Alipan to local.
+
+    Args:
+        remote (str): Remote path (Alipan).
+        local (str): Local path (local filesystem).
+    """
+    from alipcs_py.alipcs import AliPCSApiMix
+    from alipcs_py.commands.download import download_file
+
+    web_refresh_token = os.environ['ALIPAN_WEB_REFRESH_TOKEN']
+    web_token_type = 'Bearer'
+    alipan_encrypt_password = os.environ.get('ALIPAN_ENCRYPT_PASSWORD', '').encode()
+
+    api = AliPCSApiMix(web_refresh_token, web_token_type=web_token_type)
+
+    obj = urllib.parse.urlparse(remote)
+    if obj.scheme != 'alipan':
+        raise ValueError(
+            f'Expected obj.scheme to be `alipan`, instead, got {obj.scheme} for remote={remote}')
+    if obj.netloc != '':
+        raise ValueError(
+            f'Expected remote to be alipan:///path/to/some, instead, got remote={remote}')
+
+    remote_path = obj.path
+    filename = pathlib.PosixPath(remote_path).name
+    localdir = pathlib.Path(local).parent
+
+    remote_pcs_file = api.get_file(remotepath=remote_path)
+    if remote_pcs_file is None:
+        raise FileNotFoundError(f'Object {remote} not found.')
+
+    download_file(
+        api,
+        remote_pcs_file,
+        localdir=localdir,
+        downloader='me',
+        concurrency=1,
+        show_progress=False,
+        encrypt_password=alipan_encrypt_password,
+    )
+    os.rename(localdir / filename, local)
+
+
 def download_from_local(remote: str, local: str) -> None:
     """Download a file from remote to local.
 
     Args:
         remote (str): Remote path (local filesystem).
         local (str): Local path (local filesystem).
     """
@@ -470,14 +515,16 @@
         download_from_azure(remote, local)
     elif remote.startswith('azure-dl://'):
         download_from_azure_datalake(remote, local)
     elif remote.startswith('dbfs:/Volumes'):
         download_from_databricks_unity_catalog(remote, local)
     elif remote.startswith('dbfs:/'):
         download_from_dbfs(remote, local)
+    elif remote.startswith('alipan://'):
+        download_from_alipan(remote, local)
     else:
         download_from_local(remote, local)
 
 
 def wait_for_download(local: str, timeout: float = 60) -> None:
     """Wait for a download by another thread/process to complete.
```

### Comparing `mosaicml-streaming-0.7.5/streaming/base/storage/upload.py` & `mosaicml-streaming-0.7.6/streaming/base/storage/upload.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,29 @@
     'CloudUploader',
     'S3Uploader',
     'GCSUploader',
     'OCIUploader',
     'AzureUploader',
     'DatabricksUnityCatalogUploader',
     'DBFSUploader',
+    'AlipanUploader',
     'LocalUploader',
 ]
 
 logger = logging.getLogger(__name__)
 
 UPLOADERS = {
     's3': 'S3Uploader',
     'gs': 'GCSUploader',
     'oci': 'OCIUploader',
     'azure': 'AzureUploader',
     'azure-dl': 'AzureDataLakeUploader',
     'dbfs:/Volumes': 'DatabricksUnityCatalogUploader',
     'dbfs': 'DBFSUploader',
+    'alipan': 'AlipanUploader',
     '': 'LocalUploader',
 }
 
 
 class GCSAuthentication(Enum):
     HMAC = 1
     SERVICE_ACCOUNT = 2
@@ -941,14 +943,145 @@
                     f'Ensure the file path or credentials are set correctly. For ' +
                     f'Databricks Unity Catalog, file path must starts with `dbfs:/Volumes` ' +
                     f'and for Databricks File System, file path must starts with `dbfs`. ' +
                     e.args[0],)
             raise e
 
 
+class AlipanUploader(CloudUploader):
+    """Upload file from local machine to Alipan.
+
+    Args:
+        out (str | Tuple[str, str]): Output dataset directory to save shard files.
+
+            1. If ``out`` is a local directory, shard files are saved locally.
+            2. If ``out`` is a remote directory, a local temporary directory is created to
+               cache the shard files and then the shard files are uploaded to a remote
+               location. At the end, the temp directory is deleted once shards are uploaded.
+            3. If ``out`` is a tuple of ``(local_dir, remote_dir)``, shard files are saved in
+               the `local_dir` and also uploaded to a remote location.
+        keep_local (bool): If the dataset is uploaded, whether to keep the local dataset
+            shard file or remove it after uploading. Defaults to ``False``.
+        progress_bar (bool): Display TQDM progress bars for uploading output dataset files to
+            a remote location. Default to ``False``.
+        retry (int): Number of times to retry uploading a file. Defaults to ``2``.
+        exist_ok (bool): When exist_ok = False, raise error if the local part of ``out`` already
+            exists and has contents. Defaults to ``False``.
+    """
+
+    def __init__(self,
+                 out: Union[str, Tuple[str, str]],
+                 keep_local: bool = False,
+                 progress_bar: bool = False,
+                 retry: int = 2,
+                 exist_ok: bool = False) -> None:
+        super().__init__(out, keep_local, progress_bar, retry, exist_ok)
+
+        obj = urllib.parse.urlparse(self.remote)
+        if obj.scheme != 'alipan':
+            raise ValueError(
+                f'Expected obj.scheme to be `alipan`, instead, got {obj.scheme} for remote={self.remote}'
+            )
+        if obj.netloc != '':
+            raise ValueError(
+                f'Expected remote to be alipan:///path/to/some, instead, got remote={self.remote}')
+
+        from alipcs_py.alipcs import AliPCSApiMix
+        from alipcs_py.commands.upload import EncryptType
+
+        web_refresh_token = os.environ['ALIPAN_WEB_REFRESH_TOKEN']
+        web_token_type = 'Bearer'
+        self.alipan_encrypt_password = os.environ.get('ALIPAN_ENCRYPT_PASSWORD', '').encode()
+        self.alipan_encrypt_type = EncryptType.No  # No encryption by default
+        encrypt_type = os.environ.get('ALIPAN_ENCRYPT_TYPE', '')
+        if encrypt_type:
+            if getattr(EncryptType, encrypt_type, None) is None:
+                raise ValueError(
+                    f'Invalid ALIPAN_ENCRYPT_TYPE: {encrypt_type}. ' +
+                    'Encryption type must be one of `Simple`, `ChaCha20`, `AES256CBC`')
+            else:
+                self.alipan_encrypt_type = getattr(EncryptType, encrypt_type)
+
+        self.api = AliPCSApiMix(web_refresh_token, web_token_type=web_token_type)
+        self.check_token()
+
+    def check_token(self):
+        """Raise an exception if the refresh_token is invalid.
+
+        Raises:
+            error: AliPCSError with code `AccessTokenInvalid`
+        """
+        self.api.refresh()
+
+    def upload_file(self, filename: str):
+        """Upload file from local instance to Alipan directory.
+
+        Args:
+            filename (str): File to upload.
+        """
+        from alipcs_py.commands import upload as alipcs_upload
+        from alipcs_py.commands.upload import EncryptType, total_len
+
+        @retry(num_attempts=self.retry)
+        def _upload_file():
+            local_filename = os.path.join(self.local, filename)
+            remote_filename = os.path.join(self.remote, filename)  # pyright: ignore
+            obj = urllib.parse.urlparse(remote_filename)
+            logger.debug(f'Uploading to {remote_filename}')
+            if self.alipan_encrypt_type == EncryptType.No:
+                file_size = os.stat(local_filename).st_size
+            else:
+                file_size = self.alipan_encrypt_type
+                encrypt_io = self.alipan_encrypt_type.encrypt_io(open(local_filename, 'rb'),
+                                                                 self.alipan_encrypt_password)
+                file_size = total_len(encrypt_io)
+            with tqdm.tqdm(total=file_size,
+                           unit='B',
+                           unit_scale=True,
+                           desc=f'Uploading to {remote_filename}',
+                           disable=(not self.progress_bar)) as pbar:
+                alipcs_upload.upload_file(
+                    self.api, (local_filename, obj.path),
+                    'overwrite',
+                    encrypt_password=self.alipan_encrypt_password,
+                    encrypt_type=self.alipan_encrypt_type,
+                    callback_for_monitor=lambda offset: pbar.update(offset - pbar.n))
+            self.clear_local(local=local_filename)
+
+        _upload_file()
+
+    def list_objects(self, prefix: Optional[str] = None) -> List[str]:
+        """List all objects in the remote path with the given prefix.
+
+        Args:
+            prefix (Optional[str], optional): The prefix to search for. Defaults to ``None``.
+
+        Returns:
+            List[str]: A list of object names that match the prefix.
+        """
+        if prefix is None:
+            prefix = ''
+
+        if self.remote is None:
+            raise ValueError('Alipan remote path must be set.')
+
+        obj = urllib.parse.urlparse(self.remote)
+        remote_pcs_file = self.api.get_file(remotepath=obj.path)
+        if remote_pcs_file is None:
+            raise FileNotFoundError(f'Alipan remote path `{obj.path}` not found.')
+
+        file_paths = []
+        for pcs_file in self.api.list_iter(remote_pcs_file.file_id, recursive=True):
+            file_path = pathlib.PosixPath(obj.path, pcs_file.path).as_posix()
+            if file_path.startswith(prefix):
+                file_paths.append(file_path)
+
+        return sorted(file_paths)
+
+
 class LocalUploader(CloudUploader):
     """Copy file from one local directory to another local directory.
 
     Args:
         out (str | Tuple[str, str]): Output dataset directory to save shard files.
 
             1. If ``out`` is a local directory, shard files are saved locally.
```

### Comparing `mosaicml-streaming-0.7.5/streaming/base/stream.py` & `mosaicml-streaming-0.7.6/streaming/base/stream.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/util.py` & `mosaicml-streaming-0.7.6/streaming/base/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/base/world.py` & `mosaicml-streaming-0.7.6/streaming/base/world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py` & `mosaicml-streaming-0.7.6/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid.py` & `mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/crawl_webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py` & `mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/multimodal/convert/webvid/extract_webvid_videos.py` & `mosaicml-streaming-0.7.6/streaming/multimodal/convert/webvid/extract_webvid_videos.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/multimodal/webvid.py` & `mosaicml-streaming-0.7.6/streaming/multimodal/webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/c4.py` & `mosaicml-streaming-0.7.6/streaming/text/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/c4.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/create_pretraining_data.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/make_train_parallel.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/merge_shard_groups.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/merge_shard_groups.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/pick_eval_samples.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/mds/tokenization.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/mds/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/count_samples.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/count_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki/tfrecord/tokenization.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki/tfrecord/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/enwiki_text.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/enwiki_text.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/convert/pile.py` & `mosaicml-streaming-0.7.6/streaming/text/convert/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/enwiki.py` & `mosaicml-streaming-0.7.6/streaming/text/enwiki.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/text/pile.py` & `mosaicml-streaming-0.7.6/streaming/text/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/ade20k.py` & `mosaicml-streaming-0.7.6/streaming/vision/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/base.py` & `mosaicml-streaming-0.7.6/streaming/vision/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/cifar10.py` & `mosaicml-streaming-0.7.6/streaming/vision/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/coco.py` & `mosaicml-streaming-0.7.6/streaming/vision/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/convert/ade20k.py` & `mosaicml-streaming-0.7.6/streaming/vision/convert/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/convert/base.py` & `mosaicml-streaming-0.7.6/streaming/vision/convert/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/convert/cifar10.py` & `mosaicml-streaming-0.7.6/streaming/vision/convert/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/convert/coco.py` & `mosaicml-streaming-0.7.6/streaming/vision/convert/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/convert/fake_cifar10.py` & `mosaicml-streaming-0.7.6/streaming/vision/convert/fake_cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/convert/imagenet.py` & `mosaicml-streaming-0.7.6/streaming/vision/convert/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/streaming/vision/imagenet.py` & `mosaicml-streaming-0.7.6/streaming/vision/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_array.py` & `mosaicml-streaming-0.7.6/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_barrier.py` & `mosaicml-streaming-0.7.6/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_compression.py` & `mosaicml-streaming-0.7.6/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_distributed.py` & `mosaicml-streaming-0.7.6/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_download.py` & `mosaicml-streaming-0.7.6/tests/test_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,14 +221,22 @@
     @pytest.mark.usefixtures('remote_local_file')
     def test_download_from_dbfs_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
         mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='dbfs:/')
         download_file(mock_remote_filepath, mock_local_filepath, 60)
         mocked_requests.assert_called_once()
         mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
 
+    @patch('streaming.base.storage.download.download_from_alipan')
+    @pytest.mark.usefixtures('remote_local_file')
+    def test_download_from_alipan_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
+        mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='alipan://')
+        download_file(mock_remote_filepath, mock_local_filepath, 60)
+        mocked_requests.assert_called_once()
+        mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
+
     @patch('streaming.base.storage.download.download_from_local')
     @pytest.mark.usefixtures('remote_local_file')
     def test_download_from_local_gets_called(self, mocked_requests: Mock, remote_local_file: Any):
         mock_remote_filepath, mock_local_filepath = remote_local_file()
         download_file(mock_remote_filepath, mock_local_filepath, 60)
         mocked_requests.assert_called_once()
         mocked_requests.assert_called_once_with(mock_remote_filepath, mock_local_filepath)
```

### Comparing `mosaicml-streaming-0.7.5/tests/test_encodings.py` & `mosaicml-streaming-0.7.6/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_eviction.py` & `mosaicml-streaming-0.7.6/tests/test_eviction.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_hashing.py` & `mosaicml-streaming-0.7.6/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_laziness.py` & `mosaicml-streaming-0.7.6/tests/test_laziness.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_local.py` & `mosaicml-streaming-0.7.6/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_mixing.py` & `mosaicml-streaming-0.7.6/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_partition.py` & `mosaicml-streaming-0.7.6/tests/test_partition.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_reader.py` & `mosaicml-streaming-0.7.6/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_sampling.py` & `mosaicml-streaming-0.7.6/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_shared.py` & `mosaicml-streaming-0.7.6/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_shuffle.py` & `mosaicml-streaming-0.7.6/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_spanner.py` & `mosaicml-streaming-0.7.6/tests/test_spanner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_stream.py` & `mosaicml-streaming-0.7.6/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_streaming.py` & `mosaicml-streaming-0.7.6/tests/test_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from multiprocessing import Process
 from typing import Any, Callable, Tuple
 
 import pytest
 from torch.utils.data import DataLoader
 
 from streaming.base import Stream, StreamingDataLoader, StreamingDataset
+from streaming.base.batching import generate_work
 from streaming.base.util import clean_stale_shared_memory
+from streaming.base.world import World
 from tests.common.utils import convert_to_mds
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_no_batch_size_exception(local_remote_dir: Tuple[str, str]):
 
     remote_dir, local_dir = local_remote_dir
@@ -174,14 +176,90 @@
     # Make sure that we see the expected number of batches, accounting for sample drops
     assert batches_seen == total_batches
 
 
 @pytest.mark.parametrize('batch_size', [4, 7])
 @pytest.mark.parametrize('seed', [2222])
 @pytest.mark.parametrize('shuffle', [True])
+@pytest.mark.parametrize('physical_nodes', [2, 8])
+@pytest.mark.parametrize('ranks_per_node', [4, 8])
+@pytest.mark.parametrize('workers_per_rank', [4, 8])
+@pytest.mark.parametrize('num_canonical_nodes', [8])
+@pytest.mark.usefixtures('local_remote_dir')
+def test_dataloader_device_per_stream_batching(local_remote_dir: Tuple[str, str], batch_size: int,
+                                               seed: int, shuffle: bool, physical_nodes: int,
+                                               ranks_per_node: int, workers_per_rank: int,
+                                               num_canonical_nodes: int):
+    # create mock datasets for 2 streams. Second one has 1.5x the samples
+    local, remote = local_remote_dir
+    local1 = os.path.join(local, 'stream1')
+    local2 = os.path.join(local, 'stream2')
+    remote1 = os.path.join(remote, 'stream1')
+    remote2 = os.path.join(remote, 'stream2')
+
+    # stream 1 has samples 0->600, sample ids 0->200
+    convert_to_mds(out_root=remote1,
+                   dataset_name='sequencedataset',
+                   num_samples=200,
+                   size_limit=1 << 8)
+    # stream 2 has samples 600 and above, sample ids 200 and above.
+    # This lets us differentiate between the samples from each stream
+    convert_to_mds(out_root=remote2,
+                   dataset_name='sequencedataset',
+                   num_samples=300,
+                   offset=600,
+                   size_limit=1 << 8)
+
+    stream1 = Stream(local=local1, remote=remote1)
+    stream2 = Stream(local=local2, remote=remote2)
+
+    # Build StreamingDataset
+    dataset = StreamingDataset(streams=[stream1, stream2],
+                               shuffle=shuffle,
+                               batch_size=batch_size,
+                               shuffle_seed=seed,
+                               num_canonical_nodes=num_canonical_nodes,
+                               batching_method='per_stream',
+                               shuffle_block_size=100)
+
+    # Get sample partition
+    fake_world = World(
+        num_nodes=physical_nodes,
+        ranks_per_node=ranks_per_node,
+        workers_per_rank=workers_per_rank,
+        worker=0,
+    )
+    sample_partition = generate_work(batching_method='device_per_stream',
+                                     dataset=dataset,
+                                     world=fake_world,
+                                     epoch=0,
+                                     sample_in_epoch=0)
+
+    # Partition shape should be:
+    # (physical nodes, ranks per node, workers per rank, batches per worker, batch size)
+    assert sample_partition.shape[0] == physical_nodes
+    assert sample_partition.shape[1] == ranks_per_node
+    assert sample_partition.shape[2] == workers_per_rank
+    assert sample_partition.shape[4] == batch_size
+
+    # Transpose and reshape sample partition to get device batches, in training traversal order.
+    sample_partition = sample_partition.transpose(3, 2, 0, 1, 4).flatten().reshape(-1, batch_size)
+
+    for device_batch in sample_partition:
+        if device_batch[0] < 200:
+            # Ensure all samples are from stream 1
+            assert (device_batch < 200).all()
+        else:
+            # Ensure all samples are from stream 2
+            assert (device_batch >= 200).all()
+
+
+@pytest.mark.parametrize('batch_size', [4, 7])
+@pytest.mark.parametrize('seed', [2222])
+@pytest.mark.parametrize('shuffle', [True])
 @pytest.mark.parametrize('drop_last', [True])
 @pytest.mark.parametrize('num_workers', [4])
 @pytest.mark.parametrize('num_canonical_nodes', [8])
 @pytest.mark.parametrize('num_stream_1_samples', [200, 255])
 @pytest.mark.parametrize('num_stream_2_samples', [342, 557])
 @pytest.mark.usefixtures('local_remote_dir')
 def test_dataloader_stratified_batching(local_remote_dir: Tuple[str, str], batch_size: int,
```

### Comparing `mosaicml-streaming-0.7.5/tests/test_streaming_remote.py` & `mosaicml-streaming-0.7.6/tests/test_streaming_remote.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_unsafe_types.py` & `mosaicml-streaming-0.7.6/tests/test_unsafe_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.7.5/tests/test_upload.py` & `mosaicml-streaming-0.7.6/tests/test_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from typing import Any, List, Tuple
 from unittest import mock
 from unittest.mock import ANY, MagicMock, Mock, patch
 
 import boto3
 import pytest
 
-from streaming.base.storage.upload import (AzureDataLakeUploader, AzureUploader, CloudUploader,
-                                           DatabricksUnityCatalogUploader, DBFSUploader,
-                                           GCSAuthentication, GCSUploader, LocalUploader,
-                                           S3Uploader)
+from streaming.base.storage.upload import (AlipanUploader, AzureDataLakeUploader, AzureUploader,
+                                           CloudUploader, DatabricksUnityCatalogUploader,
+                                           DBFSUploader, GCSAuthentication, GCSUploader,
+                                           LocalUploader, S3Uploader)
 from tests.conftest import MY_BUCKET, R2_URL
 
 MY_PREFIX = 'train'
 
 
 @pytest.fixture(scope='function')
 def remote_local_dir() -> Any:
@@ -484,14 +484,49 @@
             local_file_path = os.path.join(local, 'file.txt')
             # Creating an empty file at specified location
             with open(local_file_path, 'w') as _:
                 pass
             _ = DBFSUploader(out=local)
 
 
+class TestAlipanUploader:
+
+    @patch('streaming.base.storage.upload.AlipanUploader.check_token')
+    @pytest.mark.usefixtures('alipan_credentials')
+    @pytest.mark.parametrize('out',
+                             ['alipan:///container/dir', ('./dir1', 'alipan:///container/dir/')])
+    def test_instantiation(self, mock_create_client: Mock, out: Any):
+        mock_create_client.side_effect = None
+        _ = AlipanUploader(out=out)
+        if not isinstance(out, str):
+            shutil.rmtree(out[0], ignore_errors=True)
+
+    @patch('streaming.base.storage.upload.AlipanUploader.check_token')
+    @pytest.mark.usefixtures('alipan_credentials')
+    @pytest.mark.parametrize('out', ['alipann://bucket/dir', ('./dir1', 'gcs://bucket/dir/')])
+    def test_invalid_remote_list(self, mock_create_client: Mock, out: Any):
+        mock_create_client.side_effect = None
+        with pytest.raises(ValueError, match=f'Invalid Cloud provider prefix.*'):
+            _ = AlipanUploader(out=out)
+
+    @patch('streaming.base.storage.upload.AlipanUploader.check_token')
+    @pytest.mark.usefixtures('alipan_credentials')
+    def test_local_directory_is_empty(self, mock_create_client: Mock,
+                                      local_remote_dir: Tuple[str, str]):
+        with pytest.raises(FileExistsError, match=f'Directory is not empty.*'):
+            mock_create_client.side_effect = None
+            local, _ = local_remote_dir
+            os.makedirs(local, exist_ok=True)
+            local_file_path = os.path.join(local, 'file.txt')
+            # Creating an empty file at specified location
+            with open(local_file_path, 'w') as _:
+                pass
+            _ = AlipanUploader(out=local)
+
+
 class TestLocalUploader:
 
     def test_upload_file(self, local_remote_dir: Tuple[str, str]):
         local, remote = local_remote_dir
         filename = 'file.txt'
         local_file_path = os.path.join(local, filename)
         remote_file_path = os.path.join(remote, filename)
```

### Comparing `mosaicml-streaming-0.7.5/tests/test_util.py` & `mosaicml-streaming-0.7.6/tests/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         StructField('id', IntegerType(), nullable=False),
         StructField('name', StringType(), nullable=False),
         StructField('amount', DecimalType(10, 2), nullable=False)
     ])
     data = [(1, 'Alice', Decimal('123.45')), (2, 'Bob', Decimal('67.89')),
             (3, 'Charlie', Decimal('987.65'))]
     df = spark.createDataFrame(data=data, schema=schema).repartition(3)
-    mds_kwargs = {'out': mds_out, 'columns': {'id': 'int', 'name': 'str'}, 'keep_local': True}
+    mds_kwargs = {'out': mds_out, 'columns': {'id': 'int32', 'name': 'str'}, 'keep_local': True}
     dataframeToMDS(df, merge_index=False, mds_kwargs=mds_kwargs)
 
     local_cu = CloudUploader.get(local, exist_ok=True, keep_local=True)
     local_index_files = [
         o for o in local_cu.list_objects() if o.endswith('.json') and not_merged_index(o, local)
     ]
 
@@ -293,15 +293,15 @@
     ])
 
     data = [(1, 'Alice', Decimal('123.45')), (2, 'Bob', Decimal('67.89')),
             (3, 'Charlie', Decimal('987.65'))]
 
     df = spark.createDataFrame(data=data, schema=schema).repartition(n_partitions)
 
-    mds_kwargs = {'out': out, 'columns': {'id': 'int', 'name': 'str'}, 'keep_local': keep_local}
+    mds_kwargs = {'out': out, 'columns': {'id': 'int32', 'name': 'str'}, 'keep_local': keep_local}
 
     mds_path, _ = dataframeToMDS(df, merge_index=False, mds_kwargs=mds_kwargs)
     merge_index(mds_path, keep_local=keep_local)
     integrity_check(mds_path, keep_local=keep_local)
 
 
 @pytest.mark.parametrize('with_args', [True, False])
```

### Comparing `mosaicml-streaming-0.7.5/tests/test_writer.py` & `mosaicml-streaming-0.7.6/tests/test_writer.py`

 * *Files identical despite different names*

