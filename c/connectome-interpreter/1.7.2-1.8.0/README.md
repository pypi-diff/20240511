# Comparing `tmp/connectome_interpreter-1.7.2.tar.gz` & `tmp/connectome_interpreter-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.7.2.tar", last modified: Sun May  5 15:11:43 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.8.0.tar", last modified: Sat May 11 20:39:56 2024, max compression
```

## Comparing `connectome_interpreter-1.7.2.tar` & `connectome_interpreter-1.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:43.781108 connectome_interpreter-1.7.2/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.2/LICENSE
--rw-rw-rw-   0        0        0     1066 2024-05-05 15:11:43.780108 connectome_interpreter-1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:43.745512 connectome_interpreter-1.7.2/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.7.2/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    35488 2024-05-05 15:10:47.000000 connectome_interpreter-1.7.2/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    22184 2024-05-01 14:15:27.000000 connectome_interpreter-1.7.2/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16135 2024-04-28 19:46:57.000000 connectome_interpreter-1.7.2/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    32991 2024-05-05 15:10:50.000000 connectome_interpreter-1.7.2/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:43.776108 connectome_interpreter-1.7.2/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1066 2024-05-05 15:11:43.000000 connectome_interpreter-1.7.2/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-05-05 15:11:43.000000 connectome_interpreter-1.7.2/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 15:11:43.000000 connectome_interpreter-1.7.2/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-05 15:11:43.000000 connectome_interpreter-1.7.2/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-05 15:11:43.000000 connectome_interpreter-1.7.2/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 15:11:43.781108 connectome_interpreter-1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     2068 2024-05-05 15:11:01.000000 connectome_interpreter-1.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 15:11:43.779108 connectome_interpreter-1.7.2/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.7.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.7.2/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.7.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:39:56.027077 connectome_interpreter-1.8.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.0/LICENSE
+-rw-rw-rw-   0        0        0     1066 2024-05-11 20:39:56.026082 connectome_interpreter-1.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-11 20:39:55.973568 connectome_interpreter-1.8.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.8.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    36418 2024-05-11 20:34:13.000000 connectome_interpreter-1.8.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    22584 2024-05-06 14:40:18.000000 connectome_interpreter-1.8.0/connectome_interpreter/compress_paths.py
+-rw-rw-rw-   0        0        0    16221 2024-05-07 10:46:28.000000 connectome_interpreter-1.8.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    35523 2024-05-06 21:27:16.000000 connectome_interpreter-1.8.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:39:56.012791 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1066 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-11 20:39:55.000000 connectome_interpreter-1.8.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 20:39:56.027077 connectome_interpreter-1.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     2068 2024-05-06 14:43:28.000000 connectome_interpreter-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 20:39:56.023090 connectome_interpreter-1.8.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.8.0/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.8.0/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.7.2/LICENSE` & `connectome_interpreter-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.2/PKG-INFO` & `connectome_interpreter-1.8.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: connectome_interpreter
-Version: 1.7.2
+Name: connectome-interpreter
+Version: 1.8.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.7.2/README.md` & `connectome_interpreter-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.2/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.8.0/connectome_interpreter/activation_maximisation.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import pandas as pd
 from scipy.sparse import issparse
 
 from tqdm import tqdm
 
 from .compress_paths import result_summary
-from .utils import adjacency_df_to_el, get_activations
+from .utils import adjacency_df_to_el, get_activations, change_model_weights
 
 
 class MultilayeredNetwork(nn.Module):
     """
     A PyTorch module representing a multilayered neural network model.
     This network architecture is designed to process temporal sequences of sensory data
     through multiple layers, with the initial layer handling sensory inputs and subsequent
@@ -120,14 +120,16 @@
 def activation_maximisation(
         model, neurons_to_activate: Dict[int, List[int]],
         neurons_to_deactivate=None,
         input_tensor=None,
         num_iterations=100, learning_rate=0.4,
         in_regularisation_lambda=0.1, custom_in_regularisation: Callable[[torch.Tensor], torch.Tensor] = None,
         out_regularisation_lambda=0.1,
+        ltd_df=None, ltd_coefficient=0.1,
+        ltp_df=None, ltp_coefficient=0.1,
         early_stopping=True, stopping_threshold=1e-6, n_runs=10,
         use_tqdm=True, print_output=True, report_memory_usage=False,
         device=None, wandb=True) -> Tuple[np.ndarray, np.ndarray, list, list]:
     """
     Performs activation maximisation on a given model to identify input patterns that maximally activate selected neurons.
 
     This method adjusts `input_tensor` over `num_iterations` to maximize the activation of specified neurons in `model`,
