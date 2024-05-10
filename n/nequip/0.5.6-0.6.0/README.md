# Comparing `tmp/nequip-0.5.6.tar.gz` & `tmp/nequip-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nequip-0.5.6.tar", last modified: Tue Dec 20 18:53:12 2022, max compression
+gzip compressed data, was "nequip-0.6.0.tar", last modified: Fri May 10 22:28:04 2024, max compression
```

## Comparing `nequip-0.5.6.tar` & `nequip-0.6.0.tar`

### file list

```diff
@@ -1,101 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.882593 nequip-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2022-12-20 18:53:02.000000 nequip-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-20 18:53:12.882593 nequip-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2022-12-20 18:53:02.000000 nequip-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.870593 nequip-0.5.6/nequip/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.870593 nequip-0.5.6/nequip/ase/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/ase/nequip_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/ase/nosehoover.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.874593 nequip-0.5.6/nequip/data/
--rw-r--r--   0 runner    (1001) docker     (123)    32290 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/AtomicData.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/AtomicDataDict.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    37880 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/data/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.874593 nequip-0.5.6/nequip/model/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/_eng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/_grads.py
--rw-r--r--   0 runner    (1001) docker     (123)    12332 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/model/builder_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.874593 nequip-0.5.6/nequip/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_atomwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_convnetlayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_grad_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_graph_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_interaction_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/cutoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.874593 nequip-0.5.6/nequip/nn/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/embedding/_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/embedding/_one_hot.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/nonlinearities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/nn/radial_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.878593 nequip-0.5.6/nequip/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16910 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/run_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.878593 nequip-0.5.6/nequip/train/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    46072 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/train/trainer_wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.878593 nequip-0.5.6/nequip/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/_global_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/auto_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/batch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/savenload.py
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.882593 nequip-0.5.6/nequip/utils/torch_geometric/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/torch_geometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/torch_geometric/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    16569 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/torch_geometric/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10012 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/torch_geometric/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/torch_geometric/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/tp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.882593 nequip-0.5.6/nequip/utils/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/unittests/model_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2022-12-20 18:53:02.000000 nequip-0.5.6/nequip/utils/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 18:53:12.870593 nequip-0.5.6/nequip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 18:53:12.000000 nequip-0.5.6/nequip.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-20 18:53:12.882593 nequip-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2022-12-20 18:53:02.000000 nequip-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.940018 nequip-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-10 22:27:56.000000 nequip-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 22:28:04.940018 nequip-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-10 22:27:56.000000 nequip-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.924018 nequip-0.6.0/nequip/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.924018 nequip-0.6.0/nequip/ase/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/ase/nequip_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/ase/nosehoover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.928018 nequip-0.6.0/nequip/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    33995 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/AtomicData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/AtomicDataDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_build.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.928018 nequip-0.6.0/nequip/data/_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_dataset/_ase_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26679 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_dataset/_base_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_dataset/_hdf5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_dataset/_npz_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/data/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.928018 nequip-0.6.0/nequip/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_eng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_grads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_pair_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/model/builder_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.932018 nequip-0.6.0/nequip/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10942 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_atomwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_convnetlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_grad_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_graph_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_graph_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_interaction_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_rescale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/cutoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.932018 nequip-0.6.0/nequip/nn/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/embedding/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/embedding/_one_hot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/nonlinearities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13495 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/pair_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/nn/radial_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.932018 nequip-0.6.0/nequip/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18694 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/run_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.936018 nequip-0.6.0/nequip/train/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46782 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/trainer_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/train/trainer_wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.936018 nequip-0.6.0/nequip/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/_global_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/auto_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/batch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11770 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/savenload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.940018 nequip-0.6.0/nequip/utils/torch_geometric/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/torch_geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/torch_geometric/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16569 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/torch_geometric/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10012 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/torch_geometric/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/torch_geometric/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/tp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.940018 nequip-0.6.0/nequip/utils/unittests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20902 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/unittests/model_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-10 22:27:56.000000 nequip-0.6.0/nequip/utils/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:28:04.924018 nequip-0.6.0/nequip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:28:04.000000 nequip-0.6.0/nequip.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-10 22:28:04.940018 nequip-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-10 22:27:56.000000 nequip-0.6.0/setup.py
```

### Comparing `nequip-0.5.6/LICENSE` & `nequip-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/README.md` & `nequip-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 **PLEASE NOTE:** the NequIP code is under active development and is still in beta versions 0.x.x. In general changes to the patch version (the third number) indicate backward compatible beta releases, but please be aware that file formats and APIs may change. Bug reports are also welcomed in the GitHub issues!
 
 ## Installation
 
 NequIP requires:
 
 * Python >= 3.7
