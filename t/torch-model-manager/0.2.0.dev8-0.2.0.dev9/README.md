# Comparing `tmp/torch_model_manager-0.2.0.dev8.tar.gz` & `tmp/torch_model_manager-0.2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.dev8.tar", last modified: Mon May  6 14:47:45 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev9.tar", last modified: Tue May  7 09:26:11 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.dev8.tar` & `torch_model_manager-0.2.0.dev9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.484921 torch_model_manager-0.2.0.dev8/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 14:47:45.480921 torch_model_manager-0.2.0.dev8/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-06 14:47:45.484921 torch_model_manager-0.2.0.dev8/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1482 2024-05-06 14:47:42.000000 torch_model_manager-0.2.0.dev8/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.472921 torch_model_manager-0.2.0.dev8/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.476921 torch_model_manager-0.2.0.dev8/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.476921 torch_model_manager-0.2.0.dev8/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.480921 torch_model_manager-0.2.0.dev8/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22114 2024-05-06 14:47:34.000000 torch_model_manager-0.2.0.dev8/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev8/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.480921 torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-06 14:47:45.000000 torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-06 14:47:45.000000 torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-06 14:47:45.000000 torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-06 14:47:45.000000 torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-06 14:47:45.000000 torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-06 14:47:45.480921 torch_model_manager-0.2.0.dev8/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev8/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     7112 2024-05-03 09:50:17.000000 torch_model_manager-0.2.0.dev8/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     8746 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     1482 2024-05-07 09:26:09.000000 torch_model_manager-0.2.0.dev9/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.310966 torch_model_manager-0.2.0.dev9/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       95 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    29212 2024-05-07 09:07:22.000000 torch_model_manager-0.2.0.dev9/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18476 2024-05-07 08:49:09.000000 torch_model_manager-0.2.0.dev9/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     8746 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      545 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       47 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-07 09:26:11.000000 torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 09:26:11.314966 torch_model_manager-0.2.0.dev9/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-07 07:29:44.000000 torch_model_manager-0.2.0.dev9/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     7112 2024-05-07 07:32:10.000000 torch_model_manager-0.2.0.dev9/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0.dev8/PKG-INFO` & `torch_model_manager-0.2.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev8/README.md` & `torch_model_manager-0.2.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev8/setup.py` & `torch_model_manager-0.2.0.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.2.0.dev8',
+    version='0.2.0.dev9',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.2.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev8/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev9/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev8/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev9/torch_model_manager/neptune_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,14 +64,16 @@
         if NeptuneManager.project_name not in management.get_project_list(api_token=NeptuneManager.api_token):
             NeptuneManager.project = management.create_project(name=NeptuneManager.project_name, 
                                 namespace=namespace, 
                                 key=key,
                                 visibility=visibility, 
                                 description=description, 
                                 api_token=api_token)
+        else:
+            NeptuneManager.project = neptune.init_project(project=NeptuneManager.project_name, api_token=NeptuneManager.api_token)
         if not os.path.exists(NeptuneManager.run_ids_path):
             # Create a JSON file
             with open(NeptuneManager.run_ids_path, 'w') as json_file:
                 json.dump({}, json_file)
             
 
     def get_project_list(self):