@@ -144,14 +146,18 @@
             Defaults to None.
         num_iterations (int, optional): The number of iterations to run the optimization for. Defaults to 100.
         learning_rate (float, optional): The learning rate for the optimizer. Defaults to 0.01.
         in_regularisation_lambda (float, optional): The regularization coefficient for punishing input neuron activation. Defaults to 0.4.
         custom_in_regularisation (Callable[[torch.Tensor], torch.Tensor], optional): A function that applies custom
             regularization to the `input_tensor`. Defaults to L1+L2 norm if None.
         out_regularisation_lambda (float, optional): The coefficient for punishing output neuron activation. Defaults to 0.1.
+        ltd_df (pd.DataFrame, optional): A DataFrame with columns 'pre' and 'post', which contain indices of the connectivity weights in model for long-term depression. Defaults to None.
+        ltd_coefficient (float, optional): The coefficient for long-term depression. Defaults to 0.1.
+        ltp_df (pd.DataFrame, optional): A DataFrame with columns 'pre' and 'post', which contain indices of the connectivity weights in model for long-term potentiation. Defaults to None.
+        ltp_coefficient (float, optional): The coefficient for long-term potentiation. Defaults to 0.1.
         early_stopping (bool, optional): Whether to stop the optimization early if the difference between the biggest and the smallest loss within the last n_runs falls below `stopping_threshold`.
             Defaults to True.
         stopping_threshold (float, optional): The threshold for early stopping. Defaults to 1e-6.
         n_runs (int, optional): The number of runs to consider for early stopping. Defaults to 10.
         use_tqdm (bool, optional): Whether to use tqdm progress bars to track optimization progress. Defaults to True.
         print_output (bool, optional): Whether to print loss information during optimization. Defaults to True.
         report_memory_usage (bool, optional): Whether to report GPU memory usage during optimization. Defaults to False.
@@ -292,14 +298,21 @@
 
         if report_memory_usage and iteration % 10 == 0:
             print(f'GPU memory at iteration {iteration}:', torch.cuda.memory_allocated(
                 device) / 1e9, 'GB')
 
         torch.cuda.empty_cache()
 
+        # plasticity
+        if ltd_df is not None:
+            change_model_weights(model, ltd_df, 'ltd', ltd_coefficient)
+
+        if ltp_df is not None:
+            change_model_weights(model, ltp_df, 'ltp', ltp_coefficient)
+
     output_after = model(input_tensor).cpu().detach().numpy()
     # first bring to cpu to save gpu memory
     input_tensor = input_tensor.cpu().detach().numpy()
     input_tensor = np.where(input_tensor >= model.threshold,
                             input_tensor, 0)
     # Limit the range between 0 and 1
     input_tensor = np.tanh(input_tensor)
```

### Comparing `connectome_interpreter-1.7.2/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.8.0/connectome_interpreter/compress_paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """This module is about compressing the paths of different lengths (either taking into account the sign of connections or not), and looking at the result (`result_summary()`).
 """
 
 import torch
 from tqdm import tqdm
 import pandas as pd
+import numpy as np
 import plotly.express as px
 from scipy.sparse import issparse
 import ipywidgets as widgets
 import seaborn as sns
 import matplotlib.pyplot as plt
 from IPython.display import display
 
 from .utils import dynamic_representation, torch_sparse_where, to_nparray, tensor_to_csc
 
 
