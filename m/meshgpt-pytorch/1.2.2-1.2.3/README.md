# Comparing `tmp/meshgpt_pytorch-1.2.2.tar.gz` & `tmp/meshgpt_pytorch-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.2.tar", last modified: Fri May 10 18:11:40 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.3.tar", last modified: Fri May 10 23:54:08 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.2.tar` & `meshgpt_pytorch-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50422 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:54:08.038430 meshgpt_pytorch-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 23:54:08.038430 meshgpt_pytorch-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:54:08.038430 meshgpt_pytorch-1.2.3/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50919 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 23:54:08.038430 meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 23:54:08.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 23:54:08.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 23:54:08.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 23:54:08.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 23:54:08.000000 meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 23:54:08.038430 meshgpt_pytorch-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 23:54:03.000000 meshgpt_pytorch-1.2.3/setup.py
```

### Comparing `meshgpt_pytorch-1.2.2/LICENSE` & `meshgpt_pytorch-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.2/PKG-INFO` & `meshgpt_pytorch-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.2
+Version: 1.2.3
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.2/README.md` & `meshgpt_pytorch-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.2/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.3/meshgpt_pytorch/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from functools import partial
 import torch
 from torch import Tensor
 from torch import is_tensor
 import torch.nn.functional as F
 from torch.utils.data import Dataset
@@ -9,15 +11,15 @@
 
 import numpy as np
 from numpy.lib.format import open_memmap
 
 from einops import rearrange, reduce
 
 from beartype import beartype
-from beartype.typing import Tuple, List, Union, Optional, Callable, Dict, Callable
+from beartype.typing import Tuple, List, Callable, Dict, Callable
 
 from torchtyping import TensorType
 
 from pytorch_custom_utils.utils import pad_or_slice_to
 
 # helper fn
 
@@ -261,15 +263,15 @@
 
 class DatasetFromTransforms(Dataset):
     @beartype
     def __init__(
         self,
         folder: str,
         transforms: Dict[str, Callable[[Path], Tuple[Vertices, Faces]]],
-        data_kwargs: Optional[List[str]] = None,
+        data_kwargs: List[str] | None = None,
         augment_fn: Callable = identity
     ):
         folder = Path(folder)
         assert folder.exists and folder.is_dir()
         self.folder = folder
 
         exts = transforms.keys()
```

### Comparing `meshgpt_pytorch-1.2.2/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.3/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 from functools import partial
 from math import ceil, pi, sqrt
 
 import torch
 from torch import nn, Tensor, einsum
 from torch.nn import Module, ModuleList
@@ -10,15 +12,15 @@
 from torch.cuda.amp import autocast
 
 from torchtyping import TensorType
 
 from pytorch_custom_utils import save_load
 
 from beartype import beartype
-from beartype.typing import Union, Tuple, Callable, Optional, List, Dict, Any
+from beartype.typing import Tuple, Callable, List, Dict, Any
 
 from einops import rearrange, repeat, reduce, pack, unpack
 from einops.layers.torch import Rearrange
 
 from einx import get_at
 
 from x_transformers import Decoder
@@ -818,15 +820,15 @@
         return rearrange(x, 'b d n -> b n d')
 
     @beartype
     @torch.no_grad()
     def decode_from_codes_to_faces(
         self,
         codes: Tensor,
-        face_mask: Optional[TensorType['b', 'n', bool]] = None,
+        face_mask: TensorType['b', 'n', bool] | None = None,
         return_discrete_codes = False
     ):
         codes = rearrange(codes, 'b ... -> b (...)')
 
         if not exists(face_mask):
             face_mask = reduce(codes != self.pad_id, 'b (nf nvf q) -> b nf', 'all', nvf = self.num_vertices_per_face, q = self.num_quantizers)
 
@@ -899,15 +901,15 @@
 
     @beartype
     def forward(
         self,
         *,
         vertices:       TensorType['b', 'nv', 3, float],
         faces:          TensorType['b', 'nf', 'nvf', int],
-        face_edges:     Optional[TensorType['b', 'e', 2, int]] = None,
+        face_edges:     TensorType['b', 'e', 2, int] | None = None,
         return_codes = False,
         return_loss_breakdown = False,
         return_recon_faces = False,
         only_return_recon_faces = False,
         rvq_sample_codebook_temp = 1.
     ):
         if not exists(face_edges):
