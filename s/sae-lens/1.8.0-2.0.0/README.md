# Comparing `tmp/sae_lens-1.8.0.tar.gz` & `tmp/sae_lens-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-1.8.0.tar", max compression
+gzip compressed data, was "sae_lens-2.0.0.tar", max compression
```

## Comparing `sae_lens-1.8.0.tar` & `sae_lens-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-09 21:45:26.992473 sae_lens-1.8.0/LICENSE
--rw-r--r--   0        0        0     2553 2024-05-09 21:45:26.992473 sae_lens-1.8.0/README.md
--rw-r--r--   0        0        0     1917 2024-05-09 21:45:28.280470 sae_lens-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-09 21:45:28.280470 sae_lens-1.8.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6643 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20496 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     6049 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    13553 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6713 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     4339 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1280 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5065 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8403 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2424 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    30629 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-09 21:45:27.004474 sae_lens-1.8.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     4196 1970-01-01 00:00:00.000000 sae_lens-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-10 23:08:15.638222 sae_lens-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3381 2024-05-10 23:08:15.638222 sae_lens-2.0.0/README.md
+-rw-r--r--   0        0        0     1917 2024-05-10 23:08:16.934232 sae_lens-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-10 23:08:16.934232 sae_lens-2.0.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6651 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20594 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     6065 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    13724 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6785 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     4377 2024-05-10 23:08:15.646222 sae_lens-2.0.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1280 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5065 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8403 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2424 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    30701 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-10 23:08:15.650222 sae_lens-2.0.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-2.0.0/PKG-INFO
```

### Comparing `sae_lens-1.8.0/LICENSE` & `sae_lens-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/README.md` & `sae_lens-2.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -17,14 +17,24 @@
 - Train your own sparse autoencoders.
 - Generate feature dashboards with the [SAE-Vis Library](https://github.com/callummcdougall/sae_vis/tree/main).
 
 SAE Lens is the result of many contributors working collectively to improve humanities understanding of neural networks, many of whom are motivated by a desire to [safeguard humanity from risks posed by artificial intelligence](https://80000hours.org/problem-profiles/artificial-intelligence/).
 
 This library is maintained by [Joseph Bloom](https://www.jbloomaus.com/) and [David Channin](https://github.com/chanind).
 
+## Tutorials
+
+- [Loading and Analysing Pre-Trained Sparse Autoencoders](tutorials/basic_loading_and_analysing.ipynb)
+ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/jbloomAus/SAELens/blob/main/tutorials/basic_loading_and_analysing.ipynb)
+ - [Understanding SAE Features with the Logit Lens](tutorials/logits_lens_with_features.ipynb)
+ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/jbloomAus/SAELens/blob/main/tutorials/logits_lens_with_features.ipynb)
+  - [Training a Sparse Autoencoder](tutorials/training_a_sparse_autoencoder.ipynb)
+ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/jbloomAus/SAELens/blob/main/tutorials/training_a_sparse_autoencoder.ipynb)
+
+
 ## Join the Slack!
 
 Feel free to join the [Open Source Mechanistic Interpretability Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA) for support!
 
 
 ## Citations and References
```

### Comparing `sae_lens-1.8.0/pyproject.toml` & `sae_lens-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "1.8.0"
+version = "2.0.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `sae_lens-1.8.0/sae_lens/__init__.py` & `sae_lens-2.0.0/sae_lens/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.8.0"
+__version__ = "2.0.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import CacheActivationsRunner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-1.8.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-2.0.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-2.0.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-2.0.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-2.0.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/analysis/tsea.py` & `sae_lens-2.0.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/pretrained_saes.yaml` & `sae_lens-2.0.0/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-2.0.0/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-2.0.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         # dataset_path = "/share/data/datasets/pile/the-eye.eu/public/AI/pile/train", # Training set of The Pile
         dataset_path="NeelNanda/openwebtext-tokenized-9b",
         is_dataset_tokenized=True,
         d_in=config["act_size"],  # type: ignore
         expansion_factor=expansion_factor,
         context_size=config["seq_len"],  # type: ignore
         device=device,