-def compress_paths(inprop, step_number, threshold=0, output_threshold=1e-4):
+def compress_paths(inprop, step_number, threshold=0, output_threshold=1e-4, root=False):
     """
     Performs iterative multiplication of a sparse matrix `inprop` for a specified number of steps, 
     applying thresholding to filter out values below a certain `threshold` to optimize memory usage 
     and computation speed. The function is optimized to run on GPU if available. 
 
     This function multiplies the connectivity matrix (input in rows; output in columns) `inprop` with itself `step_number` times, 
     with each step's result being thresholded to zero out elements below a given threshold. 
@@ -28,14 +29,15 @@
     Args:
         inprop (scipy.sparse.matrix): The connectivity matrix as a scipy sparse matrix.
         step_number (int): The number of iterations to perform the matrix multiplication.
         threshold (float, optional): The threshold value to apply after each multiplication. 
                                      Values below this threshold are set to zero. Defaults to 0.
         output_threshold (float, optional): The threshold value to apply to the final output, 
                                             used to reduce memory footprint. Defaults to 1e-4.
+        root (bool, optional): Whether to take the nth root of the output. This can be understood as "the average direct connection strength" (when root=True), as opposed to "the proportion of influence among all partners n steps away" (when root=False). Defaults to False.
 
     Returns:
         list: A list of scipy.sparse.csc_matrix objects, each representing connectivity from all neurons to all neurons n steps away. 
 
     Note:
         This function requires PyTorch and is designed to automatically utilize CUDA-enabled GPU devices 
         if available to accelerate computations. The input matrix `inprop` is converted to a dense tensor 
@@ -56,44 +58,48 @@
 
     for i in tqdm(range(step_number)):
         if i == 0:
             out_tensor = inprop_tensor
         else:
             out_tensor = torch.matmul(out_tensor, inprop_tensor)
 
-            # # Downgrade the previous one to save memory
-            # steps_fast[-1] = torch.where(steps_fast[-1] >= output_threshold,
-            #                              steps_fast[-1], torch.tensor(0.0, device=device))
-            # steps_fast[-1] = steps_fast[-1].to_sparse()
-
         # Thresholding during matmul
         if threshold != 0:
             out_tensor = torch.where(
                 out_tensor >= threshold, out_tensor, torch.tensor(0.0, device=device))
+        # Dynamic representation based on density
+        # out_tensor = dynamic_representation(out_tensor)
+
+        if root:
+            out_csc = torch.pow(out_tensor, 1/(i+1))
+        else:
+            out_csc = out_tensor.clone()
 
-        # Thresholding for output
-        out_csc = torch.where(out_tensor >= output_threshold,
-                              out_tensor, torch.tensor(0.0, device=device))
+        if output_threshold > 0:
+            out_csc = torch_sparse_where(out_csc, output_threshold)
         out_csc = tensor_to_csc(out_csc.to('cpu'))
+        out_csc.eliminate_zeros()
+
         steps_fast.append(out_csc)
 
     torch.cuda.empty_cache()
     return steps_fast
 
 
-def compress_paths_signed(inprop, idx_to_sign, target_layer_number, threshold=0, output_threshold=1e-4):
+def compress_paths_signed(inprop, idx_to_sign, target_layer_number, threshold=0, output_threshold=1e-4, root=False):
     """
     Calculates the excitatory and inhibitory influences across specified layers of a neural network, using PyTorch for GPU acceleration. This function processes a connectivity matrix (where presynaptic neurons are represented by rows and postsynaptic neurons by columns) to distinguish and compute the influence of excitatory and inhibitory neurons at each layer.
 
     Args:
         inprop (scipy.sparse.csc_matrix): The initial connectivity matrix representing direct connections between adjacent layers. 
         idx_to_sign (dict): A dictionary mapping neuron indices to their types (1 for excitatory, -1 for inhibitory), used to differentiate between excitatory and inhibitory influences.
         target_layer_number (int): The number of layers through which to calculate influences, starting from the second layer (with the first layer's influence, the direct connectivity, being defined by `inprop`).
         threshold (float, optional): A value to threshold the influences; influences below this value are set to zero, and not passed on in future layers. Defaults to 0.
         output_threshold (float, optional): A threshold for the final output to reduce memory usage, with values below this threshold set to zero. Defaults to 1e-4.
+        root (bool, optional): Whether to take the nth root of the output. This can be understood as "the average direct connection strength" (when root=True), as opposed to "the proportion of influence among all partners n steps away" (when root=False). Defaults to False.
 
     Returns:
         Tuple[List[scipy.sparse.csc_matrix], List[scipy.sparse.csc_matrix]]: Two lists of sparse matrices representing the excitatory and inhibitory influences, respectively, up to the specified target layer. 
 
     Note:
         This function is ideal with GPU support. Ensure your environment supports CUDA and that PyTorch is correctly installed.
     """
@@ -133,38 +139,35 @@
                 lni_new = torch_sparse_where(lni_new, threshold)
 
             # Dynamic representation based on density
             lne = dynamic_representation(lne_new)
             lni = dynamic_representation(lni_new)
             torch.cuda.empty_cache()
 
-        # steps_excitatory.append(lne)
-        # steps_inhibitory.append(lni)
+        # possible alternative implementation: first root and threshold, then move to CPU. But not sure if can root sparse tensor. So:
+        stepe_csc = tensor_to_csc(lne.to('cpu'))
+        stepi_csc = tensor_to_csc(lni.to('cpu'))
+
+        if root:
+            stepe_csc.data = np.power(stepe_csc.data, 1/(layer+1))
+            stepi_csc.data = np.power(stepi_csc.data, 1/(layer+1))
+
+        # then threshold
+        if output_threshold > 0:
+            stepe_csc.data = np.where(
+                stepe_csc.data >= output_threshold, stepe_csc.data, 0)
+            stepi_csc.data = np.where(
+                stepi_csc.data >= output_threshold, stepi_csc.data, 0)
 
-        # Thresholding for output
-        stepe_csc = torch_sparse_where(lne, output_threshold)
-        stepe_csc = tensor_to_csc(stepe_csc.to('cpu'))
-        steps_excitatory.append(stepe_csc)
+        stepe_csc.eliminate_zeros()
+        stepi_csc.eliminate_zeros()
 
-        stepi_csc = torch_sparse_where(lni, output_threshold)
-        stepi_csc = tensor_to_csc(stepi_csc.to('cpu'))
+        steps_excitatory.append(stepe_csc)
         steps_inhibitory.append(stepi_csc)
 
-    #     # Downgrade previous matrices to save memory
-    #     if steps_excitatory:
-    #         steps_excitatory[-1] = torch_sparse_where(
-    #             steps_excitatory[-1], output_threshold).to_sparse()
-    #         steps_inhibitory[-1] = torch_sparse_where(
-    #             steps_inhibitory[-1], output_threshold).to_sparse()
-
-    # # Downgrade the last one to save memory
-    # steps_excitatory[-1] = torch_sparse_where(
-    #     steps_excitatory[-1], output_threshold).to_sparse()
-    # steps_inhibitory[-1] = torch_sparse_where(
-    #     steps_inhibitory[-1], output_threshold).to_sparse()
     torch.cuda.empty_cache()
 
     return steps_excitatory, steps_inhibitory
 
 
 def add_first_n_matrices(matrices, n):
     """
@@ -240,14 +243,17 @@
         outidx_map = inidx_map
 
     # remove nan values in inidx and outidx
     inidx = to_nparray(inidx)
     outidx = to_nparray(outidx)
 
     if issparse(stepsn):
+        # if stepsn is coo, turn into csc
+        if stepsn.format == 'coo':
+            stepsn = stepsn.tocsc()
         matrix = stepsn[:, outidx][inidx, :].toarray()
     else:
         matrix = stepsn[inidx, :][:, outidx]
 
     if include_undefined_groups:
         # fill the nan values in inidx_map (e.g. 17726: nan) and outidx_map with 'undefined'
         inidx_map = {k: v if pd.notna(
```

### Comparing `connectome_interpreter-1.7.2/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.8.0/connectome_interpreter/path_finding.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,17 @@
     positions = {}
 
     all_names = set(df['pre_layer']) | set(df['post_layer'])
     name_to_idx = dict(zip(df.pre_layer, df.pre))
     name_to_idx.update(dict(zip(df.post_layer, df.post)))
 
     for layer in range(0, number_of_layers + 1):
-        layer_name = [item for item in all_names if '_'+str(layer) in item]
+        # if the last characters match
+        layer_name = [item for item in all_names if '_' +
+                      str(layer) == item[-len(str(layer))-1:]]
         if sort_dict is not None:
             layer_name = sorted(layer_name, key=lambda x: sort_dict[x])
 
         if priority_indices is not None:
             layer_name_priority = [
                 item for item in layer_name if name_to_idx[item] in priority_indices]
             layer_name_not = [
```

### Comparing `connectome_interpreter-1.7.2/connectome_interpreter/utils.py` & `connectome_interpreter-1.8.0/connectome_interpreter/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -684,7 +684,57 @@
     edge_labels = {(u, v): f'{data["weight"]:.{weight_decimals}f}' for u,
                    v, data in G.edges(data=True)}
     nx.draw_networkx_edge_labels(G, pos=positions, edge_labels=edge_labels,
                                  #  font_color='red'
                                  ax=ax)
     ax.set_ylim(0, 1)
     plt.show()
+
+
+def change_model_weights(model, df, mode, coefficient=0.1):
+    """
+    Change the weights of the model based on the provided DataFrame.
+    The DataFrame should contain columns 'pre' and 'post', which contain indices of the connectivity weights in model. The weights are modified proportional to: 
+    1. The similarity of pre and post activations (i.e. the sum of element-wise multiplication of activations across time), and 
+    2. The coefficient provided.
+    The 'mode' column should specify whether the weight change is ltp or ltd.
+
+    Args:
+        model (torch.nn.Module): The model containing the weights to change.
+        df (pd.DataFrame): A DataFrame containing the columns 'pre' and 'post'.
+        mode (str): The mode of weight change, either 'ltp' or 'ltd'.
+
+    Returns:
+        None: This function modifies the model weights in place.
+    """
+
+    df.loc[:, ['pre_local_idx']] = pd.factorize(df.pre)[0]
+    df.loc[:, ['post_local_idx']] = pd.factorize(df.post)[0]
+
+    # piggy back on matrix multiplication, and calculate between each pair of neurons:
+    # sum of unitary product of activity across timesteps
+    # then multiply this sum with the coefficient
+    weight_changes = torch.matmul(model.activations[df.pre.unique(), :],
+                                  model.activations.t()[:, df.post.unique()]) * coefficient
+    # only select the pairs present in the original ltd/ltp_df
+    mask = torch.zeros_like(
+        weight_changes, dtype=torch.bool, device=weight_changes.device)
+    mask[df.pre_local_idx.values[:, None], df.post_local_idx.values] = True
+    # the rest have no change
+    weight_changes[~mask] = 0
+
+    # take out the weights to change
+    # NOTE: all_weights have pre in the columns, post in the rows
+    weights_subset = model.all_weights[df.post.unique()[
+        :, None], df.pre.unique()]
+    # change the weights: keep the signs separate, strengthen (ltp) / weaken (ltd) the connection by using the absolute values
+    if mode == 'ltp':
+        # strengthen connectivity
+        weights_subset_abs = torch.abs(weights_subset) + weight_changes.t()
+    elif mode == 'ltd':
+        # weaken connectivity
+        weights_subset_abs = torch.abs(weights_subset) - weight_changes.t()
+    weights_subset = torch.sign(weights_subset) * \
+        torch.clamp(weights_subset_abs, 0)
+    # finally modify in the big weights matrix.
+    model.all_weights[df.post.unique()[:, None], df.pre.unique()
+                      ] = weights_subset
```

### Comparing `connectome_interpreter-1.7.2/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.8.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: connectome-interpreter
-Version: 1.7.2
+Name: connectome_interpreter
+Version: 1.8.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
```

### Comparing `connectome_interpreter-1.7.2/connectome_interpreter.egg-info/SOURCES.txt` & `connectome_interpreter-1.8.0/connectome_interpreter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.2/setup.py` & `connectome_interpreter-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.7.2',
+    version='1.8.0',
     packages=find_packages(),
     install_requires=install_requires_list,
     extras_require={
         'get_ngl_link': ['nglscenes'],
         'wandb': ['wandb'],
     },
     # Optional metadata
```

### Comparing `connectome_interpreter-1.7.2/tests/test_compress_paths.py` & `connectome_interpreter-1.8.0/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.7.2/tests/test_utils.py` & `connectome_interpreter-1.8.0/tests/test_utils.py`

 * *Files identical despite different names*

