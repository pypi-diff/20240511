# Comparing `tmp/fc_pruning-0.0.5.tar.gz` & `tmp/fc_pruning-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fc_pruning-0.0.5.tar", last modified: Thu May  2 10:57:32 2024, max compression
+gzip compressed data, was "fc_pruning-0.0.6.tar", last modified: Sat May 11 14:18:40 2024, max compression
```

## Comparing `fc_pruning-0.0.5.tar` & `fc_pruning-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.341402 fc_pruning-0.0.5/
--rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.5/LICENSE
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-02 10:57:32.341262 fc_pruning-0.0.5/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.5/README.md
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.339312 fc_pruning-0.0.5/fc_pruning/
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.340916 fc_pruning-0.0.5/fc_pruning/Compress/
--rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/Compress/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     5689 2024-04-30 18:40:51.000000 fc_pruning-0.0.5/fc_pruning/Compress/compress.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4983 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/Compress/utils.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/__init__.py
--rw-r--r--   0 aidamehammed   (501) staff       (20)     4112 2024-04-30 18:22:57.000000 fc_pruning-0.0.5/fc_pruning/utils.py
-drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-02 10:57:32.340250 fc_pruning-0.0.5/fc_pruning.egg-info/
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/PKG-INFO
--rw-r--r--   0 aidamehammed   (501) staff       (20)      331 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/SOURCES.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/dependency_links.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/requires.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-02 10:57:32.000000 fc_pruning-0.0.5/fc_pruning.egg-info/top_level.txt
--rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-02 10:57:32.341458 fc_pruning-0.0.5/setup.cfg
--rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-02 10:54:24.000000 fc_pruning-0.0.5/setup.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.194762 fc_pruning-0.0.6/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)    11352 2024-04-30 18:18:40.000000 fc_pruning-0.0.6/LICENSE
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-11 14:18:40.194653 fc_pruning-0.0.6/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      556 2024-04-30 18:18:40.000000 fc_pruning-0.0.6/README.md
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.193179 fc_pruning-0.0.6/fc_pruning/
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.194312 fc_pruning-0.0.6/fc_pruning/Compress/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       49 2024-04-30 18:22:57.000000 fc_pruning-0.0.6/fc_pruning/Compress/__init__.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     5650 2024-05-11 14:18:14.000000 fc_pruning-0.0.6/fc_pruning/Compress/compress.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     4137 2024-05-11 14:18:14.000000 fc_pruning-0.0.6/fc_pruning/Compress/utils.py
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        0 2024-04-30 18:22:57.000000 fc_pruning-0.0.6/fc_pruning/__init__.py
+drwxr-xr-x   0 aidamehammed   (501) staff       (20)        0 2024-05-11 14:18:40.193751 fc_pruning-0.0.6/fc_pruning.egg-info/
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1102 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/PKG-INFO
+-rw-r--r--   0 aidamehammed   (501) staff       (20)      311 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/SOURCES.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)        1 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/dependency_links.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       27 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/requires.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       11 2024-05-11 14:18:40.000000 fc_pruning-0.0.6/fc_pruning.egg-info/top_level.txt
+-rw-r--r--   0 aidamehammed   (501) staff       (20)       38 2024-05-11 14:18:40.194813 fc_pruning-0.0.6/setup.cfg
+-rw-r--r--   0 aidamehammed   (501) staff       (20)     1202 2024-05-11 14:18:28.000000 fc_pruning-0.0.6/setup.py
```

### Comparing `fc_pruning-0.0.5/LICENSE` & `fc_pruning-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.5/PKG-INFO` & `fc_pruning-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc_pruning
-Version: 0.0.5
+Version: 0.0.6
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.5/README.md` & `fc_pruning-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fc_pruning-0.0.5/fc_pruning/Compress/compress.py` & `fc_pruning-0.0.6/fc_pruning/Compress/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from FeatureCloud.app.engine.app import AppState
 from typing import TypedDict, Union, List, Type
 import torch
 import torch_pruning as tp
 import sys
-print(sys.executable)
 
 import fc_pruning.Compress.utils as pf
 
