# Comparing `tmp/meshgpt_pytorch-1.2.1.tar.gz` & `tmp/meshgpt_pytorch-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshgpt_pytorch-1.2.1.tar", last modified: Fri May 10 17:58:44 2024, max compression
+gzip compressed data, was "meshgpt_pytorch-1.2.2.tar", last modified: Fri May 10 18:11:40 2024, max compression
```

## Comparing `meshgpt_pytorch-1.2.1.tar` & `meshgpt_pytorch-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/meshgpt_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    50407 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/meshgpt_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 17:58:44.000000 meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:58:44.670256 meshgpt_pytorch-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 17:58:40.000000 meshgpt_pytorch-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/meshgpt_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10668 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50422 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/meshgpt_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 18:11:40.000000 meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 18:11:40.151964 meshgpt_pytorch-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-10 18:11:31.000000 meshgpt_pytorch-1.2.2/setup.py
```

### Comparing `meshgpt_pytorch-1.2.1/LICENSE` & `meshgpt_pytorch-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.1/PKG-INFO` & `meshgpt_pytorch-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.1
+Version: 1.2.2
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
@@ -26,8 +26,8 @@
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: taylor-series-linear-attention>=0.1.6
 Requires-Dist: torch>=2.1
 Requires-Dist: torch_geometric
 Requires-Dist: torchtyping
 Requires-Dist: tqdm
 Requires-Dist: vector-quantize-pytorch>=1.14.22
-Requires-Dist: x-transformers>=1.26.0
+Requires-Dist: x-transformers>=1.29.2
```

### Comparing `meshgpt_pytorch-1.2.1/README.md` & `meshgpt_pytorch-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.1/meshgpt_pytorch/data.py` & `meshgpt_pytorch-1.2.2/meshgpt_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.1/meshgpt_pytorch/meshgpt_pytorch.py` & `meshgpt_pytorch-1.2.2/meshgpt_pytorch/meshgpt_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1021,15 +1021,15 @@
         max_seq_len = 8192,
         flash_attn = True,
         attn_depth = 12,
         attn_dim_head = 64,
         attn_heads = 16,
         attn_kwargs: dict = dict(
             ff_glu = True,
-            num_mem_kv = 4
+            attn_num_mem_kv = 4
         ),
         cross_attn_num_mem_kv = 4, # needed for preventing nan when dropping out text condition
         dropout = 0.,
         coarse_pre_gateloop_depth = 2,
         fine_pre_gateloop_depth = 2,
         gateloop_use_heinsen = False,
         fine_attn_depth = 2,
@@ -1104,16 +1104,16 @@
 
         # main autoregressive attention network
         # attending to a face token
 
         self.decoder = Decoder(
             dim = dim,
             depth = attn_depth,
-            dim_head = attn_dim_head,
             heads = attn_heads,
+            attn_dim_head = attn_dim_head,
             attn_flash = flash_attn,
             attn_dropout = dropout,
             ff_dropout = dropout,
             cross_attend = condition_on_text,
             cross_attn_dim_context = cross_attn_dim_context,
             cross_attn_num_mem_kv = cross_attn_num_mem_kv,
             **attn_kwargs
@@ -1128,16 +1128,16 @@
         self.fine_gateloop_block = GateLoopBlock(dim, depth = fine_pre_gateloop_depth) if fine_pre_gateloop_depth > 0 else None
 
         # decoding the vertices, 2-stage hierarchy
 
         self.fine_decoder = Decoder(
             dim = dim_fine,
             depth = fine_attn_depth,
-            dim_head = attn_dim_head,
             heads = attn_heads,
+            attn_dim_head = attn_dim_head,
             attn_flash = flash_attn,
             attn_dropout = dropout,
             ff_dropout = dropout,
             **attn_kwargs
         )
 
         # to logits
```

### Comparing `meshgpt_pytorch-1.2.1/meshgpt_pytorch/trainer.py` & `meshgpt_pytorch-1.2.2/meshgpt_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `meshgpt_pytorch-1.2.1/meshgpt_pytorch.egg-info/PKG-INFO` & `meshgpt_pytorch-1.2.2/meshgpt_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshgpt-pytorch
-Version: 1.2.1
+Version: 1.2.2
 Summary: MeshGPT Pytorch
 Home-page: https://github.com/lucidrains/meshgpt-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention mechanisms,transformers,mesh generation
 Classifier: Development Status :: 4 - Beta
@@ -26,8 +26,8 @@
 Requires-Dist: pytorch-custom-utils>=0.0.9
 Requires-Dist: taylor-series-linear-attention>=0.1.6
 Requires-Dist: torch>=2.1
 Requires-Dist: torch_geometric
 Requires-Dist: torchtyping
 Requires-Dist: tqdm
 Requires-Dist: vector-quantize-pytorch>=1.14.22
-Requires-Dist: x-transformers>=1.26.0
+Requires-Dist: x-transformers>=1.29.2
```

### Comparing `meshgpt_pytorch-1.2.1/setup.py` & `meshgpt_pytorch-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'pytorch-custom-utils>=0.0.9',
     'taylor-series-linear-attention>=0.1.6',
     'torch>=2.1',
     'torch_geometric',
     'torchtyping',
     'tqdm',
     'vector-quantize-pytorch>=1.14.22',
-    'x-transformers>=1.26.0',
+    'x-transformers>=1.29.2',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