-        store_batch_size=32,
+        store_batch_size_prompts=32,
         n_batches_in_buffer=10,
         prepend_bos=False,
         verbose=False,
         dtype=torch.float32,
     )
 
     ae_alt = SparseAutoencoder(cfg)
```

### Comparing `sae_lens-1.8.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-2.0.0/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/activations_store.py` & `sae_lens-2.0.0/sae_lens/training/activations_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             hook_point=cfg.hook_point,
             hook_point_layers=listify(cfg.hook_point_layer),
             hook_point_head_index=cfg.hook_point_head_index,
             context_size=cfg.context_size,
             d_in=cfg.d_in,
             n_batches_in_buffer=cfg.n_batches_in_buffer,
             total_training_tokens=cfg.training_tokens,
-            store_batch_size=cfg.store_batch_size,
-            train_batch_size=cfg.train_batch_size,
+            store_batch_size_prompts=cfg.store_batch_size_prompts,
+            train_batch_size_tokens=cfg.train_batch_size_tokens,
             prepend_bos=cfg.prepend_bos,
             normalize_activations=cfg.normalize_activations,
             device=cfg.device,
             dtype=cfg.dtype,
             cached_activations_path=cached_activations_path,
             model_kwargs=cfg.model_kwargs,
         )
@@ -82,16 +82,16 @@
         hook_point: str,
         hook_point_layers: list[int],
         hook_point_head_index: int | None,
         context_size: int,
         d_in: int,
         n_batches_in_buffer: int,
         total_training_tokens: int,
-        store_batch_size: int,
-        train_batch_size: int,
+        store_batch_size_prompts: int,
+        train_batch_size_tokens: int,
         prepend_bos: bool,
         normalize_activations: bool,
         device: str | torch.device,
         dtype: str | torch.dtype,
         cached_activations_path: str | None = None,
         model_kwargs: dict[str, Any] | None = None,
     ):
@@ -107,16 +107,16 @@
         self.hook_point = hook_point
         self.hook_point_layers = hook_point_layers
         self.hook_point_head_index = hook_point_head_index
         self.context_size = context_size
         self.d_in = d_in
         self.n_batches_in_buffer = n_batches_in_buffer
         self.total_training_tokens = total_training_tokens
-        self.store_batch_size = store_batch_size
-        self.train_batch_size = train_batch_size
+        self.store_batch_size_prompts = store_batch_size_prompts
+        self.train_batch_size_tokens = train_batch_size_tokens
         self.prepend_bos = prepend_bos
         self.normalize_activations = normalize_activations
         self.device = device
         self.dtype = dtype
         self.cached_activations_path = cached_activations_path
 
         self.n_dataset_processed = 0
@@ -192,15 +192,15 @@
         return self._dataloader
 
     def get_batch_tokens(self, batch_size: int | None = None):
         """
         Streams a batch of tokens from a dataset.
         """
         if not batch_size:
-            batch_size = self.store_batch_size
+            batch_size = self.store_batch_size_prompts
         context_size = self.context_size
         device = self.device
 
         batch_tokens = torch.zeros(
             size=(0, context_size), device=device, dtype=torch.long, requires_grad=False
         )
 
@@ -302,15 +302,15 @@
             else:
                 stacked_activations[:, :, i] = layerwise_activations[act_name]
 
         return stacked_activations
 
     def get_buffer(self, n_batches_in_buffer: int) -> torch.Tensor:
         context_size = self.context_size
-        batch_size = self.store_batch_size
+        batch_size = self.store_batch_size_prompts
         d_in = self.d_in
         total_size = batch_size * n_batches_in_buffer
         num_layers = len(self.hook_point_layers)  # Number of hook points or layers
 
         if self.cached_activations_path is not None:
             # Load the activations from disk
             buffer_size = total_size * context_size