-print('running')
 
 class PruningType(TypedDict):
     model: torch.nn.Module
     reference_model: Union[List[torch.nn.Module], None]
     imp: Type[tp.pruner.importance.Importance]
     ignored_layers: Union[List[torch.nn.Module], None]
     pruning_ratio: float
```

### Comparing `fc_pruning-0.0.5/fc_pruning/Compress/utils.py` & `fc_pruning-0.0.6/fc_pruning/Compress/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,153 +1,138 @@
 import torch_pruning as tp
 import torch
 import torch.nn as nn
-import torch.optim as optim
 import copy
 import os
 
 
+def print_test():
+    print(' It works ')
+
+
 def get_weights(model):
     return [param.data for param in model.parameters()]
 
+
 def get_last_layer(model):
     last_layer = None
     for layer in model.modules():
         if isinstance(layer, nn.Linear):
             last_layer = layer
     return last_layer
-    
+
+
 def create_channel_mask(pruned_model):
     mask_list = []
 
     for param in pruned_model.parameters():
         mask = torch.ones_like(param)
         for idx, val in enumerate(param.view(-1)):
             if val == 0:
                 mask.view(-1)[idx] = 0
         mask_list.append(mask)
 
     return mask_list
-    
-def soft_prune(model, imp, example_inputs, iterative_steps=None, pruning_ratio=None, ignored_layers=None):
+
+
+def soft_prune(model, imp, example_inputs, pruning_ratio=None, ignored_layers=None):
     pmodel = copy.deepcopy(model)
 
     pruner = tp.pruner.MetaPruner(
         pmodel,
         example_inputs,
         importance=imp,
-        iterative_steps=iterative_steps,
         pruning_ratio=pruning_ratio,
         ignored_layers=ignored_layers
     )
 
-    for i in range(iterative_steps):
-        print('Applying soft pruning step')
-        for group in pruner.step(interactive=True):
-            #print(group)
-            for dep, idxs in group:
-                target_layer = dep.target.module
-                pruning_fn = dep.handler
-                if pruning_fn in [tp.prune_conv_in_channels, tp.prune_linear_in_channels]:
-                    target_layer.weight.data[:, idxs] *= 0
-                elif pruning_fn in [tp.prune_conv_out_channels, tp.prune_linear_out_channels]:
-                    target_layer.weight.data[idxs] *= 0
-                    if target_layer.bias is not None:
-                        target_layer.bias.data[idxs] *= 0
-                elif pruning_fn in [tp.prune_batchnorm_out_channels]:
-                    target_layer.weight.data[idxs] *= 0
+    print('Applying soft pruning step')
+    for group in pruner.step(interactive=True):
+        # print(group)
+        for dep, idxs in group:
+            target_layer = dep.target.module
+            pruning_fn = dep.handler
+            if pruning_fn in [tp.prune_conv_in_channels, tp.prune_linear_in_channels]:
+                target_layer.weight.data[:, idxs] *= 0
+            elif pruning_fn in [tp.prune_conv_out_channels, tp.prune_linear_out_channels]:
+                target_layer.weight.data[idxs] *= 0
+                if target_layer.bias is not None:
                     target_layer.bias.data[idxs] *= 0
+            elif pruning_fn in [tp.prune_batchnorm_out_channels]:
+                target_layer.weight.data[idxs] *= 0
+                target_layer.bias.data[idxs] *= 0
 
     mask_client_list = create_channel_mask(pmodel)
 
     return pmodel, mask_client_list
 
-def hard_prune_and_finetune(model, imp, example_inputs,learning_rate, iterative_steps=None, pruning_ratio=None, ignored_layers=None,
-                            epochs=None, train_loader=None):
+
+def hard_prune(model, imp, example_inputs, pruning_ratio=None, ignored_layers=None):
     pmodel = copy.deepcopy(model)
 
