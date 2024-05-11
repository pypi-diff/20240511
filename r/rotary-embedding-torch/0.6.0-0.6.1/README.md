# Comparing `tmp/rotary_embedding_torch-0.6.0.tar.gz` & `tmp/rotary_embedding_torch-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rotary_embedding_torch-0.6.0.tar", last modified: Thu May  9 14:26:52 2024, max compression
+gzip compressed data, was "rotary_embedding_torch-0.6.1.tar", last modified: Sat May 11 15:32:54 2024, max compression
```

## Comparing `rotary_embedding_torch-0.6.0.tar` & `rotary_embedding_torch-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/rotary_embedding_torch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8907 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch/rotary_embedding_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 14:26:52.000000 rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:26:52.161379 rotary_embedding_torch-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 14:26:45.000000 rotary_embedding_torch-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:32:54.135856 rotary_embedding_torch-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 15:32:54.131856 rotary_embedding_torch-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:32:54.131856 rotary_embedding_torch-0.6.1/rotary_embedding_torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch/rotary_embedding_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 15:32:54.131856 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 15:32:54.000000 rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 15:32:54.135856 rotary_embedding_torch-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-11 15:32:49.000000 rotary_embedding_torch-0.6.1/setup.py
```

### Comparing `rotary_embedding_torch-0.6.0/LICENSE` & `rotary_embedding_torch-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rotary_embedding_torch-0.6.0/PKG-INFO` & `rotary_embedding_torch-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.6.0
+Version: 0.6.1
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary_embedding_torch-0.6.0/README.md` & `rotary_embedding_torch-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,33 @@
 k = rotary_emb.rotate_queries_or_keys(k)
 
 # then do your attention with your queries (q) and keys (k) as usual
 ```
 
 If you do all the steps above correctly, you should see a dramatic improvement during training
 
+## Inference Key-Value Cache
+
+When dealing with key / value caches at inference, the query position needs to be offset with the `key_value_seq_length - query_seq_length`
+
+To make this easy, use the `rotate_queries_with_cached_keys` method
+
+```python
+q = torch.randn(1, 8, 1, 64)     # only one query at a time
+k = torch.randn(1, 8, 1024, 64)  # key / values with cache concatted
+
+q, k = rotary_emb.rotate_queries_with_cached_keys(q, k)
+```
+
+You can also do this manually like so
+
+```python
+q = rotary_emb.rotate_queries_or_keys(q, offset = k.shape[-2] - q.shape[-2])
+```
+
 ## Axial Rotary Embeddings
 
 For easy use of n-dimensional axial relative positional embedding, ie. video transformers
 
 ```python
 import torch