@@ -422,15 +422,15 @@
         Return a torch.utils.dataloader which you can get batches from.
 
         Should automatically refill the buffer when it gets to n % full.
         (better mixing if you refill and shuffle regularly).
 
         """
 
-        batch_size = self.train_batch_size
+        batch_size = self.train_batch_size_tokens
 
         # 1. # create new buffer by mixing stored and new buffer
         mixing_buffer = torch.cat(
             [self.get_buffer(self.n_batches_in_buffer // 2), self.storage_buffer],
             dim=0,
         )
```

### Comparing `sae_lens-1.8.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-2.0.0/sae_lens/training/cache_activations_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         bytes_per_token = (
             self.cfg.d_in * self.cfg.dtype.itemsize
             if isinstance(self.cfg.dtype, torch.dtype)
             else DTYPE_MAP[self.cfg.dtype].itemsize
         )
         tokens_in_buffer = (
             self.cfg.n_batches_in_buffer
-            * self.cfg.store_batch_size
+            * self.cfg.store_batch_size_prompts
             * self.cfg.context_size
         )
         total_training_tokens = self.cfg.training_tokens
         total_disk_space_gb = total_training_tokens * bytes_per_token / 10**9
 
         return (
             f"Activation Cache Runner:\n"
@@ -71,15 +71,15 @@
                     f"Activations directory ({new_cached_activations_path}) is not empty. Please delete it or specify a different path. Exiting the script to prevent accidental deletion of files."
                 )
         else:
             os.makedirs(new_cached_activations_path)
 
         print(f"Started caching {self.cfg.training_tokens} activations")
         tokens_per_buffer = (
-            self.cfg.store_batch_size
+            self.cfg.store_batch_size_prompts
             * self.cfg.context_size
             * self.cfg.n_batches_in_buffer
         )
 
         n_buffers = math.ceil(self.cfg.training_tokens / tokens_per_buffer)
 
         for i in tqdm(range(n_buffers), desc="Caching activations"):
```

### Comparing `sae_lens-1.8.0/sae_lens/training/config.py` & `sae_lens-2.0.0/sae_lens/training/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     decoder_heuristic_init: bool = False
     init_encoder_as_decoder_transpose: bool = False
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
     training_tokens: int = 2_000_000
     finetuning_tokens: int = 0
-    store_batch_size: int = 32
-    train_batch_size: int = 4096
+    store_batch_size_prompts: int = 32
+    train_batch_size_tokens: int = 4096
     normalize_activations: bool = False
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"  # type: ignore #
     prepend_bos: bool = True
@@ -71,15 +71,15 @@
     llm_compilation_mode: str | None = None  # which torch.compile mode to use
     compile_sae: bool = False  # use torch.compile on the SAE
     sae_compilation_mode: str | None = None
 
     # Training Parameters
 
     ## Batch size
-    train_batch_size: int = 4096
+    train_batch_size_tokens: int = 4096
 
     ## Adam
     adam_beta1: float | list[float] = 0
     adam_beta2: float | list[float] = 0.999
 
     ## Loss Function
     mse_loss_normalization: Optional[str] = None
@@ -110,15 +110,15 @@
     feature_sampling_window: int = 2000
     dead_feature_window: int = 1000  # unless this window is larger feature sampling,
 
     dead_feature_threshold: float = 1e-8
 
     # Evals
     n_eval_batches: int = 10
-    n_eval_seqs: int | None = None  # useful if evals cause OOM
+    eval_batch_size_prompts: int | None = None  # useful if evals cause OOM
 
     # WANDB
     log_to_wandb: bool = True
     log_activations_store_to_wandb: bool = False
     log_optimizer_state_to_wandb: bool = False
     wandb_project: str = "mats_sae_training_language_model"
     wandb_id: Optional[str] = None
@@ -145,15 +145,15 @@
                 self.hook_point,
                 self.hook_point_head_index,
             )
 
         if not isinstance(self.expansion_factor, list):
             self.d_sae = self.d_in * self.expansion_factor
         self.tokens_per_buffer = (
-            self.train_batch_size * self.context_size * self.n_batches_in_buffer
+            self.train_batch_size_tokens * self.context_size * self.n_batches_in_buffer
         )
 
         if self.run_name is None:
             self.run_name = f"{self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
 
         if self.b_dec_init_method not in ["geometric_median", "mean", "zeros"]:
             raise ValueError(
@@ -199,47 +199,51 @@
 
         if self.verbose:
             print(
                 f"Run name: {self.d_sae}-L1-{self.l1_coefficient}-LR-{self.lr}-Tokens-{self.training_tokens:3.3e}"
             )
             # Print out some useful info:
             n_tokens_per_buffer = (
-                self.store_batch_size * self.context_size * self.n_batches_in_buffer
+                self.store_batch_size_prompts
+                * self.context_size
+                * self.n_batches_in_buffer
             )
             print(f"n_tokens_per_buffer (millions): {n_tokens_per_buffer / 10 ** 6}")
-            n_contexts_per_buffer = self.store_batch_size * self.n_batches_in_buffer
+            n_contexts_per_buffer = (
+                self.store_batch_size_prompts * self.n_batches_in_buffer
+            )
             print(
                 f"Lower bound: n_contexts_per_buffer (millions): {n_contexts_per_buffer / 10 ** 6}"
             )
 
             total_training_steps = (
                 self.training_tokens + self.finetuning_tokens
-            ) // self.train_batch_size
+            ) // self.train_batch_size_tokens
             print(f"Total training steps: {total_training_steps}")
 
             total_wandb_updates = total_training_steps // self.wandb_log_frequency
             print(f"Total wandb updates: {total_wandb_updates}")
 
             # how many times will we sample dead neurons?
             # assert self.dead_feature_window <= self.feature_sampling_window, "dead_feature_window must be smaller than feature_sampling_window"
             n_feature_window_samples = (
                 total_training_steps // self.feature_sampling_window
             )
             print(
-                f"n_tokens_per_feature_sampling_window (millions): {(self.feature_sampling_window * self.context_size * self.train_batch_size) / 10 ** 6}"
+                f"n_tokens_per_feature_sampling_window (millions): {(self.feature_sampling_window * self.context_size * self.train_batch_size_tokens) / 10 ** 6}"
             )
             print(
-                f"n_tokens_per_dead_feature_window (millions): {(self.dead_feature_window * self.context_size * self.train_batch_size) / 10 ** 6}"
+                f"n_tokens_per_dead_feature_window (millions): {(self.dead_feature_window * self.context_size * self.train_batch_size_tokens) / 10 ** 6}"
             )
             print(
                 f"We will reset the sparsity calculation {n_feature_window_samples} times."
             )
-            # print("Number tokens in dead feature calculation window: ", self.dead_feature_window * self.train_batch_size)
+            # print("Number tokens in dead feature calculation window: ", self.dead_feature_window * self.train_batch_size_tokens)
             print(
-                f"Number tokens in sparsity calculation window: {self.feature_sampling_window * self.train_batch_size:.2e}"
+                f"Number tokens in sparsity calculation window: {self.feature_sampling_window * self.train_batch_size_tokens:.2e}"
             )
 
         if not isinstance(self.use_ghost_grads, list) and self.use_ghost_grads:
             print("Using Ghost Grads.")
 
     def get_checkpoints_by_step(self) -> tuple[dict[int, str], bool]:
         """
