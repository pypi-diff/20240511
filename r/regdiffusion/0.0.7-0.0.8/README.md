# Comparing `tmp/regdiffusion-0.0.7.tar.gz` & `tmp/regdiffusion-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regdiffusion-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "regdiffusion-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `regdiffusion-0.0.7.tar` & `regdiffusion-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11341 2023-11-05 15:52:36.085365 regdiffusion-0.0.7/LICENSE
--rw-r--r--   0        0        0     3910 2024-04-29 14:28:13.415126 regdiffusion-0.0.7/README.md
--rw-r--r--   0        0        0      786 2024-04-29 14:10:50.881907 regdiffusion-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py
--rw-r--r--   0        0        0    18237 2024-04-05 04:43:37.672632 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py
--rw-r--r--   0        0        0     5120 2024-01-25 21:19:10.168299 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py
--rw-r--r--   0        0        0    11432 2024-03-14 17:20:42.308017 regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py
--rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.7/regdiffusion/__init__.py
--rw-r--r--   0        0        0      149 2024-03-02 14:07:24.969670 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     4272 2024-02-01 03:02:39.297276 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py
--rw-r--r--   0        0        0     2654 2024-03-07 17:17:15.538130 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py
--rw-r--r--   0        0        0      567 2024-01-25 21:19:10.293030 regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0        0        0      366 2024-03-29 20:40:52.511868 regdiffusion-0.0.7/regdiffusion/data/__init__.py
--rw-r--r--   0        0        0     3697 2024-03-29 20:40:52.521726 regdiffusion-0.0.7/regdiffusion/data/beeline.py
--rw-r--r--   0        0        0     4278 2024-03-29 20:40:52.535236 regdiffusion-0.0.7/regdiffusion/data/microglia.py
--rw-r--r--   0        0        0      567 2024-01-25 21:19:10.333274 regdiffusion-0.0.7/regdiffusion/data/utils.py
--rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.7/regdiffusion/evaluator.py
--rw-r--r--   0        0        0    18097 2024-04-16 15:03:49.420584 regdiffusion-0.0.7/regdiffusion/grn.py
--rw-r--r--   0        0        0     5906 2024-03-27 03:46:34.074272 regdiffusion-0.0.7/regdiffusion/logger.py
--rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.7/regdiffusion/models/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     6363 2024-03-22 04:52:28.581539 regdiffusion-0.0.7/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py
--rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.7/regdiffusion/models/__init__.py
--rw-r--r--   0        0        0     6331 2024-03-29 20:40:52.560257 regdiffusion-0.0.7/regdiffusion/models/regdiffusion.py
--rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.7/regdiffusion/plot/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.7/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py
--rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.7/regdiffusion/plot/__init__.py
--rw-r--r--   0        0        0     2218 2024-04-16 15:24:20.971807 regdiffusion-0.0.7/regdiffusion/plot/pyvis.py
--rw-r--r--   0        0        0    17126 2024-04-16 15:03:49.445516 regdiffusion-0.0.7/regdiffusion/trainer.py
--rw-r--r--   0        0        0     4518 1970-01-01 00:00:00.000000 regdiffusion-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-11-05 15:52:36.085365 regdiffusion-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4117 2024-05-11 13:19:49.921871 regdiffusion-0.0.8/README.md
+-rw-r--r--   0        0        0      786 2024-05-11 15:00:15.015994 regdiffusion-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py
+-rw-r--r--   0        0        0    18097 2024-05-11 14:55:45.000819 regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py
+-rw-r--r--   0        0        0     5120 2024-01-25 21:19:10.168299 regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py
+-rw-r--r--   0        0        0    11432 2024-03-14 17:20:42.308017 regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py
+-rw-r--r--   0        0        0      423 2024-04-16 15:21:41.073897 regdiffusion-0.0.8/regdiffusion/__init__.py
+-rw-r--r--   0        0        0      149 2024-03-02 14:07:24.969670 regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     4272 2024-02-01 03:02:39.297276 regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py
+-rw-r--r--   0        0        0     2654 2024-03-07 17:17:15.538130 regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py
+-rw-r--r--   0        0        0      567 2024-01-25 21:19:10.293030 regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py
+-rw-r--r--   0        0        0      366 2024-03-29 20:40:52.511868 regdiffusion-0.0.8/regdiffusion/data/__init__.py
+-rw-r--r--   0        0        0     3697 2024-03-29 20:40:52.521726 regdiffusion-0.0.8/regdiffusion/data/beeline.py
+-rw-r--r--   0        0        0     4278 2024-03-29 20:40:52.535236 regdiffusion-0.0.8/regdiffusion/data/microglia.py
+-rw-r--r--   0        0        0      567 2024-01-25 21:19:10.333274 regdiffusion-0.0.8/regdiffusion/data/utils.py
+-rw-r--r--   0        0        0     3350 2024-03-21 21:26:05.086388 regdiffusion-0.0.8/regdiffusion/evaluator.py
+-rw-r--r--   0        0        0    18097 2024-05-11 14:55:45.000819 regdiffusion-0.0.8/regdiffusion/grn.py
+-rw-r--r--   0        0        0     5906 2024-03-27 03:46:34.074272 regdiffusion-0.0.8/regdiffusion/logger.py
+-rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.8/regdiffusion/models/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     6363 2024-03-22 04:52:28.581539 regdiffusion-0.0.8/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py
+-rw-r--r--   0        0        0       39 2024-03-07 16:35:41.777169 regdiffusion-0.0.8/regdiffusion/models/__init__.py
+-rw-r--r--   0        0        0     6331 2024-03-29 20:40:52.560257 regdiffusion-0.0.8/regdiffusion/models/regdiffusion.py
+-rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.8/regdiffusion/plot/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     2471 2024-05-11 14:55:20.576624 regdiffusion-0.0.8/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py
+-rw-r--r--   0        0        0       30 2024-04-16 15:03:49.428592 regdiffusion-0.0.8/regdiffusion/plot/__init__.py
+-rw-r--r--   0        0        0     2471 2024-05-11 14:55:20.576624 regdiffusion-0.0.8/regdiffusion/plot/pyvis.py
+-rw-r--r--   0        0        0    17124 2024-05-11 03:14:34.167603 regdiffusion-0.0.8/regdiffusion/trainer.py
+-rw-r--r--   0        0        0     4725 1970-01-01 00:00:00.000000 regdiffusion-0.0.8/PKG-INFO
```

### Comparing `regdiffusion-0.0.7/LICENSE` & `regdiffusion-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/README.md` & `regdiffusion-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # RegDiffusion <a href="https://tuftsbcb.github.io/RegDiffusion/"><img src="https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/docs/_static/regdiffusion.png" align="right" alt="logo" width="140" height = "140" style = "border: none; float: right;"></a>
 