```

#### html2text {}

```diff
@@ -13,22 +13,30 @@
 dimensions (batch, heads, etc) q = torch.randn(1, 8, 1024, 64) # queries -
 (batch, heads, seq len, dimension of head) k = torch.randn(1, 8, 1024, 64) #
 keys # apply the rotations to your queries and keys after the heads have been
 split out, but prior to the dot product and subsequent softmax (attention) q =
 rotary_emb.rotate_queries_or_keys(q) k = rotary_emb.rotate_queries_or_keys(k) #
 then do your attention with your queries (q) and keys (k) as usual ``` If you
 do all the steps above correctly, you should see a dramatic improvement during
-training ## Axial Rotary Embeddings For easy use of n-dimensional axial
-relative positional embedding, ie. video transformers ```python import torch
-from rotary_embedding_torch import ( RotaryEmbedding, apply_rotary_emb )
-pos_emb = RotaryEmbedding( dim = 16, freqs_for = 'pixel', max_freq = 256 ) #
-queries and keys for frequencies to be rotated into # say for a video with 8
-frames, and rectangular image (feature dimension comes last) q = torch.randn(1,
-8, 64, 32, 64) k = torch.randn(1, 8, 64, 32, 64) # get axial frequencies - (8,
-64, 32, 16 * 3 = 48) # will automatically do partial rotary freqs =
+training ## Inference Key-Value Cache When dealing with key / value caches at
+inference, the query position needs to be offset with the `key_value_seq_length
+- query_seq_length` To make this easy, use the
+`rotate_queries_with_cached_keys` method ```python q = torch.randn(1, 8, 1, 64)
+# only one query at a time k = torch.randn(1, 8, 1024, 64) # key / values with
+cache concatted q, k = rotary_emb.rotate_queries_with_cached_keys(q, k) ``` You
+can also do this manually like so ```python q =
+rotary_emb.rotate_queries_or_keys(q, offset = k.shape[-2] - q.shape[-2]) ``` ##
+Axial Rotary Embeddings For easy use of n-dimensional axial relative positional
+embedding, ie. video transformers ```python import torch from
+rotary_embedding_torch import ( RotaryEmbedding, apply_rotary_emb ) pos_emb =
+RotaryEmbedding( dim = 16, freqs_for = 'pixel', max_freq = 256 ) # queries and
+keys for frequencies to be rotated into # say for a video with 8 frames, and
+rectangular image (feature dimension comes last) q = torch.randn(1, 8, 64, 32,
+64) k = torch.randn(1, 8, 64, 32, 64) # get axial frequencies - (8, 64, 32, 16
+* 3 = 48) # will automatically do partial rotary freqs =
 pos_emb.get_axial_freqs(8, 64, 32) # rotate in frequencies q = apply_rotary_emb
 (freqs, q) k = apply_rotary_emb(freqs, k) ``` ## Length Extrapolatable Rotary
 Embeddings In _t_h_i_s_ _p_a_p_e_r, they were able to fix length extrapolation issue with
 rotary embeddings by giving it a decay similar to ALiBi. They named this
 technique XPos, and you can use it by setting `use_xpos = True` on
 initialization. This can only be used for autoregressive transformers ```python
 import torch from rotary_embedding_torch import RotaryEmbedding # instantiate
```

### Comparing `rotary_embedding_torch-0.6.0/rotary_embedding_torch/rotary_embedding_torch.py` & `rotary_embedding_torch-0.6.1/rotary_embedding_torch/rotary_embedding_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,16 @@
 
     def rotate_queries_with_cached_keys(self, q, k, seq_dim = None, offset = 0):
         seq_dim = default(seq_dim, self.default_seq_dim)
 
         q_len, k_len = q.shape[seq_dim], k.shape[seq_dim]
         assert q_len <= k_len
 
-        rotated_q = self.rotate_queries_or_keys(q, seq_dim = seq_dim, offset = k_len - q_len)
-        rotated_k = self.rotate_queries_or_keys(k, seq_dim = seq_dim)
+        rotated_q = self.rotate_queries_or_keys(q, seq_dim = seq_dim, offset = k_len - q_len + offset)
+        rotated_k = self.rotate_queries_or_keys(k, seq_dim = seq_dim, offset = offset)
 
         rotated_q = rotated_q.type(q.dtype)
         rotated_k = rotated_k.type(k.dtype)
 
         return rotated_q, rotated_k
 
     def rotate_queries_and_keys(self, q, k, seq_dim = None):
```

### Comparing `rotary_embedding_torch-0.6.0/rotary_embedding_torch.egg-info/PKG-INFO` & `rotary_embedding_torch-0.6.1/rotary_embedding_torch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rotary-embedding-torch
-Version: 0.6.0
+Version: 0.6.1
 Summary: Rotary Embedding - Pytorch
 Home-page: https://github.com/lucidrains/rotary-embedding-torch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,positional embedding
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rotary_embedding_torch-0.6.0/setup.py` & `rotary_embedding_torch-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'rotary-embedding-torch',
   packages = find_packages(),
-  version = '0.6.0',
+  version = '0.6.1',
   license='MIT',
   description = 'Rotary Embedding - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/rotary-embedding-torch',
   keywords = [
```