@@ -95,14 +97,180 @@
 
         Returns:
             The runs table as a pandas DataFrame.
         """
         runs_table_df = NeptuneManager.project.fetch_runs_table().to_pandas()
         return runs_table_df
     
+    def log_files(self, data, namespace, from_path=None, extension=None, wait = False):
+ 
+        try:
+            if from_path is not None:
+                NeptuneManager.project[namespace].upload(File.from_path(from_path, extension=extension), wait=wait)
+            else:
+                print(NeptuneManager.project)
+                NeptuneManager.project[namespace].upload(File.as_pickle(data), wait=wait)
+            print(Fore.GREEN+"The data are successfully loaded to the project."+Fore.WHITE)
+        except:
+            print(Fore.RED+"The data are not loaded to the project. Please check the path or the data format.\
+                This also might due to the existence of the same path in the namespace which risks to be overweighted."+Fore.WHITE)  
+        
+    def delete_data(self, namespaces, wait = False):
+        """
+        Delete data from the run.
+
+        Args:
+            namespaces: The namespaces to delete.
+        """
+        for namespace in namespaces:
+            NeptuneManager.project.pop(namespace, wait = wait)
+
+    def fetch_files(self, namespace):
+        ns = namespace.split("/")
+        
+        struct = NeptuneManager.project.get_structure()
+        for elem in ns :
+            struct = struct[elem]
+        
+        return list(struct.keys())
+
+    def log_tensors(self, 
+                    tensors, 
+                    descriptions: List[str] = None, 
+                    names: List[str] = None, 
+                    paths: List[str] = None, 
+                    namespace: str = None, 
+                    on_series: bool = False):
+        """
+        Log tensors to Neptune.
+
+        Args:
+            tensors: The tensors to log.
+            descriptions (List[str], optional): The descriptions of the tensors. Defaults to None.
+            names (List[str], optional): The names of the tensors. Defaults to None.
+            paths (List[str], optional): The paths of the tensors. Defaults to None.
+            namespace (str, optional): The namespace to log the tensors. Defaults to None.
+            on_series (bool, optional): Whether to log the tensors in series. Defaults to False.
+        """
+        # Transform the tensor to PIL image
+        to_pil = transforms.ToPILImage()
+        
+        # If the images are not uploaded in series, log them separately each one with its path
+        if not on_series:
+            for path, tensor in zip(paths, tensors) :
+                NeptuneManager.project[path].upload(File.as_image(to_pil(tensor)))
+        
+        # If the images are uploaded in series, log them in the same namespace
+        else:
+            if descriptions is not None:
+                for name, description, tensor in zip(names, descriptions, tensors):
+                    NeptuneManager.project[namespace].append(File.as_image(to_pil(tensor)), name=name, description=description)
+            else:
+                for name, tensor in zip(names, tensors):
+                    NeptuneManager.project[namespace].append(File.as_image(to_pil(tensor)), name=name)            
+
+        print(Fore.GREEN+"The tensors are successfully uploaded to Neptune.", Fore.WHITE)
+
+    def log_hidden_conv2d(self, 
+                          model: nn.Module,
+                          input_data: torch.Tensor, 
+                          indexes, 
+                          method="layercam",
+                          row_index: List[str] = None, 
+                          save_path=None,
+                          namespace=None,
+                          **kwargs) :
+        """
+        Log hidden conv2d layer outputs.
+
+        Args:
+            model (nn.Module): The model to log the hidden conv2d layer outputs for.
+            input_data (torch.Tensor): The input data.
+            indexes: The indexes of the layers.
+            method (str, optional): The method to use for generating the CAMs. Defaults to "layercam".
+            row_index (List[str], optional): The row indexes. Defaults to None.
+            save_path (str, optional): The path to save the figure. Defaults to None.
+            namespace (str, optional): The namespace to log the hidden conv2d layer outputs. Defaults to None.
+        """
+        assert namespace is not None, "Please provide an image namespace."
+        explainers = {
+            "layercam": LayerCAM,
+            "gradcam": GradCAM,
+            "smooth_gradcampp": SmoothGradCAMpp,
+            "gradcampp": GradCAMpp,
+            "scorecam": ScoreCAM,
+            "sscam": SSCAM,
+            "iscam": ISCAM,
+            "xgradcam": XGradCAM
+                
+        }
+        explainer = explainers[method]
+            
+        # Define the model mnager
+        model_manager= tmm.TorchModelManager(model)
+            
+        # Get the needed layers
+        layers = model_manager.get_layers_by_indexes(indexes)
+            
+        result = []
+        for im in input_data:
+            # Set the model to evaluation mode
+            tmp_model = model.eval()
+
+            # Extract the CAMs
+            layer_extractor = explainer(tmp_model, layers)
+            out = tmp_model(im.unsqueeze(0))
+            cams = layer_extractor(out.squeeze(0).argmax().item(), out)
+                
+                
+            if method != "layercam":
+                alpha = kwargs.get("alpha", 0.5)
+                to_pil_image = transforms.ToPILImage()
+                    
+                row_imgs = []
+                # Resize the CAM and overlay it
+                for cam in cams:
+                    cams = overlay_mask(to_pil_image(im), to_pil_image(cam.squeeze(0)), alpha=alpha)
+                    cams = transforms.ToTensor()(cams)
+                    row_imgs.append(cams)
+                    cams = row_imgs
+                # Display it
+                    
+                
+            result.append(cams)
+
+
+        if row_index is None:
+            row_index = np.arange(input_data.shape[0])
+            
+        # Parse the indexes
+        col_index = [helpers.parse_list(index, joiner='->') for index in indexes]
+
+        # Concatenate the images
+        figure = helpers.resize_and_concat_images(result)
+            
+        # Save the figure to disk if save_path is provided
+        if save_path is not None:
+            to_pil = transforms.ToPILImage()
+            pil_image = to_pil(figure)
+
+            # Save the PIL image to disk
+            pil_image.save(save_path)
+        
+        # Log the figure to Neptune
+        for res_row, row_ind in zip(result, row_index):
+            
+            self.log_tensors(tensors=res_row, 
+                            names = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
+                            namespace=namespace,
+                            on_series=True)
+                
+        print(Fore.GREEN+"The hidden conv2d layer outputs are successfully logged to Neptune.", Fore.WHITE)
+        return result, row_index, col_index 
+        
     class Run:
         """
         A class representing a Neptune run.
         """
         def __init__(self, 
                     name: str, 
                     description: str = None, 
@@ -269,15 +437,15 @@
             Args:
                 model (nn.Module): The model to track the metric for.
                 metric (Union[float, int]): The metric value.
                 namespace (str): The namespace to log the metric.
             """
             self.run[namespace].append(metric, step=step, timestamp=timestamp, wait=wait)
 