@@ -309,16 +313,16 @@
     cached_activations_path: Optional[str] = None
     # SAE Parameters
     d_in: int = 512
 
     # Activation Store Parameters
     n_batches_in_buffer: int = 20
     training_tokens: int = 2_000_000
-    store_batch_size: int = 32
-    train_batch_size: int = 4096
+    store_batch_size_prompts: int = 32
+    train_batch_size_tokens: int = 4096
     normalize_activations: bool = False
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
     dtype: str | torch.dtype = "float32"
     prepend_bos: bool = True
```

### Comparing `sae_lens-1.8.0/sae_lens/training/evals.py` & `sae_lens-2.0.0/sae_lens/training/evals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 def run_evals(
     sparse_autoencoder: SparseAutoencoder,
     activation_store: ActivationsStore,
     model: HookedRootModule,
     n_training_steps: int,
     suffix: str = "",
     n_eval_batches: int = 10,
-    n_eval_seqs: int | None = None,
+    eval_batch_size_prompts: int | None = None,
 ) -> Mapping[str, Any]:
     hook_point = sparse_autoencoder.cfg.hook_point
     hook_point_layer = sparse_autoencoder.hook_point_layer
     hook_point_head_index = sparse_autoencoder.cfg.hook_point_head_index
     hook_point_eval = sparse_autoencoder.cfg.hook_point_eval.format(
         layer=hook_point_layer
     )
     ### Evals