-    pruner = tp.pruner.MagnitudePruner(
+    pruner = tp.pruner.MetaPruner(
         pmodel,
         example_inputs,
         importance=imp,
-        iterative_steps=iterative_steps,
         pruning_ratio=pruning_ratio,
         ignored_layers=ignored_layers,
     )
 
-    for i in range(iterative_steps):
-        print('Applying hard pruning step')
+    print('Applying hard pruning step')
+
+    if isinstance(imp, tp.importance.TaylorImportance):
+        # Taylor expansion requires gradients for importance estimation
+        loss = pmodel(example_inputs).sum()  # a dummy loss for TaylorImportance
+        loss.backward()  # before pruner.step()
+        print(loss)
+    pruner.step()
 
-        if isinstance(imp, tp.importance.TaylorImportance):
-            # Taylor expansion requires gradients for importance estimation
-            loss = pmodel(example_inputs).sum()  # a dummy loss for TaylorImportance
-            loss.backward()  # before pruner.step()
-            pruner.regularize(pmodel, loss)
-            print(loss)
-        pruner.step()
-
-
-    # finetune model
-    criterion = nn.CrossEntropyLoss()
-    optimizer = optim.Adam(model.parameters(), lr=learning_rate)
-
-    for epoch in range(epochs):
-        model.train()
-        for i, (data, target) in enumerate(train_loader):
-            optimizer.zero_grad()
-            out = model(data)
-            loss = criterion(out, target)
-            loss.backward()
-            optimizer.step()
-            print(f'round:{epoch + 1}, loss:{loss.item()}')
     return pmodel
 
+
 def reconstruct_model(pruned_model_params, binary_mask, reference_model):
     pruned_idx = 0
 
     if reference_model is not None:
-
         flattened_params_ref = [tensor.flatten() for tensor in get_weights(reference_model)]
         reference_model_flat = torch.cat(flattened_params_ref, dim=0)
 
-
     flattened_params = [tensor.flatten() for tensor in pruned_model_params]
     pruned_model_flat = torch.cat(flattened_params, dim=0)
 
     flattened_tensors = [param.view(-1) for param in binary_mask]
     binary_mask_flat = torch.cat(flattened_tensors, dim=0)
 
     # Number of Parameters
     nr_param = len(binary_mask_flat)
 
     # Reconstruct by setting all zero
     reconstructed_model_flat = torch.zeros_like(binary_mask_flat)
 
     for idx in range(nr_param):
-      if binary_mask_flat[idx] == 1:
+        if binary_mask_flat[idx] == 1:
 
-        reconstructed_model_flat[idx] = pruned_model_flat[pruned_idx]
-        pruned_idx += 1
-      else:
-        if reference_model is not None:
-            reconstructed_model_flat[idx] = reference_model_flat[idx]
+            reconstructed_model_flat[idx] = pruned_model_flat[pruned_idx]
+            pruned_idx += 1
         else:
-            reconstructed_model_flat[idx]= 0.0
+            if reference_model is not None:
+                reconstructed_model_flat[idx] = reference_model_flat[idx]
+            else:
+                reconstructed_model_flat[idx] = 0.0
 
     desired_shape = [param_tensor.shape for param_tensor in binary_mask]
 
     reconstructed_model = []
     start = 0
     for shape in desired_shape:
         end = start + shape.numel()
         reconstructed_model.append(reconstructed_model_flat[start:end].reshape(shape))
         start = end
 
     return reconstructed_model
 
+
 def print_size_of_model(model):
     torch.save(model.state_dict(), "temp.p")
     size = os.path.getsize("temp.p") / 1e6  # size in MB
     os.remove('temp.p')
-    return size
-
-
+    return size
```

### Comparing `fc_pruning-0.0.5/fc_pruning.egg-info/PKG-INFO` & `fc_pruning-0.0.6/fc_pruning.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-pruning
-Version: 0.0.5
+Version: 0.0.6
 Summary: FC Pruning
 Home-page: https://github.com/AidaMehammed/fc_pruning
 Author: Aida Mehammed
 Author-email: aida.mehammed@studium.uni-hamburg.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AidaMehammed/fc_pruning/issues
 Platform: UNKNOWN
```

### Comparing `fc_pruning-0.0.5/setup.py` & `fc_pruning-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(name="fc_pruning",
-                 version="0.0.5",
+                 version="0.0.6",
                  author="Aida Mehammed",
                  author_email="aida.mehammed@studium.uni-hamburg.de",
                  description="FC Pruning",
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url="https://github.com/AidaMehammed/fc_pruning",
                  project_urls={
```