-        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, wait=False, **kwargs):
+        def log_checkpoint(self, namespace, model, optimizer, loss, epoch, keep_only_last = True, wait=False, **kwargs):
             state_dict = {
                 "model_state_dict": model.state_dict(),
                 "optimizer_state_dict": optimizer.state_dict(),
                 "loss": loss,
                 "epoch": epoch,
                 **kwargs
             }
@@ -499,17 +667,17 @@
             
             return list(struct.keys())
         
         def fetch_data(self, namespace):
             return self.run[namespace].fetch_values()
         
         
-# nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-#                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-#                     run_ids_path="run_ids.json")
+nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
+                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
+                    run_ids_path="run_ids.json")
 
 
 
 # run = nm.Run(name="Image GAT Message Passing")
 # data = run.fetch_pkl_data("embeddings")
 # print(data)
```

### Comparing `torch_model_manager-0.2.0.dev8/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev9/torch_model_manager/torch_model_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from utils import helpers
 from typing import List
 from torchviz import make_dot
 import torch
 from torchvision import transforms
 from torchcam.methods import LayerCAM
 from torchvision import models
+from torch.nn.init import xavier_uniform_, kaiming_uniform_, constant_, dirac_, kaiming_normal_, \
+                            xavier_normal_, uniform_, eye_, normal_, sparse_, ones_, orthogonal_, \
+                            zeros_, trunc_normal_
+                                
 
 class TorchModelManager:
     """
     A class for managing PyTorch models.
 
     Attributes:
         model: The PyTorch model to manage.
@@ -465,9 +469,41 @@
                                             names = helpers.concatenate_with_character(col_index, f"{row_ind} -> ", mode='pre'), 
                                             workspace=image_workspace,
                                             on_series=True)
                 
 
         return result, row_index, col_index
     
+    def init_model_parameters(self, method_weight, method_bias, **kwargs):
+        weight_args = kwargs.get('weight_args', None)
+        bias_args = kwargs.get('bias_args', None)
+        
+        for layer in self.model.children():
+            if isinstance(layer, (nn.Conv2d, 
+                        nn.Linear, 
+                        nn.ConvTranspose2d, 
+                        nn.Conv3d, 
+                        nn.ConvTranspose3d,
+                        nn.Embedding)):
+                
+                weight_initializer = eval(method_weight)
+                bias_initializer = eval(method_bias)
+                
+                weight_initializer(layer.weight, weight_args)
+                if layer.bias is not None:
+                    bias_initializer(layer.bias, bias_args)
+                    
+                
+                            
+                
+                
+                        
+# model = nn.Embedding(12, 13)
+# for layer in model.modules():
+#     if isinstance(layer, (nn.Conv2d, nn.Linear, nn.Embedding)):
+#         layer.weight.data.fill_(1)
 
-
+        
+# for layer in model.modules():
+#     if isinstance(layer, (nn.Conv2d, nn.Linear, nn.Embedding)):
+#         print(layer.weight.data)
+
```

### Comparing `torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0.dev8/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev9/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0.dev8/utils/helpers.py` & `torch_model_manager-0.2.0.dev9/utils/helpers.py`

 * *Files identical despite different names*