@@ -1013,15 +1015,15 @@
 @save_load(version = __version__)
 class MeshTransformer(Module):
     @beartype
     def __init__(
         self,
         autoencoder: MeshAutoencoder,
         *,
-        dim: Union[int, Tuple[int, int]] = 512,
+        dim: int | Tuple[int, int] = 512,
         max_seq_len = 8192,
         flash_attn = True,
         attn_depth = 12,
         attn_dim_head = 64,
         attn_heads = 16,
         attn_kwargs: dict = dict(
             ff_glu = True,
@@ -1133,14 +1135,17 @@
             dim = dim_fine,
             depth = fine_attn_depth,
             heads = attn_heads,
             attn_dim_head = attn_dim_head,
             attn_flash = flash_attn,
             attn_dropout = dropout,
             ff_dropout = dropout,
+            cross_attend = condition_on_text,
+            cross_attn_dim_context = cross_attn_dim_context,
+            cross_attn_num_mem_kv = cross_attn_num_mem_kv,
             **attn_kwargs
         )
 
         # to logits
 
         self.to_logits = nn.Linear(dim_fine, self.codebook_size + 1)
 
@@ -1152,15 +1157,15 @@
 
     @property
     def device(self):
         return next(self.parameters()).device
 
     @beartype
     @torch.no_grad()
-    def embed_texts(self, texts: Union[str, List[str]]):
+    def embed_texts(self, texts: str | List[str]):
         single_text = not isinstance(texts, list)
         if single_text:
             texts = [texts]
 
         assert exists(self.conditioner)
         text_embeds = self.conditioner.embed_texts(texts).detach()
 
@@ -1170,26 +1175,26 @@
         return text_embeds
 
     @eval_decorator
     @torch.no_grad()
     @beartype
     def generate(
         self,
-        prompt: Optional[Tensor] = None,
-        batch_size: Optional[int] = None,
+        prompt: Tensor | None = None,
+        batch_size: int | None = None,
         filter_logits_fn: Callable = top_k,
         filter_kwargs: dict = dict(),
         temperature = 1.,
         return_codes = False,
-        texts: Optional[List[str]] = None,
-        text_embeds: Optional[Tensor] = None,
+        texts: List[str] | None = None,
+        text_embeds: Tensor | None = None,
         cond_scale = 1.,
         cache_kv = True,
         max_seq_len = None,
-        face_coords_to_file: Optional[Callable[[Tensor], Any]] = None
+        face_coords_to_file: Callable[[Tensor], Any] | None = None
     ):
         max_seq_len = default(max_seq_len, self.max_seq_len)
 
         if exists(prompt):
             assert not exists(batch_size)
 
             prompt = rearrange(prompt, 'b ... -> b (...)')
@@ -1288,17 +1293,17 @@
         return files
 
     def forward(
         self,
         *,
         vertices:       TensorType['b', 'nv', 3, int],
         faces:          TensorType['b', 'nf', 'nvf', int],
-        face_edges:     Optional[TensorType['b', 'e', 2, int]] = None,
-        codes:          Optional[Tensor] = None,
-        cache:          Optional[LayerIntermediates] = None,
+        face_edges:     TensorType['b', 'e', 2, int] | None = None,
+        codes:          Tensor | None = None,
+        cache:          LayerIntermediates | None = None,
         **kwargs
     ):
         if not exists(codes):
             codes = self.autoencoder.tokenize(
                 vertices = vertices,
                 faces = faces,
                 face_edges = face_edges
@@ -1310,16 +1315,16 @@
     def forward_on_codes(
         self,
         codes = None,
         return_loss = True,
         return_cache = False,
         append_eos = True,
         cache = None,
-        texts: Optional[List[str]] = None,
-        text_embeds: Optional[Tensor] = None,
+        texts: List[str] | None = None,
+        text_embeds: Tensor | None = None,
         cond_drop_prob = None
     ):
         # handle text conditions
 
         attn_context_kwargs = dict()
 
         if self.condition_on_text:
@@ -1332,17 +1337,19 @@
                 assert text_embeds.shape[0] == codes.shape[0], 'batch size of texts or text embeddings is not equal to the batch size of the mesh codes'
 
             _, maybe_dropped_text_embeds = self.conditioner(
                 text_embeds = text_embeds,
                 cond_drop_prob = cond_drop_prob
             )
 
+            text_embed, text_mask = maybe_dropped_text_embeds
+
             attn_context_kwargs = dict(
-                context = maybe_dropped_text_embeds.embed,
-                context_mask = maybe_dropped_text_embeds.mask
+                context = text_embed,
+                context_mask = text_mask
             )
 
         # take care of codes that may be flattened
 
         if codes.ndim > 2:
             codes = rearrange(codes, 'b ... -> b (...)')
 
@@ -1465,16 +1472,16 @@
 
         sos = repeat(self.sos_token, 'd -> b d', b = batch)
 
         # condition sos token if needed
 
         if self.condition_on_text:
             pooled_text_embed = masked_mean(
-                maybe_dropped_text_embeds.embed,
-                maybe_dropped_text_embeds.mask,
+                text_embed,
+                text_mask,
                 dim = 1
             )
 
             sos_cond = self.to_sos_text_cond(pooled_text_embed)
             sos = sos + sos_cond
 
         # auto prepend sos token
@@ -1506,23 +1513,33 @@
             if exists(fine_cache):
                 for attn_intermediate in fine_cache.attn_intermediates:
                     ck, cv = attn_intermediate.cached_kv
                     ck, cv = map(lambda t: rearrange(t, '(b nf) ... -> b nf ...', b = batch), (ck, cv))
                     ck, cv = map(lambda t: t[:, -1, :, :curr_vertex_pos], (ck, cv))
                     attn_intermediate.cached_kv = (ck, cv)
 
-        one_face = fine_vertex_codes.shape[1] == 1
+        num_faces = fine_vertex_codes.shape[1]
+        one_face = num_faces == 1
 
         fine_vertex_codes = rearrange(fine_vertex_codes, 'b nf n d -> (b nf) n d')
 
         if one_face:
             fine_vertex_codes = fine_vertex_codes[:, :(curr_vertex_pos + 1)]
 
+        fine_attn_context_kwargs = dict()
+
+        if self.condition_on_text:
+            fine_attn_context_kwargs = dict(
+                context = repeat(text_embed, 'b ... -> (b nf) ...', nf = num_faces),
+                context_mask = repeat(text_mask, 'b ... -> (b nf) ...', nf = num_faces)
+            )
+
         attended_vertex_codes, fine_cache = self.fine_decoder(
             fine_vertex_codes,
+            **fine_attn_context_kwargs,
             cache = fine_cache,
             return_hiddens = True
         )
 
         if not should_cache_fine:
             fine_cache = None
```

### Comparing `meshgpt_pytorch-1.2.2/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.3/meshgpt_pytorch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 
 from accelerate import Accelerator
 from accelerate.utils import DistributedDataParallelKwargs
 
 from beartype import beartype
 from beartype.door import is_bearable
-from beartype.typing import Optional, Tuple, Type, List
+from beartype.typing import Tuple, Type, List
 
 from ema_pytorch import EMA
 
 from meshgpt_pytorch.data import custom_collate
 
 from meshgpt_pytorch.version import __version__
 
@@ -71,22 +71,22 @@
     def __init__(
         self,
         model: MeshAutoencoder,
         dataset: Dataset,
         num_train_steps: int,
         batch_size: int,
         grad_accum_every: int,
-        val_dataset: Optional[Dataset] = None,
+        val_dataset: Dataset | None = None,
         val_every: int = 100,
         val_num_batches: int = 5,
         learning_rate: float = 1e-4,
         weight_decay: float = 0.,
-        max_grad_norm: Optional[float] = None,
+        max_grad_norm: float | None = None,
         ema_kwargs: dict = dict(),
-        scheduler: Optional[Type[_LRScheduler]] = None,
+        scheduler: Type[_LRScheduler] | None = None,
         scheduler_kwargs: dict = dict(),
         accelerator_kwargs: dict = dict(),
         optimizer_kwargs: dict = dict(),
         checkpoint_every = 1000,
         checkpoint_folder = './checkpoints',
         data_kwargs: Tuple[str, ...] = ['vertices', 'faces', 'face_edges'],
         warmup_steps = 1000,
@@ -330,19 +330,19 @@
         model: MeshTransformer,
         dataset: Dataset,
         num_train_steps: int,
         batch_size: int,
         grad_accum_every: int,
         learning_rate: float = 2e-4,
         weight_decay: float = 0.,
-        max_grad_norm: Optional[float] = 0.5,
-        val_dataset: Optional[Dataset] = None,
+        max_grad_norm: float | None = 0.5,
+        val_dataset: Dataset | None = None,
         val_every = 1,
         val_num_batches = 5,
-        scheduler: Optional[Type[_LRScheduler]] = None,
+        scheduler: Type[_LRScheduler] | None = None,
         scheduler_kwargs: dict = dict(),
         ema_kwargs: dict = dict(),
         accelerator_kwargs: dict = dict(),
         optimizer_kwargs: dict = dict(),
         checkpoint_every = 1000,
         checkpoint_folder = './checkpoints',
         data_kwargs: Tuple[str, ...] = ['vertices', 'faces', 'face_edges', 'texts'],
```

### Comparing `meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.3/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.2
+Version: 1.2.3
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshgpt_pytorch-1.2.2/setup.py` & `meshgpt_pytorch-1.2.3/setup.py`

 * *Files identical despite different names*