+[![Downloads](https://static.pepy.tech/badge/regdiffusion)](https://pepy.tech/project/regdiffusion)
+[![Downloads](https://static.pepy.tech/badge/regdiffusion/month)](https://pepy.tech/project/regdiffusion)
+
 RegDiffusion is a very fast regulatory network inference algorithm based on probabilistic diffusion model. It works well on genes and is capable to rapidly (<5min) predict biologically verifiable links from large single cell RNA-seq data with 14,000+ genes.
 
 ```
 From Noise to Knowledge: Probabilistic Diffusion-Based Neural Inference of Gene Regulatory Networks
 Hao Zhu, Donna K. Slonim
 bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/2023.11.05.565675
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
-# RegDiffusion _[_l_o_g_o_]RegDiffusion is a very fast regulatory network inference
+# RegDiffusion _[_l_o_g_o_][![Downloads](https://static.pepy.tech/badge/
+regdiffusion)](https://pepy.tech/project/regdiffusion) [![Downloads](https://
+static.pepy.tech/badge/regdiffusion/month)](https://pepy.tech/project/
+regdiffusion) RegDiffusion is a very fast regulatory network inference
 algorithm based on probabilistic diffusion model. It works well on genes and is
 capable to rapidly (<5min) predict biologically verifiable links from large
 single cell RNA-seq data with 14,000+ genes. ``` From Noise to Knowledge:
 Probabilistic Diffusion-Based Neural Inference of Gene Regulatory Networks Hao
 Zhu, Donna K. Slonim bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/
 2023.11.05.565675 ``` ![](https://raw.githubusercontent.com/TuftsBCB/
 RegDiffusion/master/resources/regdiffusion_structure.png) ## Installation
```

### Comparing `regdiffusion-0.0.7/pyproject.toml` & `regdiffusion-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     { name = "Donna Slonim", email="donna.slonim@tufts.edu"}
 ]
 maintainers = [
     { name = "Hao Zhu", email = "haozhu233@gmail.com" }
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
-version = "0.0.7"
+version = "0.0.8"
 description = "Gene Regulatory Networks Inference using diffusion model"
 
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 
 dependencies = [
     "numpy>=1.16.5",
     "pandas>=1.1.1",
```

### Comparing `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/evaluator-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/grn-checkpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 from datetime import datetime
 from collections import deque, Counter
 from scipy.sparse import csr_matrix
 import h5py
-import pyvis
 from typing import List, Dict, Union
+import concurrent.futures
+from .plot import plot_pyvis
 
 class GRN:
     """ 
     A Object to save and analyze gene regulatory network
 
     A GRN object includes the adjacency matrix between transcriptional factors 
     and target genes. In many cases, when TFs are not specified, we have a 
@@ -70,45 +71,58 @@
             self.cutoff_threshold = np.percentile(
                 np.abs(sampled_values), 100-top_gene_percentile
             )
             adj_matrix = adj_matrix.copy()
             adj_matrix[np.abs(adj_matrix) < self.cutoff_threshold] = 0
 
         self.adj_matrix = adj_matrix
+        # TODO: make it tf safe. 
+        if self.n_tfs == self.n_genes:
+            self.adj_matrix_2way = np.concatenate([
+                adj_matrix, adj_matrix.transpose()
+            ], axis=0)
+        else:
+            self.adj_matrix_2way = None
 
         self.gene_indices = {g: i for i, g in enumerate(gene_names)}
         self.tf_indices = {g: i for i, g in enumerate(tf_names)}
 
-    def generate_adj_list(self) -> pd.DataFrame:
+        self.calculated_neighbors = {}
+
+    def get_edgelist(self, k: int = 20, workers: int = 2) -> pd.DataFrame:
         """
-        Simply generate a dataframe to hold the adjacency list.
+        Simply generate a dataframe to hold the edge list.
 
         The dataframe will have 3 columns: `source`, `target`, `weight`. 
+
+        Args:
+            k (int): Top-k edges to inspect on each node. If k=-1, export all.
+            workers (int): Number of concurrent workers. Default is 2. 
         """
-        all_edges = []
-        for r in tqdm(range(self.n_tfs)):
-            for c in range(self.n_genes):
-                if self.adj_matrix[r, c] != 0:
-                    all_edges.append({
-                        'source': self.tf_names[r],
-                        'target': self.gene_names[c],
-                        'weight': self.adj_matrix[r, c]
-                    })
-        return pd.DataFrame(all_edges)
+        with concurrent.futures.ThreadPoolExecutor(
+            max_workers=workers) as executor:
+            futures = [
+                executor.submit(
+                    self.extract_node_neighbors, g, k
+                ) for g in list(self.gene_names)]
+        
+            all_edges = [
+                future.result() for future in 
+                concurrent.futures.as_completed(futures)]
+        return pd.concat(all_edges).reset_index(drop=True)
                 
 
     def extract_node_sources_as_indices(self, gene: str, k: int = 20) -> Dict:
         """
         Generate a dictionary for the top direct edge pointing to the 
         selected gene. It is slightly faster than the dataframe version. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
         """
         gene_idx = self.gene_indices[gene]
         node_neighbors = self.adj_matrix[:, gene_idx]
         node_neighbors_abs = np.abs(node_neighbors)
         if k!=-1:
             top_indices = np.argpartition(node_neighbors_abs, -k)[-k:]
         else:
@@ -125,16 +139,15 @@
         Generate a pandas dataframe for the top direct edge pointing to the 
         selected gene. 
 
         The dataframe will have 3 columns: `source`, `target`, `weight`. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
         """
         source_indices = self.extract_node_sources_as_indices(gene, k)
         top_gene_names = [
             self.tf_names[i] for i in source_indices['tf_indices']
         ]
         output = pd.DataFrame({
             'source': top_gene_names, 
@@ -146,16 +159,15 @@
     def extract_node_targets_as_indices(self, gene: str, k: int = 20) -> Dict:
         """
         Generate a dictionary for the top direct edge pointing from the 
         selected gene. It is slightly faster than the dataframe version. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
         """
         gene_idx = self.tf_indices[gene]
         node_neighbors = self.adj_matrix[gene_idx, :]
         node_neighbors_abs = np.abs(node_neighbors)
         if k!=-1:
             top_indices = np.argpartition(node_neighbors_abs, -k)[-k:]
         else:
@@ -172,16 +184,15 @@
         Generate a pandas dataframe for the top direct edge pointing from the 
         selected gene. 
 
         The dataframe will have 3 columns: `source`, `target`, `weight`. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
         """
         target_indices = self.extract_node_targets_as_indices(gene, k)
         top_gene_names = [
             self.gene_names[i] for i in target_indices['gene_indices']
         ]
         output = pd.DataFrame({
             'source': gene,
@@ -193,192 +204,172 @@
     def extract_node_neighbors_as_indices(self, gene: str, k: int = 20) -> Dict:
         """
         Generate a dictionary for the top direct neighbors of selected gene. 
         It is slightly faster than the dataframe version. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
         """
-        sources = self.extract_node_sources_as_indices(gene, k)
-        targets = self.extract_node_targets_as_indices(gene, k)
-        all_weights = np.abs(np.concatenate([
-            sources['weights'], targets['weights']
-        ]))
-        cutoff = np.partition(all_weights, -k)[-k]
-        source_crit = (sources['weights'] >= cutoff)
-        target_crit = (targets['weights'] >= cutoff)
+        gene_idx = self.gene_indices[gene]
+        if (gene_idx, k) in self.calculated_neighbors:
+            return self.calculated_neighbors[(gene_idx, k)]
+        node_neighbors = self.adj_matrix_2way[:, gene_idx]
+        node_neighbors_abs = np.abs(node_neighbors)
+        if k!=-1:
+            top_indices = np.argpartition(node_neighbors_abs, -k)[-k:]
+        else:
+            top_indices = np.where(node_neighbors_abs!=0)[0]
+        top_edge_weights = node_neighbors[top_indices]
+        top_source_indices = top_indices[top_indices < self.n_tfs]
+        top_source_weights = top_edge_weights[top_indices < self.n_tfs]
+        top_target_indices = top_indices[top_indices >= self.n_tfs] - self.n_tfs
+        top_target_weights = top_edge_weights[top_indices >= self.n_tfs]
         output = {
-            'sources': {
-                'tf_indices': sources['tf_indices'][source_crit],
-                'weights': sources['weights'][source_crit]
-            },
-            'targets': {
-                'gene_indices': targets['gene_indices'][target_crit],
-                'weights': targets['weights'][target_crit]
-            }
+            'source_indices': top_source_indices, 
+            'source_weights': top_source_weights,
+            'target_indices': top_target_indices, 
+            'target_weights': top_target_weights
         }
+        self.calculated_neighbors[(gene_idx, k)] = output
         return output
 
     def extract_node_neighbors(self, gene: str, k: int = 20) -> pd.DataFrame:
         """
         Generate a pandas dataframe for the top direct neighbors of selected 
         gene. The dataframe will be sorted by the absolute weight of edges. 
 
         The dataframe will have 3 columns: `source`, `target`, `weight`. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
         """
-        top_sources = self.extract_node_sources(gene, k)
-        top_targets = self.extract_node_targets(gene, k)
-
-        output = pd.concat([top_sources, top_targets])
-        output['abs_weight'] = output.weight.abs()
-        output = output.sort_values(
-            'abs_weight', ascending=False
-        ).head(k).reset_index(drop=True)
-        del output['abs_weight']
-        return output
+        neighbor_indices = self.extract_node_neighbors_as_indices(gene, k)
+        source_gene_names = [
+            self.tf_names[i] for i in neighbor_indices['source_indices']
+        ]
+        source_tbl = pd.DataFrame({
+            'source': source_gene_names, 
+            'target': gene, 
+            'weight': neighbor_indices['source_weights']
+        })
+        target_gene_names = [
+            self.gene_names[i] for i in neighbor_indices['target_indices']
+        ]
+        target_tbl = pd.DataFrame({
+            'source': gene,
+            'target': target_gene_names, 
+            'weight': neighbor_indices['target_weights']
+        })    
+        return pd.concat([source_tbl, target_tbl])
 
-    def extract_node_2hop_neighborhood(
-        self, genes: Union[str, List[str]], k: int = 20
+    def extract_local_neighborhood(
+        self, genes: Union[str, List[str]], k: int = 20, hops: str = "2.5"
     ) -> pd.DataFrame:
         """
-        Generate a pandas dataframe for the local neighborhood (2-hop) around 
-        selected gene(s). 
+        Generate a pandas dataframe for the 2.5 or 1.5 hop local neighborhood 
+        around selected gene(s). "2.5 hop local neighborhood" includes all the 
+        nodes and edges reachable by a 2-hop search from the selected genes and 
+        the edges connecting all the 2-hop nodes. "1.5 hop local neighborhood"
+        is defined in a similar way but smaller. 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
+            k (int): Top-k edges to inspect on each node. If k=-1, export all
+            hops (str): Number of hops to explore. We can either do a "2.5" or 
+            "1.5" hop travesal around selected genes. Default is "2.5". 
         """
         if isinstance(genes, str):
             genes = [genes]
         hop0_genes = set(genes)
-        hop1 = pd.concat([
-            self.extract_node_neighbors(g, k=k) for g in hop0_genes
-        ])
-        hop1['hop'] = 0
-        hop1_genes = set()
-        for g in hop1.source:
-            if g not in hop0_genes:
-                hop1_genes.add(g)
-        for g in hop1.target:
-            if g not in hop0_genes:
-                hop1_genes.add(g)
-        hop2s = pd.concat([
-            self.extract_node_neighbors(g, k=k) for g in hop1_genes
-        ])
-        hop2s['hop'] = 1
-        hop2_genes = set()
-        for g in hop2s.source:
-            if g not in hop0_genes and g not in hop1_genes:
-                hop2_genes.add(g)
-        for g in hop2s.target:
-            if g not in hop0_genes and g not in hop1_genes:
-                hop2_genes.add(g)
-        hop3s = []
-        for g in hop2_genes:
-            hop3 = self.extract_node_neighbors(g, k=k)
-            hop3 = hop3[
-                hop3.source.isin(hop2_genes) & hop3.target.isin(hop2_genes)
-            ]
-            hop3s.append(hop3)
-        hop3s = pd.concat(hop3s)
-        hop3s['hop'] = 2
-        adj_table = pd.concat([hop1, hop2s, hop3s]).reset_index(drop=True)
-        return adj_table
 
-    def extract_node_1hop_neighborhood(
-        self, genes: Union[str, List[str]], k: int = 20
-    ) -> pd.DataFrame:
-        """
-        Generate a pandas dataframe for the local neighborhood (1-hop) around 
-        selected gene(s). 
-
-        Args:
-            genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
-        """
-        if isinstance(genes, str):
-            genes = [genes]
-        hop0_genes = set(genes)
+        # Hop 1
         hop1 = pd.concat([
             self.extract_node_neighbors(g, k=k) for g in hop0_genes
         ])
         hop1['hop'] = 0
         hop1_genes = set()
         for g in hop1.source:
             if g not in hop0_genes:
                 hop1_genes.add(g)
         for g in hop1.target:
             if g not in hop0_genes:
                 hop1_genes.add(g)
-        hop2s = []
-        for g in hop1_genes:
-            hop2 = self.extract_node_neighbors(g, k=k)
-            hop2 = hop2[
-                hop2.source.isin(hop1_genes) & hop2.target.isin(hop1_genes)
-            ]
-            hop2s.append(hop2)
-        hop2s = pd.concat(hop2s)
-        hop2s['hop'] = 1
-        adj_table = pd.concat([hop1, hop2s]).reset_index(drop=True)
-        return adj_table
+
+        # Hop 2
+        if hops == "1.5":
+            hop2s = []
+            for g in hop1_genes:
+                hop2 = self.extract_node_neighbors(g, k=k)
+                hop2 = hop2[
+                    hop2.source.isin(hop1_genes) & hop2.target.isin(hop1_genes)
+                ]
+                hop2s.append(hop2)
+            hop2s = pd.concat(hop2s)
+            hop2s['hop'] = 1
+            adj_table = pd.concat([hop1, hop2s]).reset_index(drop=True)
+            return adj_table
+        elif hops == "2.5":   
+            hop2s = pd.concat([
+                self.extract_node_neighbors(g, k=k) for g in hop1_genes
+            ])
+            hop2s['hop'] = 1
+            hop2_genes = set()
+            for g in hop2s.source:
+                if g not in hop0_genes and g not in hop1_genes:
+                    hop2_genes.add(g)
+            for g in hop2s.target:
+                if g not in hop0_genes and g not in hop1_genes:
+                    hop2_genes.add(g)
+    
+            # Hop 2.5
+            hop3s = []
+            for g in hop2_genes:
+                hop3 = self.extract_node_neighbors(g, k=k)
+                hop3 = hop3[
+                    hop3.source.isin(hop2_genes) & hop3.target.isin(hop2_genes)
+                ]
+                hop3s.append(hop3)
+            hop3s = pd.concat(hop3s)
+            hop3s['hop'] = 2
+            adj_table = pd.concat([hop1, hop2s, hop3s]).reset_index(drop=True)
+            return adj_table
 
     def visualize_local_neighborhood(
-        self, genes: Union[str, List[str]], k: int = 20, 
-        node_size: int = 8, edge_widths: List[int] = [2, 1, 0.5], 
-        font_size: int = 30,
-        node_group_dict: Dict = None, 
-        cdn_resources: str = 'remote', notebook: bool = True):
+        self, genes: Union[str, List[str]], k: int = 20, hops: str = "2.5",
+        edge_widths: List[int] = [2, 1, 0.5], 
+        plot_engine: str = 'pyvis', *args, **kwargs):
         """
         Generate a vis.js network visualization of the local neighborhood 
         (2-hop) around selected gene(s). 
 
         Args:
             genes (str, List(str)): A single gene or a list of genes to inspect.
-            k (int): Top-k edges to inspect on each node.
-            node_size (int): The size of nodes in the visualization.
-            edge_widths (List): The widths for edges (1st, 2nd, between 2nd 
-                hops).
-            font_size (int): The font size for nodes labels.
-            node_group_dict (dict): A dictionary with keys being the names of 
-                genes and values being the groups. Genes from the same group 
-                will be colored using the same color.
-            cdn_resources (str): Where to load vis.js resources. Default is
-                'remote'.
-            notebook (bool): Boolean value indicating whether the visualization
-                happens in a jupyter notebook. 
+            k (int): Top-k edges to inspect on each node. If k=-1, export all.
+            hops (str): Number of hops of the neighborhood to explore. Default
+            is "2.5". 
+            edge_widths (List): The widths for edges for different edge width
+            levels.
+            plot_engine (str): Choose which network plot engine to use. Default
+            is "pyvis". 
+            **kwargs: Keyword arguments to be passed to ``plot_pyvis``.
         """
-        local_adj_table = self.extract_node_2hop_neighborhood(genes, k)
-        local_adj_table.weight = local_adj_table.weight.map(
+        if isinstance(genes, str):
+            genes = [genes]
+        local_adj_table = self.extract_local_neighborhood(genes, k, hops)
+        local_adj_table['edge_width'] = local_adj_table.hop.map(
             lambda x: edge_widths[x])
-        
-        g = pyvis.network.Network(
-            cdn_resources=cdn_resources, 
-            notebook=notebook
-        )
-        
-        for node in set(local_adj_table['source']) | set(local_adj_table['target']):
-            node_shape = 'star' if node in genes else 'dot'
-            node_group = None if node_group_dict is None else node_group_dict[node]
-            g.add_node(node, label=node, size=node_size, 
-                       shape=node_shape, group=node_group, 
-                       font={"size": font_size})
-        
-        for _, row in local_adj_table.iterrows():
-            g.add_edge(row['source'], row['target'], width=row['hop'])
-        
-        g.repulsion()
+
+        if plot_engine == 'pyvis':
+            g = plot_pyvis(
+                pandas_edgelist = local_adj_table, 
+                star_genes = genes, *args, **kwargs)
+        else: 
+            raise Exception("Not implemented yet")
         return g
 
     def to_hdf5(self, file_path: str, as_sparse: bool = False):
         """
         Save GRN into a HDF5 file. You have the option to save as a sparse 
         matrix. This option is preferred when most of the values in the 
         adjacency matrix are zeros.
```

### Comparing `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/logger-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/.ipynb_checkpoints/trainer-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/beeline-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/microglia-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/data/.ipynb_checkpoints/utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/data/beeline.py` & `regdiffusion-0.0.8/regdiffusion/data/beeline.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/data/microglia.py` & `regdiffusion-0.0.8/regdiffusion/data/microglia.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/data/utils.py` & `regdiffusion-0.0.8/regdiffusion/data/utils.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/evaluator.py` & `regdiffusion-0.0.8/regdiffusion/evaluator.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/grn.py` & `regdiffusion-0.0.8/regdiffusion/grn.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/logger.py` & `regdiffusion-0.0.8/regdiffusion/logger.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/models/.ipynb_checkpoints/regdiffusion-checkpoint.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/models/regdiffusion.py` & `regdiffusion-0.0.8/regdiffusion/models/regdiffusion.py`

 * *Files identical despite different names*

### Comparing `regdiffusion-0.0.7/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py` & `regdiffusion-0.0.8/regdiffusion/plot/.ipynb_checkpoints/pyvis-checkpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 from typing import List, Dict, Union
 
 def plot_pyvis(
     pandas_edgelist: pd.DataFrame, star_genes: List[str] = [],
     node_size: int = 8, 
     font_size: int = 30,
     node_color_dict: Dict = None, 
+    node_group_dict: Dict = None,
     cdn_resources: str = 'remote', notebook: bool = True):
     """
     Generate a vis.js network visualization given an edge list 
     representation of a graph in data frame. 
 
     Args:
         pandas_edgelist (pd.DataFrame): an edge list representation of 
         a graph in a pandas data frame. It should at least have columns 
         with the name `source` and `target`. You can also (optionally) 
         provide an `edge_width` column for the width of the edges
         star_genes (List): A list of genes to be starred. 
         font_size (int): The font size for nodes labels.
         node_color_dict (dict): A dictionary with keys being the names of 
             genes and values being the color. 
+        node_group_dict (dict): A dictionary with keys being the names of 
+            genes and values being the group. 
         cdn_resources (str): Where to load vis.js resources. Default is
             'remote'.
         notebook (bool): Boolean value indicating whether the visualization
             happens in a jupyter notebook. 
     """    
     g = pyvis.network.Network(
         cdn_resources=cdn_resources, 
@@ -37,16 +40,17 @@
         if len(star_genes) == 0:
             node_shape = 'dot'
             this_node_size = node_size
         else:
             node_shape = 'star' if node in star_genes else 'dot'
             this_node_size = 2 * node_size if node in star_genes else node_size
         node_color = None if node_color_dict is None else node_color_dict[node]
+        node_group = None if node_group_dict is None else node_group_dict[node]
         g.add_node(node, label=node, size=this_node_size, 
-                   shape=node_shape, color=node_color, 
+                   shape=node_shape, color=node_color, group=node_group,
                    font={"size": font_size})
 
     if 'edge_width' in pandas_edgelist.columns:
         for _, row in pandas_edgelist.iterrows():
             g.add_edge(row['source'], row['target'], width=row['edge_width'])
     else:
         for _, row in pandas_edgelist.iterrows():
```

### Comparing `regdiffusion-0.0.7/regdiffusion/plot/pyvis.py` & `regdiffusion-0.0.8/regdiffusion/plot/pyvis.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 from typing import List, Dict, Union
 
 def plot_pyvis(
     pandas_edgelist: pd.DataFrame, star_genes: List[str] = [],
     node_size: int = 8, 
     font_size: int = 30,
     node_color_dict: Dict = None, 
+    node_group_dict: Dict = None,
     cdn_resources: str = 'remote', notebook: bool = True):
     """
     Generate a vis.js network visualization given an edge list 
     representation of a graph in data frame. 
 
     Args:
         pandas_edgelist (pd.DataFrame): an edge list representation of 
         a graph in a pandas data frame. It should at least have columns 
         with the name `source` and `target`. You can also (optionally) 
         provide an `edge_width` column for the width of the edges
         star_genes (List): A list of genes to be starred. 
         font_size (int): The font size for nodes labels.
         node_color_dict (dict): A dictionary with keys being the names of 
             genes and values being the color. 
+        node_group_dict (dict): A dictionary with keys being the names of 
+            genes and values being the group. 
         cdn_resources (str): Where to load vis.js resources. Default is
             'remote'.
         notebook (bool): Boolean value indicating whether the visualization
             happens in a jupyter notebook. 
     """    
     g = pyvis.network.Network(
         cdn_resources=cdn_resources, 
@@ -37,16 +40,17 @@
         if len(star_genes) == 0:
             node_shape = 'dot'
             this_node_size = node_size
         else:
             node_shape = 'star' if node in star_genes else 'dot'
             this_node_size = 2 * node_size if node in star_genes else node_size
         node_color = None if node_color_dict is None else node_color_dict[node]
+        node_group = None if node_group_dict is None else node_group_dict[node]
         g.add_node(node, label=node, size=this_node_size, 
-                   shape=node_shape, color=node_color, 
+                   shape=node_shape, color=node_color, group=node_group,
                    font={"size": font_size})
 
     if 'edge_width' in pandas_edgelist.columns:
         for _, row in pandas_edgelist.iterrows():
             g.add_edge(row['source'], row['target'], width=row['edge_width'])
     else:
         for _, row in pandas_edgelist.iterrows():
```

### Comparing `regdiffusion-0.0.7/regdiffusion/trainer.py` & `regdiffusion-0.0.8/regdiffusion/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
         alpha_bars = torch.cumprod(self.alphas, axis=0)
         self.mean_schedule = torch.sqrt(alpha_bars).to(device)
         self.std_schedule = torch.sqrt(1. - alpha_bars).to(device)
     
         # Prepare Data ---------------------------------------------------------
         if (exp_array.sum(0) == 0).sum() > 0:
             warnings.warn(
-                "Some columns in the exp_array contains all zero values, ",
-                "which often causes trouble in inference. Please consider ",
+                "Some columns in the exp_array contains all zero values, "
+                "which often causes trouble in inference. Please consider "
                 "removing these columns before continuing. "
             )
         if cell_types is None:
             cell_types = np.zeros(exp_array.shape[0], dtype=int)
         self.n_celltype = len(np.unique(cell_types))
         n_cell, n_gene = exp_array.shape
         self.n_cell = n_cell
```

### Comparing `regdiffusion-0.0.7/PKG-INFO` & `regdiffusion-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regdiffusion
-Version: 0.0.7
+Version: 0.0.8
 Summary: Gene Regulatory Networks Inference using diffusion model
 Author-email: Hao Zhu <haozhu233@gmail.com>, Donna Slonim <donna.slonim@tufts.edu>
 Maintainer-email: Hao Zhu <haozhu233@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: numpy>=1.16.5
 Requires-Dist: pandas>=1.1.1
@@ -14,14 +14,17 @@
 Requires-Dist: scikit-learn
 Requires-Dist: h5py
 Requires-Dist: pyvis
 Project-URL: Home, https://github.com/TuftsBCB/RegDiffusion
 
 # RegDiffusion <a href="https://tuftsbcb.github.io/RegDiffusion/"><img src="https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/docs/_static/regdiffusion.png" align="right" alt="logo" width="140" height = "140" style = "border: none; float: right;"></a>
 
+[![Downloads](https://static.pepy.tech/badge/regdiffusion)](https://pepy.tech/project/regdiffusion)
+[![Downloads](https://static.pepy.tech/badge/regdiffusion/month)](https://pepy.tech/project/regdiffusion)
+
 RegDiffusion is a very fast regulatory network inference algorithm based on probabilistic diffusion model. It works well on genes and is capable to rapidly (<5min) predict biologically verifiable links from large single cell RNA-seq data with 14,000+ genes.
 
 ```
 From Noise to Knowledge: Probabilistic Diffusion-Based Neural Inference of Gene Regulatory Networks
 Hao Zhu, Donna K. Slonim
 bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/2023.11.05.565675
 ```
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
-Metadata-Version: 2.1 Name: regdiffusion Version: 0.0.7 Summary: Gene
+Metadata-Version: 2.1 Name: regdiffusion Version: 0.0.8 Summary: Gene
 Regulatory Networks Inference using diffusion model Author-email: Hao Zhu
 gmail.com>, Donna Slonim
 tufts.edu> Maintainer-email: Hao Zhu
 gmail.com> Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: Apache Software License Requires-Dist: numpy>=1.16.5 Requires-Dist:
 pandas>=1.1.1 Requires-Dist: torch Requires-Dist: tqdm Requires-Dist: scanpy
 Requires-Dist: scikit-learn Requires-Dist: h5py Requires-Dist: pyvis Project-
-URL: Home, https://github.com/TuftsBCB/RegDiffusion # RegDiffusion
-_[_l_o_g_o_]RegDiffusion is a very fast regulatory network inference algorithm based
-on probabilistic diffusion model. It works well on genes and is capable to
-rapidly (<5min) predict biologically verifiable links from large single cell
-RNA-seq data with 14,000+ genes. ``` From Noise to Knowledge: Probabilistic
-Diffusion-Based Neural Inference of Gene Regulatory Networks Hao Zhu, Donna K.
-Slonim bioRxiv 2023.11.05.565675; doi: https://doi.org/10.1101/
-2023.11.05.565675 ``` ![](https://raw.githubusercontent.com/TuftsBCB/
-RegDiffusion/master/resources/regdiffusion_structure.png) ## Installation
-RegDiffusion is on pypi. ``` pip install regdiffusion ``` Check out the [this
-tutorial](https://tuftsbcb.github.io/RegDiffusion/quick_tour.html) for a quick
-tour of how to use RegDiffusion for your research! ## Quick Tour This package
-`regdiffusion` provides the official implementation of the RegDiffusion
-algorithm and a set of easy-to-use companion tools to evaluate, analyze, and
-visualize the inferred network. We also provide access tools to GRN benchmarks
-and preprocessed single cell datasets for evaluation. We tried to keep the top
-level interface straightforward. Right now, it only consists of 4 components:
-the `RegDiffusionTrainer` class, the `GRN` class, the `GRNEvaluator` class, and
-the `data` module. - `RegDiffusionTrainer`: You can use it to train a
+URL: Home, https://github.com/TuftsBCB/RegDiffusion # RegDiffusion _[_l_o_g_o_][!
+[Downloads](https://static.pepy.tech/badge/regdiffusion)](https://pepy.tech/
+project/regdiffusion) [![Downloads](https://static.pepy.tech/badge/
+regdiffusion/month)](https://pepy.tech/project/regdiffusion) RegDiffusion is a
+very fast regulatory network inference algorithm based on probabilistic
+diffusion model. It works well on genes and is capable to rapidly (<5min)
+predict biologically verifiable links from large single cell RNA-seq data with
+14,000+ genes. ``` From Noise to Knowledge: Probabilistic Diffusion-Based
+Neural Inference of Gene Regulatory Networks Hao Zhu, Donna K. Slonim bioRxiv
+2023.11.05.565675; doi: https://doi.org/10.1101/2023.11.05.565675 ``` ![]
+(https://raw.githubusercontent.com/TuftsBCB/RegDiffusion/master/resources/
+regdiffusion_structure.png) ## Installation RegDiffusion is on pypi. ``` pip
+install regdiffusion ``` Check out the [this tutorial](https://
+tuftsbcb.github.io/RegDiffusion/quick_tour.html) for a quick tour of how to use
+RegDiffusion for your research! ## Quick Tour This package `regdiffusion`
+provides the official implementation of the RegDiffusion algorithm and a set of
+easy-to-use companion tools to evaluate, analyze, and visualize the inferred
+network. We also provide access tools to GRN benchmarks and preprocessed single
+cell datasets for evaluation. We tried to keep the top level interface
+straightforward. Right now, it only consists of 4 components: the
+`RegDiffusionTrainer` class, the `GRN` class, the `GRNEvaluator` class, and the
+`data` module. - `RegDiffusionTrainer`: You can use it to train a
 `RegDiffusion` model by providing log transformed expression data in a `numpy`
 array. The training process could be either started or continued using the
 `.train()` method. You can export the inferred `GRN` using the `.get_grn()`
 method. - `GRN`: The `GRN` class provides a container to save the inferred
 adjacency matrix and the corresponding gene names. You can save the `GRN`
 object to a local `HDF5` file using the `.to_hdf5()` method and reload the
 saved file using the `read_hdf5()` function. It also comes with functionalities
```