-    eval_tokens = activation_store.get_batch_tokens(n_eval_seqs)
+    eval_tokens = activation_store.get_batch_tokens(eval_batch_size_prompts)
 
     # Get Reconstruction Score
     losses_df = recons_loss_batched(
         sparse_autoencoder,
         model,
         activation_store,
         n_batches=n_eval_batches,
-        n_eval_seqs=n_eval_seqs,
+        eval_batch_size_prompts=eval_batch_size_prompts,
     )
 
     recons_score = losses_df["score"].mean()
     ntp_loss = losses_df["loss"].mean()
     recons_loss = losses_df["recons_loss"].mean()
     zero_abl_loss = losses_df["zero_abl_loss"].mean()
 
@@ -99,19 +99,19 @@
 
 
 def recons_loss_batched(
     sparse_autoencoder: SparseAutoencoder,
     model: HookedRootModule,
     activation_store: ActivationsStore,
     n_batches: int = 100,
-    n_eval_seqs: int | None = None,
+    eval_batch_size_prompts: int | None = None,
 ):
     losses = []
     for _ in range(n_batches):
-        batch_tokens = activation_store.get_batch_tokens(n_eval_seqs)
+        batch_tokens = activation_store.get_batch_tokens(eval_batch_size_prompts)
         score, loss, recons_loss, zero_abl_loss = get_recons_loss(
             sparse_autoencoder, model, batch_tokens
         )
         losses.append(
             (
                 score.mean().item(),
                 loss.mean().item(),
```

### Comparing `sae_lens-1.8.0/sae_lens/training/geometric_median.py` & `sae_lens-2.0.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/lm_runner.py` & `sae_lens-2.0.0/sae_lens/training/lm_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 activations_loader,
                 sparse_autoencoder,
                 train_contexts,
             ) = load_checkpoint(
                 checkpoint_path=checkpoint_path,
                 cfg=cfg,
                 model=model,
-                batch_size=cfg.train_batch_size,
+                batch_size=cfg.train_batch_size_tokens,
             )
         # no checkpoints found, don't resume
         except FileNotFoundError:
             print(traceback.format_exc())
             print("failed to find checkpoint to resume from, setting resume to False")
             cfg.resume = False
 
@@ -102,22 +102,22 @@
     # train SAE
     sparse_autoencoder = train_sae_group_on_language_model(
         model=model,  # pyright: ignore [reportPossiblyUnboundVariable] # type: ignore
         sae_group=sparse_autoencoder,  # pyright: ignore [reportPossiblyUnboundVariable]
         activation_store=activations_loader,  # pyright: ignore [reportPossiblyUnboundVariable]
         train_contexts=train_contexts,
         training_run_state=training_run_state,
-        batch_size=cfg.train_batch_size,
+        batch_size=cfg.train_batch_size_tokens,
         n_checkpoints=cfg.n_checkpoints,
         feature_sampling_window=cfg.feature_sampling_window,
         use_wandb=cfg.log_to_wandb,
         wandb_log_frequency=cfg.wandb_log_frequency,
         eval_every_n_wandb_logs=cfg.eval_every_n_wandb_logs,
         autocast=cfg.autocast,
         n_eval_batches=cfg.n_eval_batches,
-        n_eval_seqs=cfg.n_eval_seqs,
+        eval_batch_size_prompts=cfg.eval_batch_size_prompts,
     ).sae_group
 
     if cfg.log_to_wandb:
         wandb.finish()
 
     return sparse_autoencoder
```

### Comparing `sae_lens-1.8.0/sae_lens/training/load_model.py` & `sae_lens-2.0.0/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/optim.py` & `sae_lens-2.0.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/sae_group.py` & `sae_lens-2.0.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/session_loader.py` & `sae_lens-2.0.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-2.0.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/toy_model_runner.py` & `sae_lens-2.0.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/toy_models.py` & `sae_lens-2.0.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-2.0.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     dead_feature_threshold: float = 1e-8,  # how infrequently a feature has to be active to be considered dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
     eval_every_n_wandb_logs: int = 100,
     autocast: bool = False,
     n_eval_batches: int = 10,
-    n_eval_seqs: int | None = None,
+    eval_batch_size_prompts: int | None = None,
 ) -> SparseAutoencoderDictionary:
     """
     @deprecated Use `train_sae_group_on_language_model` instead. This method is kept for backward compatibility.
     """
     return train_sae_group_on_language_model(
         model=model,
         sae_group=sae_group,
@@ -202,15 +202,15 @@
         n_checkpoints=n_checkpoints,
         feature_sampling_window=feature_sampling_window,
         use_wandb=use_wandb,
         wandb_log_frequency=wandb_log_frequency,
         eval_every_n_wandb_logs=eval_every_n_wandb_logs,
         autocast=autocast,
         n_eval_batches=n_eval_batches,
-        n_eval_seqs=n_eval_seqs,
+        eval_batch_size_prompts=eval_batch_size_prompts,
     ).sae_group
 
 
 def get_total_training_tokens(sae_group: SparseAutoencoderDictionary) -> int:
     return sae_group.cfg.training_tokens + sae_group.cfg.finetuning_tokens
 
 