-* PyTorch >= 1.8, !=1.9, <=1.11.*. PyTorch can be installed following the [instructions from their documentation](https://pytorch.org/get-started/locally/). Note that neither `torchvision` nor `torchaudio`, included in the default install command, are needed for NequIP.
+* PyTorch == `1.11.*` or `1.13.*` or later (do **not** use `1.12`). (Some users have observed silent issues with PyTorch 2+, as reported in #311. Please report any similar issues you encounter.) PyTorch can be installed following the [instructions from their documentation](https://pytorch.org/get-started/locally/). Note that neither `torchvision` nor `torchaudio`, included in the default install command, are needed for NequIP.
+
+**You must install PyTorch before installing NequIP, however it is not marked as a dependency of `nequip` to prevent `pip` from trying to overwrite your PyTorch installation.**
 
 To install:
 
-* We use [Weights&Biases](https://wandb.ai) to keep track of experiments. This is not a strict requirement — you can use our package without it — but it may make your life easier. If you want to use it, create an account [here](https://wandb.ai) and install the Python package:
+* We use [Weights&Biases](https://wandb.ai) (or TensorBoard) to keep track of experiments. This is not a strict requirement — you can use our package without it — but it may make your life easier. If you want to use it, create an account [here](https://wandb.ai) and install the Python package:
 
   ```
   pip install wandb
   ```
 
 * Install NequIP
 
@@ -126,14 +128,20 @@
 ```
 pair_style	nequip
 pair_coeff	* * deployed.pth <NequIP type for LAMMPS type 1> <NequIP type for LAMMPS type 2> ...
 ```
 
 For installation instructions, please see the [`pair_nequip` repository](https://github.com/mir-group/pair_nequip).
 
+## Plugins / extending `nequip`
+
+`nequip` is a modular framework and extension packages can provide new model components, architectures, etc. The main extension package(s) currently available are:
+ - [Allegro](https://github.com/mir-group/allegro): implements the highly parallelizable Allegro model architecture.
+
+Details on writing and using plugins can be found in the [Allegro tutorial](https://colab.research.google.com/drive/1yq2UwnET4loJYg_Fptt9kpklVaZvoHnq) and in [`nequip-example-extension`](https://github.com/mir-group/nequip-example-extension/).
 
 ## References & citing
 
 The theory behind NequIP is described in our preprint (1). NequIP's backend builds on e3nn, a general framework for building E(3)-equivariant neural networks (2). If you use this repository in your work, please consider citing NequIP (1) and e3nn (3):
 
  1. https://www.nature.com/articles/s41467-022-29939-5
  2. https://e3nn.org
@@ -146,17 +154,17 @@
  - Simon Batzner
  - Albert Musaelian
  - Lixin Sun
  - Anders Johansson
  - Mario Geiger
  - Tess Smidt
 
-under the guidance of [Boris Kozinsky at Harvard](https://bkoz.seas.harvard.edu/).
+under the guidance of [Boris Kozinsky at Harvard](https://mir.g.harvard.edu/).
 
 ## Contact, questions, and contributing
 
-If you have questions, please don't hesitate to reach out at batzner[at]g[dot]harvard[dot]edu. 
-
 If you find a bug or have a proposal for a feature, please post it in the [Issues](https://github.com/mir-group/nequip/issues).
 If you have a question, topic, or issue that isn't obviously one of those, try our [GitHub Discussions](https://github.com/mir-group/nequip/discussions).
 
 If you want to contribute to the code, please read [`CONTRIBUTING.md`](CONTRIBUTING.md).
+
+We can also be reached at albym[dot]seas[dt]harvard[dot].edu.
```

### Comparing `nequip-0.5.6/nequip/ase/nequip_calculator.py` & `nequip-0.6.0/nequip/ase/nequip_calculator.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/ase/nosehoover.py` & `nequip-0.6.0/nequip/ase/nosehoover.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/data/AtomicData.py` & `nequip-0.6.0/nequip/data/AtomicData.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """AtomicData: neighbor graphs in (periodic) real space.
 
 Authors: Albert Musaelian
 """
 
 import warnings
 from copy import deepcopy
-from typing import Union, Tuple, Dict, Optional, List, Set, Sequence
+from typing import Union, Tuple, Dict, Optional, List, Set, Sequence, Final
 from collections.abc import Mapping
+import os
 
 import numpy as np
 import ase.neighborlist
 import ase
 from ase.calculators.singlepoint import SinglePointCalculator, SinglePointDFTCalculator
 from ase.calculators.calculator import all_properties as ase_all_properties
 from ase.stress import voigt_6_to_full_3x3_stress, full_3x3_to_voigt_6_stress
@@ -45,21 +46,24 @@
 _DEFAULT_EDGE_FIELDS: Set[str] = {
     AtomicDataDict.EDGE_CELL_SHIFT_KEY,
     AtomicDataDict.EDGE_VECTORS_KEY,
     AtomicDataDict.EDGE_LENGTH_KEY,
     AtomicDataDict.EDGE_ATTRS_KEY,
     AtomicDataDict.EDGE_EMBEDDING_KEY,
     AtomicDataDict.EDGE_FEATURES_KEY,
+    AtomicDataDict.EDGE_CUTOFF_KEY,
+    AtomicDataDict.EDGE_ENERGY_KEY,
 }
 _DEFAULT_GRAPH_FIELDS: Set[str] = {
     AtomicDataDict.TOTAL_ENERGY_KEY,
     AtomicDataDict.STRESS_KEY,
     AtomicDataDict.VIRIAL_KEY,
     AtomicDataDict.PBC_KEY,
     AtomicDataDict.CELL_KEY,
+    AtomicDataDict.BATCH_PTR_KEY,
 }
 _NODE_FIELDS: Set[str] = set(_DEFAULT_NODE_FIELDS)
 _EDGE_FIELDS: Set[str] = set(_DEFAULT_EDGE_FIELDS)
 _GRAPH_FIELDS: Set[str] = set(_DEFAULT_GRAPH_FIELDS)
 _LONG_FIELDS: Set[str] = set(_DEFAULT_LONG_FIELDS)
 
 
@@ -74,14 +78,15 @@
     Args:
         node_permute_fields: fields that are equivariant to node permutations.
         edge_permute_fields: fields that are equivariant to edge permutations.
     """
     node_fields: set = set(node_fields)
     edge_fields: set = set(edge_fields)
     graph_fields: set = set(graph_fields)
+    long_fields: set = set(long_fields)
     allfields = node_fields.union(edge_fields, graph_fields)
     assert len(allfields) == len(node_fields) + len(edge_fields) + len(graph_fields)
     _NODE_FIELDS.update(node_fields)
     _EDGE_FIELDS.update(edge_fields)
     _GRAPH_FIELDS.update(graph_fields)
     _LONG_FIELDS.update(long_fields)
     if len(set.union(_NODE_FIELDS, _EDGE_FIELDS, _GRAPH_FIELDS)) < (
@@ -105,14 +110,25 @@
         assert f not in _DEFAULT_EDGE_FIELDS, "Cannot deregister built-in field"
         assert f not in _DEFAULT_GRAPH_FIELDS, "Cannot deregister built-in field"
         _NODE_FIELDS.discard(f)
         _EDGE_FIELDS.discard(f)
         _GRAPH_FIELDS.discard(f)
 
 
+def _register_field_prefix(prefix: str) -> None:
+    """Re-register all registered fields as the same type, but with `prefix` added on."""
+    assert prefix.endswith("_")
+    register_fields(
+        node_fields=[prefix + e for e in _NODE_FIELDS],
+        edge_fields=[prefix + e for e in _EDGE_FIELDS],
+        graph_fields=[prefix + e for e in _GRAPH_FIELDS],
+        long_fields=[prefix + e for e in _LONG_FIELDS],
+    )
+
+
 def _process_dict(kwargs, ignore_fields=[]):
     """Convert a dict of data into correct dtypes/shapes according to key"""
     # Deal with _some_ dtype issues
     for k, v in kwargs.items():
         if k in ignore_fields:
             continue
 
@@ -137,14 +153,21 @@
             # Force scalars to be tensors with a data dimension
             # This makes them play well with irreps
             kwargs[k] = torch.as_tensor(v, dtype=torch.get_default_dtype())
         elif isinstance(v, torch.Tensor) and len(v.shape) == 0:
             # ^ this tensor is a scalar; we need to give it
             # a data dimension to play nice with irreps
             kwargs[k] = v
+        elif isinstance(v, torch.Tensor):
+            # This is a tensor, so we just don't do anything except avoid the warning in the `else`
+            pass
+        else:
+            warnings.warn(
+                f"Value for field {k} was of unsupported type {type(v)} (value was {v})"
+            )
 
     if AtomicDataDict.BATCH_KEY in kwargs:
         num_frames = kwargs[AtomicDataDict.BATCH_KEY].max() + 1
     else:
         num_frames = 1
 
     for k, v in kwargs.items():
@@ -209,15 +232,14 @@
         atom_type (Tensor [n_atom]): optional.
         **kwargs: other data, optional.
     """
 
     def __init__(
         self, irreps: Dict[str, e3nn.o3.Irreps] = {}, _validate: bool = True, **kwargs
     ):
-
         # empty init needed by get_example
         if len(kwargs) == 0 and len(irreps) == 0:
             super().__init__()
             return
 
         # Check the keys
         if _validate:
@@ -400,15 +422,14 @@
                 key_mapping.get(k, k): v
                 for k, v in atoms.info.items()
                 if k in include_keys
             }
         )
 
         if atoms.calc is not None:
-
             if isinstance(
                 atoms.calc, (SinglePointCalculator, SinglePointDFTCalculator)
             ):
                 add_fields.update(
                     {
                         key_mapping.get(k, k): deepcopy(v)
                         for k, v in atoms.calc.results.items()
@@ -676,14 +697,26 @@
                     new_dict[k] = self[k]
 
         new_dict["irreps"] = self.__irreps__
 
         return type(self)(**new_dict)
 
 
+_ERROR_ON_NO_EDGES: bool = os.environ.get("NEQUIP_ERROR_ON_NO_EDGES", "true").lower()
+assert _ERROR_ON_NO_EDGES in ("true", "false")
+_ERROR_ON_NO_EDGES = _ERROR_ON_NO_EDGES == "true"
+
+_NEQUIP_MATSCIPY_NL: Final[bool] = os.environ.get("NEQUIP_MATSCIPY_NL", "false").lower()
+assert _NEQUIP_MATSCIPY_NL in ("true", "false")
+_NEQUIP_MATSCIPY_NL = _NEQUIP_MATSCIPY_NL == "true"
+
+if _NEQUIP_MATSCIPY_NL:
+    import matscipy.neighbours
+
+
 def neighbor_list_and_relative_vec(
     pos,
     r_max,
     self_interaction=False,
     strict_self_interaction=True,
     cell=None,
     pbc=False,
@@ -753,30 +786,40 @@
         # ASE will "complete" this correctly.
         temp_cell = np.zeros((3, 3), dtype=temp_pos.dtype)
         cell_tensor = torch.as_tensor(temp_cell, device=out_device, dtype=out_dtype)
 
     # ASE dependent part
     temp_cell = ase.geometry.complete_cell(temp_cell)
 
-    first_idex, second_idex, shifts = ase.neighborlist.primitive_neighbor_list(
-        "ijS",
-        pbc,
-        temp_cell,
-        temp_pos,
-        cutoff=float(r_max),
-        self_interaction=strict_self_interaction,  # we want edges from atom to itself in different periodic images!
-        use_scaled_positions=False,
-    )
+    if _NEQUIP_MATSCIPY_NL:
+        assert strict_self_interaction and not self_interaction
+        first_idex, second_idex, shifts = matscipy.neighbours.neighbour_list(
+            "ijS",
+            pbc=pbc,
+            cell=temp_cell,
+            positions=temp_pos,
+            cutoff=float(r_max),
+        )
+    else:
+        first_idex, second_idex, shifts = ase.neighborlist.primitive_neighbor_list(
+            "ijS",
+            pbc,
+            temp_cell,
+            temp_pos,
+            cutoff=float(r_max),
+            self_interaction=strict_self_interaction,  # we want edges from atom to itself in different periodic images!
+            use_scaled_positions=False,
+        )
 
     # Eliminate true self-edges that don't cross periodic boundaries
     if not self_interaction:
         bad_edge = first_idex == second_idex
         bad_edge &= np.all(shifts == 0, axis=1)
         keep_edge = ~bad_edge
-        if not np.any(keep_edge):
+        if _ERROR_ON_NO_EDGES and (not np.any(keep_edge)):
             raise ValueError(
                 f"Every single atom has no neighbors within the cutoff r_max={r_max} (after eliminating self edges, no edges remain in this system)"
             )
         first_idex = first_idex[keep_edge]
         second_idex = second_idex[keep_edge]
         shifts = shifts[keep_edge]
```

### Comparing `nequip-0.5.6/nequip/data/AtomicDataDict.py` & `nequip-0.6.0/nequip/data/AtomicDataDict.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,8 +107,16 @@
     """
     if _keys.BATCH_KEY in data:
         return data
     else:
         pos = data[_keys.POSITIONS_KEY]
         batch = torch.zeros(len(pos), dtype=torch.long, device=pos.device)
         data[_keys.BATCH_KEY] = batch
+        # ugly way to make a tensor of [0, len(pos)], but it avoids transfers or casts
+        data[_keys.BATCH_PTR_KEY] = torch.arange(
+            start=0,
+            end=len(pos) + 1,
+            step=len(pos),
+            dtype=torch.long,
+            device=pos.device,
+        )
         return data
```

### Comparing `nequip-0.5.6/nequip/data/__init__.py` & `nequip-0.6.0/nequip/data/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 from .AtomicData import (
     AtomicData,
     PBC,
     register_fields,
     deregister_fields,
+    _register_field_prefix,
     _NODE_FIELDS,
     _EDGE_FIELDS,
     _GRAPH_FIELDS,
+    _LONG_FIELDS,
 )
-from .dataset import AtomicDataset, AtomicInMemoryDataset, NpzDataset, ASEDataset
-from .dataloader import DataLoader, Collater
+from ._dataset import (
+    AtomicDataset,
+    AtomicInMemoryDataset,
+    NpzDataset,
+    ASEDataset,
+    HDF5Dataset,
+)
+from .dataloader import DataLoader, Collater, PartialSampler
 from ._build import dataset_from_config
 from ._test_data import EMTTestDataset
 
 __all__ = [
     AtomicData,
     PBC,
     register_fields,
     deregister_fields,
+    _register_field_prefix,
     AtomicDataset,
     AtomicInMemoryDataset,
     NpzDataset,
     ASEDataset,
+    HDF5Dataset,
     DataLoader,
     Collater,
+    PartialSampler,
     dataset_from_config,
     _NODE_FIELDS,
     _EDGE_FIELDS,
     _GRAPH_FIELDS,
+    _LONG_FIELDS,
     EMTTestDataset,
 ]
```

### Comparing `nequip-0.5.6/nequip/data/_build.py` & `nequip-0.6.0/nequip/data/_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,18 +53,18 @@
                 elif k.lower() == dataset_name:
                     class_name = v
 
     if class_name is None:
         raise NameError(f"dataset type {dataset_name} does not exists")
 
     # if dataset r_max is not found, use the universal r_max
-    eff_key = "extra_fixed_fields"
-    prefixed_eff_key = f"{prefix}_{eff_key}"
+    atomicdata_options_key = "AtomicData_options"
+    prefixed_eff_key = f"{prefix}_{atomicdata_options_key}"
     config[prefixed_eff_key] = get_w_prefix(
-        eff_key, {}, prefix=prefix, arg_dicts=config
+        atomicdata_options_key, {}, prefix=prefix, arg_dicts=config
     )
     config[prefixed_eff_key]["r_max"] = get_w_prefix(
         "r_max",
         prefix=prefix,
         arg_dicts=[config[prefixed_eff_key], config],
     )
```

### Comparing `nequip-0.5.6/nequip/data/_keys.py` & `nequip-0.6.0/nequip/data/_keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,35 +41,41 @@
 # A [n_edge] tensor of the lengths of EDGE_VECTORS
 EDGE_LENGTH_KEY: Final[str] = "edge_lengths"
 # [n_edge, dim] (possibly equivariant) attributes of each edge
 EDGE_ATTRS_KEY: Final[str] = "edge_attrs"
 # [n_edge, dim] invariant embedding of the edges
 EDGE_EMBEDDING_KEY: Final[str] = "edge_embedding"
 EDGE_FEATURES_KEY: Final[str] = "edge_features"
+# [n_edge, 1] invariant of the radial cutoff envelope for each edge, allows reuse of cutoff envelopes
+EDGE_CUTOFF_KEY: Final[str] = "edge_cutoff"
+# edge energy as in Allegro
+EDGE_ENERGY_KEY: Final[str] = "edge_energy"
 
 NODE_FEATURES_KEY: Final[str] = "node_features"
 NODE_ATTRS_KEY: Final[str] = "node_attrs"
 
 PER_ATOM_ENERGY_KEY: Final[str] = "atomic_energy"
 TOTAL_ENERGY_KEY: Final[str] = "total_energy"
 FORCE_KEY: Final[str] = "forces"
 PARTIAL_FORCE_KEY: Final[str] = "partial_forces"
 STRESS_KEY: Final[str] = "stress"
 VIRIAL_KEY: Final[str] = "virial"
 
 ALL_ENERGY_KEYS: Final[List[str]] = [
+    EDGE_ENERGY_KEY,
     PER_ATOM_ENERGY_KEY,
     TOTAL_ENERGY_KEY,
     FORCE_KEY,
     PARTIAL_FORCE_KEY,
     STRESS_KEY,
     VIRIAL_KEY,
 ]
 
 BATCH_KEY: Final[str] = "batch"
+BATCH_PTR_KEY: Final[str] = "ptr"
 
 # Make a list of allowed keys
 ALLOWED_KEYS: List[str] = [
     getattr(sys.modules[__name__], k)
     for k in sys.modules[__name__].__dict__.keys()
     if k.endswith("_KEY")
 ]
```

### Comparing `nequip-0.5.6/nequip/data/_test_data.py` & `nequip-0.6.0/nequip/data/_test_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 
 import ase
 import ase.build
 from ase.calculators.emt import EMT
 
-from nequip.data import AtomicInMemoryDataset, AtomicData, AtomicDataDict
+from nequip.data import AtomicInMemoryDataset, AtomicData
 from .transforms import TypeMapper
 
 
 class EMTTestDataset(AtomicInMemoryDataset):
     """Test dataset with PBC based on the toy EMT potential included in ASE.
 
     Randomly generates (in a reproducable manner) a basic bulk with added
@@ -26,32 +26,31 @@
         supercell: Tuple[int, int, int] = (4, 4, 4),
         sigma: float = 0.1,
         element: str = "Cu",
         num_frames: int = 10,
         dataset_seed: int = 123456,
         file_name: Optional[str] = None,
         url: Optional[str] = None,
-        extra_fixed_fields: Dict[str, Any] = {},
+        AtomicData_options: Dict[str, Any] = {},
         include_frames: Optional[List[int]] = None,
         type_mapper: TypeMapper = None,
     ):
         # Set properties for hashing
         assert element in ("Cu", "Pd", "Au", "Pt", "Al", "Ni", "Ag")
         self.element = element
         self.sigma = sigma
-        self.supercell = supercell
+        self.supercell = tuple(supercell)
         self.num_frames = num_frames
         self.dataset_seed = dataset_seed
 
         super().__init__(
             file_name=file_name,
             url=url,
             root=root,
-            force_fixed_keys=[AtomicDataDict.CELL_KEY, AtomicDataDict.PBC_KEY],
-            extra_fixed_fields=extra_fixed_fields,
+            AtomicData_options=AtomicData_options,
             include_frames=include_frames,
             type_mapper=type_mapper,
         )
 
     @property
     def raw_file_names(self):
         return []
@@ -74,11 +73,11 @@
 
             datas.append(
                 AtomicData.from_ase(
                     base_atoms.copy(),
                     forces=base_atoms.get_forces(),
                     total_energy=base_atoms.get_potential_energy(),
                     stress=base_atoms.get_stress(voigt=False),
-                    **self.extra_fixed_fields
+                    **self.AtomicData_options
                 )
             )
-        return (datas,)
+        return datas
```

### Comparing `nequip-0.5.6/nequip/data/dataset.py` & `nequip-0.6.0/nequip/data/_dataset/_base_datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import numpy as np
 import logging
-import tempfile
 import inspect
-import functools
 import itertools
 import yaml
 import hashlib
-from os.path import dirname, basename, abspath
-from typing import Tuple, Dict, Any, List, Callable, Union, Optional, Sequence
-
-import ase
-import ase.io
+import math
+from typing import Tuple, Dict, Any, List, Callable, Union, Optional
 
 import torch
-import torch.multiprocessing as mp
 
 from torch_runstats.scatter import scatter_std, scatter_mean
 
 from nequip.utils.torch_geometric import Batch, Dataset
 from nequip.utils.torch_geometric.utils import download_url, extract_zip
 
 import nequip
@@ -27,30 +21,29 @@
     _NODE_FIELDS,
     _EDGE_FIELDS,
     _GRAPH_FIELDS,
 )
 from nequip.utils.batch_ops import bincount
 from nequip.utils.regressor import solver
 from nequip.utils.savenload import atomic_write
-from nequip.utils.multiprocessing import num_tasks
-from .transforms import TypeMapper
-from .AtomicData import _process_dict
+from ..transforms import TypeMapper
 
 
 class AtomicDataset(Dataset):
     """The base class for all NequIP datasets."""
 
-    fixed_fields: Dict[str, Any]
     root: str
+    dtype: torch.dtype
 
     def __init__(
         self,
         root: str,
         type_mapper: Optional[TypeMapper] = None,
     ):
+        self.dtype = torch.get_default_dtype()
         super().__init__(root=root, transform=type_mapper)
 
     def statistics(
         self,
         fields: List[Union[str, Callable]],
         modes: List[str],
         stride: int = 1,
@@ -76,15 +69,15 @@
         }
         params = {
             k: getattr(self, k)
             for k in pnames
             if k not in IGNORE_KEYS and hasattr(self, k)
         }
         # Add other relevant metadata:
-        params["dtype"] = str(torch.get_default_dtype())
+        params["dtype"] = str(self.dtype)
         params["nequip_version"] = nequip.__version__
         return params
 
     @property
     def processed_dir(self) -> str:
         # We want the file name to change when the parameters change
         # So, first we get all parameters:
@@ -113,46 +106,39 @@
     Subclasses may implement:
      - ``download()`` or ``self.url`` or ``ClassName.URL``
 
     Args:
         root (str, optional): Root directory where the dataset should be saved. Defaults to current working directory.
         file_name (str, optional): file name of data source. only used in children class
         url (str, optional): url to download data source
-        force_fixed_keys (list, optional): keys to move from AtomicData to fixed_fields dictionary
-        extra_fixed_fields (dict, optional): extra key that are not stored in data but needed for AtomicData initialization
+        AtomicData_options (dict, optional): extra key that are not stored in data but needed for AtomicData initialization
         include_frames (list, optional): the frames to process with the constructor.
         type_mapper (TypeMapper): the transformation to map atomic information to species index. Optional
     """
 
     def __init__(
         self,
         root: str,
         file_name: Optional[str] = None,
         url: Optional[str] = None,
-        force_fixed_keys: List[str] = [],
-        extra_fixed_fields: Dict[str, Any] = {},
+        AtomicData_options: Dict[str, Any] = {},
         include_frames: Optional[List[int]] = None,
         type_mapper: Optional[TypeMapper] = None,
     ):
         # TO DO, this may be simplified
         # See if a subclass defines some inputs
         self.file_name = (
             getattr(type(self), "FILE_NAME", None) if file_name is None else file_name
         )
-        force_fixed_keys = set(force_fixed_keys).union(
-            getattr(type(self), "FORCE_FIXED_KEYS", [])
-        )
         self.url = getattr(type(self), "URL", url)
 
-        self.force_fixed_keys = force_fixed_keys
-        self.extra_fixed_fields = extra_fixed_fields
+        self.AtomicData_options = AtomicData_options
         self.include_frames = include_frames
 
         self.data = None
-        self.fixed_fields = None
 
         # !!! don't delete this block.
         # otherwise the inherent children class
         # will ignore the download function here
         class_type = type(self)
         if class_type != AtomicInMemoryDataset:
             if "download" not in self.__class__.__dict__:
@@ -161,17 +147,15 @@
                 class_type.process = AtomicInMemoryDataset.process
 
         # Initialize the InMemoryDataset, which runs download and process
         # See https://pytorch-geometric.readthedocs.io/en/latest/notes/create_dataset.html#creating-in-memory-datasets
         # Then pre-process the data if disk files are not found
         super().__init__(root=root, type_mapper=type_mapper)
         if self.data is None:
-            self.data, self.fixed_fields, include_frames = torch.load(
-                self.processed_paths[0]
-            )
+            self.data, include_frames = torch.load(self.processed_paths[0])
             if not np.all(include_frames == self.include_frames):
                 raise ValueError(
                     f"the include_frames is changed. "
                     f"please delete the processed folder and rerun {self.processed_paths[0]}"
                 )
 
     def len(self):
@@ -191,19 +175,17 @@
         self,
     ) -> Union[Tuple[Dict[str, Any], Dict[str, Any]], List[AtomicData]]:
         """Get the data --- called from ``process()``, can assume that ``raw_file_names()`` exist.
 
         Note that parameters for graph construction such as ``pbc`` and ``r_max`` should be included here as (likely, but not necessarily, fixed) fields.
 
         Returns:
-        A two-tuple of:
+        A dict:
             fields: dict
                 mapping a field name ('pos', 'cell') to a list-like sequence of tensor-like objects giving that field's value for each example.
-            fixed_fields: dict
-                mapping field names to their constant values for every example in the dataset.
         Or:
             data_list: List[AtomicData]
         """
         raise NotImplementedError
 
     def download(self):
         if (not hasattr(self, "url")) or (self.url is None):
@@ -212,93 +194,78 @@
         else:
             download_path = download_url(self.url, self.raw_dir)
             if download_path.endswith(".zip"):
                 extract_zip(download_path, self.raw_dir)
 
     def process(self):
         data = self.get_data()
-        if len(data) == 1:
+        if isinstance(data, list):
 
             # It's a data list
-            data_list = data[0]
-            if not (self.include_frames is None or data[0] is None):
+            data_list = data
+            if not (self.include_frames is None or data_list is None):
                 data_list = [data_list[i] for i in self.include_frames]
             assert all(isinstance(e, AtomicData) for e in data_list)
             assert all(AtomicDataDict.BATCH_KEY not in e for e in data_list)
 
-            fields, fixed_fields = {}, {}
-
-            # take the force_fixed_keys away from the fields
-            for key in self.force_fixed_keys:
-                if key in data_list[0]:
-                    fixed_fields[key] = data_list[0][key]
-
-            fixed_fields.update(self.extra_fixed_fields)
+            fields = {}
 
-        elif len(data) == 2:
-
-            # It's fields and fixed_fields
+        elif isinstance(data, dict):
+            # It's fields
             # Get our data
-            fields, fixed_fields = data
-
-            fixed_fields.update(self.extra_fixed_fields)
+            fields = data
 
             # check keys
-            all_keys = set(fields.keys()).union(fixed_fields.keys())
-            assert len(all_keys) == len(fields) + len(
-                fixed_fields
-            ), "No overlap in keys between data and fixed fields allowed!"
+            all_keys = set(fields.keys())
             assert AtomicDataDict.BATCH_KEY not in all_keys
             # Check bad key combinations, but don't require that this be a graph yet.
             AtomicDataDict.validate_keys(all_keys, graph_required=False)
 
-            # take the force_fixed_keys away from the fields
-            for key in self.force_fixed_keys:
-                if key in fields:
-                    fixed_fields[key] = fields.pop(key)[0]
-
-            # check dimesionality
+            # check dimensionality
             num_examples = set([len(a) for a in fields.values()])
             if not len(num_examples) == 1:
+                shape_dict = {f: v.shape for f, v in fields.items()}
                 raise ValueError(
-                    f"This dataset is invalid: expected all fields to have same length (same number of examples), but they had shapes { {f: v.shape for f, v in fields.items() } }"
+                    f"This dataset is invalid: expected all fields to have same length (same number of examples), but they had shapes {shape_dict}"
                 )
             num_examples = next(iter(num_examples))
 
             include_frames = self.include_frames
             if include_frames is None:
                 include_frames = range(num_examples)
 
             # Make AtomicData from it:
             if AtomicDataDict.EDGE_INDEX_KEY in all_keys:
                 # This is already a graph, just build it
                 constructor = AtomicData
             else:
                 # do neighborlist from points
                 constructor = AtomicData.from_points
-                assert "r_max" in all_keys
+                assert "r_max" in self.AtomicData_options
                 assert AtomicDataDict.POSITIONS_KEY in all_keys
 
             data_list = [
-                constructor(**{**{f: v[i] for f, v in fields.items()}, **fixed_fields})
+                constructor(
+                    **{
+                        **{f: v[i] for f, v in fields.items()},
+                        **self.AtomicData_options,
+                    }
+                )
                 for i in include_frames
             ]
 
         else:
             raise ValueError("Invalid return from `self.get_data()`")
 
         # Batch it for efficient saving
         # This limits an AtomicInMemoryDataset to a maximum of LONG_MAX atoms _overall_, but that is a very big number and any dataset that large is probably not "InMemory" anyway
-        data = Batch.from_data_list(data_list, exclude_keys=fixed_fields.keys())
+        data = Batch.from_data_list(data_list)
         del data_list
         del fields
 
-        # type conversion
-        _process_dict(fixed_fields, ignore_fields=["r_max"])
-
         total_MBs = sum(item.numel() * item.element_size() for _, item in data) / (
             1024 * 1024
         )
         logging.info(
             f"Loaded data: {data}\n    processed data size: ~{total_MBs:.2f} MB"
         )
         del total_MBs
@@ -306,29 +273,53 @@
         # use atomic writes to avoid race conditions between
         # different trainings that use the same dataset
         # since those separate trainings should all produce the same results,
         # it doesn't matter if they overwrite each others cached'
         # datasets. It only matters that they don't simultaneously try
         # to write the _same_ file, corrupting it.
         with atomic_write(self.processed_paths[0], binary=True) as f:
-            torch.save((data, fixed_fields, self.include_frames), f)
+            torch.save((data, self.include_frames), f)
         with atomic_write(self.processed_paths[1], binary=False) as f:
             yaml.dump(self._get_parameters(), f)
 
         logging.info("Cached processed data to disk")
 
         self.data = data
-        self.fixed_fields = fixed_fields
 
     def get(self, idx):
-        out = self.data.get_example(idx)
-        # Add back fixed fields
-        for f, v in self.fixed_fields.items():
-            out[f] = v
-        return out
+        return self.data.get_example(idx)
+
+    def _selectors(
+        self,
+        stride: int = 1,
+    ):
+        if self._indices is not None:
+            graph_selector = torch.as_tensor(self._indices)[::stride]
+            # note that self._indices is _not_ necessarily in order,
+            # while self.data --- which we take our arrays from ---
+            # is always in the original order.
+            # In particular, the values of `self.data.batch`
+            # are indexes in the ORIGINAL order
+            # thus we need graph level properties to also be in the original order
+            # so that batch values index into them correctly
+            # since self.data.batch is always sorted & contiguous
+            # (because of Batch.from_data_list)
+            # we sort it:
+            graph_selector, _ = torch.sort(graph_selector)
+        else:
+            graph_selector = torch.arange(0, self.len(), stride)
+
+        node_selector = torch.as_tensor(
+            np.in1d(self.data.batch.numpy(), graph_selector.numpy())
+        )
+
+        edge_index = self.data[AtomicDataDict.EDGE_INDEX_KEY]
+        edge_selector = node_selector[edge_index[0]] & node_selector[edge_index[1]]
+
+        return (graph_selector, node_selector, edge_selector)
 
     def statistics(
         self,
         fields: List[Union[str, Callable]],
         modes: List[str],
         stride: int = 1,
         unbiased: bool = True,
@@ -370,99 +361,68 @@
         """
 
         # Short circut:
         assert len(modes) == len(fields)
         if len(fields) == 0:
             return []
 
-        if self._indices is not None:
-            graph_selector = torch.as_tensor(self._indices)[::stride]
-            # note that self._indices is _not_ necessarily in order,
-            # while self.data --- which we take our arrays from ---
-            # is always in the original order.
-            # In particular, the values of `self.data.batch`
-            # are indexes in the ORIGINAL order
-            # thus we need graph level properties to also be in the original order
-            # so that batch values index into them correctly
-            # since self.data.batch is always sorted & contiguous
-            # (because of Batch.from_data_list)
-            # we sort it:
-            graph_selector, _ = torch.sort(graph_selector)
-        else:
-            graph_selector = torch.arange(0, self.len(), stride)
-        num_graphs = len(graph_selector)
+        graph_selector, node_selector, edge_selector = self._selectors(stride=stride)
 
-        node_selector = torch.as_tensor(
-            np.in1d(self.data.batch.numpy(), graph_selector.numpy())
-        )
+        num_graphs = len(graph_selector)
         num_nodes = node_selector.sum()
-
-        edge_index = self.data[AtomicDataDict.EDGE_INDEX_KEY]
-        edge_selector = node_selector[edge_index[0]] & node_selector[edge_index[1]]
         num_edges = edge_selector.sum()
-        del edge_index
 
         if self.transform is not None:
-            # pre-transform the fixed fields and data so that statistics process transformed data
-            ff_transformed = self.transform(self.fixed_fields, types_required=False)
+            # pre-transform the data so that statistics process transformed data
             data_transformed = self.transform(self.data.to_dict(), types_required=False)
         else:
-            ff_transformed = self.fixed_fields
             data_transformed = self.data.to_dict()
         # pre-select arrays
         # this ensures that all following computations use the right data
         all_keys = set()
         selectors = {}
-        for k in list(ff_transformed.keys()) + list(data_transformed.keys()):
+        for k in data_transformed.keys():
             all_keys.add(k)
             if k in _NODE_FIELDS:
                 selectors[k] = node_selector
             elif k in _GRAPH_FIELDS:
                 selectors[k] = graph_selector
             elif k == AtomicDataDict.EDGE_INDEX_KEY:
                 selectors[k] = (slice(None, None, None), edge_selector)
             elif k in _EDGE_FIELDS:
                 selectors[k] = edge_selector
         # TODO: do the batch indexes, edge_indexes, etc. after selection need to be
         # "compacted" to subtract out their offsets? For now, we just punt this
         # onto the writer of the callable field.
-        # do not actually select on fixed fields, since they are constant
-        # but still only select fields that are correctly registered
-        ff_transformed = {k: v for k, v in ff_transformed.items() if k in selectors}
         # apply selector to actual data
         data_transformed = {
             k: data_transformed[k][selectors[k]]
             for k in data_transformed.keys()
             if k in selectors
         }
 
         atom_types: Optional[torch.Tensor] = None
         out: list = []
         for ifield, field in enumerate(fields):
             if callable(field):
                 # make a joined thing? so it includes fixed fields
                 arr, arr_is_per = field(data_transformed)
-                arr = arr.to(
-                    torch.get_default_dtype()
-                )  # all statistics must be on floating
+                arr = arr.to(self.dtype)  # all statistics must be on floating
                 assert arr_is_per in ("node", "graph", "edge")
             else:
                 if field not in all_keys:
                     raise RuntimeError(
                         f"The field key `{field}` is not present in this dataset"
                     )
                 if field not in selectors:
                     # this means field is not selected and so not available
                     raise RuntimeError(
                         f"Only per-node and per-graph fields can have statistics computed; `{field}` has not been registered as either. If it is per-node or per-graph, please register it as such using `nequip.data.register_fields`"
                     )
-                if field in ff_transformed:
-                    arr = ff_transformed[field]
-                else:
-                    arr = data_transformed[field]
+                arr = data_transformed[field]
                 if field in _NODE_FIELDS:
                     arr_is_per = "node"
                 elif field in _GRAPH_FIELDS:
                     arr_is_per = "graph"
                 elif field in _EDGE_FIELDS:
                     arr_is_per = "edge"
                 else:
@@ -471,15 +431,15 @@
             # Check arr
             if arr is None:
                 raise ValueError(
                     f"Cannot compute statistics over field `{field}` whose value is None!"
                 )
             if not isinstance(arr, torch.Tensor):
                 if np.issubdtype(arr.dtype, np.floating):
-                    arr = torch.as_tensor(arr, dtype=torch.get_default_dtype())
+                    arr = torch.as_tensor(arr, dtype=self.dtype)
                 else:
                     arr = torch.as_tensor(arr)
             if arr_is_per == "node":
                 arr = arr.view(num_nodes, -1)
             elif arr_is_per == "graph":
                 arr = arr.view(num_graphs, -1)
             elif arr_is_per == "edge":
@@ -495,34 +455,33 @@
                 out.append((uniq, counts))
             elif ana_mode == "rms":
                 # root-mean-square
                 out.append((torch.sqrt(torch.mean(arr * arr)),))
 
             elif ana_mode == "mean_std":
                 # mean and std
+                if len(arr) < 2:
+                    raise ValueError(
+                        "Can't do per species standard deviation without at least two samples"
+                    )
                 mean = torch.mean(arr, dim=0)
                 std = torch.std(arr, dim=0, unbiased=unbiased)
                 out.append((mean, std))
 
+            elif ana_mode == "absmax":
+                out.append((arr.abs().max(),))
+
             elif ana_mode.startswith("per_species_"):
                 # per-species
                 algorithm_kwargs = kwargs.pop(field + ana_mode, {})
 
                 ana_mode = ana_mode[len("per_species_") :]
 
                 if atom_types is None:
-                    if AtomicDataDict.ATOM_TYPE_KEY in data_transformed:
-                        atom_types = data_transformed[AtomicDataDict.ATOM_TYPE_KEY]
-                    elif AtomicDataDict.ATOM_TYPE_KEY in ff_transformed:
-                        atom_types = ff_transformed[AtomicDataDict.ATOM_TYPE_KEY]
-                        atom_types = (
-                            atom_types.unsqueeze(0)
-                            .expand((num_graphs,) + atom_types.shape)
-                            .reshape(-1)
-                        )
+                    atom_types = data_transformed[AtomicDataDict.ATOM_TYPE_KEY]
 
                 results = self._per_species_statistics(
                     ana_mode,
                     arr,
                     arr_is_per=arr_is_per,
                     batch=data_transformed[AtomicDataDict.BATCH_KEY],
                     atom_types=atom_types,
@@ -569,26 +528,32 @@
         assert N.ndim == 2
         assert N.shape == (len(arr), 1)
         assert arr.ndim >= 2
         data_dim = arr.shape[1:]
         arr = arr / N
         assert arr.shape == (len(N),) + data_dim
         if ana_mode == "mean_std":
+            if len(arr) < 2:
+                raise ValueError(
+                    "Can't do standard deviation without at least two samples"
+                )
             mean = torch.mean(arr, dim=0)
             std = torch.std(arr, unbiased=unbiased, dim=0)
             return mean, std
         elif ana_mode == "rms":
             return (torch.sqrt(torch.mean(arr.square())),)
+        elif ana_mode == "absmax":
+            return (torch.max(arr.abs()),)
         else:
             raise NotImplementedError(
                 f"{ana_mode} for per-atom analysis is not implemented"
             )
 
-    @staticmethod
     def _per_species_statistics(
+        self,
         ana_mode: str,
         arr: torch.Tensor,
         arr_is_per: str,
         atom_types: torch.Tensor,
         batch: torch.Tensor,
         unbiased: bool = True,
         algorithm_kwargs: Optional[dict] = {},
@@ -606,370 +571,94 @@
         if arr_is_per == "graph":
 
             if ana_mode != "mean_std":
                 raise NotImplementedError(
                     f"{ana_mode} for per species analysis is not implemented for shape {arr.shape}"
                 )
 
-            N = N.type(torch.get_default_dtype())
+            N = N.type(self.dtype)
 
             return solver(N, arr, **algorithm_kwargs)
 
         elif arr_is_per == "node":
-            arr = arr.type(torch.get_default_dtype())
+            arr = arr.type(self.dtype)
 
             if ana_mode == "mean_std":
+                # There need to be at least two occurances of each atom type in the
+                # WHOLE dataset, not in any given frame:
+                if torch.any(N.sum(dim=0) < 2):
+                    raise ValueError(
+                        "Can't do per species standard deviation without at least two samples per species"
+                    )
                 mean = scatter_mean(arr, atom_types, dim=0)
                 assert mean.shape[1:] == arr.shape[1:]  # [N, dims] -> [type, dims]
                 assert len(mean) == N.shape[1]
                 std = scatter_std(arr, atom_types, dim=0, unbiased=unbiased)
                 assert std.shape == mean.shape
                 return mean, std
             elif ana_mode == "rms":
                 square = scatter_mean(arr.square(), atom_types, dim=0)
                 assert square.shape[1:] == arr.shape[1:]  # [N, dims] -> [type, dims]
                 assert len(square) == N.shape[1]
                 dims = len(square.shape) - 1
                 for i in range(dims):
                     square = square.mean(axis=-1)
                 return (torch.sqrt(square),)
+            else:
+                raise NotImplementedError(
+                    f"Statistics mode {ana_mode} isn't yet implemented for per_species_"
+                )
 
         else:
             raise NotImplementedError
 
+    def rdf(
+        self, bin_width: float, stride: int = 1
+    ) -> Dict[Tuple[int, int], Tuple[np.ndarray, np.ndarray]]:
+        """Compute the pairwise RDFs of the dataset.
 
-class NpzDataset(AtomicInMemoryDataset):
-    """Load data from an npz file.
+        Args:
+            bin_width: width of the histogram bin in distance units
+            stride: stride of data to include
 
-    To avoid loading unneeded data, keys are ignored by default unless they are in ``key_mapping``, ``include_keys``,
-    ``npz_fixed_fields_keys`` or ``extra_fixed_fields``.
+        Returns:
+            dictionary mapping `(type1, type2)` to tuples of `(hist, bin_edges)` in the style of `np.histogram`.
+        """
+        graph_selector, node_selector, edge_selector = self._selectors(stride=stride)
 
-    Args:
-        key_mapping (Dict[str, str]): mapping of npz keys to ``AtomicData`` keys. Optional
-        include_keys (list): the attributes to be processed and stored. Optional
-        npz_fixed_field_keys: the attributes that only have one instance but apply to all frames. Optional
-            Note that the mapped keys (as determined by the _values_ in ``key_mapping``) should be used in
-            ``npz_fixed_field_keys``, not the original npz keys from before mapping. If an npz key is not
-            present in ``key_mapping``, it is mapped to itself, and this point is not relevant.
-
-    Example: Given a npz file with 10 configurations, each with 14 atoms.
-
-        position: (10, 14, 3)
-        force: (10, 14, 3)
-        energy: (10,)
-        Z: (14)
-        user_label1: (10)        # per config
-        user_label2: (10, 14, 3) # per atom
-
-    The input yaml should be
-
-    ```yaml
-    dataset: npz
-    dataset_file_name: example.npz
-    include_keys:
-      - user_label1
-      - user_label2
-    npz_fixed_field_keys:
-      - cell
-      - atomic_numbers
-    key_mapping:
-      position: pos
-      force: forces
-      energy: total_energy
-      Z: atomic_numbers
-    ```
+        data = AtomicData.to_AtomicDataDict(self.data)
+        data = AtomicDataDict.with_edge_vectors(data, with_lengths=True)
 
-    """
+        results = {}
 
-    def __init__(
-        self,
-        root: str,
-        key_mapping: Dict[str, str] = {
-            "positions": AtomicDataDict.POSITIONS_KEY,
-            "energy": AtomicDataDict.TOTAL_ENERGY_KEY,
-            "force": AtomicDataDict.FORCE_KEY,
-            "forces": AtomicDataDict.FORCE_KEY,
-            "Z": AtomicDataDict.ATOMIC_NUMBERS_KEY,
-            "atomic_number": AtomicDataDict.ATOMIC_NUMBERS_KEY,
-        },
-        include_keys: List[str] = [],
-        npz_fixed_field_keys: List[str] = [],
-        file_name: Optional[str] = None,
-        url: Optional[str] = None,
-        force_fixed_keys: List[str] = [],
-        extra_fixed_fields: Dict[str, Any] = {},
-        include_frames: Optional[List[int]] = None,
-        type_mapper: TypeMapper = None,
-    ):
-        self.key_mapping = key_mapping
-        self.npz_fixed_field_keys = npz_fixed_field_keys
-        self.include_keys = include_keys
-
-        super().__init__(
-            file_name=file_name,
-            url=url,
-            root=root,
-            force_fixed_keys=force_fixed_keys,
-            extra_fixed_fields=extra_fixed_fields,
-            include_frames=include_frames,
-            type_mapper=type_mapper,
-        )
-
-    @property
-    def raw_file_names(self):
-        return [basename(self.file_name)]
+        types = self.type_mapper(data)[AtomicDataDict.ATOM_TYPE_KEY]
 
-    @property
-    def raw_dir(self):
-        return dirname(abspath(self.file_name))
-
-    def get_data(self):
+        edge_types = torch.index_select(
+            types, 0, data[AtomicDataDict.EDGE_INDEX_KEY].reshape(-1)
+        ).view(2, -1)
+        types_center = edge_types[0].numpy()
+        types_neigh = edge_types[1].numpy()
 
-        data = np.load(self.raw_dir + "/" + self.raw_file_names[0], allow_pickle=True)
+        r_max: float = self.AtomicData_options["r_max"]
+        # + 1 to always have a zero bin at the end
+        n_bins: int = int(math.ceil(r_max / bin_width)) + 1
+        # +1 since these are bin_edges including rightmost
+        bins = bin_width * np.arange(n_bins + 1)
 
-        # only the keys explicitly mentioned in the yaml file will be parsed
-        keys = set(list(self.key_mapping.keys()))
-        keys.update(self.npz_fixed_field_keys)
-        keys.update(self.include_keys)
-        keys.update(list(self.extra_fixed_fields.keys()))
-        keys = keys.intersection(set(list(data.keys())))
-
-        mapped = {self.key_mapping.get(k, k): data[k] for k in keys}
-
-        # TODO: generalize this?
-        for intkey in (
-            AtomicDataDict.ATOMIC_NUMBERS_KEY,
-            AtomicDataDict.ATOM_TYPE_KEY,
-            AtomicDataDict.EDGE_INDEX_KEY,
+        for type1, type2 in itertools.combinations_with_replacement(
+            range(self.type_mapper.num_types), 2
         ):
-            if intkey in mapped:
-                mapped[intkey] = mapped[intkey].astype(np.int64)
-
-        fields = {k: v for k, v in mapped.items() if k not in self.npz_fixed_field_keys}
-        # note that we don't deal with extra_fixed_fields here; AtomicInMemoryDataset does that.
-        fixed_fields = {
-            k: v for k, v in mapped.items() if k in self.npz_fixed_field_keys
-        }
-        return fields, fixed_fields
-
-
-def _ase_dataset_reader(
-    rank: int,
-    world_size: int,
-    tmpdir: str,
-    ase_kwargs: dict,
-    atomicdata_kwargs: dict,
-    include_frames,
-    global_options: dict,
-) -> Union[str, List[AtomicData]]:
-    """Parallel reader for all frames in file."""
-    if world_size > 1:
-        from nequip.utils._global_options import _set_global_options
-
-        # ^ avoid import loop
-        # we only `multiprocessing` if world_size > 1
-        _set_global_options(global_options)
-    # interleave--- in theory it is better for performance for the ranks
-    # to read consecutive blocks, but the way ASE is written the whole
-    # file gets streamed through all ranks anyway, so just trust the OS
-    # to cache things sanely, which it will.
-    # ASE handles correctly the case where there are no frames in index
-    # and just gives an empty list, so that will succeed:
-    index = slice(rank, None, world_size)
-    if include_frames is None:
-        # count includes 0, 1, ..., inf
-        include_frames = itertools.count()
-
-    datas = []
-    # stream them from ase too using iread
-    for i, atoms in enumerate(ase.io.iread(**ase_kwargs, index=index, parallel=False)):
-        global_index = rank + (world_size * i)
-        datas.append(
-            (
-                global_index,
-                AtomicData.from_ase(atoms=atoms, **atomicdata_kwargs)
-                if global_index in include_frames
-                # in-memory dataset will ignore this later, but needed for indexing to work out
-                else None,
+            # Try to do as much of this as possible in-place
+            mask = types_center == type1
+            np.logical_and(mask, types_neigh == type2, out=mask)
+            np.logical_and(mask, edge_selector, out=mask)
+            mask = mask.astype(np.int32)
+            results[(type1, type2)] = np.histogram(
+                data[AtomicDataDict.EDGE_LENGTH_KEY],
+                weights=mask,
+                bins=bins,
+                density=True,
             )
-        )
-    # Save to a tempfile---
-    # there can be a _lot_ of tensors here, and rather than dealing with
-    # the complications of running out of file descriptors and setting
-    # sharing methods, since this is a one time thing, just make it simple
-    # and avoid shared memory entirely.
-    if world_size > 1:
-        path = f"{tmpdir}/rank{rank}.pth"
-        torch.save(datas, path)
-        return path
-    else:
-        return datas
-
+            # RDF is symmetric
+            results[(type2, type1)] = results[(type1, type2)]
 
-class ASEDataset(AtomicInMemoryDataset):
-    """
-
-    Args:
-        ase_args (dict): arguments for ase.io.read
-        include_keys (list): in addition to forces and energy, the keys that needs to
-             be parsed into dataset
-             The data stored in ase.atoms.Atoms.array has the lowest priority,
-             and it will be overrided by data in ase.atoms.Atoms.info
-             and ase.atoms.Atoms.calc.results. Optional
-        key_mapping (dict): rename some of the keys to the value str. Optional
-
-    Example: Given an atomic data stored in "H2.extxyz" that looks like below:
-
-    ```H2.extxyz
-    2
-    Properties=species:S:1:pos:R:3 energy=-10 user_label=2.0 pbc="F F F"
-     H       0.00000000       0.00000000       0.00000000
-     H       0.00000000       0.00000000       1.02000000
-    ```
-
-    The yaml input should be
-
-    ```
-    dataset: ase
-    dataset_file_name: H2.extxyz
-    ase_args:
-      format: extxyz
-    include_keys:
-      - user_label
-    key_mapping:
-      user_label: label0
-    chemical_symbols:
-      - H
-    ```
-
-    for VASP parser, the yaml input should be
-    ```
-    dataset: ase
-    dataset_file_name: OUTCAR
-    ase_args:
-      format: vasp-out
-    key_mapping:
-      free_energy: total_energy
-    chemical_symbols:
-      - H
-    ```
-
-    """
-
-    def __init__(
-        self,
-        root: str,
-        ase_args: dict = {},
-        file_name: Optional[str] = None,
-        url: Optional[str] = None,
-        force_fixed_keys: List[str] = [],
-        extra_fixed_fields: Dict[str, Any] = {},
-        include_frames: Optional[List[int]] = None,
-        type_mapper: TypeMapper = None,
-        key_mapping: Optional[dict] = None,
-        include_keys: Optional[List[str]] = None,
-    ):
-        self.ase_args = {}
-        self.ase_args.update(getattr(type(self), "ASE_ARGS", dict()))
-        self.ase_args.update(ase_args)
-        assert "index" not in self.ase_args
-        assert "filename" not in self.ase_args
-
-        self.include_keys = include_keys
-        self.key_mapping = key_mapping
-
-        super().__init__(
-            file_name=file_name,
-            url=url,
-            root=root,
-            force_fixed_keys=force_fixed_keys,
-            extra_fixed_fields=extra_fixed_fields,
-            include_frames=include_frames,
-            type_mapper=type_mapper,
-        )
-
-    @classmethod
-    def from_atoms_list(cls, atoms: Sequence[ase.Atoms], **kwargs):
-        """Make an ``ASEDataset`` from a list of ``ase.Atoms`` objects.
-
-        If `root` is not provided, a temporary directory will be used.
-
-        Please note that this is a convinience method that does NOT avoid a round-trip to disk; the provided ``atoms`` will be written out to a file.
-
-        Ignores ``kwargs["file_name"]`` if it is provided.
-
-        Args:
-            atoms
-            **kwargs: passed through to the constructor
-        Returns:
-            The constructed ``ASEDataset``.
-        """
-        if "root" not in kwargs:
-            tmpdir = tempfile.TemporaryDirectory()
-            kwargs["root"] = tmpdir.name
-        else:
-            tmpdir = None
-        kwargs["file_name"] = tmpdir.name + "/atoms.xyz"
-        atoms = list(atoms)
-        # Write them out
-        ase.io.write(kwargs["file_name"], atoms, format="extxyz")
-        # Read them in
-        obj = cls(**kwargs)
-        if tmpdir is not None:
-            # Make it keep a reference to the tmpdir to keep it alive
-            # When the dataset is garbage collected, the tmpdir will
-            # be too, and will (hopefully) get deleted eventually.
-            # Or at least by end of program...
-            obj._tmpdir_ref = tmpdir
-        return obj
-
-    @property
-    def raw_file_names(self):
-        return [basename(self.file_name)]
-
-    @property
-    def raw_dir(self):
-        return dirname(abspath(self.file_name))
-
-    def get_data(self):
-        ase_args = {"filename": self.raw_dir + "/" + self.raw_file_names[0]}
-        ase_args.update(self.ase_args)
-
-        # skip the None arguments
-        kwargs = dict(
-            include_keys=self.include_keys,
-            key_mapping=self.key_mapping,
-        )
-        kwargs = {k: v for k, v in kwargs.items() if v is not None}
-        kwargs.update(self.extra_fixed_fields)
-        n_proc = num_tasks()
-        with tempfile.TemporaryDirectory() as tmpdir:
-            from nequip.utils._global_options import _get_latest_global_options
-
-            # ^ avoid import loop
-            reader = functools.partial(
-                _ase_dataset_reader,
-                world_size=n_proc,
-                tmpdir=tmpdir,
-                ase_kwargs=ase_args,
-                atomicdata_kwargs=kwargs,
-                include_frames=self.include_frames,
-                # get the global options of the parent to initialize the worker correctly
-                global_options=_get_latest_global_options(),
-            )
-            if n_proc > 1:
-                # things hang for some obscure OpenMP reason on some systems when using `fork` method
-                ctx = mp.get_context("forkserver")
-                with ctx.Pool(processes=n_proc) as p:
-                    # map it over the `rank` argument
-                    datas = p.map(reader, list(range(n_proc)))
-                # clean up the pool before loading the data
-                datas = [torch.load(d) for d in datas]
-                datas = sum(datas, [])
-                # un-interleave the datas
-                datas = sorted(datas, key=lambda e: e[0])
-            else:
-                datas = reader(rank=0)
-                # datas here is already in order, stride 1 start 0
-                # no need to un-interleave
-        # return list of AtomicData:
-        return ([e[1] for e in datas],)
+        return results
```

### Comparing `nequip-0.5.6/nequip/data/transforms.py` & `nequip-0.6.0/nequip/data/transforms.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 
 
 class TypeMapper:
     """Based on a configuration, map atomic numbers to types."""
 
     num_types: int
     chemical_symbol_to_type: Optional[Dict[str, int]]
+    type_to_chemical_symbol: Optional[Dict[int, str]]
     type_names: List[str]
     _min_Z: int
 
     def __init__(
         self,
         type_names: Optional[List[str]] = None,
         chemical_symbol_to_type: Optional[Dict[str, int]] = None,
+        type_to_chemical_symbol: Optional[Dict[int, str]] = None,
         chemical_symbols: Optional[List[str]] = None,
     ):
         if chemical_symbols is not None:
             if chemical_symbol_to_type is not None:
                 raise ValueError(
                     "Cannot provide both `chemical_symbols` and `chemical_symbol_to_type`"
                 )
@@ -33,14 +35,22 @@
             # https://stackoverflow.com/questions/29876580/how-to-sort-a-list-according-to-another-list-python
             chemical_symbols = [
                 e[1] for e in sorted(zip(atomic_nums, chemical_symbols))
             ]
             chemical_symbol_to_type = {k: i for i, k in enumerate(chemical_symbols)}
             del chemical_symbols
 
+        if type_to_chemical_symbol is not None:
+            type_to_chemical_symbol = {
+                int(k): v for k, v in type_to_chemical_symbol.items()
+            }
+            assert all(
+                v in ase.data.chemical_symbols for v in type_to_chemical_symbol.values()
+            )
+
         # Build from chem->type mapping, if provided
         self.chemical_symbol_to_type = chemical_symbol_to_type
         if self.chemical_symbol_to_type is not None:
             # Validate
             for sym, type in self.chemical_symbol_to_type.items():
                 assert sym in ase.data.atomic_numbers, f"Invalid chemical symbol {sym}"
                 assert 0 <= type, f"Invalid type number {type}"
@@ -71,27 +81,38 @@
             self._Z_to_index = Z_to_index
             self._index_to_Z = torch.zeros(
                 size=(len(self.chemical_symbol_to_type),), dtype=torch.long
             )
             for sym, type_idx in self.chemical_symbol_to_type.items():
                 self._index_to_Z[type_idx] = ase.data.atomic_numbers[sym]
             self._valid_set = set(valid_atomic_numbers)
+            true_type_to_chemical_symbol = {
+                type_id: sym for sym, type_id in self.chemical_symbol_to_type.items()
+            }
+            if type_to_chemical_symbol is not None:
+                assert type_to_chemical_symbol == true_type_to_chemical_symbol
+            else:
+                type_to_chemical_symbol = true_type_to_chemical_symbol
+
         # check
         if type_names is None:
             raise ValueError(
                 "None of chemical_symbols, chemical_symbol_to_type, nor type_names was provided; exactly one is required"
             )
         # validate type names
         assert all(
             n.isalnum() for n in type_names
         ), "Type names must contain only alphanumeric characters"
         # Set to however many maps specified -- we already checked contiguous
         self.num_types = len(type_names)
         # Check type_names
         self.type_names = type_names
+        self.type_to_chemical_symbol = type_to_chemical_symbol
+        if self.type_to_chemical_symbol is not None:
+            assert set(type_to_chemical_symbol.keys()) == set(range(self.num_types))
 
     def __call__(
         self, data: Union[AtomicDataDict.Type, AtomicData], types_required: bool = True
     ) -> Union[AtomicDataDict.Type, AtomicData]:
         if AtomicDataDict.ATOM_TYPE_KEY in data:
             if AtomicDataDict.ATOMIC_NUMBERS_KEY in data:
                 warnings.warn(
```

### Comparing `nequip-0.5.6/nequip/model/__init__.py` & `nequip-0.6.0/nequip/model/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ._grads import ForceOutput, PartialForceOutput, StressForceOutput
 from ._scaling import RescaleEnergyEtc, PerSpeciesRescale
 from ._weight_init import (
     uniform_initialize_FCs,
     initialize_from_state,
     load_model_state,
 )
+from ._gmm import GaussianMixtureModelUncertainty
+from ._pair_potential import PairPotential, PairPotentialTerm
 
 from ._build import model_from_config
 
 from . import builder_utils
 
 __all__ = [
     SimpleIrrepsConfig,
@@ -18,10 +20,13 @@
     PartialForceOutput,
     StressForceOutput,
     RescaleEnergyEtc,
     PerSpeciesRescale,
     uniform_initialize_FCs,
     initialize_from_state,
     load_model_state,
+    GaussianMixtureModelUncertainty,
     model_from_config,
+    PairPotential,
+    PairPotentialTerm,
     builder_utils,
 ]
```

### Comparing `nequip-0.5.6/nequip/model/_eng.py` & `nequip-0.6.0/nequip/model/_eng.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/model/_grads.py` & `nequip-0.6.0/nequip/model/_grads.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/model/_scaling.py` & `nequip-0.6.0/nequip/model/_scaling.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,36 +19,34 @@
 ):
     return GlobalRescale(
         model=model,
         config=config,
         dataset=dataset,
         initialize=initialize,
         module_prefix="global_rescale",
-        default_scale=f"dataset_{AtomicDataDict.FORCE_KEY}_rms"
-        if AtomicDataDict.FORCE_KEY in model.irreps_out
-        else f"dataset_{AtomicDataDict.TOTAL_ENERGY_KEY}_std",
+        default_scale=(
+            f"dataset_{AtomicDataDict.FORCE_KEY}_rms"
+            if AtomicDataDict.FORCE_KEY in model.irreps_out
+            else f"dataset_{AtomicDataDict.TOTAL_ENERGY_KEY}_std"
+        ),
         default_shift=None,
         default_scale_keys=AtomicDataDict.ALL_ENERGY_KEYS,
         default_shift_keys=[AtomicDataDict.TOTAL_ENERGY_KEY],
-        default_related_scale_keys=[AtomicDataDict.PER_ATOM_ENERGY_KEY],
-        default_related_shift_keys=[],
     )
 
 
 def GlobalRescale(
     model: GraphModuleMixin,
     config,
     initialize: bool,
     module_prefix: str,
     default_scale: Union[str, float, list],
     default_shift: Union[str, float, list],
     default_scale_keys: list,
     default_shift_keys: list,
-    default_related_scale_keys: list,
-    default_related_shift_keys: list,
     dataset: Optional[AtomicDataset] = None,
 ):
     """Add global rescaling for energy(-based quantities).
 
     If ``initialize`` is false, doesn't compute statistics.
     """
 
@@ -109,73 +107,88 @@
             global_shift = 0.0  # it has some kind of value
         if global_scale is not None:
             global_scale = 1.0  # same,
 
     error_string = "keys need to be a list"
     assert isinstance(default_scale_keys, list), error_string
     assert isinstance(default_shift_keys, list), error_string
-    assert isinstance(default_related_scale_keys, list), error_string
-    assert isinstance(default_related_shift_keys, list), error_string
 
     # == Build the model ==
     return RescaleOutput(
         model=model,
         scale_keys=[k for k in default_scale_keys if k in model.irreps_out],
         scale_by=global_scale,
         shift_keys=[k for k in default_shift_keys if k in model.irreps_out],
         shift_by=global_shift,
-        related_scale_keys=default_related_scale_keys,
-        related_shift_keys=default_related_shift_keys,
         shift_trainable=config.get(f"{module_prefix}_shift_trainable", False),
         scale_trainable=config.get(f"{module_prefix}_scale_trainable", False),
+        default_dtype=config.get("default_dtype", None),
     )
 
 
 def PerSpeciesRescale(
     model: GraphModuleMixin,
     config,
     initialize: bool,
     dataset: Optional[AtomicDataset] = None,
 ):
-    """Add global rescaling for energy(-based quantities).
-
-    If ``initialize`` is false, doesn't compute statistics.
-    """
+    """Add per-atom rescaling (and shifting) for per-atom energies."""
     module_prefix = "per_species_rescale"
 
-    # = Determine energy rescale type =
-    scales = config.get(
-        module_prefix + "_scales",
-        f"dataset_{AtomicDataDict.FORCE_KEY}_rms"
-        # if `train_on_keys` isn't provided, assume conservatively
-        # that we aren't "training" on anything (i.e. take the
-        # most general defaults)
-        if AtomicDataDict.FORCE_KEY in config.get("train_on_keys", [])
-        else f"dataset_per_atom_{AtomicDataDict.TOTAL_ENERGY_KEY}_std",
-    )
-    shifts = config.get(
-        module_prefix + "_shifts",
-        f"dataset_per_atom_{AtomicDataDict.TOTAL_ENERGY_KEY}_mean",
-    )
-
     # Check for common double shift mistake with defaults
     if "RescaleEnergyEtc" in config.get("model_builders", []):
         # if the defaults are enabled, then we will get bad double shift
         # THIS CHECK IS ONLY GOOD ENOUGH FOR EMITTING WARNINGS
         has_global_shift = config.get("global_rescale_shift", None) is not None
         if has_global_shift:
-            if shifts is not None:
+            if config.get(module_prefix + "_shifts", True) is not None:
                 # using default of per_atom shift
                 raise RuntimeError(
                     "A global_rescale_shift was provided, but the default per-atom energy shift was not disabled."
                 )
         del has_global_shift
 
-    # = Determine what statistics need to be compute =\
-    arguments_in_dataset_units = None
+    return _PerSpeciesRescale(
+        scales_default=None,
+        shifts_default=f"dataset_per_atom_{AtomicDataDict.TOTAL_ENERGY_KEY}_mean",
+        field=AtomicDataDict.PER_ATOM_ENERGY_KEY,
+        out_field=AtomicDataDict.PER_ATOM_ENERGY_KEY,
+        module_prefix=module_prefix,
+        insert_before="total_energy_sum",
+        model=model,
+        config=config,
+        initialize=initialize,
+        dataset=dataset,
+    )
+
+
+def _PerSpeciesRescale(
+    scales_default,
+    shifts_default,
+    field: str,
+    out_field: str,
+    module_prefix: str,
+    insert_before: str,
+    model: GraphModuleMixin,
+    config,
+    initialize: bool,
+    dataset: Optional[AtomicDataset] = None,
+):
+    """Add per-atom rescaling (and shifting) for a field
+
+    If ``initialize`` is false, doesn't compute statistics.
+    """
+    scales = config.get(module_prefix + "_scales", scales_default)
+    shifts = config.get(module_prefix + "_shifts", shifts_default)
+
+    # = Determine what statistics need to be compute =
+    assert config.get(
+        module_prefix + "_arguments_in_dataset_units", True
+    ), f"The PerSpeciesRescale builder is only compatible with {module_prefix + '_arguments_in_dataset_units'} set to True"
+
     if initialize:
         str_names = []
         for value in [scales, shifts]:
             if isinstance(value, str):
                 str_names += [value]
             elif (
                 value is None
@@ -184,83 +197,70 @@
                 or isinstance(value, torch.Tensor)
             ):
                 # valid values
                 pass
             else:
                 raise ValueError(f"Invalid value `{value}` of type {type(value)}")
 
-        if len(str_names) == 2:
-            # Both computed from dataset
-            arguments_in_dataset_units = True
-        elif len(str_names) == 1:
-            if None in [scales, shifts]:
-                # if the one that isnt str is null, it's just disabled
-                # that has no units
-                # so it's ok to have just one and to be in dataset units
-                arguments_in_dataset_units = True
-            else:
-                assert config[
-                    module_prefix + "_arguments_in_dataset_units"
-                ], "Requested to set either the shifts or scales of the per_species_rescale using dataset values, but chose to provide the other in non-dataset units. Please give the explictly specified shifts/scales in dataset units and set per_species_rescale_arguments_in_dataset_units"
-
         # = Compute shifts and scales =
         if len(str_names) > 0:
             computed_stats = _compute_stats(
                 str_names=str_names,
                 dataset=dataset,
                 stride=config.dataset_statistics_stride,
                 kwargs=config.get(module_prefix + "_kwargs", {}),
             )
 
         if isinstance(scales, str):
             s = scales
-            scales = computed_stats[str_names.index(scales)].squeeze(-1)  # energy is 1D
+            # energy or other property is 1D:
+            scales = computed_stats[str_names.index(scales)].squeeze(-1)
             logging.info(f"Replace string {s} to {scales}")
         elif isinstance(scales, (list, float)):
             scales = torch.as_tensor(scales)
 
         if isinstance(shifts, str):
             s = shifts
-            shifts = computed_stats[str_names.index(shifts)].squeeze(-1)  # energy is 1D
+            # energy or other property is 1D:
+            shifts = computed_stats[str_names.index(shifts)].squeeze(-1)
             logging.info(f"Replace string {s} to {shifts}")
         elif isinstance(shifts, (list, float)):
             shifts = torch.as_tensor(shifts)
 
+        # TODO kind of weird error to check for here
         if scales is not None and torch.min(scales) < RESCALE_THRESHOLD:
             raise ValueError(
-                f"Per species energy scaling was very low: {scales}. Maybe try setting {module_prefix}_scales = 1."
+                f"Per species scaling was very low: {scales}. Maybe try setting {module_prefix}_scales = 1."
             )
 
         logging.info(
             f"Atomic outputs are scaled by: {TypeMapper.format(scales, config.type_names)}, shifted by {TypeMapper.format(shifts, config.type_names)}."
         )
 
     else:
         # Put dummy values
         # the real ones will be loaded from the state dict later
         # note that the state dict includes buffers,
         # so this is fine regardless of whether its trainable.
         scales = 1.0 if scales is not None else None
         shifts = 0.0 if shifts is not None else None
-        # values correctly scaled according to where the come from
-        # will be brought from the state dict later,
-        # so what you set this to doesnt matter:
-        arguments_in_dataset_units = False
+        # values from the previously initialized model
+        # will be brought in from the state dict later,
+        # so these values (and rescaling them) doesn't matter
 
     # insert in per species shift
     params = dict(
-        field=AtomicDataDict.PER_ATOM_ENERGY_KEY,
-        out_field=AtomicDataDict.PER_ATOM_ENERGY_KEY,
+        field=field,
+        out_field=out_field,
         shifts=shifts,
         scales=scales,
+        arguments_in_dataset_units=True,
     )
-
-    params["arguments_in_dataset_units"] = arguments_in_dataset_units
     model.insert_from_parameters(
-        before="total_energy_sum",
+        before=insert_before,
         name=module_prefix,
         shared_params=config,
         builder=PerSpeciesScaleShift,
         params=params,
     )
 
     # == Build the model ==
@@ -284,15 +284,15 @@
     # parse the list of string to field, mode
     # and record which quantity correspond to which computed_item
     stat_modes = []
     stat_fields = []
     stat_strs = []
     ids = []
     tuple_ids = []
-    tuple_id_map = {"mean": 0, "std": 1, "rms": 0}
+    tuple_id_map = {"mean": 0, "std": 1, "rms": 0, "absmax": 0}
     input_kwargs = {}
     for name in str_names:
 
         # remove dataset prefix
         if name.startswith("dataset_"):
             name = name[len("dataset_") :]
         # identify per_species and per_atom modes
@@ -305,17 +305,17 @@
             prefix = "per_atom_"
 
         stat = name.split("_")[-1]
         field = "_".join(name.split("_")[:-1])
         if stat in ["mean", "std"]:
             stat_mode = prefix + "mean_std"
             stat_str = field + prefix + "mean_std"
-        elif stat in ["rms"]:
-            stat_mode = prefix + "rms"
-            stat_str = field + prefix + "rms"
+        elif stat in ["rms", "absmax"]:
+            stat_mode = prefix + stat
+            stat_str = field + prefix + stat
         else:
             raise ValueError(f"Cannot handle {stat} type quantity")
 
         if stat_str in stat_strs:
             ids += [stat_strs.index(stat_str)]
         else:
             ids += [len(stat_strs)]
```

### Comparing `nequip-0.5.6/nequip/model/_weight_init.py` & `nequip-0.6.0/nequip/model/_weight_init.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 import math
+import logging
 
 import torch
 
 import e3nn.o3
 import e3nn.nn
 
-from nequip.nn import GraphModuleMixin
+from nequip.nn import GraphModuleMixin, GraphModel
 from nequip.utils import Config
 
 
 # == Load old state ==
-def initialize_from_state(config: Config, model: GraphModuleMixin, initialize: bool):
+def initialize_from_state(
+    config: Config, graph_model: GraphModel, initialize: bool
+) -> GraphModel:
     """Initialize the model from the state dict file given by the config options `initial_model_state`.
 
     Only loads the state dict if `initialize` is `True`; this is meant for, say, starting a training from a previous state.
 
     If `initial_model_state_strict` controls
     > whether to strictly enforce that the keys in state_dict
     > match the keys returned by this module's state_dict() function
 
     See https://pytorch.org/docs/stable/generated/torch.nn.Module.html?highlight=load_state_dict#torch.nn.Module.load_state_dict.
     """
     if not initialize:
-        return model  # do nothing
+        return graph_model  # do nothing
     return load_model_state(
-        config=config, model=model, initialize=initialize, _prefix="initial_model_state"
+        config=config,
+        graph_model=graph_model,
+        initialize=initialize,
+        _prefix="initial_model_state",
     )
 
 
 def load_model_state(
     config: Config,
-    model: GraphModuleMixin,
+    graph_model: GraphModel,
     initialize: bool,
     _prefix: str = "load_model_state",
-):
+) -> GraphModel:
     """Load the model from the state dict file given by the config options `load_model_state`.
 
     Loads the state dict always; this is meant, for example, for building a new model to deploy with a given state dict.
 
     If `load_model_state_strict` controls
     > whether to strictly enforce that the keys in state_dict
     > match the keys returned by this module's state_dict() function
 
     See https://pytorch.org/docs/stable/generated/torch.nn.Module.html?highlight=load_state_dict#torch.nn.Module.load_state_dict.
     """
     if _prefix not in config:
         raise KeyError(
             f"initialize_from_state requires the `{_prefix}` option specifying the state to initialize from"
         )
-    state = torch.load(config[_prefix])
-    model.load_state_dict(state, strict=config.get(_prefix + "_strict", True))
-    return model
+    # Make sure we map to CPU if there is no GPU, otherwise just leave it alone
+    state = torch.load(
+        config[_prefix], map_location=None if torch.cuda.is_available() else "cpu"
+    )
+    strict: bool = config.get(_prefix + "_strict", True)
+    graph_model.load_state_dict(state, strict=strict)
+    logging.info(
+        f"Loaded model state {'' if strict else ' with strict=False'} (parameters/weights/persistent buffers) from state {_prefix}={config[_prefix]}"
+    )
+    return graph_model
 
 
 # == Init functions ==
 def unit_uniform_init_(t: torch.Tensor):
     """Uniform initialization with <x_i^2> = 1"""
     t.uniform_(-math.sqrt(3), math.sqrt(3))
```

### Comparing `nequip-0.5.6/nequip/model/builder_utils.py` & `nequip-0.6.0/nequip/model/builder_utils.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/nn/_atomwise.py` & `nequip-0.6.0/nequip/nn/_atomwise.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 import torch.nn.functional
 from torch_runstats.scatter import scatter
 
 from e3nn.o3 import Linear
 
 from nequip.data import AtomicDataDict
 from nequip.data.transforms import TypeMapper
+from nequip.utils import dtype_from_name
+from nequip.utils.versions import _TORCH_IS_GE_1_13
 from ._graph_mixin import GraphModuleMixin
+from ._rescale import RescaleOutput
 
 
 class AtomwiseOperation(GraphModuleMixin, torch.nn.Module):
     def __init__(self, operation, field: str, irreps_in=None):
         super().__init__()
         self.operation = operation
         self.field = field
@@ -76,32 +79,50 @@
             self.constant = float(avg_num_atoms) ** -0.5
             reduce = "sum"
         self.reduce = reduce
         self.field = field
         self.out_field = f"{reduce}_{field}" if out_field is None else out_field
         self._init_irreps(
             irreps_in=irreps_in,
-            irreps_out={self.out_field: irreps_in[self.field]}
-            if self.field in irreps_in
-            else {},
+            irreps_out=(
+                {self.out_field: irreps_in[self.field]}
+                if self.field in irreps_in
+                else {}
+            ),
         )
 
     def forward(self, data: AtomicDataDict.Type) -> AtomicDataDict.Type:
-        data = AtomicDataDict.with_batch(data)
-        data[self.out_field] = scatter(
-            data[self.field], data[AtomicDataDict.BATCH_KEY], dim=0, reduce=self.reduce
-        )
+        field = data[self.field]
+        if AtomicDataDict.BATCH_KEY in data:
+            result = scatter(
+                field,
+                data[AtomicDataDict.BATCH_KEY],
+                dim=0,
+                dim_size=len(data[AtomicDataDict.BATCH_PTR_KEY]) - 1,
+                reduce=self.reduce,
+            )
+        else:
+            # We can significantly simplify and avoid scatters
+            if self.reduce == "sum":
+                result = field.sum(dim=0, keepdim=True)
+            elif self.reduce == "mean":
+                result = field.mean(dim=0, keepdim=True)
+            else:
+                assert False
         if self.constant != 1.0:
-            data[self.out_field] = data[self.out_field] * self.constant
+            result = result * self.constant
+        data[self.out_field] = result
         return data
 
 
 class PerSpeciesScaleShift(GraphModuleMixin, torch.nn.Module):
     """Scale and/or shift a predicted per-atom property based on (learnable) per-species/type parameters.
 
+    Note that scaling/shifting is always done (casting into) ``default_dtype``, even if ``model_dtype`` is lower precision.
+
     Args:
         field: the per-atom field to scale/shift.
         num_types: the number of types in the model.
         shifts: the initial shifts to use, one per atom type.
         scales: the initial scales to use, one per atom type.
         arguments_in_dataset_units: if ``True``, says that the provided shifts/scales are in dataset
             units (in which case they will be rescaled appropriately by any global rescaling later
@@ -115,86 +136,137 @@
 
     field: str
     out_field: str
     scales_trainble: bool
     shifts_trainable: bool
     has_scales: bool
     has_shifts: bool
+    default_dtype: torch.dtype
+    _use_fma: bool
 
     def __init__(
         self,
         field: str,
         num_types: int,
         type_names: List[str],
         shifts: Optional[List[float]],
         scales: Optional[List[float]],
         arguments_in_dataset_units: bool,
         out_field: Optional[str] = None,
         scales_trainable: bool = False,
         shifts_trainable: bool = False,
+        default_dtype: Optional[str] = None,
         irreps_in={},
     ):
         super().__init__()
         self.num_types = num_types
         self.type_names = type_names
         self.field = field
         self.out_field = f"shifted_{field}" if out_field is None else out_field
         self._init_irreps(
             irreps_in=irreps_in,
             my_irreps_in={self.field: "0e"},  # input to shift must be a single scalar
             irreps_out={self.out_field: irreps_in[self.field]},
         )
 
+        self.default_dtype = dtype_from_name(
+            torch.get_default_dtype() if default_dtype is None else default_dtype
+        )
+
         self.has_shifts = shifts is not None
         if shifts is not None:
-            shifts = torch.as_tensor(shifts, dtype=torch.get_default_dtype())
+            shifts = torch.as_tensor(shifts, dtype=self.default_dtype)
             if len(shifts.reshape([-1])) == 1:
-                shifts = torch.ones(num_types) * shifts
+                shifts = (
+                    torch.ones(num_types, dtype=shifts.dtype, device=shifts.device)
+                    * shifts
+                )
             assert shifts.shape == (num_types,), f"Invalid shape of shifts {shifts}"
             self.shifts_trainable = shifts_trainable
             if shifts_trainable:
                 self.shifts = torch.nn.Parameter(shifts)
             else:
                 self.register_buffer("shifts", shifts)
+        else:
+            self.register_buffer("shifts", torch.Tensor())
 
         self.has_scales = scales is not None
         if scales is not None:
-            scales = torch.as_tensor(scales, dtype=torch.get_default_dtype())
+            scales = torch.as_tensor(scales, dtype=self.default_dtype)
             if len(scales.reshape([-1])) == 1:
-                scales = torch.ones(num_types) * scales
+                scales = (
+                    torch.ones(num_types, dtype=scales.dtype, device=scales.device)
+                    * scales
+                )
             assert scales.shape == (num_types,), f"Invalid shape of scales {scales}"
             self.scales_trainable = scales_trainable
             if scales_trainable:
                 self.scales = torch.nn.Parameter(scales)
             else:
                 self.register_buffer("scales", scales)
+        else:
+            self.register_buffer("scales", torch.Tensor())
 
+        assert isinstance(arguments_in_dataset_units, bool)
         self.arguments_in_dataset_units = arguments_in_dataset_units
 
+        # we can use FMA for performance but its type promotion is broken until 1.13
+        self._use_fma = _TORCH_IS_GE_1_13
+
     def forward(self, data: AtomicDataDict.Type) -> AtomicDataDict.Type:
 
         if not (self.has_scales or self.has_shifts):
             return data
 
-        species_idx = data[AtomicDataDict.ATOM_TYPE_KEY]
+        species_idx = data[AtomicDataDict.ATOM_TYPE_KEY].squeeze(-1)
         in_field = data[self.field]
         assert len(in_field) == len(
             species_idx
         ), "in_field doesnt seem to have correct per-atom shape"
-        if self.has_scales:
-            in_field = self.scales[species_idx].view(-1, 1) * in_field
-        if self.has_shifts:
-            in_field = self.shifts[species_idx].view(-1, 1) + in_field
+
+        if self._use_fma and self.has_scales and self.has_shifts:
+            # we can used an FMA for performance
+            # addcmul computes
+            # input + tensor1 * tensor2 elementwise
+            # it will promote to widest dtype, which comes from shifts/scales
+            in_field = torch.addcmul(
+                torch.index_select(self.shifts, 0, species_idx).view(-1, 1),
+                torch.index_select(self.scales, 0, species_idx).view(-1, 1),
+                in_field,
+            )
+        else:
+            # fallback path for torch<1.13 OR mix of enabled shifts and scales
+            # multiplication / addition promotes dtypes already, so no cast is needed
+            # this is specifically because self.*[species_idx].view(-1, 1)
+            # is never a scalar (ndim == 0), since it is always [n_atom, 1]
+            if self.has_scales:
+                in_field = (
+                    torch.index_select(self.scales, 0, species_idx).view(-1, 1)
+                    * in_field
+                )
+            if self.has_shifts:
+                in_field = (
+                    torch.index_select(self.shifts, 0, species_idx).view(-1, 1)
+                    + in_field
+                )
         data[self.out_field] = in_field
         return data
 
-    def update_for_rescale(self, rescale_module):
-        if hasattr(rescale_module, "related_scale_keys"):
-            if self.out_field not in rescale_module.related_scale_keys:
-                return
+    def update_for_rescale(self, rescale_module: RescaleOutput):
+        if not self.arguments_in_dataset_units:
+            # nothing to rescale, arguments are in normalized units already / unitless
+            return
+        # are we scaling something related to the global rescaling?
+        if self.field not in rescale_module.scale_keys:
+            return
+        # now check that we have the right rescaling in the specific energy case
+        if self.field == AtomicDataDict.PER_ATOM_ENERGY_KEY and not (
+            set(rescale_module.scale_keys) <= set(AtomicDataDict.ALL_ENERGY_KEYS)
+        ):
+            raise AssertionError("Some unsupported energy scaling arangement...")
         if self.arguments_in_dataset_units and rescale_module.has_scale:
             logging.debug(
                 f"PerSpeciesScaleShift's arguments were in dataset units; rescaling:\n  "
                 f"Original scales: {TypeMapper.format(self.scales, self.type_names) if self.has_scales else 'n/a'} "
                 f"shifts: {TypeMapper.format(self.shifts, self.type_names) if self.has_shifts else 'n/a'}"
             )
             with torch.no_grad():
```

### Comparing `nequip-0.5.6/nequip/nn/_concat.py` & `nequip-0.6.0/nequip/nn/_concat.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/nn/_convnetlayer.py` & `nequip-0.6.0/nequip/nn/_convnetlayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         irreps_in,
         feature_irreps_hidden,
         convolution=InteractionBlock,
         convolution_kwargs: dict = {},
         num_layers: int = 3,
         resnet: bool = False,
         nonlinearity_type: str = "gate",
-        nonlinearity_scalars: Dict[int, Callable] = {"e": "ssp", "o": "tanh"},
-        nonlinearity_gates: Dict[int, Callable] = {"e": "ssp", "o": "abs"},
+        nonlinearity_scalars: Dict[int, Callable] = {"e": "silu", "o": "tanh"},
+        nonlinearity_gates: Dict[int, Callable] = {"e": "silu", "o": "tanh"},
     ):
         super().__init__()
         # initialization
         assert nonlinearity_type in ("gate", "norm")
         # make the nonlin dicts from parity ints instead of convinience strs
         nonlinearity_scalars = {
             1: nonlinearity_scalars["e"],
```

### Comparing `nequip-0.5.6/nequip/nn/_grad_output.py` & `nequip-0.6.0/nequip/nn/_grad_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List, Union, Optional
-import warnings
 
 import torch
 
 from e3nn.o3 import Irreps
 from e3nn.util.jit import compile_mode
 
 from nequip.data import AtomicDataDict
@@ -189,41 +188,43 @@
     def __init__(
         self,
         func: GraphModuleMixin,
         do_forces: bool = True,
     ):
         super().__init__()
 
-        warnings.warn(
-            "!! Stresses in NequIP are in BETA and UNDER DEVELOPMENT: _please_ carefully check the sanity of your results and report any (potential) issues on the GitHub"
-        )
-
         if not do_forces:
             raise NotImplementedError
         self.do_forces = do_forces
 
         self.func = func
 
         # check and init irreps
         self._init_irreps(
             irreps_in=self.func.irreps_in.copy(),
             irreps_out=self.func.irreps_out.copy(),
         )
         self.irreps_out[AtomicDataDict.FORCE_KEY] = "1o"
-        self.irreps_out[AtomicDataDict.STRESS_KEY] = "3x1o"
-        self.irreps_out[AtomicDataDict.VIRIAL_KEY] = "3x1o"
+        self.irreps_out[AtomicDataDict.STRESS_KEY] = "1o"
+        self.irreps_out[AtomicDataDict.VIRIAL_KEY] = "1o"
 
         # for torchscript compat
         self.register_buffer("_empty", torch.Tensor())
 
     def forward(self, data: AtomicDataDict.Type) -> AtomicDataDict.Type:
-        data = AtomicDataDict.with_batch(data)
+        assert AtomicDataDict.EDGE_VECTORS_KEY not in data
+
+        if AtomicDataDict.BATCH_KEY in data:
+            batch = data[AtomicDataDict.BATCH_KEY]
+            num_batch: int = len(data[AtomicDataDict.BATCH_PTR_KEY]) - 1
+        else:
+            # Special case for efficiency
+            batch = self._empty
+            num_batch: int = 1
 
-        batch = data[AtomicDataDict.BATCH_KEY]
-        num_batch: int = int(batch.max().cpu().item()) + 1
         pos = data[AtomicDataDict.POSITIONS_KEY]
 
         has_cell: bool = AtomicDataDict.CELL_KEY in data
 
         if has_cell:
             orig_cell = data[AtomicDataDict.CELL_KEY]
             # Make the cell per-batch
@@ -239,18 +240,21 @@
         # https://github.com/atomistic-machine-learning/schnetpack/blob/master/src/schnetpack/atomistic/model.py#L45
         # SchNetPack issue:
         # https://github.com/atomistic-machine-learning/schnetpack/issues/165
         # Paper they worked from:
         # Knuth et. al. Comput. Phys. Commun 190, 33-50, 2015
         # https://pure.mpg.de/rest/items/item_2085135_9/component/file_2156800/content
         displacement = torch.zeros(
-            (num_batch, 3, 3),
+            (3, 3),
             dtype=pos.dtype,
             device=pos.device,
         )
+        if num_batch > 1:
+            # add n_batch dimension
+            displacement = displacement.view(-1, 3, 3).expand(num_batch, 3, 3)
         displacement.requires_grad_(True)
         data["_displacement"] = displacement
         # in the above paper, the infinitesimal distortion is *symmetric*
         # so we symmetrize the displacement before applying it to
         # the positions/cell
         # This is not strictly necessary (reasoning thanks to Mario):
         # the displacement's asymmetric 1o term corresponds to an
@@ -259,30 +263,47 @@
         # That said, due to numerical error, this will never be
         # exactly true. So, we symmetrize the deformation to
         # take advantage of this understanding and not rely on
         # the invariance here:
         symmetric_displacement = 0.5 * (displacement + displacement.transpose(-1, -2))
         did_pos_req_grad: bool = pos.requires_grad
         pos.requires_grad_(True)
-        # bmm is natom in batch
-        data[AtomicDataDict.POSITIONS_KEY] = pos + torch.bmm(
-            pos.unsqueeze(-2), symmetric_displacement[batch]
-        ).squeeze(-2)
+        if num_batch > 1:
+            # bmm is natom in batch
+            # batched [natom, 1, 3] @ [natom, 3, 3] -> [natom, 1, 3] -> [natom, 3]
+            data[AtomicDataDict.POSITIONS_KEY] = pos + torch.bmm(
+                pos.unsqueeze(-2), torch.index_select(symmetric_displacement, 0, batch)
+            ).squeeze(-2)
+        else:
+            # [natom, 3] @ [3, 3] -> [natom, 3]
+            data[AtomicDataDict.POSITIONS_KEY] = torch.addmm(
+                pos, pos, symmetric_displacement
+            )
+        # assert torch.equal(pos, data[AtomicDataDict.POSITIONS_KEY])
         # we only displace the cell if we have one:
         if has_cell:
             # bmm is num_batch in batch
             # here we apply the distortion to the cell as well
             # this is critical also for the correctness
             # if we didn't symmetrize the distortion, since without this
             # there would then be an infinitesimal rotation of the positions
             # but not cell, and it thus wouldn't be global and have
             # no effect due to equivariance/invariance.
-            data[AtomicDataDict.CELL_KEY] = cell + torch.bmm(
-                cell, symmetric_displacement
-            )
+            if num_batch > 1:
+                # [n_batch, 3, 3] @ [n_batch, 3, 3]
+                data[AtomicDataDict.CELL_KEY] = cell + torch.bmm(
+                    cell, symmetric_displacement
+                )
+            else:
+                # [3, 3] @ [3, 3] --- enforced to these shapes
+                tmpcell = cell.squeeze(0)
+                data[AtomicDataDict.CELL_KEY] = torch.addmm(
+                    tmpcell, tmpcell, symmetric_displacement
+                ).unsqueeze(0)
+            # assert torch.equal(cell, data[AtomicDataDict.CELL_KEY])
 
         # Call model and get gradients
         data = self.func(data)
 
         grads = torch.autograd.grad(
             [data[AtomicDataDict.TOTAL_ENERGY_KEY].sum()],
             [pos, data["_displacement"]],
@@ -298,27 +319,29 @@
         data[AtomicDataDict.FORCE_KEY] = forces
 
         # Store virial
         virial = grads[1]
         if virial is None:
             # condition needed to unwrap optional for torchscript
             assert False, "failed to compute virial autograd"
+        virial = virial.view(num_batch, 3, 3)
 
         # we only compute the stress (1/V * virial) if we have a cell whose volume we can compute
         if has_cell:
             # ^ can only scale by cell volume if we have one...:
             # Rescale stress tensor
             # See https://github.com/atomistic-machine-learning/schnetpack/blob/master/src/schnetpack/atomistic/output_modules.py#L180
+            # See also https://en.wikipedia.org/wiki/Triple_product
+            # See also https://gitlab.com/ase/ase/-/blob/master/ase/cell.py,
+            #          which uses np.abs(np.linalg.det(cell))
             # First dim is batch, second is vec, third is xyz
-            volume = torch.einsum(
-                "zi,zi->z",
-                cell[:, 0, :],
-                torch.cross(cell[:, 1, :], cell[:, 2, :], dim=1),
-            ).unsqueeze(-1)
-            stress = virial / volume.view(-1, 1, 1)
+            # Note the .abs(), since volume should always be positive
+            # det is equal to a dot (b cross c)
+            volume = torch.linalg.det(cell).abs().unsqueeze(-1)
+            stress = virial / volume.view(num_batch, 1, 1)
             data[AtomicDataDict.CELL_KEY] = orig_cell
         else:
             stress = self._empty  # torchscript
         data[AtomicDataDict.STRESS_KEY] = stress
 
         # see discussion in https://github.com/libAtoms/QUIP/issues/227 about sign convention
         # they say the standard convention is virial = -stress x volume
```

### Comparing `nequip-0.5.6/nequip/nn/_graph_mixin.py` & `nequip-0.6.0/nequip/nn/_graph_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,51 +213,57 @@
 
             built_modules.append(instance)
 
         return cls(
             OrderedDict(zip(layers.keys(), built_modules)),
         )
 
+    @torch.jit.unused
     def append(self, name: str, module: GraphModuleMixin) -> None:
         r"""Append a module to the SequentialGraphNetwork.
 
         Args:
             name (str): the name for the module
             module (GraphModuleMixin): the module to append
         """
         assert AtomicDataDict._irreps_compatible(self.irreps_out, module.irreps_in)
         self.add_module(name, module)
         self.irreps_out = dict(module.irreps_out)
         return
 
+    @torch.jit.unused
     def append_from_parameters(
         self,
         shared_params: Mapping,
         name: str,
         builder: Callable,
         params: Dict[str, Any] = {},
-    ) -> None:
+    ) -> GraphModuleMixin:
         r"""Build a module from parameters and append it.
 
         Args:
             shared_params (dict-like): shared parameters from which to pull when instantiating the module
             name (str): the name for the module
             builder (callable): a class or function to build a module
             params (dict, optional): extra specific parameters for this module that take priority over those in ``shared_params``
+
+        Returns:
+            the build module
         """
         instance, _ = instantiate(
             builder=builder,
             prefix=name,
             positional_args=(dict(irreps_in=self[-1].irreps_out)),
             optional_args=params,
             all_args=shared_params,
         )
         self.append(name, instance)
-        return
+        return instance
 
+    @torch.jit.unused
     def insert(
         self,
         name: str,
         module: GraphModuleMixin,
         after: Optional[str] = None,
         before: Optional[str] = None,
     ) -> None:
@@ -307,32 +313,36 @@
             next_module._add_independent_irreps(module.irreps_out)
 
         # update the final wrapper irreps_out
         self.irreps_out = dict(module_list[-1].irreps_out)
 
         return
 
+    @torch.jit.unused
     def insert_from_parameters(
         self,
         shared_params: Mapping,
         name: str,
         builder: Callable,
         params: Dict[str, Any] = {},
         after: Optional[str] = None,
         before: Optional[str] = None,
-    ) -> None:
+    ) -> GraphModuleMixin:
         r"""Build a module from parameters and insert it after ``after``.
 
         Args:
             shared_params (dict-like): shared parameters from which to pull when instantiating the module
             name (str): the name for the module
             builder (callable): a class or function to build a module
             params (dict, optional): extra specific parameters for this module that take priority over those in ``shared_params``
             after: the name of the module to insert after
             before: the name of the module to insert before
+
+        Returns:
+            the inserted module
         """
         if (before is None) is (after is None):
             raise ValueError("Only one of before or after argument needs to be defined")
         elif before is None:
             insert_location = after
         else:
             insert_location = before
@@ -343,15 +353,15 @@
             builder=builder,
             prefix=name,
             positional_args=(dict(irreps_in=self[idx].irreps_out)),
             optional_args=params,
             all_args=shared_params,
         )
         self.insert(after=after, before=before, name=name, module=instance)
-        return
+        return instance
 
     # Copied from https://pytorch.org/docs/stable/_modules/torch/nn/modules/container.html#Sequential
     # with type annotations added
     def forward(self, input: AtomicDataDict.Type) -> AtomicDataDict.Type:
         for module in self:
             input = module(input)
         return input
```

### Comparing `nequip-0.5.6/nequip/nn/_interaction_block.py` & `nequip-0.6.0/nequip/nn/_interaction_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self,
         irreps_in,
         irreps_out,
         invariant_layers=1,
         invariant_neurons=8,
         avg_num_neighbors=None,
         use_sc=True,
-        nonlinearity_scalars: Dict[int, Callable] = {"e": "ssp"},
+        nonlinearity_scalars: Dict[int, Callable] = {"e": "silu"},
     ) -> None:
         """
         InteractionBlock.
 
         :param irreps_node_attr: Nodes attribute irreps
         :param irreps_edge_attr: Edge attribute irreps
         :param irreps_out: Output irreps, in our case typically a single scalar
@@ -164,20 +164,21 @@
         if self.sc is not None:
             sc = self.sc(x, data[AtomicDataDict.NODE_ATTRS_KEY])
 
         x = self.linear_1(x)
         edge_features = self.tp(
             x[edge_src], data[AtomicDataDict.EDGE_ATTRS_KEY], weight
         )
-        x = scatter(edge_features, edge_dst, dim=0, dim_size=len(x))
-
+        # divide first for numerics, scatter is linear
         # Necessary to get TorchScript to be able to type infer when its not None
         avg_num_neigh: Optional[float] = self.avg_num_neighbors
         if avg_num_neigh is not None:
-            x = x.div(avg_num_neigh**0.5)
+            edge_features = edge_features.div(avg_num_neigh**0.5)
+        # now scatter down
+        x = scatter(edge_features, edge_dst, dim=0, dim_size=len(x))
 
         x = self.linear_2(x)
 
         if self.sc is not None:
             x = x + sc
 
         data[AtomicDataDict.NODE_FEATURES_KEY] = x
```

### Comparing `nequip-0.5.6/nequip/nn/_rescale.py` & `nequip-0.6.0/nequip/nn/_rescale.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-from typing import Sequence, List, Union
+from typing import Sequence, List, Union, Optional
 
 import torch
 
 from e3nn.util.jit import compile_mode
 
 from nequip.data import AtomicDataDict
 from nequip.nn import GraphModuleMixin
+from nequip.utils import dtype_from_name
 
 
 @compile_mode("script")
 class RescaleOutput(GraphModuleMixin, torch.nn.Module):
     """Wrap a model and rescale its outputs when in ``eval()`` mode.
 
+    Note that scaling/shifting is always done (casting into) ``default_dtype``, even if ``model_dtype`` is lower precision.
+
     Args:
         model : GraphModuleMixin
             The model whose outputs are to be rescaled.
         scale_keys : list of keys, default []
             Which fields to rescale.
         shift_keys : list of keys, default []
             Which fields to shift after rescaling.
-        related_scale_keys: list of keys that could be contingent to this rescale
-        related_shift_keys: list of keys that could be contingent to this rescale
         scale_by : floating or Tensor, default 1.
             The scaling factor by which to multiply fields in ``scale``.
         shift_by : floating or Tensor, default 0.
             The shift to add to fields in ``shift``.
         irreps_in : dict, optional
             Extra inputs expected by this beyond those of `model`; this is only present for compatibility.
     """
 
     scale_keys: List[str]
     shift_keys: List[str]
-    related_scale_keys: List[str]
-    related_shift_keys: List[str]
     scale_trainble: bool
     rescale_trainable: bool
+    _all_keys: List[str]
 
     has_scale: bool
     has_shift: bool
 
+    default_dtype: torch.dtype
+
     def __init__(
         self,
         model: GraphModuleMixin,
         scale_keys: Union[Sequence[str], str] = [],
         shift_keys: Union[Sequence[str], str] = [],
-        related_shift_keys: Union[Sequence[str], str] = [],
-        related_scale_keys: Union[Sequence[str], str] = [],
         scale_by=None,
         shift_by=None,
         shift_trainable: bool = False,
         scale_trainable: bool = False,
+        default_dtype: Optional[str] = None,
         irreps_in: dict = {},
     ):
         super().__init__()
 
         self.model = model
         scale_keys = [scale_keys] if isinstance(scale_keys, str) else scale_keys
         shift_keys = [shift_keys] if isinstance(shift_keys, str) else shift_keys
@@ -77,21 +78,24 @@
                 )
 
         irreps_in.update(model.irreps_in)
         self._init_irreps(irreps_in=irreps_in, irreps_out=model.irreps_out)
 
         self.scale_keys = list(scale_keys)
         self.shift_keys = list(shift_keys)
-        self.related_scale_keys = list(set(related_scale_keys).union(scale_keys))
-        self.related_shift_keys = list(set(related_shift_keys).union(shift_keys))
+        self._all_keys = list(all_keys)
+
+        self.default_dtype = dtype_from_name(
+            torch.get_default_dtype() if default_dtype is None else default_dtype
+        )
 
         self.has_scale = scale_by is not None
         self.scale_trainble = scale_trainable
         if self.has_scale:
-            scale_by = torch.as_tensor(scale_by)
+            scale_by = torch.as_tensor(scale_by, dtype=self.default_dtype)
             if self.scale_trainble:
                 self.scale_by = torch.nn.Parameter(scale_by)
             else:
                 self.register_buffer("scale_by", scale_by)
         elif self.scale_trainble:
             raise ValueError(
                 "Asked for a scale_trainable, but this RescaleOutput has no scaling (`scale_by = None`)"
@@ -99,15 +103,15 @@
         else:
             # register dummy for TorchScript
             self.register_buffer("scale_by", torch.Tensor())
 
         self.has_shift = shift_by is not None
         self.rescale_trainable = shift_trainable
         if self.has_shift:
-            shift_by = torch.as_tensor(shift_by)
+            shift_by = torch.as_tensor(shift_by, dtype=self.default_dtype)
             if self.rescale_trainable:
                 self.shift_by = torch.nn.Parameter(shift_by)
             else:
                 self.register_buffer("shift_by", shift_by)
         elif self.rescale_trainable:
             raise ValueError(
                 "Asked for a shift_trainable, but this RescaleOutput has no shift (`shift_by = None`)"
@@ -135,24 +139,37 @@
         while isinstance(model, RescaleOutput):
             model = model.model
         return model
 
     def forward(self, data: AtomicDataDict.Type) -> AtomicDataDict.Type:
         data = self.model(data)
         if self.training:
-            return data
+            # no scaling, but still need to promote for consistent dtype behavior
+            # this is hopefully a no-op in most circumstances due to a
+            # preceeding PerSpecies rescale promoting to default_dtype anyway:
+            for field in self._all_keys:
+                data[field] = data[field].to(dtype=self.default_dtype)
         else:
             # Scale then shift
+            # * and + promote dtypes by default, but not when the other
+            # operand is a scalar, which `scale/shift_by` are.
+            # We solve this by expanding `scale/shift_by` to tensors
+            # This is free and doesn't allocate new memory on CUDA:
+            # https://pytorch.org/docs/stable/generated/torch.Tensor.expand.html#torch.Tensor.expand
+            # confirmed in PyTorch slack
+            # https://pytorch.slack.com/archives/C3PDTEV8E/p1671652283801129
             if self.has_scale:
                 for field in self.scale_keys:
-                    data[field] = data[field] * self.scale_by
+                    v = data[field]
+                    data[field] = v * self.scale_by.expand(v.shape)
             if self.has_shift:
                 for field in self.shift_keys:
-                    data[field] = data[field] + self.shift_by
-            return data
+                    v = data[field]
+                    data[field] = v + self.shift_by.expand(v.shape)
+        return data
 
     @torch.jit.export
     def scale(
         self,
         data: AtomicDataDict.Type,
         force_process: bool = False,
     ) -> AtomicDataDict.Type:
```

### Comparing `nequip-0.5.6/nequip/nn/_util.py` & `nequip-0.6.0/nequip/nn/_util.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/nn/cutoffs.py` & `nequip-0.6.0/nequip/nn/cutoffs.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/nn/embedding/_edge.py` & `nequip-0.6.0/nequip/nn/embedding/_edge.py`

 * *Files 18% similar despite different names*

```diff
@@ -72,18 +72,43 @@
     ):
         super().__init__()
         self.basis = basis(**basis_kwargs)
         self.cutoff = cutoff(**cutoff_kwargs)
         self.out_field = out_field
         self._init_irreps(
             irreps_in=irreps_in,
-            irreps_out={self.out_field: o3.Irreps([(self.basis.num_basis, (0, 1))])},
+            irreps_out={
+                self.out_field: o3.Irreps([(self.basis.num_basis, (0, 1))]),
+                AtomicDataDict.EDGE_CUTOFF_KEY: "0e",
+            },
         )
 
     def forward(self, data: AtomicDataDict.Type) -> AtomicDataDict.Type:
         data = AtomicDataDict.with_edge_vectors(data, with_lengths=True)
         edge_length = data[AtomicDataDict.EDGE_LENGTH_KEY]
-        edge_length_embedded = (
-            self.basis(edge_length) * self.cutoff(edge_length)[:, None]
-        )
+        cutoff = self.cutoff(edge_length).unsqueeze(-1)
+        edge_length_embedded = self.basis(edge_length) * cutoff
         data[self.out_field] = edge_length_embedded
+        data[AtomicDataDict.EDGE_CUTOFF_KEY] = cutoff
+        return data
+
+
+@compile_mode("script")
+class AddRadialCutoffToData(GraphModuleMixin, torch.nn.Module):
+    def __init__(
+        self,
+        cutoff=PolynomialCutoff,
+        cutoff_kwargs={},
+        irreps_in=None,
+    ):
+        super().__init__()
+        self.cutoff = cutoff(**cutoff_kwargs)
+        self._init_irreps(
+            irreps_in=irreps_in, irreps_out={AtomicDataDict.EDGE_CUTOFF_KEY: "0e"}
+        )
+
+    def forward(self, data: AtomicDataDict.Type) -> AtomicDataDict.Type:
+        data = AtomicDataDict.with_edge_vectors(data, with_lengths=True)
+        edge_length = data[AtomicDataDict.EDGE_LENGTH_KEY]
+        cutoff = self.cutoff(edge_length).unsqueeze(-1)
+        data[AtomicDataDict.EDGE_CUTOFF_KEY] = cutoff
         return data
```

### Comparing `nequip-0.5.6/nequip/nn/embedding/_one_hot.py` & `nequip-0.6.0/nequip/nn/embedding/_one_hot.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/nn/radial_basis.py` & `nequip-0.6.0/nequip/nn/radial_basis.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/scripts/_logger.py` & `nequip-0.6.0/nequip/scripts/_logger.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/scripts/benchmark.py` & `nequip-0.6.0/nequip/scripts/benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import tempfile
 import itertools
 import time
 import logging
 import sys
 import pdb
 import traceback
+import pickle
 
 import torch
 from torch.utils.benchmark import Timer, Measurement
 from torch.utils.benchmark.utils.common import trim_sigfig, select_unit
 
 from e3nn.util.jit import script
 
@@ -53,27 +54,21 @@
         type=str,
         default=None,
     )
     parser.add_argument(
         "-n",
         help="Number of trials.",
         type=int,
-        default=30,
+        default=None,
     )
     parser.add_argument(
         "--n-data",
         help="Number of frames to use.",
         type=int,
-        default=1,
-    )
-    parser.add_argument(
-        "--timestep",
-        help="MD timestep for ns/day esimation, in fs. Defauts to 1fs.",
-        type=float,
-        default=1,
+        default=2,
     )
     parser.add_argument(
         "--no-compile",
         help="Don't compile the model to TorchScript",
         action="store_true",
     )
     parser.add_argument(
@@ -112,28 +107,30 @@
 
     # Load dataset to get something to benchmark on
     print("Loading dataset... ")
     dataset_time = time.time()
     dataset = dataset_from_config(config)
     dataset_time = time.time() - dataset_time
     print(f"    loading dataset took {dataset_time:.4f}s")
+    print(
+        f"    loaded dataset of size {len(dataset)} and sampled --n-data={args.n_data} frames"
+    )
     dataset_rng = torch.Generator()
     dataset_rng.manual_seed(config.get("dataset_seed", config.get("seed", 12345)))
+    dataset = dataset.index_select(
+        torch.randperm(len(dataset), generator=dataset_rng)[: args.n_data]
+    )
     datas_list = [
-        AtomicData.to_AtomicDataDict(dataset[i].to(device))
-        for i in torch.randperm(len(dataset), generator=dataset_rng)[: args.n_data]
+        AtomicData.to_AtomicDataDict(dataset[i].to(device)) for i in range(args.n_data)
     ]
     n_atom: int = len(datas_list[0]["pos"])
     if not all(len(d["pos"]) == n_atom for d in datas_list):
         raise NotImplementedError(
             "nequip-benchmark does not currently handle benchmarking on data frames with variable number of atoms"
         )
-    print(
-        f"    loaded dataset of size {len(dataset)} and sampled --n-data={args.n_data} frames"
-    )
     # print some dataset information
     print("    benchmark frames statistics:")
     print(f"         number of atoms: {n_atom}")
     print(f"         number of types: {dataset.type_mapper.num_types}")
     print(
         f"          avg. num edges: {sum(d[AtomicDataDict.EDGE_INDEX_KEY].shape[1] for d in datas_list) / len(datas_list)}"
     )
@@ -153,14 +150,16 @@
     # cycle over the datas we loaded
     datas = itertools.cycle(datas_list)
 
     # short circut
     if args.n == 0:
         print("Got -n 0, so quitting without running benchmark.")
         return
+    elif args.n is None:
+        args.n = 5 if args.profile else 30
 
     # Load model:
     if args.model is None:
         print("Building model... ")
         model_time = time.time()
         try:
             model = model_from_config(
@@ -235,16 +234,19 @@
             + ([torch.profiler.ProfilerActivity.CUDA] if device.type == "cuda" else []),
             schedule=torch.profiler.schedule(
                 wait=1, warmup=warmup, active=args.n, repeat=1
             ),
             on_trace_ready=trace_handler,
         ) as p:
             for _ in range(1 + warmup + args.n):
-                model(next(datas).copy())
+                out = model(next(datas).copy())
+                out[AtomicDataDict.TOTAL_ENERGY_KEY].item()
                 p.step()
+
+        print(p.key_averages().table(sort_by="cuda_time_total", row_limit=100))
     elif args.pdb:
         print("Running model under debugger...")
         try:
             for _ in range(args.n):
                 model(next(datas).copy())
         except:  # noqa: E722
             traceback.print_exc()
@@ -266,56 +268,63 @@
             "    shifts to the (atomic) energy can cause\n"
             "    catastrophic cancellation and give incorrectly\n"
             "    the equivariance error as zero for those fields.\n"
             f"{errstr}"
         )
         del errstr
     else:
+        if args.memory_summary and torch.cuda.is_available():
+            torch.cuda.memory._record_memory_history(
+                True,
+                # keep 100,000 alloc/free events from before the snapshot
+                trace_alloc_max_entries=100000,
+                # record stack information for the trace events
+                trace_alloc_record_context=True,
+            )
         print("Warmup...")
         warmup_time = time.time()
         for _ in range(warmup):
             model(next(datas).copy())
         warmup_time = time.time() - warmup_time
         print(f"    {warmup} calls of warmup took {warmup_time:.4f}s")
 
         print("Benchmarking...")
+
         # just time
         t = Timer(
-            stmt="model(next(datas).copy())", globals={"model": model, "datas": datas}
+            stmt="model(next(datas).copy())['total_energy'].item()",
+            globals={"model": model, "datas": datas},
         )
         perloop: Measurement = t.timeit(args.n)
 
         if args.memory_summary and torch.cuda.is_available():
             print("Memory usage summary:")
             print(torch.cuda.memory_summary())
+            snapshot = torch.cuda.memory._snapshot()
+
+            with open("snapshot.pickle", "wb") as f:
+                pickle.dump(snapshot, f)
 
         print(" -- Results --")
         print(
             f"PLEASE NOTE: these are speeds for the MODEL, evaluated on --n-data={args.n_data} configurations kept in memory."
         )
         print(
-            "    \\_ MD itself, memory copies, and other overhead will affect real-world performance."
+            "A variety of factors affect the performance in real molecular dynamics calculations:"
+        )
+        print(
+            "!!! Molecular dynamics speeds should be measured in LAMMPS; speeds from nequip-benchmark should only be used as an estimate of RELATIVE speed among different hyperparameters."
+        )
+        print(
+            "Please further note that relative speed ordering of hyperparameters is NOT NECESSARILY CONSISTENT across different classes of GPUs (i.e. A100 vs V100 vs consumer) or GPUs vs CPUs."
         )
         print()
         trim_time = trim_sigfig(perloop.times[0], perloop.significant_figures)
         time_unit, time_scale = select_unit(trim_time)
         time_str = ("{:.%dg}" % perloop.significant_figures).format(
             trim_time / time_scale
         )
         print(f"The average call took {time_str}{time_unit}")
-        print(
-            "Assuming linear scaling — which is ALMOST NEVER true in practice, especially on GPU —"
-        )
-        per_atom_time = trim_time / n_atom
-        time_unit_per, time_scale_per = select_unit(per_atom_time)
-        print(
-            f"    \\_ this comes out to {per_atom_time/time_scale_per:g} {time_unit_per}/atom/call"
-        )
-        ns_day = (86400.0 / trim_time) * args.timestep * 1e-6
-        #     day in s^   s/step^         ^ fs / step      ^ ns / fs
-        print(
-            f"For this system, at a {args.timestep:.2f}fs timestep, this comes out to {ns_day:.2f} ns/day"
-        )
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nequip-0.5.6/nequip/scripts/evaluate.py` & `nequip-0.6.0/nequip/scripts/evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,97 @@
-from typing import Optional
+from typing import Optional, Tuple, List
 import sys
 import argparse
 import logging
 import textwrap
 from pathlib import Path
 import contextlib
 from tqdm.auto import tqdm
 
 import ase.io
 
 import torch
 
-from nequip.data import AtomicData, Collater, dataset_from_config, register_fields
-from nequip.scripts.deploy import load_deployed_model, R_MAX_KEY
+from nequip.data import (
+    AtomicData,
+    Collater,
+    dataset_from_config,
+    register_fields,
+    _register_field_prefix,
+)
+from nequip.scripts.deploy import load_deployed_model, R_MAX_KEY, TYPE_NAMES_KEY
 from nequip.scripts._logger import set_up_script_logger
 from nequip.scripts.train import default_config, check_code_version
 from nequip.utils._global_options import _set_global_options
 from nequip.train import Trainer, Loss, Metrics
 from nequip.utils import load_file, instantiate, Config
 
-
-ORIGINAL_DATASET_INDEX_KEY: str = "original_dataset_index"
+ORIGINAL_DATASET_PREFIX: str = "original_dataset_"
+ORIGINAL_DATASET_INDEX_KEY: str = ORIGINAL_DATASET_PREFIX + "index"
 register_fields(graph_fields=[ORIGINAL_DATASET_INDEX_KEY])
 
 
+def _load_deployed_or_traindir(
+    path: Path, device, freeze: bool = True
+) -> Tuple[torch.nn.Module, bool, float, List[str]]:
+    loaded_deployed_model: bool = False
+    model_r_max = None
+    type_names = None
+    try:
+        model, metadata = load_deployed_model(
+            path,
+            device=device,
+            set_global_options=True,  # don't warn that setting
+            freeze=freeze,
+        )
+        # the global settings for a deployed model are set by
+        # set_global_options in the call to load_deployed_model
+        # above
+        model_r_max = float(metadata[R_MAX_KEY])
+        type_names = metadata[TYPE_NAMES_KEY].split(" ")
+        loaded_deployed_model = True
+    except ValueError:  # its not a deployed model
+        loaded_deployed_model = False
+    # we don't do this in the `except:` block to avoid "during handing of this exception another exception"
+    # chains if there is an issue loading the training session model. This makes the error messages more
+    # comprehensible:
+    if not loaded_deployed_model:
+        # Use the model config, regardless of dataset config
+        global_config = path.parent / "config.yaml"
+        global_config = Config.from_file(str(global_config), defaults=default_config)
+        _set_global_options(global_config)
+        check_code_version(global_config)
+        del global_config
+
+        # load a training session model
+        model, model_config = Trainer.load_model_from_training_session(
+            traindir=path.parent, model_name=path.name
+        )
+        model = model.to(device)
+        model_r_max = model_config["r_max"]
+        type_names = model_config["type_names"]
+    model.eval()
+    return model, loaded_deployed_model, model_r_max, type_names
+
+
 def main(args=None, running_as_script: bool = True):
     # in results dir, do: nequip-deploy build --train-dir . deployed.pth
     parser = argparse.ArgumentParser(
         description=textwrap.dedent(
             """Compute the error of a model on a test set using various metrics.
 
             The model, metrics, dataset, etc. can specified in individual YAML config files, or a training session can be indicated with `--train-dir`.
             In order of priority, the global settings (dtype, TensorFloat32, etc.) are taken from:
               (1) the model config (for a training session),
               (2) the dataset config (for a deployed model),
               or (3) the defaults.
 
             Prints only the final result in `name = num` format to stdout; all other information is `logging.debug`ed to stderr.
 
-            WARNING: Please note that results of CUDA models are rarely exactly reproducible, and that even CPU models can be nondeterministic.
+            Please note that results of CUDA models are rarely exactly reproducible, and that even CPU models can be nondeterministic. This is very rarely important in practice, but can be unintuitive.
             """
         )
     )
     parser.add_argument(
         "--train-dir",
         help="Path to a working directory from a training session.",
         type=Path,
@@ -64,15 +113,15 @@
         "--metrics-config",
         help="A YAML config file specifying the metrics to compute. If omitted, `config.yaml` in `train_dir` will be used. If the config does not specify `metrics_components`, the default is to logging.debug MAEs and RMSEs for all fields given in the loss function. If the literal string `None`, no metrics will be computed.",
         type=str,
         default=None,
     )
     parser.add_argument(
         "--test-indexes",
-        help="Path to a file containing the indexes in the dataset that make up the test set. If omitted, all data frames *not* used as training or validation data in the training session `train_dir` will be used.",
+        help="Path to a file containing the indexes in the dataset that make up the test set. If omitted, all data frames *not* used as training or validation data in the training session `train_dir` will be used. PyTorch, YAML, and JSON formats containing a list of integers are supported.",
         type=Path,
         default=None,
     )
     parser.add_argument(
         "--batch-size",
         help="Batch size to use. Larger is usually faster on GPU. If you run out of memory, lower this. You can also try to raise this for faster evaluation. Default: 50.",
         type=int,
@@ -109,14 +158,20 @@
     parser.add_argument(
         "--output-fields",
         help="Extra fields (names comma separated with no spaces) to write to the `--output`.",
         type=str,
         default="",
     )
     parser.add_argument(
+        "--output-fields-from-original-dataset",
+        help="Extra fields from the ORIGINAL REFERENCE DATASET (names comma separated with no spaces) to write to the `--output` with the added prefix `original_dataset_*`",
+        type=str,
+        default="",
+    )
+    parser.add_argument(
         "--log",
         help="log file to store all the metrics and screen logging.debug",
         type=Path,
         default=None,
     )
     # Something has to be provided
     # See https://stackoverflow.com/questions/22368458/how-to-make-argparse-logging.debug-usage-when-no-option-is-given-to-the-code
@@ -160,17 +215,28 @@
         )
     if args.model is None:
         raise ValueError("--model or --train-dir must be provided")
     output_type: Optional[str] = None
     if args.output is not None:
         if args.output.suffix != ".xyz":
             raise ValueError("Only .xyz format for `--output` is supported.")
-        args.output_fields = [e for e in args.output_fields.split(",") if e != ""] + [
-            ORIGINAL_DATASET_INDEX_KEY
+        args.output_fields_from_original_dataset = [
+            e for e in args.output_fields_from_original_dataset.split(",") if e != ""
         ]
+        args.output_fields = [e for e in args.output_fields.split(",") if e != ""]
+        ase_all_fields = (
+            args.output_fields
+            + [
+                ORIGINAL_DATASET_PREFIX + e
+                for e in args.output_fields_from_original_dataset
+            ]
+            + [ORIGINAL_DATASET_INDEX_KEY]
+        )
+        if len(args.output_fields_from_original_dataset) > 0:
+            _register_field_prefix(ORIGINAL_DATASET_PREFIX)
         output_type = "xyz"
     else:
         assert args.output_fields == ""
         args.output_fields = []
 
     if args.device is None:
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
@@ -181,60 +247,29 @@
         set_up_script_logger(args.log)
     logger = logging.getLogger("nequip-evaluate")
     logger.setLevel(logging.INFO)
 
     logger.info(f"Using device: {device}")
     if device.type == "cuda":
         logger.info(
-            "WARNING: please note that models running on CUDA are usually nondeterministc and that this manifests in the final test errors; for a _more_ deterministic result, please use `--device cpu`",
+            "Please note that _all_ machine learning models running on CUDA hardware are generally somewhat nondeterministic and that this can manifest in small, generally unimportant variation in the final test errors.",
         )
 
     if args.use_deterministic_algorithms:
         logger.info(
             "Telling PyTorch to try to use deterministic algorithms... please note that this will likely error on CUDA/GPU"
         )
         torch.use_deterministic_algorithms(True)
 
     # Load model:
     logger.info("Loading model... ")
-    loaded_deployed_model: bool = False
-    model_r_max = None
-    try:
-        model, metadata = load_deployed_model(
-            args.model,
-            device=device,
-            set_global_options=True,  # don't warn that setting
-        )
-        logger.info("loaded deployed model.")
-        # the global settings for a deployed model are set by
-        # set_global_options in the call to load_deployed_model
-        # above
-        model_r_max = float(metadata[R_MAX_KEY])
-        loaded_deployed_model = True
-    except ValueError:  # its not a deployed model
-        loaded_deployed_model = False
-    # we don't do this in the `except:` block to avoid "during handing of this exception another exception"
-    # chains if there is an issue loading the training session model. This makes the error messages more
-    # comprehensible:
-    if not loaded_deployed_model:
-        # Use the model config, regardless of dataset config
-        global_config = args.model.parent / "config.yaml"
-        global_config = Config.from_file(str(global_config), defaults=default_config)
-        _set_global_options(global_config)
-        check_code_version(global_config)
-        del global_config
-
-        # load a training session model
-        model, model_config = Trainer.load_model_from_training_session(
-            traindir=args.model.parent, model_name=args.model.name
-        )
-        model = model.to(device)
-        logger.info("loaded model from training session")
-        model_r_max = model_config["r_max"]
-    model.eval()
+    model, loaded_deployed_model, model_r_max, _ = _load_deployed_or_traindir(
+        args.model, device=device
+    )
+    logger.info(f"    loaded{' deployed' if loaded_deployed_model else ''} model")
 
     # Load a config file
     logger.info(
         f"Loading {'original ' if dataset_is_from_training else ''}dataset...",
     )
     dataset_config = Config.from_file(
         str(args.dataset_config), defaults={"r_max": model_r_max}
@@ -370,30 +405,35 @@
             batch = c.collate(datas)
             batch = batch.to(device)
             out = model(AtomicData.to_AtomicDataDict(batch))
 
             with torch.no_grad():
                 # Write output
                 if output_type == "xyz":
+                    output_out = out.copy()
                     # add test frame to the output:
-                    out[ORIGINAL_DATASET_INDEX_KEY] = torch.LongTensor(
+                    output_out[ORIGINAL_DATASET_INDEX_KEY] = torch.LongTensor(
                         this_batch_test_indexes
                     )
+                    for field in args.output_fields_from_original_dataset:
+                        # batch is from the original dataset
+                        output_out[ORIGINAL_DATASET_PREFIX + field] = batch[field]
                     # append to the file
                     ase.io.write(
                         output,
-                        AtomicData.from_AtomicDataDict(out)
+                        AtomicData.from_AtomicDataDict(output_out)
                         .to(device="cpu")
                         .to_ase(
                             type_mapper=dataset.type_mapper,
-                            extra_fields=args.output_fields,
+                            extra_fields=ase_all_fields,
                         ),
                         format="extxyz",
                         append=True,
                     )
+                    del output_out
 
                 # Accumulate metrics
                 if do_metrics:
                     metrics(out, batch)
                     display_bar.set_description_str(
                         " | ".join(
                             f"{k} = {v:4.4f}"
```

### Comparing `nequip-0.5.6/nequip/scripts/run_md.py` & `nequip-0.6.0/nequip/scripts/run_md.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/scripts/train.py` & `nequip-0.6.0/nequip/scripts/train.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,50 +12,61 @@
 
 import torch
 
 from nequip.model import model_from_config
 from nequip.utils import Config
 from nequip.data import dataset_from_config
 from nequip.utils import load_file
+from nequip.utils.config import _GLOBAL_ALL_ASKED_FOR_KEYS
 from nequip.utils.test import assert_AtomicData_equivariant
 from nequip.utils.versions import check_code_version
+from nequip.utils.misc import get_default_device_name
 from nequip.utils._global_options import _set_global_options
 from nequip.scripts._logger import set_up_script_logger
 
 default_config = dict(
     root="./",
-    run_name="NequIP",
+    tensorboard=False,
     wandb=False,
-    wandb_project="NequIP",
     model_builders=[
         "SimpleIrrepsConfig",
         "EnergyModel",
         "PerSpeciesRescale",
-        "ForceOutput",
+        "StressForceOutput",
         "RescaleEnergyEtc",
     ],
     dataset_statistics_stride=1,
-    default_dtype="float32",
-    allow_tf32=False,  # TODO: until we understand equivar issues
+    device=get_default_device_name(),
+    default_dtype="float64",
+    model_dtype="float32",
+    allow_tf32=True,
     verbose="INFO",
     model_debug_mode=False,
     equivariance_test=False,
     grad_anomaly_mode=False,
+    gpu_oom_offload=False,
     append=False,
+    warn_unused=False,
     _jit_bailout_depth=2,  # avoid 20 iters of pain, see https://github.com/pytorch/pytorch/issues/52286
     # Quote from eelison in PyTorch slack:
     # https://pytorch.slack.com/archives/CDZD1FANA/p1644259272007529?thread_ts=1644064449.039479&cid=CDZD1FANA
     # > Right now the default behavior is to specialize twice on static shapes and then on dynamic shapes.
     # > To reduce warmup time you can do something like setFusionStrartegy({{FusionBehavior::DYNAMIC, 3}})
     # > ... Although we would wouldn't really expect to recompile a dynamic shape fusion in a model,
     # > provided broadcasting patterns remain fixed
     # We default to DYNAMIC alone because the number of edges is always dynamic,
     # even if the number of atoms is fixed:
     _jit_fusion_strategy=[("DYNAMIC", 3)],
+    # Due to what appear to be ongoing bugs with nvFuser, we default to NNC (fuser1) for now:
+    # TODO: still default to NNC on CPU regardless even if change this for GPU
+    # TODO: default for ROCm?
+    _jit_fuser="fuser1",
 )
+# All default_config keys are valid / requested
+_GLOBAL_ALL_ASKED_FOR_KEYS.update(default_config.keys())
 
 
 def main(args=None, running_as_script: bool = True):
     config = parse_command_line(args)
 
     if running_as_script:
         set_up_script_logger(config.get("log", None), config.verbose)
@@ -71,15 +82,30 @@
     if not found_restart_file:
         trainer = fresh_start(config)
     else:
         trainer = restart(config)
 
     # Train
     trainer.save()
-    trainer.train()
+    if config.get("gpu_oom_offload", False):
+        if not torch.cuda.is_available():
+            raise RuntimeError(
+                "CUDA is not available; --gpu-oom-offload doesn't make sense."
+            )
+        warnings.warn(
+            "! GPU OOM Offloading is ON:\n"
+            "This is meant for training models that would be impossible otherwise due to OOM.\n"
+            "Note that this comes at a speed cost and SHOULD NOT be used if your training fits in GPU memory without it.\n"
+            "Please also consider whether a smaller model is a more appropriate solution!\n"
+            "Also, a warning from PyTorch: 'If you overuse pinned memory, it can cause serious problems when running low on RAM!'"
+        )
+        with torch.autograd.graph.save_on_cpu(pin_memory=True):
+            trainer.train()
+    else:
+        trainer.train()
 
     return
 
 
 def parse_command_line(args=None):
     parser = argparse.ArgumentParser(
         description="Train (or restart training of) a NequIP model."
@@ -101,48 +127,70 @@
     )
     parser.add_argument(
         "--grad-anomaly-mode",
         help="enable PyTorch autograd anomaly mode to debug NaN gradients. Do not use for production training!",
         action="store_true",
     )
     parser.add_argument(
+        "--gpu-oom-offload",
+        help="Use `torch.autograd.graph.save_on_cpu` to offload intermediate tensors to CPU (host) memory in order to train models that would be impossible otherwise due to OOM. Note that this comes as at a speed cost and SHOULD NOT be used if your training fits in GPU memory without it. Please also consider whether a smaller model is a more appropriate solution.",
+        action="store_true",
+    )
+    parser.add_argument(
         "--log",
         help="log file to store all the screen logging",
         type=Path,
         default=None,
     )
+    parser.add_argument(
+        "--warn-unused",
+        help="Warn instead of error when the config contains unused keys",
+        action="store_true",
+    )
     args = parser.parse_args(args=args)
 
     config = Config.from_file(args.config, defaults=default_config)
-    for flag in ("model_debug_mode", "equivariance_test", "grad_anomaly_mode"):
+    for flag in (
+        "model_debug_mode",
+        "equivariance_test",
+        "grad_anomaly_mode",
+        "warn_unused",
+        "gpu_oom_offload",
+    ):
         config[flag] = getattr(args, flag) or config[flag]
 
     return config
 
 
 def fresh_start(config):
     # we use add_to_config cause it's a fresh start and need to record it
     check_code_version(config, add_to_config=True)
     _set_global_options(config)
+    if config["default_dtype"] != "float64":
+        warnings.warn(
+            f"default_dtype={config['default_dtype']} but we strongly recommend float64"
+        )
 
     # = Make the trainer =
     if config.wandb:
+
         import wandb  # noqa: F401
-        from nequip.train.trainer_wandb import TrainerWandB
+        from nequip.train.trainer_wandb import TrainerWandB as Trainer
 
         # download parameters from wandb in case of sweeping
         from nequip.utils.wandb import init_n_update
 
         config = init_n_update(config)
 
-        trainer = TrainerWandB(model=None, **dict(config))
+    elif config.tensorboard:
+        from nequip.train.trainer_tensorboard import TrainerTensorBoard as Trainer
     else:
         from nequip.train.trainer import Trainer
 
-        trainer = Trainer(model=None, **dict(config))
+    trainer = Trainer(model=None, **Config.as_dict(config))
 
     # what is this
     # to update wandb data?
     config.update(trainer.params)
 
     # = Load the dataset =
     dataset = dataset_from_config(config, prefix="dataset")
@@ -161,17 +209,14 @@
 
     # = Build model =
     final_model = model_from_config(
         config=config, initialize=True, dataset=trainer.dataset_train
     )
     logging.info("Successfully built the network...")
 
-    # by doing this here we check also any keys custom builders may have added
-    _check_old_keys(config)
-
     # Equivar test
     if config.equivariance_test > 0:
         n_train: int = len(trainer.dataset_train)
         assert config.equivariance_test <= n_train
         final_model.eval()
         indexes = torch.randperm(n_train)[: config.equivariance_test]
         errstr = assert_AtomicData_equivariant(
@@ -191,14 +236,27 @@
 
     # Set the trainer
     trainer.model = final_model
 
     # Store any updated config information in the trainer
     trainer.update_kwargs(config)
 
+    # Only run the unused check as a callback after the trainer has
+    # initialized everything (metrics, early stopping, etc.)
+    def _unused_check():
+        unused = config._unused_keys()
+        if len(unused) > 0:
+            message = f"The following keys in the config file were not used, did you make a typo?: {', '.join(unused)}. (If this sounds wrong, please file an issue. You can turn this error into a warning with `--warn-unused`, but please make sure that the key really is correctly spelled and used!.)"
+            if config.warn_unused:
+                warnings.warn(message)
+            else:
+                raise KeyError(message)
+
+    trainer._post_init_callback = _unused_check
+
     return trainer
 
 
 def restart(config):
     # load the dictionary
     restart_file = f"{config.root}/{config.run_name}/trainer.pth"
     dictionary = load_file(
@@ -258,20 +316,9 @@
         # It couldn't be found
         validation_dataset = None
     trainer.set_dataset(dataset, validation_dataset)
 
     return trainer
 
 
-def _check_old_keys(config) -> None:
-    """check ``config`` for old/depricated keys and emit corresponding errors/warnings"""
-    # compile_model
-    k = "compile_model"
-    if k in config:
-        if config[k]:
-            raise ValueError("the `compile_model` option has been removed")
-        else:
-            warnings.warn("the `compile_model` option has been removed")
-
-
 if __name__ == "__main__":
     main(running_as_script=True)
```

### Comparing `nequip-0.5.6/nequip/train/_loss.py` & `nequip-0.6.0/nequip/train/_loss.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import logging
 
 import torch.nn
 from torch_runstats.scatter import scatter, scatter_mean
 
-from nequip.data import AtomicDataDict
+from nequip.data import AtomicDataDict, _GRAPH_FIELDS
 from nequip.utils import instantiate_from_cls_name
 
 
 class SimpleLoss:
     """wrapper to compute weighted loss function
 
     Args:
@@ -40,61 +40,70 @@
     def __call__(
         self,
         pred: dict,
         ref: dict,
         key: str,
         mean: bool = True,
     ):
+        ref = ref[key]
+        # make sure prediction is promoted to dtype of reference
+        pred = pred[key].to(ref.dtype)
         # zero the nan entries
-        has_nan = self.ignore_nan and torch.isnan(ref[key].mean())
+        has_nan = self.ignore_nan and torch.isnan(ref.mean())
         if has_nan:
-            not_nan = (ref[key] == ref[key]).int()
-            loss = self.func(pred[key], torch.nan_to_num(ref[key], nan=0.0)) * not_nan
+            not_nan = (ref == ref).int()
+            loss = self.func(pred, torch.nan_to_num(ref, nan=0.0)) * not_nan
             if mean:
                 return loss.sum() / not_nan.sum()
             else:
                 return loss
         else:
-            loss = self.func(pred[key], ref[key])
+            loss = self.func(pred, ref)
             if mean:
                 return loss.mean()
             else:
                 return loss
 
 
 class PerAtomLoss(SimpleLoss):
     def __call__(
         self,
         pred: dict,
         ref: dict,
         key: str,
         mean: bool = True,
     ):
+        if key not in _GRAPH_FIELDS:
+            raise RuntimeError(
+                f"Doesn't make sense to do a `PerAtom` loss on field `{key}`, which isn't registered as a graph (global) field. If it is a graph-level field, register it with `graph_fields: [\"{key}\"]`; otherwise you don't need to specify `PerAtom` for loss on per-node fields."
+            )
+        ref_dict = ref
+        ref = ref[key]
+        # make sure prediction is promoted to dtype of reference
+        pred = pred[key].to(ref.dtype)
         # zero the nan entries
-        has_nan = self.ignore_nan and torch.isnan(ref[key].sum())
-        N = torch.bincount(ref[AtomicDataDict.BATCH_KEY])
+        has_nan = self.ignore_nan and torch.isnan(ref.sum())
+        N = torch.bincount(ref_dict[AtomicDataDict.BATCH_KEY])
         N = N.reshape((-1, 1))
         if has_nan:
-            not_nan = (ref[key] == ref[key]).int()
-            loss = (
-                self.func(pred[key], torch.nan_to_num(ref[key], nan=0.0)) * not_nan / N
-            )
+            not_nan = (ref == ref).int()
+            loss = self.func(pred, torch.nan_to_num(ref, nan=0.0)) * not_nan / N
             if self.func_name == "MSELoss":
                 loss = loss / N
-            assert loss.shape == pred[key].shape  # [atom, dim]
+            assert loss.shape == pred.shape  # [atom, dim]
             if mean:
                 return loss.sum() / not_nan.sum()
             else:
                 return loss
         else:
-            loss = self.func(pred[key], ref[key])
+            loss = self.func(pred, ref)
             loss = loss / N
             if self.func_name == "MSELoss":
                 loss = loss / N
-            assert loss.shape == pred[key].shape  # [atom, dim]
+            assert loss.shape == pred.shape  # [atom, dim]
             if mean:
                 return loss.mean()
             else:
                 return loss
 
 
 class PerSpeciesLoss(SimpleLoss):
@@ -109,28 +118,30 @@
         pred: dict,
         ref: dict,
         key: str,
         mean: bool = True,
     ):
         if not mean:
             raise NotImplementedError("Cannot handle this yet")
+        ref = ref[key]
+        # make sure prediction is promoted to dtype of reference
+        pred_dict = pred
+        pred = pred[key].to(ref.dtype)
 
-        has_nan = self.ignore_nan and torch.isnan(ref[key].mean())
+        has_nan = self.ignore_nan and torch.isnan(ref.mean())
 
         if has_nan:
-            not_nan = (ref[key] == ref[key]).int()
-            per_atom_loss = (
-                self.func(pred[key], torch.nan_to_num(ref[key], nan=0.0)) * not_nan
-            )
+            not_nan = (ref == ref).int()
+            per_atom_loss = self.func(pred, torch.nan_to_num(ref, nan=0.0)) * not_nan
         else:
-            per_atom_loss = self.func(pred[key], ref[key])
+            per_atom_loss = self.func(pred, ref)
 
         reduce_dims = tuple(i + 1 for i in range(len(per_atom_loss.shape) - 1))
 
-        spe_idx = pred[AtomicDataDict.ATOM_TYPE_KEY].squeeze(-1)
+        spe_idx = pred_dict[AtomicDataDict.ATOM_TYPE_KEY].squeeze(-1)
         if has_nan:
             if len(reduce_dims) > 0:
                 per_atom_loss = per_atom_loss.sum(dim=reduce_dims)
             assert per_atom_loss.ndim == 1
 
             per_species_loss = scatter(per_atom_loss, spe_idx, dim=0)
```

### Comparing `nequip-0.5.6/nequip/train/early_stopping.py` & `nequip-0.6.0/nequip/train/early_stopping.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/train/loss.py` & `nequip-0.6.0/nequip/train/loss.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,18 +35,15 @@
         - outputs a vector with the same shape as pred/ref
 
     """
 
     def __init__(
         self,
         coeffs: Union[dict, str, List[str]],
-        coeff_schedule: str = "constant",
     ):
-
-        self.coeff_schedule = coeff_schedule
         self.coeffs = {}
         self.funcs = {}
         self.keys = []
 
         mseloss = find_loss_function("MSELoss", {})
         if isinstance(coeffs, str):
             self.coeffs[coeffs] = 1.0
```

### Comparing `nequip-0.5.6/nequip/train/metrics.py` & `nequip-0.6.0/nequip/train/metrics.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/train/trainer.py` & `nequip-0.6.0/nequip/train/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,30 +22,38 @@
     # has backport of nullcontext
     import contextlib2 as contextlib
 
 import numpy as np
 import torch
 from torch_ema import ExponentialMovingAverage
 
-from nequip.data import DataLoader, AtomicData, AtomicDataDict, AtomicDataset
+from nequip.data import (
+    DataLoader,
+    PartialSampler,
+    AtomicData,
+    AtomicDataDict,
+    AtomicDataset,
+)
+from nequip.nn import GraphModel
 from nequip.utils import (
     Output,
     Config,
     instantiate_from_cls_name,
     instantiate,
     save_file,
     load_file,
     load_callable,
     atomic_write,
     finish_all_writes,
     atomic_write_group,
-    dtype_from_name,
 )
 from nequip.utils.versions import check_code_version
 from nequip.model import model_from_config
+from nequip.utils.config import _GLOBAL_ALL_ASKED_FOR_KEYS
+from nequip.utils.misc import get_default_device_name
 
 from .loss import Loss, LossStat
 from .metrics import Metrics
 from ._key import ABBREV, LOSS_KEY, TRAIN, VALIDATION
 from .early_stopping import EarlyStopping
 
 
@@ -146,14 +154,15 @@
         optimizer_name (str): name for optimizer
         optim_kwargs (dict): parameters to initialize the optimizer
 
         batch_size (int): size of each batch
         validation_batch_size (int): batch size for evaluating the model for validation
         shuffle (bool): parameters for dataloader
         n_train (int): # of frames for training
+        n_train_per_epoch (optional int): how many frames from `n_train` to use each epoch; see `PartialSampler`. When `None`, all `n_train` frames will be used each epoch.
         n_val (int): # of frames for validation
         exclude_keys (list):  fields from dataset to ignore.
         dataloader_num_workers (int): `num_workers` for the `DataLoader`s
         train_idcs (optional, list):  list of frames to use for training
         val_idcs (list):  list of frames to use for validation
         train_val_split (str):  "random" or "sequential"
 
@@ -207,19 +216,21 @@
     """
 
     stop_keys = ["max_epochs", "early_stopping", "early_stopping_kwargs"]
     object_keys = ["lr_sched", "optim", "ema", "early_stopping_conds"]
     lr_scheduler_module = torch.optim.lr_scheduler
     optim_module = torch.optim
 
+    model: GraphModel
+
     def __init__(
         self,
         model,
         model_builders: Optional[list] = [],
-        device: str = "cuda" if torch.cuda.is_available() else "cpu",
+        device: str = get_default_device_name(),
         seed: Optional[int] = None,
         dataset_seed: Optional[int] = None,
         loss_coeffs: Union[dict, str] = AtomicDataDict.TOTAL_ENERGY_KEY,
         train_on_keys: Optional[List[str]] = None,
         metrics_components: Optional[Union[dict, str]] = None,
         metrics_key: str = f"{VALIDATION}_" + ABBREV.get(LOSS_KEY, LOSS_KEY),
         early_stopping_conds: Optional[EarlyStopping] = None,
@@ -236,25 +247,27 @@
         ema_decay: float = 0.999,
         ema_use_num_updates=True,
         exclude_keys: list = [],
         batch_size: int = 5,
         validation_batch_size: int = 5,
         shuffle: bool = True,
         n_train: Optional[int] = None,
+        n_train_per_epoch: Optional[int] = None,
         n_val: Optional[int] = None,
         dataloader_num_workers: int = 0,
         train_idcs: Optional[list] = None,
         val_idcs: Optional[list] = None,
         train_val_split: str = "random",
         init_callbacks: list = [],
+        start_of_epoch_callbacks: list = [],
         end_of_epoch_callbacks: list = [],
         end_of_batch_callbacks: list = [],
         end_of_train_callbacks: list = [],
         final_callbacks: list = [],
-        log_batch_freq: int = 1,
+        log_batch_freq: int = 100,
         log_epoch_freq: int = 1,
         save_checkpoint_freq: int = -1,
         save_ema_checkpoint_freq: int = -1,
         report_init_validation: bool = True,
         verbose="INFO",
         **kwargs,
     ):
@@ -265,14 +278,16 @@
         # store all init arguments
         self.model = model
 
         _local_kwargs = {}
         for key in self.init_keys:
             setattr(self, key, locals()[key])
             _local_kwargs[key] = locals()[key]
+            # all init_keys of the Trainer are valid config keys
+            _GLOBAL_ALL_ASKED_FOR_KEYS.add(key)
 
         self.ema = None
 
         output = Output.get_output(dict(**_local_kwargs, **kwargs))
         self.output = output
 
         self.logfile = output.open_logfile("log", propagate=True)
@@ -291,21 +306,22 @@
 
         # add filenames if not defined
         self.best_model_path = output.generate_file("best_model.pth")
         self.last_model_path = output.generate_file("last_model.pth")
         self.trainer_save_path = output.generate_file("trainer.pth")
         self.config_path = self.output.generate_file("config.yaml")
 
-        if seed is not None:
-            torch.manual_seed(seed)
-            np.random.seed(seed)
+        if seed is None:
+            raise ValueError("seed is required")
+
+        torch.manual_seed(seed)
+        np.random.seed(seed)
 
         self.dataset_rng = torch.Generator()
-        if dataset_seed is not None:
-            self.dataset_rng.manual_seed(dataset_seed)
+        self.dataset_rng.manual_seed(dataset_seed if dataset_seed is not None else seed)
 
         self.logger.info(f"Torch device: {self.device}")
         self.torch_device = torch.device(self.device)
 
         # sort out all the other parameters
         # for samplers, optimizer and scheduler
         self.kwargs = deepcopy(kwargs)
@@ -326,34 +342,20 @@
         )
         self.loss_stat = LossStat(self.loss)
 
         # what do we train on?
         self.train_on_keys = self.loss.keys
         if train_on_keys is not None:
             assert set(train_on_keys) == set(self.train_on_keys)
-        self._remove_from_model_input = set(self.train_on_keys)
-        if (
-            len(
-                self._remove_from_model_input.intersection(
-                    AtomicDataDict.ALL_ENERGY_KEYS
-                )
-            )
-            > 0
-        ):
-            # if we are training on _any_ of the energy quantities (energy, force, partials, stress, etc.)
-            # then none of them should be fed into the model
-            self._remove_from_model_input = self._remove_from_model_input.union(
-                AtomicDataDict.ALL_ENERGY_KEYS
-            )
-        if kwargs.get("_override_allow_truth_label_inputs", False):
-            # needed for unit testing models
-            self._remove_from_model_input = set()
 
         # load all callbacks
         self._init_callbacks = [load_callable(callback) for callback in init_callbacks]
+        self._start_of_epoch_callbacks = [
+            load_callable(callback) for callback in start_of_epoch_callbacks
+        ]
         self._end_of_epoch_callbacks = [
             load_callable(callback) for callback in end_of_epoch_callbacks
         ]
         self._end_of_batch_callbacks = [
             load_callable(callback) for callback in end_of_batch_callbacks
         ]
         self._end_of_train_callbacks = [
@@ -667,59 +669,60 @@
     @staticmethod
     def load_model_from_training_session(
         traindir,
         model_name="best_model.pth",
         device="cpu",
         config_dictionary: Optional[dict] = None,
     ) -> Tuple[torch.nn.Module, Config]:
+        """Load a model from a training session.
+
+        Note that this uses ``model_from_config`` internally and is thus not thread safe.
+
+        Args:
+            traindir: the training session
+            model_name: which checkpoint to load; defaults to ``best_model.pth``
+            device: target device to load to, defaults to ``cpu``
+            config_dictionary: optionally use this config instead of ``traindir/config.yaml``
+
+        Returns:
+            (model, config)
+        """
         traindir = str(traindir)
         model_name = str(model_name)
 
         if config_dictionary is not None:
             config = Config.from_dict(config_dictionary)
         else:
             config = Config.from_file(traindir + "/config.yaml")
 
+        # model_from_config takes care of dtypes already
         model = model_from_config(
             config=config,
             initialize=False,
         )
-        if model is not None:  # TODO: why would it be?
-            # TODO: this is not exactly equivalent to building with
-            # this set as default dtype... does it matter?
-            model.to(
-                device=torch.device(device),
-                dtype=dtype_from_name(config.default_dtype),
-            )
-            model_state_dict = torch.load(
-                traindir + "/" + model_name, map_location=device
-            )
-            model.load_state_dict(model_state_dict)
+        model.to(device=torch.device(device))
+        model_state_dict = torch.load(traindir + "/" + model_name, map_location=device)
+        model.load_state_dict(model_state_dict)
 
         return model, config
 
     def init(self):
         """initialize optimizer"""
         if self.model is None:
             return
+        assert isinstance(self.model, GraphModel)
 
         self.model.to(self.torch_device)
 
         self.num_weights = sum(p.numel() for p in self.model.parameters())
         self.logger.info(f"Number of weights: {self.num_weights}")
         self.logger.info(
             f"Number of trainable weights: {sum(p.numel() for p in self.model.parameters() if p.requires_grad)}"
         )
 
-        self.rescale_layers = []
-        outer_layer = self.model
-        while hasattr(outer_layer, "unscale"):
-            self.rescale_layers.append(outer_layer)
-            outer_layer = getattr(outer_layer, "model", None)
-
         self.init_objects()
 
         self._initialized = True
         self.cumulative_wall = 0
 
     def init_metrics(self):
         if self.metrics_components is None:
@@ -769,14 +772,17 @@
             if self.iepoch == -1:
                 self.save()
             if self.iepoch in [-1, 0]:
                 self.save_config()
 
         self.init_metrics()
 
+        if getattr(self, "_post_init_callback", None) is not None:
+            self._post_init_callback()
+
         while not self.stop_cond:
 
             self.epoch_step()
             self.end_of_epoch_save()
 
         for callback in self._final_callbacks:
             callback(self)
@@ -795,40 +801,30 @@
         else:
             self.model.train()
 
         # Do any target rescaling
         data = data.to(self.torch_device)
         data = AtomicData.to_AtomicDataDict(data)
 
-        data_unscaled = data
-        for layer in self.rescale_layers:
-            # This means that self.model is RescaleOutputs
-            # this will normalize the targets
-            # in validation (eval mode), it does nothing
-            # in train mode, if normalizes the targets
-            data_unscaled = layer.unscale(data_unscaled)
+        # this will normalize the targets
+        # in both validation and train we want targets normalized _for the loss_
+        data_for_loss = self.model.unscale(data, force_process=True)
 
         # Run model
         # We make a shallow copy of the input dict in case the model modifies it
-        input_data = {
-            k: v
-            for k, v in data_unscaled.items()
-            if k not in self._remove_from_model_input
-        }
-        out = self.model(input_data)
-        del input_data
+        out = self.model(data_for_loss)
 
         # If we're in evaluation mode (i.e. validation), then
-        # data_unscaled's target prop is unnormalized, and out's has been rescaled to be in the same units
-        # If we're in training, data_unscaled's target prop has been normalized, and out's hasn't been touched, so they're both in normalized units
-        # Note that either way all normalization was handled internally by RescaleOutput
+        # data_for_loss's target prop is unnormalized, and out's has been rescaled to be in the same units
+        # If we're in training, data_for_loss's target prop has been normalized, and out's hasn't been touched, so they're both in normalized units
+        # Note that either way all normalization was handled internally by GraphModel via RescaleOutput
 
         if not validation:
             # Actually do an optimization step, since we're training:
-            loss, loss_contrib = self.loss(pred=out, ref=data_unscaled)
+            loss, loss_contrib = self.loss(pred=out, ref=data_for_loss)
             # see https://pytorch.org/tutorials/recipes/recipes/tuning_guide.html#use-parameter-grad-none-instead-of-model-zero-grad-or-optimizer-zero-grad
             self.optim.zero_grad(set_to_none=True)
             loss.backward()
 
             # See https://stackoverflow.com/a/56069467
             # Has to happen after .backward() so there are grads to clip
             if self.max_gradient_norm < float("inf"):
@@ -842,33 +838,34 @@
                 self.ema.update()
 
             if self.lr_scheduler_name == "CosineAnnealingWarmRestarts":
                 self.lr_sched.step(self.iepoch + self.ibatch / self.n_batches)
 
         with torch.no_grad():
             if validation:
-                scaled_out = out
-                _data_unscaled = data
-                for layer in self.rescale_layers:
-                    # loss function always needs to be in normalized unit
-                    scaled_out = layer.unscale(scaled_out, force_process=True)
-                    _data_unscaled = layer.unscale(_data_unscaled, force_process=True)
-                loss, loss_contrib = self.loss(pred=scaled_out, ref=_data_unscaled)
+                # loss function always needs to be in normalized unit
+                normalized_units_out = self.model.unscale(out, force_process=True)
+                # data_for_loss is always forced into normalized units
+                loss, loss_contrib = self.loss(
+                    pred=normalized_units_out, ref=data_for_loss
+                )
+                del normalized_units_out
+                # everything else is already in real units for metrics, so do nothing
             else:
                 # If we are in training mode, we need to bring the prediction
-                # into real units
-                for layer in self.rescale_layers[::-1]:
-                    out = layer.scale(out, force_process=True)
+                # into real units for metrics
+                out = self.model.scale(out, force_process=True)
 
             # save metrics stats
             self.batch_losses = self.loss_stat(loss, loss_contrib)
-            # in validation mode, data is in real units and the network scales
+            # in validation mode, reference data is in real units and the network scales
             # out to be in real units interally.
-            # in training mode, data is still in real units, and we rescaled
-            # out to be in real units above.
+            # in training mode, reference data is still in real units, and we rescaled
+            # network predicted out to be in real units right above
+            # thus, we get metrics in real units always:
             self.batch_metrics = self.metrics(pred=out, ref=data)
 
     @property
     def stop_cond(self):
         """kill the training early"""
 
         if self.early_stopping_conds is not None and hasattr(self, "mae_dict"):
@@ -890,20 +887,26 @@
     def reset_metrics(self):
         self.loss_stat.reset()
         self.loss_stat.to(self.torch_device)
         self.metrics.reset()
         self.metrics.to(self.torch_device)
 
     def epoch_step(self):
+        for callback in self._start_of_epoch_callbacks:
+            callback(self)
 
         dataloaders = {TRAIN: self.dl_train, VALIDATION: self.dl_val}
         categories = [TRAIN, VALIDATION] if self.iepoch >= 0 else [VALIDATION]
         dataloaders = [
             dataloaders[c] for c in categories
         ]  # get the right dataloaders for the catagories we actually run
+        if TRAIN in categories:
+            # We have to step the sampler so it knows what epoch it is
+            self.dl_train_sampler.step_epoch(self.iepoch)
+
         self.metrics_dict = {}
         self.loss_dict = {}
 
         for category, dataset in zip(categories, dataloaders):
             if category == VALIDATION and self.use_ema:
                 cm = self.ema.average_parameters()
             else:
@@ -1217,18 +1220,29 @@
             # PyTorch recommends this for GPU since it makes copies much faster
             pin_memory=(self.torch_device != torch.device("cpu")),
             # avoid getting stuck
             timeout=(10 if self.dataloader_num_workers > 0 else 0),
             # use the right randomness
             generator=self.dataset_rng,
         )
+        if self.n_train_per_epoch is not None:
+            assert self.n_train_per_epoch % self.batch_size == 0
+        self.dl_train_sampler = PartialSampler(
+            data_source=self.dataset_train,
+            # training should shuffle (if enabled)
+            shuffle=self.shuffle,
+            # if n_train_per_epoch is None (default), it's set to len(self.dataset_train) == n_train
+            # i.e. use all `n_train` frames each epoch
+            num_samples_per_epoch=self.n_train_per_epoch,
+            generator=self.dataset_rng,
+        )
         self.dl_train = DataLoader(
             dataset=self.dataset_train,
-            shuffle=self.shuffle,  # training should shuffle
             batch_size=self.batch_size,
+            sampler=self.dl_train_sampler,
             **dl_kwargs,
         )
         # validation, on the other hand, shouldn't shuffle
         # we still pass the generator just to be safe
         self.dl_val = DataLoader(
             dataset=self.dataset_val,
             batch_size=self.validation_batch_size,
```

### Comparing `nequip-0.5.6/nequip/train/trainer_wandb.py` & `nequip-0.6.0/nequip/train/trainer_wandb.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/__init__.py` & `nequip-0.6.0/nequip/utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     atomic_write,
     finish_all_writes,
     atomic_write_group,
 )
 from .config import Config
 from .output import Output
 from .modules import find_first_of_type
-from .misc import dtype_from_name
+from .misc import dtype_from_name, torch_default_dtype
 
 __all__ = [
     instantiate_from_cls_name,
     instantiate,
     get_w_prefix,
     save_file,
     load_file,
@@ -26,8 +26,9 @@
     atomic_write,
     finish_all_writes,
     atomic_write_group,
     Config,
     Output,
     find_first_of_type,
     dtype_from_name,
+    torch_default_dtype,
 ]
```

### Comparing `nequip-0.5.6/nequip/utils/auto_init.py` & `nequip-0.6.0/nequip/utils/auto_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Union, List
 import inspect
 import logging
 
-from .config import Config
+from .config import Config, _GLOBAL_ALL_ASKED_FOR_KEYS
 
 
 def instantiate_from_cls_name(
     module,
     class_name: str,
     prefix: Optional[Union[str, List[str]]] = [],
     positional_args: dict = {},
@@ -136,15 +136,15 @@
     if "all" in key_mapping and "optional" in key_mapping:
         key_mapping["all"] = {
             k: v
             for k, v in key_mapping["all"].items()
             if k not in key_mapping["optional"]
         }
 
-    final_optional_args = dict(config)
+    final_optional_args = Config.as_dict(config)
 
     # for nested argument, it is possible that the positional args contain unnecesary keys
     if len(parent_builders) > 0:
         _positional_args = {
             k: v for k, v in positional_args.items() if k in config.allow_list()
         }
         positional_args = _positional_args
@@ -209,29 +209,40 @@
 
     # remove duplicates
     for key in positional_args:
         final_optional_args.pop(key, None)
         for t in key_mapping:
             key_mapping[t].pop(key, None)
 
-    if return_args_only:
-        return key_mapping, final_optional_args
-
     # debug info
-    logging.debug(f"instantiate {builder.__name__}")
-    for t in key_mapping:
-        for k, v in key_mapping[t].items():
-            string = f" {t:>10s}_args :  {k:>50s}"
-            if k != v:
-                string += f" <- {v:>50s}"
-            logging.debug(string)
-    logging.debug(f"...{builder.__name__}_param = dict(")
-    logging.debug(f"...   optional_args = {final_optional_args},")
-    logging.debug(f"...   positional_args = {positional_args})")
+    if len(parent_builders) == 0:
+        # ^ we only want to log or consume arguments for the "unused keys" check
+        #   if this is a root-level build. For subbuilders, we don't want to log
+        #   or, worse, mark keys without prefixes as consumed.
+        logging.debug(
+            f"{'get args for' if return_args_only else 'instantiate'} {builder.__name__}"
+        )
+        for t in key_mapping:
+            for k, v in key_mapping[t].items():
+                string = f" {t:>10s}_args :  {k:>50s}"
+                # key mapping tells us how values got from the
+                # users config (v) to the object being built (k)
+                # thus v is by definition a valid key
+                _GLOBAL_ALL_ASKED_FOR_KEYS.add(v)
+                if k != v:
+                    string += f" <- {v:>50s}"
+                logging.debug(string)
+        logging.debug(f"...{builder.__name__}_param = dict(")
+        logging.debug(f"...   optional_args = {final_optional_args},")
+        logging.debug(f"...   positional_args = {positional_args})")
 
+    # Short circuit for return_args_only
+    if return_args_only:
+        return key_mapping, final_optional_args
+    # Otherwise, actually build the thing:
     try:
         instance = builder(**positional_args, **final_optional_args)
     except Exception as e:
         raise RuntimeError(
             f"Failed to build object with prefix `{prefix}` using builder `{builder.__name__}`"
         ) from e
```

### Comparing `nequip-0.5.6/nequip/utils/batch_ops.py` & `nequip-0.6.0/nequip/utils/batch_ops.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/config.py` & `nequip-0.6.0/nequip/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,23 +30,30 @@
     ```
     config.update(dictionary={'a':3, 'b':4})
     ```
 
     If a parameter is updated, the updated value will be formatted back to the same type.
 
 """
+from typing import Set, Dict, Any, List
+
 import inspect
 
 from copy import deepcopy
 from typing import Optional
 
 from nequip.utils.savenload import save_file, load_file
 
 
+_GLOBAL_ALL_ASKED_FOR_KEYS: Set[str] = set()
+
+
 class Config(object):
+    _items: Dict[str, Any]
+
     def __init__(
         self,
         config: Optional[dict] = None,
         allow_list: Optional[list] = None,
         exclude_keys: Optional[list] = None,
     ):
 
@@ -72,18 +79,28 @@
 
     def keys(self):
         return self._items.keys()
 
     def _as_dict(self):
         return self._items
 
-    def as_dict(self):
-        return dict(self)
+    @staticmethod
+    def as_dict(obj):
+        # don't use `dict(self)`, since that
+        # calls __getitem__
+        if isinstance(obj, dict):
+            return obj.copy()
+        elif isinstance(obj, Config):
+            return obj._items.copy()
+        else:
+            raise TypeError
 
     def __getitem__(self, key):
+        # any requested key is a valid key
+        _GLOBAL_ALL_ASKED_FOR_KEYS.add(key)
         return self._items[key]
 
     def get_type(self, key):
         """Get Typehint from item_types dict or previous defined value
         Args:
 
             key: name of the variable
@@ -111,15 +128,14 @@
         )
         self.update(default_values)
 
     def allow_list(self):
         return self._allow_list
 
     def __setitem__(self, key, val):
-
         # typehint
         if key.endswith("_type") and key.startswith("_"):
 
             k = key[1:-5]
             if (not self._allow_all) and key not in self._allow_list:
                 return None
 
@@ -153,14 +169,15 @@
     def __getattr__(self, key):
         return self.__getitem__(key)
 
     def __contains__(self, key):
         return key in self._items
 
     def pop(self, *args):
+        _GLOBAL_ALL_ASKED_FOR_KEYS.add(args[0])
         return self._items.pop(*args)
 
     def update_w_prefix(
         self,
         dictionary: dict,
         prefix: str,
         allow_val_change=None,
@@ -183,15 +200,15 @@
         l_prefix = len(prefix) + 1
         prefix_dict = {
             k[l_prefix:]: v for k, v in dictionary.items() if k.startswith(prefix + "_")
         }
         keys = self.update(prefix_dict, allow_val_change=allow_val_change)
         keys = {k: f"{prefix}_{k}" for k in keys}
 
-        for suffix in ["params", "kwargs"]:
+        for suffix in ["kwargs"]:
             if f"{prefix}_{suffix}" in dictionary:
                 key3 = self.update(
                     dictionary[f"{prefix}_{suffix}"],
                     allow_val_change=allow_val_change,
                 )
                 keys.update({k: f"{prefix}_{suffix}.{k}" for k in key3})
         return keys
@@ -223,14 +240,15 @@
         for k, value in dictionary.items():
             if not k.startswith("_"):
                 keys += [self.__setitem__(k, value)]
 
         return set(keys) - set([None])
 
     def get(self, *args):
+        _GLOBAL_ALL_ASKED_FOR_KEYS.add(args[0])
         return self._items.get(*args)
 
     def persist(self):
         """mock wandb.config function"""
         pass
 
     def setdefaults(self, d):
@@ -250,22 +268,49 @@
             supported_formats=supported_formats,
             filename=filename,
             enforced_format=format,
         )
 
     @staticmethod
     def from_file(filename: str, format: Optional[str] = None, defaults: dict = {}):
-        """Load arguments from file"""
+        """Load arguments from file
+
+        Has support for including another config file as a baseline with:
+        ```
+        # example of using another config as a baseline and overriding only selected options
+        # this option will read in configs/minimal.yaml and take ALL keys from that file
+        include_file_as_baseline_config: configs/minimal.yaml
+        # keys specified in this file WILL OVERRIDE keys from the `include_file_as_baseline_config` file
+        l_max: 1  # overrides l_max: 2 in minimal.yaml
+        ```
+        """
 
         supported_formats = {"yaml": ("yml", "yaml"), "json": "json"}
         dictionary = load_file(
             supported_formats=supported_formats,
             filename=filename,
             enforced_format=format,
         )
+        k: str = "include_file_as_baseline_config"
+        if k in dictionary:
+            # allow one level of subloading
+            baseline_fname = dictionary.pop(k)
+            dictionary_baseline = load_file(
+                supported_formats=supported_formats,
+                filename=baseline_fname,
+                enforced_format=format,
+            )
+            if k in dictionary_baseline:
+                raise NotImplementedError(
+                    f"Multiple levels of `{k}` are not allowed, but {baseline_fname} contained `{k}`"
+                )
+            # override baseline options with the main config
+            dictionary_baseline.update(dictionary)
+            dictionary = dictionary_baseline
+            del dictionary_baseline, baseline_fname
         return Config.from_dict(dictionary, defaults)
 
     @staticmethod
     def from_dict(dictionary: dict, defaults: dict = {}):
         c = Config(defaults)
         c.update(dictionary)
         return c
@@ -334,7 +379,14 @@
         elif "kwargs" in param_keys:
             param_keys.remove("kwargs")
             return Config(config=default_params, allow_list=param_keys)
         else:
             return Config(config=default_params, allow_list=param_keys)
 
     load = from_file
+
+    def _get_nomark(self, key: str) -> Any:
+        return self._items.get(key)
+
+    def _unused_keys(self) -> List[str]:
+        unused = [k for k in self.keys() if k not in _GLOBAL_ALL_ASKED_FOR_KEYS]
+        return unused
```

### Comparing `nequip-0.5.6/nequip/utils/git.py` & `nequip-0.6.0/nequip/utils/git.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/multiprocessing.py` & `nequip-0.6.0/nequip/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/output.py` & `nequip-0.6.0/nequip/utils/output.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/regressor.py` & `nequip-0.6.0/nequip/utils/regressor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import torch
 
 from torch import matmul
-from torch.linalg import solve, inv
 from typing import Optional, Sequence
 from opt_einsum import contract
 
 
 def solver(X, y, alpha: Optional[float] = 0.001, stride: Optional[int] = 1, **kwargs):
     # results are in the same "units" as y, so same dtype too:
     dtype_out = y.dtype
@@ -22,24 +21,28 @@
     X = X / X_norm
     y = y / X_norm
 
     y_mean = torch.sum(y) / torch.sum(X)
 
     feature_rms = torch.sqrt(torch.mean(X**2, axis=0))
 
-    alpha_mat = torch.diag(feature_rms) * alpha * alpha
+    alpha_mat = torch.diag(feature_rms) * (alpha * alpha)
 
     A = matmul(X.T, X) + alpha_mat
     dy = y - (torch.sum(X, axis=1, keepdim=True) * y_mean).reshape(y.shape)
     Xy = matmul(X.T, dy)
 
-    mean = solve(A, Xy)
+    # A is symmetric positive semidefinite <=> A=(X + alpha*I)^T (X + alpha*I),
+    # so we can use cholesky:
+    A_cholesky = torch.linalg.cholesky(A)
+    mean = torch.cholesky_solve(Xy.unsqueeze(-1), A_cholesky).squeeze(-1)
+    Ainv = torch.cholesky_inverse(A_cholesky)
+    del A_cholesky
 
     sigma2 = torch.var(matmul(X, mean) - dy)
-    Ainv = inv(A)
     cov = torch.sqrt(sigma2 * contract("ij,kj,kl,li->i", Ainv, X, X, Ainv))
 
     mean = mean + y_mean.reshape([-1])
 
     logging.debug(f"Ridge Regression, residue {sigma2}")
 
     return mean.to(dtype_out), cov.to(dtype_out)
@@ -66,11 +69,14 @@
     new_X = torch.zeros(
         (n_types * n_points, X.shape[1]), dtype=X.dtype, device=X.device
     )
     new_y = torch.zeros((n_types * n_points), dtype=y.dtype, device=y.device)
     for i in range(n_types):
         ids = sort_by[id_start[i] : id_end[i]]
         for j, p in enumerate(percentage):
-            new_y[i * n_points + j] = torch.quantile(y[ids], p, interpolation="linear")
+            # it defaults to linear anyway, and `interpolation` was a 1.11 addition
+            # so we leave out `, interpolation="linear")`
+            # https://pytorch.org/docs/1.11/generated/torch.quantile.html?highlight=quantile#torch.quantile
+            new_y[i * n_points + j] = torch.quantile(y[ids], p)
             new_X[i * n_points + j] = unique_comps[i]
 
     return new_X, new_y
```

### Comparing `nequip-0.5.6/nequip/utils/savenload.py` & `nequip-0.6.0/nequip/utils/savenload.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/test.py` & `nequip-0.6.0/nequip/utils/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Union, Optional, List
 
 import torch
 from e3nn import o3
 from e3nn.util.test import equivariance_error, FLOAT_TOLERANCE
 
-from nequip.nn import GraphModuleMixin
+from nequip.nn import GraphModuleMixin, GraphModel
 from nequip.data import (
     AtomicData,
     AtomicDataDict,
     _NODE_FIELDS,
     _EDGE_FIELDS,
 )
 
 
-PERMUTATION_FLOAT_TOLERANCE = {torch.float32: 1e-5, torch.float64: 1e-10}
+# This has to be somewhat large because of float32 sum reductions over many edges/atoms
+PERMUTATION_FLOAT_TOLERANCE = {torch.float32: 1e-4, torch.float64: 1e-10}
 
 
 # https://discuss.pytorch.org/t/how-to-quickly-inverse-a-permutation-by-using-pytorch/116205/4
 def _inverse_permutation(perm):
     inv = torch.empty_like(perm)
     inv[perm] = torch.arange(perm.size(0), device=perm.device)
     return inv
@@ -39,15 +40,19 @@
         func: the module or model to test
         data_in: the example input data to test with
     """
     # Prevent pytest from showing this function in the traceback
     __tracebackhide__ = True
 
     if tolerance is None:
-        atol = PERMUTATION_FLOAT_TOLERANCE[torch.get_default_dtype()]
+        atol = PERMUTATION_FLOAT_TOLERANCE[
+            func.model_dtype
+            if isinstance(func, GraphModel)
+            else torch.get_default_dtype()
+        ]
     else:
         atol = tolerance
 
     data_in = data_in.copy()
     device = data_in[AtomicDataDict.POSITIONS_KEY].device
 
     node_permute_fields = _NODE_FIELDS
@@ -138,15 +143,15 @@
 
 def assert_AtomicData_equivariant(
     func: GraphModuleMixin,
     data_in: Union[
         AtomicData, AtomicDataDict.Type, List[Union[AtomicData, AtomicDataDict.Type]]
     ],
     permutation_tolerance: Optional[float] = None,
-    o3_tolerance: Optional[float] = None,
+    e3_tolerance: Optional[float] = None,
     **kwargs,
 ) -> str:
     r"""Test the rotation, translation, parity, and permutation equivariance of ``func``.
 
     For details on permutation testing, see ``assert_permutation_equivariant``.
     For details on geometric equivariance testing, see ``e3nn.util.test.assert_equivariant``.
 
@@ -178,28 +183,34 @@
     )
 
     # == Test rotation, parity, and translation using e3nn ==
     irreps_in = {k: None for k in AtomicDataDict.ALLOWED_KEYS}
     irreps_in.update(func.irreps_in)
     irreps_in = {k: v for k, v in irreps_in.items() if k in data_in[0]}
     irreps_out = func.irreps_out.copy()
+    # Remove batch-related keys from the irreps_out, if we aren't using batched inputs
+    irreps_out = {
+        k: v
+        for k, v in irreps_out.items()
+        if not (k in ("batch", "ptr") and "batch" not in data_in)
+    }
     # for certain things, we don't care what the given irreps are...
     # make sure that we test correctly for equivariance:
     for irps in (irreps_in, irreps_out):
         if AtomicDataDict.POSITIONS_KEY in irps:
             # it should always have been 1o vectors
             # since that's actually a valid Irreps
             assert o3.Irreps(irps[AtomicDataDict.POSITIONS_KEY]) == o3.Irreps("1o")
             irps[AtomicDataDict.POSITIONS_KEY] = "cartesian_points"
         if AtomicDataDict.CELL_KEY in irps:
             prev_cell_irps = irps[AtomicDataDict.CELL_KEY]
             assert prev_cell_irps is None or o3.Irreps(prev_cell_irps) == o3.Irreps(
-                "3x1o"
+                "1o"
             )
-            # must be this to actually rotate it
+            # must be this to actually rotate it when flattened
             irps[AtomicDataDict.CELL_KEY] = "3x1o"
 
     stress_keys = (AtomicDataDict.STRESS_KEY, AtomicDataDict.VIRIAL_KEY)
     for k in stress_keys:
         irreps_in.pop(k, None)
     if any(k in irreps_out for k in stress_keys):
         from e3nn.io import CartesianTensor
@@ -227,15 +238,17 @@
                 val = output[key]
                 assert val.shape[-2:] == (3, 3)
                 output[key] = val.reshape(val.shape[:-2] + (9,))
         # stress is also a special case,
         # we need it to be decomposed into irreps for equivar testing
         for k in stress_keys:
             if k in output:
-                output[k] = stress_cart_tensor.from_cartesian(output[k], rtp=stress_rtp)
+                output[k] = stress_cart_tensor.from_cartesian(
+                    output[k], rtp=stress_rtp.to(output[k].dtype)
+                )
         return [output[k] for k in irreps_out]
 
     # prepare input data
     for d in data_in:
         # cell is a special case
         if AtomicDataDict.CELL_KEY in d:
             # flatten
@@ -253,31 +266,35 @@
         )
         for d in data_in
     ]
 
     # take max across errors
     errs = {k: torch.max(torch.vstack([e[k] for e in errs]), dim=0)[0] for k in errs[0]}
 
-    if o3_tolerance is None:
-        o3_tolerance = FLOAT_TOLERANCE[torch.get_default_dtype()]
+    current_dtype = (
+        func.model_dtype if isinstance(func, GraphModel) else torch.get_default_dtype()
+    )
+    if e3_tolerance is None:
+        e3_tolerance = FLOAT_TOLERANCE[current_dtype]
     all_errs = []
     for case, err in errs.items():
         for key, this_err in zip(irreps_out.keys(), err):
             all_errs.append(case + (key, this_err))
-    is_problem = [e[-1] > o3_tolerance for e in all_errs]
+    is_problem = [e[-1] > e3_tolerance for e in all_errs]
 
     message = (permutation_message + "\n") + "\n".join(
-        "   (parity_k={:1d}, did_translate={:5}, field={:20})     -> max error={:.3e}".format(
-            int(k[0]), str(bool(k[1])), str(k[2]), float(k[3])
-        )
+        f"   (parity_k={int(k[0]):1d}, did_translate={str(bool(k[1])):5}, field={str(k[2]):20})     -> max error={float(k[3]):.3e}{'  FAIL' if prob else ''}"
         for k, prob in zip(all_errs, is_problem)
+        if irreps_out[str(k[2])] is not None
     )
 
-    if sum(is_problem) > 0 or "FAIL" in permutation_message:
-        raise AssertionError(f"Equivariance test failed for cases:\n{message}")
+    if any(is_problem) or " FAIL" in permutation_message:
+        raise AssertionError(
+            f"Equivariance test of {type(func).__name__} failed:\n   default dtype: {torch.get_default_dtype()} (assumed) model dtype: {current_dtype}  E(3) tolerance: {e3_tolerance}\n{message}"
+        )
 
     return message
 
 
 _DEBUG_HOOKS = None
 
 
@@ -319,23 +336,21 @@
         inp = inp[0]
         if not (isinstance(inp, dict) or isinstance(inp, Data)):
             raise TypeError(
                 f"Module {mname} should have received a dict or a torch_geometric Data, instead got a {type(inp).__name__}"
             )
         for k, ir in mod.irreps_in.items():
             if k not in inp:
-                raise KeyError(
-                    f"Field {k} with irreps {ir} expected to be input to {mname}; not present"
-                )
+                pass
             elif isinstance(inp[k], torch.Tensor) and isinstance(ir, o3.Irreps):
-                if inp[k].ndim == 1:
+                if inp[k].ndim == 1 and inp[k].numel() > 0:
                     raise ValueError(
                         f"Field {k} in input to module {mname} has only one dimension (assumed to be batch-like); it must have a second irreps dimension even if irreps.dim == 1 (i.e. a single per atom scalar must have shape [N_at, 1], not [N_at])"
                     )
-                elif inp[k].shape[-1] != ir.dim:
+                elif inp[k].shape[-1] != ir.dim and inp[k].numel() > 0:
                     raise ValueError(
                         f"Field {k} in input to module {mname} has last dimension {inp[k].shape[-1]} but its irreps {ir} indicate last dimension {ir.dim}"
                     )
         return
 
     h1 = torch.nn.modules.module.register_module_forward_pre_hook(pre_hook)
 
@@ -346,23 +361,21 @@
         mname = type(mod).__name__
         if not (isinstance(out, dict) or isinstance(out, Data)):
             raise TypeError(
                 f"Module {mname} should have returned a dict or a torch_geometric Data, instead got a {type(out).__name__}"
             )
         for k, ir in mod.irreps_out.items():
             if k not in out:
-                raise KeyError(
-                    f"Field {k} with irreps {ir} expected to be in output from {mname}; not present"
-                )
+                pass
             elif isinstance(out[k], torch.Tensor) and isinstance(ir, o3.Irreps):
-                if out[k].ndim == 1:
+                if out[k].ndim == 1 and out[k].numel() > 0:
                     raise ValueError(
                         f"Field {k} in output from module {mname} has only one dimension (assumed to be batch-like); it must have a second irreps dimension even if irreps.dim == 1 (i.e. a single per atom scalar must have shape [N_at, 1], not [N_at])"
                     )
-                elif out[k].shape[-1] != ir.dim:
+                elif out[k].shape[-1] != ir.dim and out[k].numel() > 0:
                     raise ValueError(
                         f"Field {k} in output from {mname} has last dimension {out[k].shape[-1]} but its irreps {ir} indicate last dimension {ir.dim}"
                     )
         return
 
     h2 = torch.nn.modules.module.register_module_forward_hook(post_hook)
```

### Comparing `nequip-0.5.6/nequip/utils/torch_geometric/batch.py` & `nequip-0.6.0/nequip/utils/torch_geometric/batch.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/torch_geometric/data.py` & `nequip-0.6.0/nequip/utils/torch_geometric/data.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/torch_geometric/dataset.py` & `nequip-0.6.0/nequip/utils/torch_geometric/dataset.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/torch_geometric/utils.py` & `nequip-0.6.0/nequip/utils/torch_geometric/utils.py`

 * *Files identical despite different names*

### Comparing `nequip-0.5.6/nequip/utils/unittests/conftest.py` & `nequip-0.6.0/nequip/utils/unittests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,27 +2,46 @@
 import numpy as np
 import pathlib
 import pytest
 import tempfile
 import os
 
 from ase.atoms import Atoms
-from ase.build import molecule
+from ase.build import molecule, bulk
 from ase.calculators.singlepoint import SinglePointCalculator
 from ase.io import write
 
 import torch
 
 from nequip.utils.test import set_irreps_debug
 from nequip.data import AtomicData, ASEDataset
 from nequip.data.transforms import TypeMapper
 from nequip.utils.torch_geometric import Batch
 from nequip.utils._global_options import _set_global_options
 from nequip.utils.misc import dtype_from_name
 
+# Sometimes we run parallel using pytest-xdist, and want to be able to use
+# as many GPUs as are available
+# https://pytest-xdist.readthedocs.io/en/latest/how-to.html#identifying-the-worker-process-during-a-test
+_is_pytest_xdist: bool = os.environ.get("PYTEST_XDIST_WORKER", "master") != "master"
+if _is_pytest_xdist and torch.cuda.is_available():
+    _xdist_worker_rank: int = int(os.environ["PYTEST_XDIST_WORKER"].lstrip("gw"))
+    _cuda_vis_devs = os.environ.get(
+        "CUDA_VISIBLE_DEVICES",
+        ",".join(str(e) for e in range(torch.cuda.device_count())),
+    ).split(",")
+    _cuda_vis_devs = [int(e) for e in _cuda_vis_devs]
+    # set this for tests that run in this process
+    _local_gpu_rank = _xdist_worker_rank % torch.cuda.device_count()
+    torch.cuda.set_device(_local_gpu_rank)
+    # set this for launched child processes
+    os.environ["CUDA_VISIBLE_DEVICES"] = str(_cuda_vis_devs[_local_gpu_rank])
+    del _xdist_worker_rank, _cuda_vis_devs, _local_gpu_rank
+
+
 if "NEQUIP_NUM_TASKS" not in os.environ:
     # Test parallelization, but don't waste time spawning tons of workers if lots of cores available
     os.environ["NEQUIP_NUM_TASKS"] = "2"
 
 # The default float tolerance
 FLOAT_TOLERANCE = {
     t: torch.as_tensor(v, dtype=dtype_from_name(t))
@@ -93,14 +112,24 @@
 def CH3CHO_no_typemap(float_tolerance) -> Tuple[Atoms, AtomicData]:
     atoms = molecule("CH3CHO")
     data = AtomicData.from_ase(atoms, r_max=2.0)
     return atoms, data
 
 
 @pytest.fixture(scope="session")
+def Cu_bulk(float_tolerance) -> Tuple[Atoms, AtomicData]:
+    atoms = bulk("Cu") * (2, 2, 1)
+    atoms.rattle()
+    data = AtomicData.from_ase(atoms, r_max=3.5)
+    tm = TypeMapper(chemical_symbol_to_type={"Cu": 0})
+    data = tm(data)
+    return atoms, data
+
+
+@pytest.fixture(scope="session")
 def molecules() -> List[Atoms]:
     atoms_list = []
     for i in range(8):
         atoms = molecule("CH3CHO" if i % 2 == 0 else "H2")
         atoms.rattle()
         atoms.calc = SinglePointCalculator(
             energy=np.random.random(),
@@ -117,15 +146,15 @@
 def nequip_dataset(molecules, temp_data, float_tolerance):
     with tempfile.NamedTemporaryFile(suffix=".xyz") as fp:
         for atoms in molecules:
             write(fp.name, atoms, format="extxyz", append=True)
         a = ASEDataset(
             file_name=fp.name,
             root=temp_data,
-            extra_fixed_fields={"r_max": 3.0},
+            AtomicData_options={"r_max": 3.0},
             ase_args=dict(format="extxyz"),
             type_mapper=TypeMapper(chemical_symbol_to_type={"H": 0, "C": 1, "O": 2}),
         )
         yield a
 
 
 @pytest.fixture(scope="session")
```

### Comparing `nequip-0.5.6/nequip/utils/unittests/model_tests.py` & `nequip-0.6.0/nequip/utils/unittests/model_tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     _GRAPH_FIELDS,
     _NODE_FIELDS,
     _EDGE_FIELDS,
 )
 from nequip.data.transforms import TypeMapper
 from nequip.model import model_from_config
 from nequip.nn import GraphModuleMixin
+from nequip.utils import Config
 from nequip.utils.test import assert_AtomicData_equivariant
 
 
 # see https://github.com/pytest-dev/pytest/issues/421#issuecomment-943386533
 # to allow external packages to import tests through subclassing
 class BaseModelTests:
     @pytest.fixture(scope="class")
@@ -51,20 +52,22 @@
         config = config.copy()
         config.update(
             {
                 "num_types": 3,
                 "types_names": ["H", "C", "O"],
             }
         )
-        model = model_from_config(config, initialize=initialize, deploy=deploy)
+        model = model_from_config(
+            Config.from_dict(config), initialize=initialize, deploy=deploy
+        )
         model = model.to(device)
         return model
 
     @pytest.fixture(scope="class")
-    def model(self, config, device):
+    def model(self, config, device, float_tolerance):
         config, out_fields = config
         model = self.make_model(config, device=device)
         return model, out_fields
 
     # == common tests for all models ==
     def test_init(self, model):
         instance, _ = model
@@ -72,53 +75,107 @@
 
     def test_jit(self, model, atomic_batch, device):
         instance, out_fields = model
         data = AtomicData.to_AtomicDataDict(atomic_batch.to(device=device))
         instance = instance.to(device=device)
         model_script = script(instance)
 
+        atol = {
+            # tight, but not that tight, since GPU nondet has to pass
+            # plus model insides are still float32 with global dtype float64 in the tests
+            torch.float32: 5e-5,
+            torch.float64: 5e-7,
+        }[torch.get_default_dtype()]
+
+        out_instance = instance(data.copy())
+        out_script = model_script(data.copy())
+
         for out_field in out_fields:
             assert torch.allclose(
-                instance(data)[out_field],
-                model_script(data)[out_field],
-                atol=1e-6,
-            )
+                out_instance[out_field],
+                out_script[out_field],
+                atol=atol,
+            ), f"JIT didn't repro non-JIT on field {out_field} with max error {(out_instance[out_field] - out_script[out_field]).abs().max().item()}"
 
         # - Try saving, loading in another process, and running -
         with tempfile.TemporaryDirectory() as tmpdir:
             # Save stuff
             model_script.save(tmpdir + "/model.pt")
             torch.save(data, tmpdir + "/dat.pt")
             # Ideally, this would be tested in a subprocess where nequip isn't imported.
             # But CUDA + torch plays very badly with subprocesses here and causes a race condition.
             # So instead we do a slightly less complete test, loading the saved model here in the original process:
             load_model = torch.jit.load(tmpdir + "/model.pt")
             load_dat = torch.load(tmpdir + "/dat.pt")
 
-            atol = {
-                # tight, but not that tight, since GPU nondet has to pass
-                torch.float32: 1e-6,
-                torch.float64: 1e-10,
-            }[torch.get_default_dtype()]
+            out_script = model_script(data.copy())
+            out_load = load_model(load_dat.copy())
 
             for out_field in out_fields:
                 assert torch.allclose(
-                    model_script(data)[out_field],
-                    load_model(load_dat)[out_field],
+                    out_script[out_field],
+                    out_load[out_field],
                     atol=atol,
-                )
+                ), f"JIT didn't repro save-and-loaded JIT on field {out_field} with max error {(out_script[out_field] - out_load[out_field]).abs().max().item()}"
 
     def test_forward(self, model, atomic_batch, device):
         instance, out_fields = model
         instance.to(device)
         data = atomic_batch.to(device)
         output = instance(AtomicData.to_AtomicDataDict(data))
         for out_field in out_fields:
             assert out_field in output
 
+    def test_wrapped_unwrapped(self, model, device, Cu_bulk, float_tolerance):
+        atoms, data_orig = Cu_bulk
+        instance, out_fields = model
+        data = AtomicData.from_ase(atoms, r_max=3.5)
+        data[AtomicDataDict.ATOM_TYPE_KEY] = data_orig[AtomicDataDict.ATOM_TYPE_KEY]
+        data.to(device)
+        out_ref = instance(AtomicData.to_AtomicDataDict(data))
+        # now put things in other periodic images
+        rng = torch.Generator(device=device).manual_seed(12345)
+        # try a few different shifts
+        for _ in range(3):
+            cell_shifts = torch.randint(
+                -5,
+                5,
+                (len(atoms), 3),
+                device=device,
+                dtype=data[AtomicDataDict.POSITIONS_KEY].dtype,
+                generator=rng,
+            )
+            shifts = torch.einsum(
+                "zi,ix->zx", cell_shifts, data[AtomicDataDict.CELL_KEY]
+            )
+            atoms2 = atoms.copy()
+            atoms2.positions += shifts.detach().cpu().numpy()
+            # must recompute the neighborlist for this, since the edge_cell_shifts changed
+            data2 = AtomicData.from_ase(atoms2, r_max=3.5)
+            data2[AtomicDataDict.ATOM_TYPE_KEY] = data[AtomicDataDict.ATOM_TYPE_KEY]
+            data2.to(device)
+            assert torch.equal(
+                data[AtomicDataDict.EDGE_INDEX_KEY],
+                data2[AtomicDataDict.EDGE_INDEX_KEY],
+            )
+            tmp = (
+                data[AtomicDataDict.EDGE_CELL_SHIFT_KEY]
+                + cell_shifts[data[AtomicDataDict.EDGE_INDEX_KEY][0]]
+                - cell_shifts[data[AtomicDataDict.EDGE_INDEX_KEY][1]]
+            )
+            assert torch.equal(
+                tmp,
+                data2[AtomicDataDict.EDGE_CELL_SHIFT_KEY],
+            )
+            out_unwrapped = instance(AtomicData.to_AtomicDataDict(data2))
+            for out_field in out_fields:
+                assert torch.allclose(
+                    out_ref[out_field], out_unwrapped[out_field], atol=float_tolerance
+                )
+
     def test_batch(self, model, atomic_batch, device, float_tolerance):
         """Confirm that the results for individual examples are the same regardless of whether they are batched."""
         allclose = functools.partial(torch.allclose, atol=float_tolerance)
         instance, out_fields = model
         instance.to(device)
         data = atomic_batch.to(device)
         data1 = data.get_example(0)
@@ -171,66 +228,89 @@
         instance, out_fields = model
         instance = instance.to(device=device)
         atomic_batch = atomic_batch.to(device=device)
         assert_AtomicData_equivariant(func=instance, data_in=atomic_batch)
 
     def test_embedding_cutoff(self, model, config, device):
         instance, out_fields = model
+
+        # make all weights nonzero in order to have the most robust test
+        # default init weights can sometimes be zero (e.g. biases) but we want
+        # to ensure smoothness for nonzero values
+        # assumes any trainable parameter will be trained and thus that
+        # nonzero values are valid
+        with torch.no_grad():
+            all_params = list(instance.parameters())
+            old_state = [p.detach().clone() for p in all_params]
+            for p in all_params:
+                p.uniform_(-1.0, 1.0)
+
         config, out_fields = config
         r_max = config["r_max"]
 
         # make a synthetic three atom example
         data = AtomicData(
             atom_types=np.random.choice([0, 1, 2], size=3),
             pos=np.array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0]]),
             edge_index=np.array([[0, 1, 0, 2], [1, 0, 2, 0]]),
         )
         data = data.to(device)
         edge_embed = instance(AtomicData.to_AtomicDataDict(data))
         if AtomicDataDict.EDGE_FEATURES_KEY in edge_embed:
             key = AtomicDataDict.EDGE_FEATURES_KEY
-        else:
+        elif AtomicDataDict.EDGE_EMBEDDING_KEY in edge_embed:
             key = AtomicDataDict.EDGE_EMBEDDING_KEY
+        else:
+            pytest.skip()
         edge_embed = edge_embed[key]
         data.pos[2, 1] = r_max  # put it past the cutoff
         edge_embed2 = instance(AtomicData.to_AtomicDataDict(data))[key]
 
         if key == AtomicDataDict.EDGE_EMBEDDING_KEY:
             # we can only check that other edges are unaffected if we know it's an embedding
             # For example, an Allegro edge feature is many body so will be affected
             assert torch.allclose(edge_embed[:2], edge_embed2[:2])
         assert edge_embed[2:].abs().sum() > 1e-6  # some nonzero terms
-        assert torch.allclose(edge_embed2[2:], torch.zeros(1, device=device))
+        assert torch.allclose(
+            edge_embed2[2:], torch.zeros(1, device=device, dtype=edge_embed2.dtype)
+        )
 
         # test gradients
         in_dict = AtomicData.to_AtomicDataDict(data)
         in_dict[AtomicDataDict.POSITIONS_KEY].requires_grad_(True)
 
         with torch.autograd.set_detect_anomaly(True):
             out = instance(in_dict)
 
             # is the edge embedding of the cutoff length edge unchanged at the cutoff?
             grads = torch.autograd.grad(
                 outputs=out[key][2:].sum(),
                 inputs=in_dict[AtomicDataDict.POSITIONS_KEY],
                 retain_graph=True,
             )[0]
-            assert torch.allclose(grads, torch.zeros(1, device=device))
+            assert torch.allclose(
+                grads, torch.zeros(1, device=device, dtype=grads.dtype)
+            )
 
             if AtomicDataDict.PER_ATOM_ENERGY_KEY in out:
                 # are the first two atom's energies unaffected by atom at the cutoff?
                 grads = torch.autograd.grad(
                     outputs=out[AtomicDataDict.PER_ATOM_ENERGY_KEY][:2].sum(),
                     inputs=in_dict[AtomicDataDict.POSITIONS_KEY],
                 )[0]
                 print(grads)
                 # only care about gradient wrt moved atom
                 assert grads.shape == (3, 3)
                 assert torch.allclose(grads[2], torch.zeros(1, device=device))
 
+        # restore previous model state
+        with torch.no_grad():
+            for p, v in zip(all_params, old_state):
+                p.copy_(v)
+
 
 class BaseEnergyModelTests(BaseModelTests):
     def test_large_separation(self, model, config, molecules, device):
         atol = {torch.float32: 1e-4, torch.float64: 1e-10}[torch.get_default_dtype()]
         instance, _ = model
         instance.to(device)
         config, out_fields = config
@@ -257,14 +337,24 @@
 
         assert torch.allclose(
             out1[AtomicDataDict.TOTAL_ENERGY_KEY]
             + out2[AtomicDataDict.TOTAL_ENERGY_KEY],
             out_both[AtomicDataDict.TOTAL_ENERGY_KEY],
             atol=atol,
         )
+        if AtomicDataDict.FORCE_KEY in out1:
+            # check forces if it's a force model
+            assert torch.allclose(
+                torch.cat(
+                    (out1[AtomicDataDict.FORCE_KEY], out2[AtomicDataDict.FORCE_KEY]),
+                    dim=0,
+                ),
+                out_both[AtomicDataDict.FORCE_KEY],
+                atol=atol,
+            )
 
         atoms_both2 = atoms1.copy()
         atoms3 = atoms2.copy()
         atoms3.positions += np.random.randn(3)
         atoms_both2.extend(atoms3)
         data_both2 = tm(AtomicData.from_ase(atoms_both2, r_max=r_max).to(device=device))
         out_both2 = instance(AtomicData.to_AtomicDataDict(data_both2))
@@ -355,15 +445,18 @@
         for k in output:
             assert k != AtomicDataDict.PARTIAL_FORCE_KEY
             assert k in output_partial
             if output[k].is_floating_point():
                 assert torch.allclose(
                     output[k],
                     output_partial[k],
-                    atol=1e-8 if k == AtomicDataDict.TOTAL_ENERGY_KEY else 1e-6,
+                    atol=1e-8
+                    if k == AtomicDataDict.TOTAL_ENERGY_KEY
+                    and torch.get_default_dtype() == torch.float64
+                    else 1e-5,
                 )
             else:
                 assert torch.equal(output[k], output_partial[k])
         n_at = data[AtomicDataDict.POSITIONS_KEY].shape[0]
         partial_forces = output_partial[AtomicDataDict.PARTIAL_FORCE_KEY]
         assert partial_forces.shape == (n_at, n_at, 3)
         # confirm that sparsity matches graph topology:
@@ -377,8 +470,44 @@
             arange = torch.arange(n_at, device=partial_forces.device)
             adjacency[arange, arange] = True  # diagonal is ofc True
         else:
             # technically only adjacent to n-th degree neighbor, but in this tiny test system that is same as all-to-all and easier to program
             adjacency = data[AtomicDataDict.BATCH_KEY].view(-1, 1) == data[
                 AtomicDataDict.BATCH_KEY
             ].view(1, -1)
-        assert torch.equal(adjacency, torch.any(partial_forces != 0, dim=-1))
+        # for non-adjacent atoms, all partial forces must be zero
+        assert torch.all(partial_forces[~adjacency] == 0)
+
+    def test_force_smoothness(self, model, config, device):
+        instance, out_fields = model
+        if AtomicDataDict.FORCE_KEY not in out_fields:
+            pytest.skip()
+        # see test_embedding_cutoff
+        with torch.no_grad():
+            all_params = list(instance.parameters())
+            old_state = [p.detach().clone() for p in all_params]
+            for p in all_params:
+                p.uniform_(-3.0, 3.0)
+        config, out_fields = config
+        r_max = config["r_max"]
+
+        # make a synthetic three atom example
+        data = AtomicData(
+            atom_types=np.random.choice([0, 1, 2], size=3),
+            pos=np.array([[0.0, 0.0, 0.0], [0.0, 1.0, 0.0], [r_max, 0.0, 0.0]]),
+            edge_index=np.array([[0, 1, 0, 2], [1, 0, 2, 0]]),
+        )
+        data = data.to(device)
+        out = instance(AtomicData.to_AtomicDataDict(data))
+        forces = out[AtomicDataDict.FORCE_KEY]
+        assert (
+            forces[:2].abs().sum() > 1e-4
+        )  # some nonzero terms on the two connected atoms
+        assert torch.allclose(
+            forces[2],
+            torch.zeros(1, device=device, dtype=forces.dtype),
+        )  # the atom at the cutoff should be zero
+
+        # restore previous model state
+        with torch.no_grad():
+            for p, v in zip(all_params, old_state):
+                p.copy_(v)
```

### Comparing `nequip-0.5.6/nequip/utils/versions.py` & `nequip-0.6.0/nequip/utils/versions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-from typing import Tuple
+from typing import Tuple, Final
+import packaging.version
 
 import logging
 
 import torch
 import e3nn
 import nequip
 
 from .git import get_commit
 
+_TORCH_IS_GE_1_13: Final[bool] = packaging.version.parse(
+    torch.__version__
+) >= packaging.version.parse("1.13.0")
+
 _DEFAULT_VERSION_CODES = [torch, e3nn, nequip]
 _DEFAULT_COMMIT_CODES = ["e3nn", "nequip"]
 
 CODE_COMMITS_KEY = "code_commits"
 
 
 def get_config_code_versions(config) -> Tuple[dict, dict]:
```

### Comparing `nequip-0.5.6/nequip/utils/wandb.py` & `nequip-0.6.0/nequip/utils/wandb.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-import wandb
 import logging
+import secrets
+
+from nequip.utils import Config
+
+import wandb
 from wandb.util import json_friendly_val
 
 
 def init_n_update(config):
-    conf_dict = dict(config)
+    conf_dict = Config.as_dict(config)
     # wandb mangles keys (in terms of type) as well, but we can't easily correct that because there are many ambiguous edge cases. (E.g. string "-1" vs int -1 as keys, are they different config keys?)
     if any(not isinstance(k, str) for k in conf_dict.keys()):
         raise TypeError(
             "Due to wandb limitations, only string keys are supported in configurations."
         )
 
-    # download from wandb set up
-    config.run_id = wandb.util.generate_id()
+    # create a run id
+    # see https://github.com/wandb/wandb/pull/4676
+    config.run_id = secrets.token_urlsafe()
 
+    # download from wandb set up
     wandb.init(
         project=config.wandb_project,
         config=conf_dict,
         name=config.run_name,
         resume="allow",
         id=config.run_id,
     )
     # # download from wandb set up
     updated_parameters = dict(wandb.config)
     for k, v_new in updated_parameters.items():
         skip = False
         if k in config.keys():
             # double check the one sanitized by wandb
-            v_old = json_friendly_val(config[k])
+            # because we're preprocessing the config and looping over
+            # _every_ key, don't mark accessed keys as valid => _get_nomark
+            v_old = json_friendly_val(config._get_nomark(k))
             if repr(v_new) == repr(v_old):
                 skip = True
         if skip:
             logging.info(f"# skipping wandb update {k} from {v_old} to {v_new}")
         else:
             config.update({k: v_new})
             logging.info(f"# wandb update {k} from {v_old} to {v_new}")
```

### Comparing `nequip-0.5.6/nequip.egg-info/SOURCES.txt` & `nequip-0.6.0/nequip.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,43 @@
 nequip/data/AtomicDataDict.py
 nequip/data/__init__.py
 nequip/data/_build.py
 nequip/data/_keys.py
 nequip/data/_test_data.py
 nequip/data/_util.py
 nequip/data/dataloader.py
-nequip/data/dataset.py
 nequip/data/transforms.py
+nequip/data/_dataset/__init__.py
+nequip/data/_dataset/_ase_dataset.py
+nequip/data/_dataset/_base_datasets.py
+nequip/data/_dataset/_hdf5_dataset.py
+nequip/data/_dataset/_npz_dataset.py
 nequip/model/__init__.py
 nequip/model/_build.py
 nequip/model/_eng.py
+nequip/model/_gmm.py
 nequip/model/_grads.py
+nequip/model/_pair_potential.py
 nequip/model/_scaling.py
 nequip/model/_weight_init.py
 nequip/model/builder_utils.py
 nequip/nn/__init__.py
 nequip/nn/_atomwise.py
 nequip/nn/_concat.py
 nequip/nn/_convnetlayer.py
+nequip/nn/_gmm.py
 nequip/nn/_grad_output.py
 nequip/nn/_graph_mixin.py
+nequip/nn/_graph_model.py
 nequip/nn/_interaction_block.py
 nequip/nn/_rescale.py
 nequip/nn/_util.py
 nequip/nn/cutoffs.py
 nequip/nn/nonlinearities.py
+nequip/nn/pair_potential.py
 nequip/nn/radial_basis.py
 nequip/nn/embedding/__init__.py
 nequip/nn/embedding/_edge.py
 nequip/nn/embedding/_one_hot.py
 nequip/scripts/__init__.py
 nequip/scripts/_logger.py
 nequip/scripts/benchmark.py
@@ -56,21 +65,23 @@
 nequip/train/__init__.py
 nequip/train/_key.py
 nequip/train/_loss.py
 nequip/train/early_stopping.py
 nequip/train/loss.py
 nequip/train/metrics.py
 nequip/train/trainer.py
+nequip/train/trainer_tensorboard.py
 nequip/train/trainer_wandb.py
 nequip/utils/__init__.py
 nequip/utils/_global_options.py
 nequip/utils/auto_init.py
 nequip/utils/batch_ops.py
 nequip/utils/config.py
 nequip/utils/git.py
+nequip/utils/gmm.py
 nequip/utils/misc.py
 nequip/utils/modules.py
 nequip/utils/multiprocessing.py
 nequip/utils/output.py
 nequip/utils/regressor.py
 nequip/utils/savenload.py
 nequip/utils/test.py
```

### Comparing `nequip-0.5.6/setup.py` & `nequip-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             "nequip-deploy = nequip.scripts.deploy:main",
         ]
     },
     install_requires=[
         "numpy",
         "ase",
         "tqdm",
-        "torch>=1.10.0,<1.13,!=1.9.0",
         "e3nn>=0.4.4,<0.6.0",
         "pyyaml",
         "contextlib2;python_version<'3.7'",  # backport of nullcontext
         'contextvars;python_version<"3.7"',  # backport of contextvars for savenload
         "typing_extensions;python_version<'3.8'",  # backport of Final
         "torch-runstats>=0.2.0",
         "torch-ema>=0.3.0",
```