@@ -224,15 +224,15 @@
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
     eval_every_n_wandb_logs: int = 100,
     autocast: bool = False,
     n_eval_batches: int = 10,
-    n_eval_seqs: int | None = None,
+    eval_batch_size_prompts: int | None = None,
 ) -> TrainSAEGroupOutput:
     total_training_tokens = get_total_training_tokens(sae_group=sae_group)
     _update_sae_lens_training_version(sae_group)
     total_training_steps = total_training_tokens // batch_size
 
     checkpoint_thresholds = []
     if n_checkpoints > 0:
@@ -328,15 +328,15 @@
                             run_evals(
                                 sparse_autoencoder,
                                 activation_store,
                                 model,
                                 training_run_state.n_training_steps,
                                 suffix=wandb_suffix,
                                 n_eval_batches=n_eval_batches,
-                                n_eval_seqs=n_eval_seqs,
+                                eval_batch_size_prompts=eval_batch_size_prompts,
                             )
                             sparse_autoencoder.train()
 
             # checkpoint if at checkpoint frequency
             if (
                 checkpoint_thresholds
                 and training_run_state.n_training_tokens > checkpoint_thresholds[0]
```

### Comparing `sae_lens-1.8.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-2.0.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-1.8.0/PKG-INFO` & `sae_lens-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 1.8.0
+Version: 2.0.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -57,14 +57,24 @@
 - Train your own sparse autoencoders.
 - Generate feature dashboards with the [SAE-Vis Library](https://github.com/callummcdougall/sae_vis/tree/main).
 
 SAE Lens is the result of many contributors working collectively to improve humanities understanding of neural networks, many of whom are motivated by a desire to [safeguard humanity from risks posed by artificial intelligence](https://80000hours.org/problem-profiles/artificial-intelligence/).
 
 This library is maintained by [Joseph Bloom](https://www.jbloomaus.com/) and [David Channin](https://github.com/chanind).
 
+## Tutorials
+
+- [Loading and Analysing Pre-Trained Sparse Autoencoders](tutorials/basic_loading_and_analysing.ipynb)
+ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/jbloomAus/SAELens/blob/main/tutorials/basic_loading_and_analysing.ipynb)
+ - [Understanding SAE Features with the Logit Lens](tutorials/logits_lens_with_features.ipynb)
+ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/jbloomAus/SAELens/blob/main/tutorials/logits_lens_with_features.ipynb)
+  - [Training a Sparse Autoencoder](tutorials/training_a_sparse_autoencoder.ipynb)
+ [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/jbloomAus/SAELens/blob/main/tutorials/training_a_sparse_autoencoder.ipynb)
+
+
 ## Join the Slack!
 
 Feel free to join the [Open Source Mechanistic Interpretability Slack](https://join.slack.com/t/opensourcemechanistic/shared_invite/zt-1qosyh8g3-9bF3gamhLNJiqCL_QqLFrA) for support!
 
 
 ## Citations and References
```

