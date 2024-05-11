# Comparing `tmp/lens_metric-0.1.1.tar.gz` & `tmp/lens_metric-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lens_metric-0.1.1.tar", last modified: Tue Jun 13 21:26:52 2023, max compression
+gzip compressed data, was "lens_metric-0.2.0.tar", last modified: Sat May 11 20:52:40 2024, max compression
```

## Comparing `lens_metric-0.1.1.tar` & `lens_metric-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.777818 lens_metric-0.1.1/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     9693 2023-06-13 21:20:38.000000 lens_metric-0.1.1/LICENSE
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      424 2023-06-13 21:26:52.780818 lens_metric-0.1.1/PKG-INFO
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1677 2023-06-13 21:20:38.000000 lens_metric-0.1.1/README.md
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.350815 lens_metric-0.1.1/lens/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/__init__.py
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.427816 lens_metric-0.1.1/lens/encoders/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      757 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/__init__.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2959 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/base.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     3482 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/bert.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2206 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/roberta.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1169 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/lens_score.py
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.572817 lens_metric-0.1.1/lens/models/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1612 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/models/__init__.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)    22468 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/models/base.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     8990 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/lru_cache.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     3703 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/metrics.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2266 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/pooling_utils.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      599 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/predict_pbar.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)    12439 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/regression_metric_multi_ref.py
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.640817 lens_metric-0.1.1/lens/modules/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      104 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/modules/__init__.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2549 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/modules/feedforward.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     5125 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/modules/layerwise_attention.py
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.759818 lens_metric-0.1.1/lens_metric.egg-info/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      424 2023-06-13 21:26:51.000000 lens_metric-0.1.1/lens_metric.egg-info/PKG-INFO
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      622 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/SOURCES.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        1 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/dependency_links.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      178 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/requires.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        5 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/top_level.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)       79 2023-06-13 21:26:52.792818 lens_metric-0.1.1/setup.cfg
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      855 2023-06-13 21:20:39.000000 lens_metric-0.1.1/setup.py
+drwxr-xr-x   0 dheineman3 (1098039) gtperson  (2626)        0 2024-05-11 20:52:40.556584 lens_metric-0.2.0/
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     9693 2024-05-11 19:11:12.000000 lens_metric-0.2.0/LICENSE
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      783 2024-05-11 20:52:40.531584 lens_metric-0.2.0/PKG-INFO
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     3308 2024-05-11 19:11:12.000000 lens_metric-0.2.0/README.md
+drwxr-xr-x   0 dheineman3 (1098039) gtperson  (2626)        0 2024-05-11 20:52:39.292595 lens_metric-0.2.0/lens/
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)       98 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/__init__.py
+drwxr-xr-x   0 dheineman3 (1098039) gtperson  (2626)        0 2024-05-11 20:52:39.464594 lens_metric-0.2.0/lens/encoders/
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      717 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/encoders/__init__.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)    15111 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/encoders/base.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     5424 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/encoders/bert.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     2256 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/encoders/roberta.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     5606 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/lens_score.py
+drwxr-xr-x   0 dheineman3 (1098039) gtperson  (2626)        0 2024-05-11 20:52:39.978589 lens_metric-0.2.0/lens/models/
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     2355 2024-05-11 20:40:08.000000 lens_metric-0.2.0/lens/models/__init__.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)    25487 2024-05-11 19:13:41.000000 lens_metric-0.2.0/lens/models/base.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     8990 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/lru_cache.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     4168 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/metrics.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     2266 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/pooling_utils.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     1204 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/predict_pbar.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     4698 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/predict_writer.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)    14966 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/regression_metric_multi_ref.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)    31848 2024-05-11 20:40:05.000000 lens_metric-0.2.0/lens/models/unified_metric.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     3173 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/models/utils.py
+drwxr-xr-x   0 dheineman3 (1098039) gtperson  (2626)        0 2024-05-11 20:52:40.107588 lens_metric-0.2.0/lens/modules/
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      104 2024-05-11 19:11:12.000000 lens_metric-0.2.0/lens/modules/__init__.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     2549 2024-05-11 19:11:13.000000 lens_metric-0.2.0/lens/modules/feedforward.py
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)     5517 2024-05-11 19:11:13.000000 lens_metric-0.2.0/lens/modules/layerwise_attention.py
+drwxr-xr-x   0 dheineman3 (1098039) gtperson  (2626)        0 2024-05-11 20:52:40.458585 lens_metric-0.2.0/lens_metric.egg-info/
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      783 2024-05-11 20:52:38.000000 lens_metric-0.2.0/lens_metric.egg-info/PKG-INFO
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      703 2024-05-11 20:52:39.000000 lens_metric-0.2.0/lens_metric.egg-info/SOURCES.txt
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)        1 2024-05-11 20:52:38.000000 lens_metric-0.2.0/lens_metric.egg-info/dependency_links.txt
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      182 2024-05-11 20:52:39.000000 lens_metric-0.2.0/lens_metric.egg-info/requires.txt
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)        5 2024-05-11 20:52:39.000000 lens_metric-0.2.0/lens_metric.egg-info/top_level.txt
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)       79 2024-05-11 20:52:40.570584 lens_metric-0.2.0/setup.cfg
+-rw-r--r--   0 dheineman3 (1098039) gtperson  (2626)      903 2024-05-11 19:17:22.000000 lens_metric-0.2.0/setup.py
```

### Comparing `lens_metric-0.1.1/LICENSE` & `lens_metric-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lens_metric-0.1.1/lens/encoders/__init__.py` & `lens_metric-0.2.0/lens/encoders/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import transformers
-from packaging import version
 
 from .bert import BERTEncoder
 from .roberta import RoBERTaEncoder
 
-
-str2encoder = {"BERT": BERTEncoder, "RoBERTa": RoBERTaEncoder}
+str2encoder = {
+    "BERT": BERTEncoder, 
+    "RoBERTa": RoBERTaEncoder
+}
```

### Comparing `lens_metric-0.1.1/lens/encoders/roberta.py` & `lens_metric-0.2.0/lens/encoders/roberta.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 RoBERTa Encoder
 ==============
     Pretrained RoBERTa  encoder from Hugging Face.
 """
 from typing import Dict
 
 import torch
-from lens.encoders.base import Encoder
-from lens.encoders.bert import BERTEncoder
+from .base import Encoder
+from .bert import BERTEncoder
 from transformers import AutoModel, AutoTokenizer
 
 
 class RoBERTaEncoder(BERTEncoder):
     """RoBERTA Encoder encoder.
 
     :param pretrained_model: Pretrained model from hugging face.
     """
 
-    def __init__(self, pretrained_model: str) -> None:
+    def __init__(self, pretrained_model: str, load_pretrained_weights: bool = True) -> None:
         super(Encoder, self).__init__()
         self.tokenizer = AutoTokenizer.from_pretrained(pretrained_model)
         self.model = AutoModel.from_pretrained(
             pretrained_model, add_pooling_layer=False
         )
         self.model.encoder.output_hidden_states = True
 
     @classmethod
-    def from_pretrained(cls, pretrained_model: str) -> Encoder:
+    def from_pretrained(cls, pretrained_model: str, load_pretrained_weights: bool = True) -> Encoder:
         """Function that loads a pretrained encoder from Hugging Face.
         :param pretrained_model: Name of the pretrain model to be loaded.
 
         :return: Encoder model
         """
         return RoBERTaEncoder(pretrained_model)
```

### Comparing `lens_metric-0.1.1/lens/models/__init__.py` & `lens_metric-0.2.0/lens/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,37 +10,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .regression_metric_multi_ref import RegressionMetricMultiReference
-from .base import CometModel
-
 import os
+from pathlib import Path
+from typing import Union
+
 import yaml
+from huggingface_hub import snapshot_download
+
+from .regression_metric_multi_ref import RegressionMetricMultiReference
+from .unified_metric import UnifiedMetric
+from .base import LensModel
+
 
 str2model = {
     "regression_metric_multi_ref": RegressionMetricMultiReference,
+    "unified_metric": UnifiedMetric,
 }
 
 
+def download_model(
+    model: str, 
+    saving_directory: Union[str, Path, None] = None
+) -> str:
+    model_path = snapshot_download(repo_id=model, cache_dir=saving_directory)
+    checkpoint_path = os.path.join(*[model_path, "checkpoints", "model.ckpt"])
+    return checkpoint_path
+
 
-def load_from_checkpoint(checkpoint_path: str) -> CometModel:
+def load_from_checkpoint(checkpoint_path: str) -> LensModel:
     """Loads models from a checkpoint path.
-    :param checkpoint_path: Path to a model checkpoint.
 
-    :return: Returns a COMET model.
+    Args:
+        checkpoint_path (str): Path to a model checkpoint.
+
+    Return:
+        COMET model.
     """
-    if not os.path.exists(checkpoint_path):
-        raise Exception(f"Invalid checkpoint path: {checkpoint_path}")
+    checkpoint_path = Path(checkpoint_path)
 
-    hparams_file = "/".join(checkpoint_path.split("/")[:-2] + ["hparams.yaml"])
-    if os.path.exists(hparams_file):
+    if not checkpoint_path.is_file():
+        raise Exception(f"Invalid checkpoint path: {checkpoint_path}")
+    
+    parent_folder = checkpoint_path.parents[1] # .parent.parent
+    hparams_file = parent_folder / "hparams.yaml"
+    
+    if hparams_file.is_file():
         with open(hparams_file) as yaml_file:
             hparams = yaml.load(yaml_file.read(), Loader=yaml.FullLoader)
         model_class = str2model[hparams["class_identifier"]]
-        model = model_class.load_from_checkpoint(checkpoint_path, **hparams)
+        # model = model_class.load_from_checkpoint(
+        #     checkpoint_path, load_pretrained_weights=False, strict=False
+        # )
+        model = model_class.load_from_checkpoint(
+            checkpoint_path, **hparams, strict=False
+        )
         return model
     else:
-        raise Exception("hparams.yaml file is missing!")
+        raise Exception(f"hparams.yaml file is missing from {parent_folder}!")
```

### Comparing `lens_metric-0.1.1/lens/models/base.py` & `lens_metric-0.2.0/lens/models/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,214 +9,233 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 r"""
-CometModel
+LensModel
 ========================
     Abstract Model class that implements some of the Pytorch Lightning logic.
-    Extend this class to create new model and metrics within COMET.
+    Extend this class to create new model and metrics within LENS.
 """
 import abc
 import logging
 import os
 import warnings
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pytorch_lightning as ptl
 import torch
-import transformers
-from lens.encoders import str2encoder
-from lens.modules import LayerwiseAttention
-from packaging import version
-from torch import nn
-from torch.utils.data import DataLoader, RandomSampler, Sampler, Subset
+from torch.utils.data import DataLoader, RandomSampler, SequentialSampler, Subset
+
+from ..encoders import str2encoder
+from ..modules import LayerwiseAttention
 
 from .lru_cache import tensor_lru_cache
 from .pooling_utils import average_pooling, max_pooling
 from .predict_pbar import PredictProgressBar
+from .predict_writer import CustomWriter
+from .utils import (
+    OrderedSampler,
+    Prediction,
+    Target,
+    flatten_metadata,
+    restore_list_order,
+)
 
-
-class OrderedSampler(Sampler[int]):
-    """
-    Sampler that returns the indices in a deterministic order.
-    """
-
-    def __init__(self, indices: List[int]):
-        self.indices = indices
-
-    def __iter__(self):
-        return iter(self.indices)
-
-    def __len__(self):
-        return len(self.indices)
-
-
-if "COMET_EMBEDDINGS_CACHE" in os.environ:
-    CACHE_SIZE = int(os.environ["COMET_EMBEDDINGS_CACHE"])
+if "LENS_EMBEDDINGS_CACHE" in os.environ:
+    CACHE_SIZE = int(os.environ["LENS_EMBEDDINGS_CACHE"])
 else:
     CACHE_SIZE = 1024
 
 
 logger = logging.getLogger(__name__)
 
 
-class CometModel(ptl.LightningModule, metaclass=abc.ABCMeta):
-    """CometModel:
+class LensModel(ptl.LightningModule, metaclass=abc.ABCMeta):
+    """LensModel: Base class for all LENS models.
 
-    :param nr_frozen_epochs: Number of epochs (% of epoch) that the encoder is frozen.
-    :param keep_embeddings_frozen: Keeps the encoder frozen during training.
-    :param optimizer: Optimizer used during training.
-    :param encoder_learning_rate: Learning rate used to fine-tune the encoder model.
-    :param learning_rate: Learning rate used to fine-tune the top layers.
-    :param layerwise_decay: Learning rate % decay from top-to-bottom encoder layers.
-    :param encoder_model: Encoder model to be used.
-    :param pretrained_model: Pretrained model from Hugging Face.
-    :param pool: Pooling strategy to derive a sentence embedding ['cls', 'max', 'avg'].
-    :param layer: Encoder layer to be used ('mix' for pooling info from all layers.)
-    :param dropout: Dropout used in the top-layers.
-    :param batch_size: Batch size used during training.
-    :param train_data: Path to a csv file containing the training data.
-    :param validation_data: Path to a csv file containing the validation data.
-    :param load_weights_from_checkpoint: Path to a checkpoint file.
-    :param class_identifier: subclass identifier.
+    Args:
+        nr_frozen_epochs (Union[float, int]): Number of epochs (% of epoch) that the
+            encoder is frozen. Defaults to 0.3.
+        keep_embeddings_frozen (bool): Keeps the encoder frozen during training. Defaults
+            to True.
+        optimizer (str): Optimizer used during training. Defaults to 'AdamW'.
+        warmup_steps (int): Warmup steps for LR scheduler.
+        encoder_learning_rate (float): Learning rate used to fine-tune the encoder model.
+            Defaults to 1.0e-06.
+        learning_rate (float): Learning rate used to fine-tune the top layers. Defaults
+            to 1.5e-05.
+        layerwise_decay (float): Learning rate % decay from top-to-bottom encoder layers.
+            Defaults to 0.95.
+        encoder_model (str): Encoder model to be used. Defaults to 'XLM-RoBERTa'.
+        pretrained_model (str): Pretrained model from Hugging Face. Defaults to
+            'xlm-roberta-large'.
+        pool (str): Type of sentence level pooling (options: 'max', 'cls', 'avg').
+            Defaults to 'avg'
+        layer (Union[str, int]): Encoder layer to be used for regression ('mix'
+            for pooling info from all layers). Defaults to 'mix'.
+        layer_transformation (str): Transformation applied when pooling info from all
+            layers (options: 'softmax', 'sparsemax'). Defaults to 'softmax'.
+        layer_norm (bool): Apply layer normalization. Defaults to 'True'.
+        loss (str): Loss function to be used. Defaults to 'mse'.
+        dropout (float): Dropout used in the top-layers. Defaults to 0.1.
+        batch_size (int): Batch size used during training. Defaults to 4.
+        train_data (Optional[List[str]]): List of paths to training data. Each file is
+            loaded consecutively for each epoch. Defaults to None.
+        validation_data (Optional[List[str]]): List of paths to validation data.
+            Validation results are averaged across validation set. Defaults to None.
     """
 
     def __init__(
         self,
         nr_frozen_epochs: Union[float, int] = 0.3,
-        keep_embeddings_frozen: bool = False,
+        keep_embeddings_frozen: bool = True,
         optimizer: str = "AdamW",
-        encoder_learning_rate: float = 1e-05,
-        learning_rate: float = 3e-05,
+        warmup_steps: int = 0,
+        encoder_learning_rate: float = 1.0e-06,
+        learning_rate: float = 1.5e-05,
         layerwise_decay: float = 0.95,
         encoder_model: str = "XLM-RoBERTa",
         pretrained_model: str = "xlm-roberta-large",
         pool: str = "avg",
         layer: Union[str, int] = "mix",
+        layer_transformation: str = "softmax",
+        layer_norm: bool = True,
+        loss: str = "mse",
         dropout: float = 0.1,
         batch_size: int = 4,
-        train_data: Optional[str] = None,
-        validation_data: Optional[str] = None,
-        load_weights_from_checkpoint: Optional[str] = None,
-        class_identifier: Optional[str] = None
+        train_data: Optional[List[str]] = None,
+        validation_data: Optional[List[str]] = None,
+        class_identifier: Optional[str] = None,
+        load_pretrained_weights: bool = True,
     ) -> None:
         super().__init__()
-        self.save_hyperparameters(
-            ignore=["train_data", "validation_data", "load_weights_from_checkpoint"]
-        )
-
-        if self.hparams.encoder_model == "XLM-RoBERTa-XL":
-            # Ensure backwards compatibility with transformer versions
-            if version.parse(transformers.__version__) < version.parse("4.17.0"):
-                raise Exception(
-                    "XLM-RoBERTa-XL requires transformers>=4.17.0. Your current version is {}".format(
-                        transformers.__version__
-                    )
-                )
+        self.save_hyperparameters()
 
         self.encoder = str2encoder[self.hparams.encoder_model].from_pretrained(
-            self.hparams.pretrained_model
+            self.hparams.pretrained_model, load_pretrained_weights
         )
 
         self.epoch_nr = 0
         if self.hparams.layer == "mix":
             self.layerwise_attention = LayerwiseAttention(
+                layer_transformation=layer_transformation,
                 num_layers=self.encoder.num_layers,
                 dropout=self.hparams.dropout,
-                layer_norm=True,
+                layer_norm=self.hparams.layer_norm,
             )
         else:
             self.layerwise_attention = None
 
         if self.hparams.nr_frozen_epochs > 0:
             self._frozen = True
             self.freeze_encoder()
         else:
             self._frozen = False
 
         if self.hparams.keep_embeddings_frozen:
             self.encoder.freeze_embeddings()
 
         self.nr_frozen_epochs = self.hparams.nr_frozen_epochs
-
-        if load_weights_from_checkpoint is not None:
-            if os.path.exists(load_weights_from_checkpoint):
-                self.load_weights(load_weights_from_checkpoint)
-            else:
-                logger.warning(f"Path {load_weights_from_checkpoint} does not exist!")
-
         self.mc_dropout = False  # Flag used to control usage of MC Dropout
         self.caching = False  # Flag used to control Embedding Caching
 
-    def set_mc_dropout(self, value: bool):
+        # If not defined here, metrics will not live in the same device as our model.
+        self.init_metrics()
+
+        # self.train_dataset = self.read_training_data(self.hparams.train_data[0])
+
+    def set_mc_dropout(self, value: int):
+        """Sets Monte Carlo Dropout runs per sample.
+
+        Args:
+            value (int): number of runs per sample.
+        """
         self.mc_dropout = value
 
-    def load_weights(self, checkpoint: str) -> None:
-        """Function that loads the weights from a given checkpoint file.
-        Note:
-            If the checkpoint model architecture is different then `self`, only
-            the common parts will be loaded.
-
-        :param checkpoint: Path to the checkpoint containing the weights to be loaded.
-        """
-        logger.info(f"Loading weights from {checkpoint}.")
-        checkpoint = torch.load(checkpoint, map_location=lambda storage, loc: storage)
-        pretrained_dict = checkpoint["state_dict"]
-        model_dict = self.state_dict()
-        # 1. filter out unnecessary keys
-        pretrained_dict = {k: v for k, v in pretrained_dict.items() if k in model_dict}
-        # 2. overwrite entries in the existing state dict
-        model_dict.update(pretrained_dict)
-        # 3. load the new state dict
-        self.load_state_dict(model_dict)
+    @abc.abstractmethod
+    def read_training_data(self) -> List[dict]:
+        """Abstract method that reads the training data.
+
+        Returns:
+            List[dict]: List with input samples in the form of a dict
+        """
+        pass
 
     @abc.abstractmethod
-    def read_csv(self):
+    def read_validation_data(self):
+        """Abstract method that reads the validation data. If validation data
+        has a columns 'system' we will output system-level accuracies for each
+        validation dataset.
+
+        Returns:
+            List[dict]: List with input samples in the form of a dict
+        """
         pass
 
     @abc.abstractmethod
     def prepare_sample(
-        self, sample: List[Dict[str, Union[str, float]]], *args, **kwargs
+        self,
+        sample: List[dict],
+        stage: str = "fit",
+        *args,
+        **kwargs,
     ):
+        """This method will be called by dataloaders to prepared data to input to the
+        model.
+
+        Args:
+            sample (List[dict]): Batch of train/val/test samples.
+            stage (str): model stage (options: 'fit', 'validate', 'test', or
+                'predict'). Defaults to 'fit'.
+
+        Returns:
+            Model inputs and (optionally) training labels/targets.
+        """
         pass
 
     @abc.abstractmethod
     def configure_optimizers(self):
+        """Pytorch Lightning method to configure optimizers and schedulers."""
         pass
 
     @abc.abstractmethod
     def init_metrics(self) -> None:
+        """Initializes train/validation metrics."""
         pass
 
     @abc.abstractmethod
-    def forward(self, *args, **kwargs) -> Dict[str, torch.Tensor]:
+    def forward(self, *args, **kwargs) -> Prediction:
+        """Pytorch model forward method."""
         pass
-    
+
     @abc.abstractmethod
-    def is_referenceless(self) -> bool:
+    def requires_references(self) -> bool:
+        """Whether or not this models work with references."""
         pass
 
     def freeze_encoder(self) -> None:
+        """Deactivates training for encoder model parameters (keeping them frozen)"""
         logger.info("Encoder model frozen.")
         self.encoder.freeze()
 
     @property
-    def loss(self) -> None:
-        return nn.MSELoss()
-
-    def compute_loss(
-        self, predictions: Dict[str, torch.Tensor], targets: Dict[str, torch.Tensor]
-    ) -> torch.Tensor:
-        return self.loss(predictions["score"].view(-1), targets["score"])
+    def loss(self):
+        """Loss function"""
+        return torch.nn.MSELoss()
+
+    def compute_loss(self, prediction: Prediction, target: Target) -> torch.Tensor:
+        """Computes Loss value between a batch Prediction and respective Target."""
+        return self.loss(prediction.scores, target.scores)
 
     def unfreeze_encoder(self) -> None:
+        """Activates fine-tuning of encoder parameters."""
         if self._frozen:
             if self.trainer.is_global_zero:
                 logger.info("Encoder model fine-tuning")
 
             self.encoder.unfreeze()
             self._frozen = False
             if self.hparams.keep_embeddings_frozen:
@@ -230,60 +249,83 @@
             self._frozen = False
 
     def set_embedding_cache(self):
         """Function that when called turns embedding caching on."""
         self.caching = True
 
     def get_sentence_embedding(
-        self, input_ids: torch.Tensor, attention_mask: torch.Tensor
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: torch.Tensor,
+        token_type_ids: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         """Function that extracts sentence embeddings for
-            a single sentence.
+        a single sentence and allows for caching embeddings.
 
-        :param tokens: sequences [batch_size x seq_len]
-        :param lengths: lengths [batch_size]
+        Args:
+            tokens (torch.Tensor): sequences [batch_size x seq_len].
+            attention_mask (torch.Tensor): attention_mask [batch_size x seq_len].
+            token_type_ids (torch.Tensor): Model token_type_ids [batch_size x seq_len].
+                Optional
 
-        :return: torch.Tensor [batch_size x hidden_size]
+        Returns:
+            torch.Tensor [batch_size x hidden_size] with sentence embeddings.
         """
         if self.caching:
-            return self.retrieve_sentence_embedding(input_ids, attention_mask)
+            return self.retrieve_sentence_embedding(
+                input_ids=input_ids,
+                attention_mask=attention_mask,
+                token_type_ids=token_type_ids,
+            )
         else:
-            return self.compute_sentence_embedding(input_ids, attention_mask)
+            return self.compute_sentence_embedding(
+                input_ids,
+                attention_mask,
+                token_type_ids=token_type_ids,
+            )
 
     @tensor_lru_cache(maxsize=CACHE_SIZE)
     def retrieve_sentence_embedding(
-        self, input_ids: torch.Tensor, attention_mask: torch.Tensor
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: torch.Tensor,
+        token_type_ids: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         """Wrapper for `get_sentence_embedding` function that caches results."""
-        return self.compute_sentence_embedding(input_ids, attention_mask)
+        return self.compute_sentence_embedding(
+            input_ids=input_ids,
+            attention_mask=attention_mask,
+            token_type_ids=token_type_ids,
+        )
 
     def compute_sentence_embedding(
-        self, input_ids: torch.Tensor, attention_mask: torch.Tensor
-    ) -> torch.Tensor:
+        self,
+        input_ids: torch.Tensor,
+        attention_mask: torch.Tensor,
+        token_type_ids: Optional[torch.Tensor] = None,
+    ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
+        """Function that extracts sentence embeddings for
+        a single sentence.
+
+        Args:
+            tokens (torch.Tensor): sequences [batch_size x seq_len].
+            attention_mask (torch.Tensor): attention_mask [batch_size x seq_len].
+            token_type_ids (torch.Tensor): Model token_type_ids [batch_size x seq_len].
+                Optional
 
-        encoder_out = self.encoder(input_ids, attention_mask)
+        Returns:
+            torch.Tensor [batch_size x hidden_size] with sentence embeddings.
+        """
+        encoder_out = self.encoder(
+            input_ids, attention_mask, token_type_ids=token_type_ids
+        )
         if self.layerwise_attention:
-            # HACK: LayerNorm is applied at the MiniBatch. This means that for big batch sizes the variance
-            # and norm within the batch will create small differences in the final score
-            # If we are predicting we split the data into equal size batches to minimize this variance.
-            if not self.training:
-                n_splits = len(torch.split(encoder_out["all_layers"][-1], 8))
-                embeddings = []
-                for split in range(n_splits):
-                    all_layers = []
-                    for layer in range(len(encoder_out["all_layers"])):
-                        layer_embs = torch.split(encoder_out["all_layers"][layer], 8)
-                        all_layers.append(layer_embs[split])
-                    split_attn = torch.split(attention_mask, 8)[split]
-                    embeddings.append(self.layerwise_attention(all_layers, split_attn))
-                embeddings = torch.cat(embeddings, dim=0)
-            else:
-                embeddings = self.layerwise_attention(
-                    encoder_out["all_layers"], attention_mask
-                )
+            embeddings = self.layerwise_attention(
+                encoder_out["all_layers"], attention_mask
+            )
 
         elif self.hparams.layer >= 0 and self.hparams.layer < self.encoder.num_layers:
             embeddings = encoder_out["all_layers"][self.hparams.layer]
 
         else:
             raise Exception("Invalid model layer {}.".format(self.hparams.layer))
 
@@ -309,278 +351,336 @@
         else:
             raise Exception("Invalid pooling technique.")
 
         return sentemb
 
     def training_step(
         self,
-        batch: Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]],
-        batch_nb: int,
+        batch: Tuple[dict, Target],
+        batch_idx: int,
     ) -> torch.Tensor:
-        """
-        Runs one training step and logs the training loss.
+        """Pytorch Lightning training step.
 
-        :param batch: The output of your prepare_sample function.
-        :param batch_nb: Integer displaying which batch this is.
+        Args:
+            batch (Tuple[dict, Target]): The output of your `prepare_sample` method.
+            batch_idx (int): Integer displaying which batch this is.
 
-        :returns: Loss value
+        Returns:
+            [torch.Tensor] Loss value
         """
         batch_input, batch_target = batch
         batch_prediction = self.forward(**batch_input)
         loss_value = self.compute_loss(batch_prediction, batch_target)
 
         if (
             self.nr_frozen_epochs < 1.0
             and self.nr_frozen_epochs > 0.0
-            and batch_nb > self.epoch_total_steps * self.nr_frozen_epochs
+            and batch_idx > self.first_epoch_total_steps * self.nr_frozen_epochs
         ):
             self.unfreeze_encoder()
             self._frozen = False
 
         self.log("train_loss", loss_value, on_step=True, on_epoch=True)
         return loss_value
 
     def validation_step(
         self,
         batch: Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]],
         batch_nb: int,
         dataloader_idx: int,
     ) -> None:
-        """
-        Runs one validation step and logs metrics.
+        """Pytorch Lightning validation step. Runs model and logs metircs.
 
-        :param batch: The output of your prepare_sample function.
-        :param batch_nb: Integer displaying which batch this is.
-        :param dataloader_idx: Integer displaying which dataloader this is.
+        Args:
+            batch (Tuple[dict, Target]): The output of your `prepare_sample` method.
+            batch_idx (int): Integer displaying which batch this is.
         """
         batch_input, batch_target = batch
         batch_prediction = self.forward(**batch_input)
-        loss_value = self.compute_loss(batch_prediction, batch_target)
-        self.log("val_loss", loss_value, on_step=True, on_epoch=True)
+        if dataloader_idx == 0:
+            self.train_metrics.update(batch_prediction.scores, batch_target["scores"])
 
-        # TODO: REMOVE if condition after torchmetrics bug fix
-        if batch_prediction["score"].view(-1).size() != torch.Size([1]):
-            if dataloader_idx == 0:
-                self.train_metrics.update(
-                    batch_prediction["score"].view(-1), batch_target["score"]
-                )
-            elif dataloader_idx == 1:
-                self.val_metrics.update(
-                    batch_prediction["score"].view(-1), batch_target["score"]
-                )
+        elif dataloader_idx > 0:
+            self.val_metrics[dataloader_idx - 1].update(
+                batch_prediction.scores,
+                batch_target["scores"],
+                batch_target["system"] if "system" in batch_target else None,
+            )
 
     def on_predict_start(self) -> None:
-        """Called when predict begins."""
+        """Called when predict begins to setup mc_dropout."""
         if self.mc_dropout:
             self.train()
         else:
             self.eval()
 
     def predict_step(
         self,
         batch: Dict[str, torch.Tensor],
         batch_idx: Optional[int] = None,
         dataloader_idx: Optional[int] = None,
     ) -> torch.Tensor:
-        """
-        Runs one prediction step and returns the predicted values.
+        """Pytorch Lightning predict step.
+
+        Args:
+            batch (Tuple[dict, Target]): The output of your `prepare_sample` method.
+            batch_idx (int): Integer displaying which batch this is.
+            dataloader_idx (int): Integer displaying which dataloader this sample is
+                coming from.
 
-        :param batch: The output of your prepare_sample function.
-        :param batch_nb: Integer displaying which batch this is.
-        :param dataloader_idx: Integer displaying which dataloader this is.
+        Return:
+            Predicion object
         """
+        # Legacy implementation
+        model_outputs = Prediction(scores=self(**batch)["scores"].view(-1))
+
+        # Implementation with Prediction object
+        # model_outputs = Prediction(scores=self(**batch).scores)
         if self.mc_dropout:
             mcd_outputs = torch.stack(
-                [self(**batch)["score"].view(-1) for _ in range(self.mc_dropout)]
+                [self(**batch).scores for _ in range(self.mc_dropout)]
             )
-            mcd_mean = mcd_outputs.mean(dim=0)
-            mcd_std = mcd_outputs.std(dim=0)
-            return mcd_mean, mcd_std
-
-        return self(**batch)["score"].view(-1)
+            model_outputs["metadata"] = Prediction(
+                mcd_scores=mcd_outputs.mean(dim=0),
+                mcd_std=mcd_outputs.std(dim=0),
+            )
+        return model_outputs
 
     def validation_epoch_end(self, *args, **kwargs) -> None:
         """Computes and logs metrics."""
-        self.log_dict(self.train_metrics.compute(), prog_bar=True)
-        self.log_dict(self.val_metrics.compute(), prog_bar=True)
+        self.log_dict(self.train_metrics.compute(), prog_bar=False)
         self.train_metrics.reset()
-        self.val_metrics.reset()
-        
 
-    def setup(self, stage) -> None:
+        val_metrics = []
+        for i in range(len(self.hparams.validation_data)):
+            results = self.val_metrics[i].compute()
+            self.val_metrics[i].reset()
+            # Log to tensorboard the results for this validation set.
+            self.log_dict(results, prog_bar=False)
+            val_metrics.append(results)
+
+        average_results = {"val_" + k.split("_")[-1]: [] for k in val_metrics[0].keys()}
+        for i in range(len(val_metrics)):
+            for k, v in val_metrics[i].items():
+                average_results["val_" + k.split("_")[-1]].append(v)
+
+        self.log_dict(
+            {k: sum(v) / len(v) for k, v in average_results.items()}, prog_bar=True
+        )
+
+    def setup(self, stage: str) -> None:
         """Data preparation function called before training by Lightning.
 
-        :param stage: either 'fit', 'validate', 'test', or 'predict'
+        stage (str): either 'fit', 'validate', 'test', or 'predict'
         """
         if stage in (None, "fit"):
-            self.train_dataset = self.read_csv(self.hparams.train_data)
-            self.validation_dataset = self.read_csv(self.hparams.validation_data)
+            train_dataset = self.read_training_data(self.hparams.train_data[0])
+
+            self.validation_sets = [
+                self.read_validation_data(d) for d in self.hparams.validation_data
+            ]
 
-            self.epoch_total_steps = len(self.train_dataset) // (
+            self.first_epoch_total_steps = len(train_dataset) // (
                 self.hparams.batch_size * max(1, self.trainer.num_devices)
             )
+
+            # Legacy implementation uses these:
+            self.epoch_total_steps = self.first_epoch_total_steps
             self.total_steps = self.epoch_total_steps * float(self.trainer.max_epochs)
 
-            # Always validate the model with 2k examples to control overfit.
-            train_subset = np.random.choice(a=len(self.train_dataset), size=2000)
-            self.train_subset = Subset(self.train_dataset, train_subset)
-            self.init_metrics()
+            # Always validate the model with part of training.
+            train_subset = np.random.choice(
+                a=len(train_dataset), size=min(1000, int(len(train_dataset) * 0.2))
+            )
+            self.train_subset = Subset(train_dataset, train_subset)
 
     def train_dataloader(self) -> DataLoader:
-        """Function that loads the train set."""
+        """Method that loads the train dataloader. Can be called every epoch to load a
+        different trainset if `reload_dataloaders_every_n_epochs=1` in Lightning
+        Trainer.
+        """
+        # I removed the lambda function as this was causing pickle problems
+
+        # Causes more pickle problems, so I loaded the data in __init__ instead.
+        # This is meant for interweaving multiple datasets, which is helpful, but we
+        # don't need this.
+        # data_path = self.hparams.train_data[
+        #     self.current_epoch % len(self.hparams.train_data)
+        # ]
+        # train_dataset = self.read_training_data(data_path)
+        # logger.info(f"Loading {data_path}.")
+
+        train_dataset = self.train_dataset
+
         return DataLoader(
-            dataset=self.train_dataset,
-            sampler=RandomSampler(self.train_dataset),
+            dataset=train_dataset,
+            sampler=RandomSampler(train_dataset),
             batch_size=self.hparams.batch_size,
-            collate_fn=self.prepare_sample,
+            collate_fn=self.prepare_sample, # lambda s: self.prepare_sample(s, stage="fit")
             num_workers=2 * self.trainer.num_devices,
         )
 
     def val_dataloader(self) -> DataLoader:
-        """Function that loads the validation set."""
-        return [
+        """Function that loads the validation sets."""
+        # I removed the lambda function as this was causing pickle problems
+        val_data = [
             DataLoader(
                 dataset=self.train_subset,
                 batch_size=self.hparams.batch_size,
-                collate_fn=self.prepare_sample,
-                num_workers=2 * self.trainer.num_devices,
-            ),
-            DataLoader(
-                dataset=self.validation_dataset,
-                batch_size=self.hparams.batch_size,
-                collate_fn=self.prepare_sample,
+                collate_fn=self.prepare_sample, # lambda s: self.prepare_sample(s, stage="validate")
                 num_workers=2 * self.trainer.num_devices,
-            ),
+            )
         ]
+        for validation_set in self.validation_sets:
+            val_data.append(
+                DataLoader(
+                    dataset=validation_set,
+                    batch_size=self.hparams.batch_size,
+                    collate_fn=self.prepare_sample, # lambda s: self.prepare_sample(s, stage="validate")
+                    num_workers=2 * self.trainer.num_devices,
+                )
+            )
+        return val_data
 
     def prepare_for_inference(self, sample):
-        """Ideally this should be a lamba function but for some reason python does not copy local lambda functions.
-        This functions replaces `collate_fn=lambda x: self.prepare_sample(x, inference=True)` from line 434.
+        """This is to avoid having a lamba function inside the predict dataloader
+        `collate_fn=lambda x: self.prepare_sample(x, inference=True)`
         """
-        return self.prepare_sample(sample, inference=True)
+        return self.prepare_sample(sample, stage="predict")
 
     def predict(
         self,
         samples: List[Dict[str, str]],
-        batch_size: int = 8,
-        gpus: int = 1,
-        mc_dropout: Union[int, bool] = False,
+        batch_size: int = 16,
+        devices: Union[List[int], str, int] = None,
+        mc_dropout: int = 0,
         progress_bar: bool = True,
-        accelerator: str = "ddp",
+        accelerator: str = "auto",
         num_workers: int = None,
         length_batching: bool = True,
-    ) -> Union[Tuple[List[float], float], Tuple[List[float], List[float], float]]:
-        """Function that receives a list of samples (dictionaries with translations, sources and/or references)
-        and returns segment level scores and a system level score. If `mc_dropout` is set, it also returns for each
-        segment score, a confidence value.
-
-        :param samples: List with dictionaries with source, translations and/or references.
-        :param batch_size: Batch size used during inference.
-        :param gpus: Number of GPUs to be used.
-        :param mc_dropout: Number of inference steps to run using MCD. Its disabled by default!
-        :param progress_bar: Flag that turns on and off the predict progress bar.
-        :param accelarator: Pytorch Lightning accelerator (e.g: dp, ddp).
-        :param num_workers: Number of workers to use when loading data from dataloaders.
-        :param length_batching: If set to true, reduces padding by sorting samples by MT length.
-
-        :return: List with segment-level scores and a system-score or segment-level scores, segment-level
-            confidence and a system-score.
-        """
-        # HACK: Workaround pytorch bug that prevents ParameterList to be used in DP
-        # https://github.com/pytorch/pytorch/issues/36035
-        if self.layerwise_attention is not None and gpus > 1:
-            self.layerwise_attention.gamma_value = float(
-                self.layerwise_attention.gamma[0]
-            )
-            self.layerwise_attention.weights = [
-                float(parameter[0])
-                for parameter in self.layerwise_attention.scalar_parameters
-            ]
+    ) -> Prediction:
+        """Method that receives a list of samples (dictionaries with translations,
+        sources and/or references) and returns segment-level scores, system level score
+        and any other metadata outputed by LENS models. If `mc_dropout` is set, it
+        also returns for each segment score, a confidence value.
+
+        Args:
+            samples (List[Dict[str, str]]): List with dictionaries with source,
+                translations and/or references.
+            batch_size (int): Batch size used during inference. Defaults to 16
+            devices (Optional[List[int]]): A sequence of device indices to be used.
+                Default: None.
+            mc_dropout (int): Number of inference steps to run using MCD. Defaults to 0
+            progress_bar (bool): Flag that turns on and off the predict progress bar.
+                Defaults to True
+            accelarator (str): Pytorch Lightning accelerator (e.g: 'cpu', 'cuda', 'hpu'
+                , 'ipu', 'mps', 'tpu'). Defaults to 'auto'
+            num_workers (int): Number of workers to use when loading and preparing
+                data. Defaults to None
+            length_batching (bool): If set to true, reduces padding by sorting samples
+                by sequence length. Defaults to True.
+
+        Return:
+            Prediction object with `scores`, `system_score` and any metadata returned
+                by the model.
+        """
+        # Don't use all GPUs if there are less samples than GPUs
+        if devices and len(devices) > 0:
+          # Don't use all GPUs if there are less samples than GPUs
+          if len(samples) < len(devices): 
+              devices = range(len(samples))
+          gpus = len(devices)
+        else:
+          gpus = 0
+        
+        if mc_dropout > 0:
+            self.set_mc_dropout(mc_dropout)
+
+        if devices is not None:
+            assert len(devices) == gpus, AssertionError(
+                "List of devices must be same size as `gpus`"
+            )
+        else:
+            devices = gpus if gpus > 0 else None
 
-        # TODO: ideally this should be based on the actual token_ids
-        # but that would require fundamentally changing the way dataloader is
-        # setup, so currently raw chars are used as an approximation
-        sampler = None
+        sampler = SequentialSampler(samples)
         if length_batching and gpus < 2:
-            sort_ids = np.argsort([len(sample["src"]) for sample in samples])
+            try:
+                sort_ids = np.argsort([len(sample["src"]) for sample in samples])
+            except KeyError:
+                sort_ids = np.argsort([i for i, sample in enumerate(samples)])
             sampler = OrderedSampler(sort_ids)
 
         if num_workers is None:
+            # Guideline for workers that typically works well.
             num_workers = 2 * gpus
 
         self.eval()
         dataloader = DataLoader(
             dataset=samples,
             batch_size=batch_size,
             sampler=sampler,
             collate_fn=self.prepare_for_inference,
             num_workers=num_workers,
         )
-        accelerator = accelerator if gpus > 1 else None
+        if gpus > 1:
+            pred_writer = CustomWriter()
+            callbacks = [pred_writer]
+        else:
+            callbacks = []
+
+        if gpus == 0: 
+          devices = 'auto'
+
+        if progress_bar:
+            enable_progress_bar = True
+            callbacks.append(PredictProgressBar())
+        else:
+            enable_progress_bar = False
 
         warnings.filterwarnings(
             "ignore",
             category=UserWarning,
             message=".*Consider increasing the value of the `num_workers` argument` .*",
         )
-        if progress_bar:
-            trainer = ptl.Trainer(
-                gpus=gpus,
-                deterministic=True,
-                logger=False,
-                callbacks=[PredictProgressBar()],
-                accelerator=accelerator,
-                max_epochs=-1
-            )
-        else:
-            trainer = ptl.Trainer(
-                gpus=gpus,
-                deterministic=True,
-                logger=False,
-                progress_bar_refresh_rate=0,
-                accelerator=accelerator,
-                max_epochs=-1
-            )
-
-        # TODO:
-        # Remove this upon resolution of:
-        # https://github.com/PyTorchLightning/pytorch-lightning/discussions/11392
-        warnings.filterwarnings(
-            "ignore",
-            category=UserWarning,
-            message="Your `predict_dataloader`'s sampler has shuffling enabled.*",
+        trainer = ptl.Trainer(
+            devices=devices,
+            logger=False,
+            callbacks=callbacks,
+            accelerator=accelerator if gpus > 0 else "cpu",
+            strategy="auto",
+            enable_progress_bar=enable_progress_bar,
+        )
+        return_predictions = False if gpus > 1 else True
+        predictions = trainer.predict(
+            self, dataloaders=dataloader, return_predictions=return_predictions
         )
+        if gpus > 1:
+            torch.distributed.barrier()  # Waits for all processes to finish predict
 
-        if mc_dropout:
-            self.set_mc_dropout(mc_dropout)
-            predictions = trainer.predict(
-                self, dataloaders=dataloader, return_predictions=True
-            )
-            mean_scores = [out[0] for out in predictions]
-            std_scores = [out[1] for out in predictions]
-            mean_scores = torch.cat(mean_scores, dim=0).tolist()
-            std_scores = torch.cat(std_scores, dim=0).tolist()
-            if length_batching and gpus < 2:
-                unsorted_mean_scores = [None for _ in range(len(samples))]
-                unsorted_std_scores = [None for _ in range(len(samples))]
-                for idx, mean_score, std_score in zip(
-                    sort_ids, mean_scores, std_scores
-                ):
-                    unsorted_mean_scores[idx] = mean_score
-                    unsorted_std_scores[idx] = std_score
-                mean_scores = unsorted_mean_scores
-                std_scores = unsorted_std_scores
-
-            return mean_scores, std_scores, sum(mean_scores) / len(mean_scores)
-
-        else:
-            predictions = trainer.predict(
-                self, dataloaders=dataloader, return_predictions=True
-            )
-            predictions = torch.cat(predictions, dim=0).tolist()
-            if length_batching and gpus < 2:
-                unsorted_predictions = [None for _ in range(len(samples))]
-                for idx, prediction in zip(sort_ids, predictions):
-                    unsorted_predictions[idx] = prediction
-                predictions = unsorted_predictions
+        # If we are in the GLOBAL RANK we need to gather all predictions
+        if gpus > 1 and trainer.is_global_zero:
+            predictions = pred_writer.gather_all_predictions()
+            # Delete Temp folder.
+            pred_writer.cleanup()
+            return predictions
+
+        elif gpus > 1 and not trainer.is_global_zero:
+            # If we are not in the GLOBAL RANK we will return None
+            exit()
+
+        scores = torch.cat([pred.scores for pred in predictions], dim=0).tolist()
+        if "metadata" in predictions[0]:
+            metadata = flatten_metadata([pred.metadata for pred in predictions])
+        else:
+            metadata = []
 
-            return predictions, sum(predictions) / len(predictions)
+        if length_batching and gpus < 2:
+            scores = restore_list_order(scores, sort_ids)
+            output = Prediction(scores=scores, system_score=sum(scores) / len(scores))
+            if metadata:
+                output["metadata"] = Prediction(
+                    **{k: restore_list_order(v, sort_ids) for k, v in metadata.items()}
+                )
+            return output
+        else:
+            return Prediction(scores=scores, system_score=sum(scores) / len(scores))
```

### Comparing `lens_metric-0.1.1/lens/models/lru_cache.py` & `lens_metric-0.2.0/lens/models/lru_cache.py`

 * *Files identical despite different names*

### Comparing `lens_metric-0.1.1/lens/models/metrics.py` & `lens_metric-0.2.0/lens/models/metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,83 +12,98 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
 Metrics
 =======
-    Regression and Ranking metrics to be used during training to measure 
+    Regression and Ranking metrics to be used during training to measure
     correlations with human judgements
 """
-import torch
-from torch import Tensor
-
-from torchmetrics import Metric
 from typing import Any, Callable, List, Optional
 import scipy.stats as stats
+import torch
+from torchmetrics import MatthewsCorrCoef, Metric
+
+
+
+class MCCMetric(MatthewsCorrCoef):
+    def __init__(self, prefix: str = "", **kwargs) -> None:
+        super().__init__(**kwargs)
+        self.prefix = prefix
+
+    def compute(self) -> torch.Tensor:
+        """Computes matthews correlation coefficient."""
+        mcc = super(MCCMetric, self).compute()
+        return {self.prefix + "_mcc": mcc}
 
 
 class RegressionMetrics(Metric):
     is_differentiable = False
     higher_is_better = True
-    preds: List[Tensor]
-    target: List[Tensor]
+    preds: List[torch.Tensor]
+    target: List[torch.Tensor]
 
     def __init__(
         self,
         prefix: str = "",
-        compute_on_step: bool = False,
+        # compute_on_step: bool = False,
         dist_sync_on_step: bool = False,
         process_group: Optional[Any] = None,
         dist_sync_fn: Optional[Callable] = None,
     ) -> None:
         super().__init__(
-            compute_on_step=compute_on_step,
+            # compute_on_step=compute_on_step,
             dist_sync_on_step=dist_sync_on_step,
             process_group=process_group,
             dist_sync_fn=dist_sync_fn,
         )
         self.add_state("preds", default=[], dist_reduce_fx="cat")
         self.add_state("target", default=[], dist_reduce_fx="cat")
         self.prefix = prefix
 
-        
-    def update(self, preds: Tensor, target: Tensor) -> None:  # type: ignore
+    def update(
+        self,
+        preds: torch.Tensor,
+        target: torch.Tensor,
+        systems: Optional[List[str]] = None,
+    ) -> None:  # type: ignore
         """Update state with predictions and targets.
+
         Args:
-            preds: Predictions from model
-            target: Ground truth values
+            preds (torch.Tensor): Predictions from model
+            target (torch.Tensor): Ground truth values
         """
         self.preds.append(preds)
         self.target.append(target)
 
-    def compute(self) -> Tensor:
-        """ Computes spearmans correlation coefficient. """
+    def compute(self) -> torch.Tensor:
+        """Computes spearmans correlation coefficient."""
         preds = torch.cat(self.preds, dim=0)
         target = torch.cat(self.target, dim=0)
         kendall, _ = stats.kendalltau(preds.tolist(), target.tolist())
         spearman, _ = stats.spearmanr(preds.tolist(), target.tolist())
         pearson, _ = stats.pearsonr(preds.tolist(), target.tolist())
         return {
             self.prefix + "_kendall": kendall,
             self.prefix + "_spearman": spearman,
-            self.prefix + "_pearson": pearson,         
+            self.prefix + "_pearson": pearson,
         }
 
 class WMTKendall(Metric):
     def __init__(
         self,
         prefix: str = "",
-        compute_on_step: bool = False,
+        # compute_on_step: bool = False,
         dist_sync_on_step: bool = False,
         process_group: Optional[Any] = None,
         dist_sync_fn: Optional[Callable] = None,
     ) -> None:
         super().__init__(
-            compute_on_step=compute_on_step,
+            # compute_on_step=compute_on_step,
             dist_sync_on_step=dist_sync_on_step,
             process_group=process_group,
             dist_sync_fn=dist_sync_fn,
         )
         self.add_state("concordance", default=torch.tensor(0), dist_reduce_fx="sum")
         self.add_state("discordance", default=torch.tensor(0), dist_reduce_fx="sum")
         self.prefix = prefix
```

### Comparing `lens_metric-0.1.1/lens/models/pooling_utils.py` & `lens_metric-0.2.0/lens/models/pooling_utils.py`

 * *Files identical despite different names*

### Comparing `lens_metric-0.1.1/lens/models/regression_metric_multi_ref.py` & `lens_metric-0.2.0/lens/models/regression_metric_multi_ref.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 r"""
 RegressionMetric
-========================
+================
     Regression Metric that learns to predict a quality assessment by looking
     at source, translation and reference.
 """
 from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
 import torch
-from lens.models.base import CometModel
-from lens.models.metrics import RegressionMetrics
-from lens.modules import FeedForward
+
 from transformers.optimization import Adafactor
 
+from .base import LensModel
+from .metrics import RegressionMetrics
+from .utils import Prediction, Target
+from ..modules import FeedForward
+
 
-class RegressionMetricMultiReference(CometModel):
+class RegressionMetricMultiReference(LensModel):
     """RegressionMetricMultiReference:
 
     :param nr_frozen_epochs: Number of epochs (% of epoch) that the encoder is frozen.
     :param keep_embeddings_frozen: Keeps the encoder frozen during training.
     :param optimizer: Optimizer used during training.
     :param encoder_learning_rate: Learning rate used to fine-tune the encoder model.
     :param learning_rate: Learning rate used to fine-tune the top layers.
@@ -90,35 +93,36 @@
             validation_data,
             load_weights_from_checkpoint,
             "regression_metric_multi_ref",
         )
         self.save_hyperparameters()
 
         self.topk = topk
-        print(self.topk)
+        print(f'Using LENS with topk={self.topk}')
 
         self.estimator = FeedForward(
             in_dim=self.encoder.output_units * 7,
             hidden_sizes=self.hparams.hidden_sizes,
             activations=self.hparams.activations,
             dropout=self.hparams.dropout,
             final_activation=self.hparams.final_activation,
         )
 
     def init_metrics(self):
+        """Initializes train/validation metrics."""
         self.train_metrics = RegressionMetrics(prefix="train")
         self.val_metrics = RegressionMetrics(prefix="val")
     
-    def is_referenceless(self) -> bool:
-        return False
+    def requires_references(self) -> bool:
+        return True
 
     def configure_optimizers(
         self,
     ) -> Tuple[List[torch.optim.Optimizer], List[torch.optim.lr_scheduler.LambdaLR]]:
-        """Sets the optimizers to be used during training."""
+        """Pytorch Lightning method to configure optimizers and schedulers."""
         layer_parameters = self.encoder.layerwise_lr(
             self.hparams.encoder_learning_rate, self.hparams.layerwise_decay
         )
         top_layers_parameters = [
             {"params": self.estimator.parameters(), "lr": self.hparams.learning_rate}
         ]
         if self.layerwise_attention:
@@ -137,31 +141,31 @@
                 params,
                 lr=self.hparams.learning_rate,
                 relative_step=False,
                 scale_parameter=False,
             )
         else:
             optimizer = torch.optim.AdamW(params, lr=self.hparams.learning_rate)
-        # scheduler = self._build_scheduler(optimizer)
         return [optimizer], []
 
     def prepare_sample(
-        self, sample: List[Dict[str, Union[str, float]]], inference: bool = False
+        self, sample: List[Dict[str, Union[str, float]]], stage: str = "train"
     ) -> Union[
         Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]], Dict[str, torch.Tensor]
     ]:
         """
         Function that prepares a sample to input the model.
 
         :param sample: list of dictionaries.
         :param inference: If set to true prepares only the model inputs.
 
         :returns: Tuple with 2 dictionaries (model inputs and targets).
             If `inference=True` returns only the model inputs.
         """
+        inference = (stage == "predict")
 
         sample = {k: [dic[k] for dic in sample] for k in sample[0]}
         if inference:
             src_inputs = self.encoder.prepare_sample(sample["src"])
             mt_inputs = self.encoder.prepare_sample(sample["mt"])
             ref_inputs = self.encoder.prepare_sample(sample["ref"])
 
@@ -185,63 +189,125 @@
             src_inputs = {"src_" + k: v for k, v in src_inputs.items()}
             mt_inputs = {"mt_" + k: v for k, v in mt_inputs.items()}
             ref_inputs = {"ref_" + k: v for k, v in ref_inputs.items()}
 
             inputs = {**src_inputs, **mt_inputs, **ref_inputs}
             all_inputs.append(inputs)
 
-        targets = {"score": torch.tensor(sample["score"], dtype=torch.float)}
+        targets = {"scores": torch.tensor(sample["scores"], dtype=torch.float)}
         return all_inputs, targets
 
     def estimate(
         self,
         src_sentemb: torch.Tensor,
         mt_sentemb: torch.Tensor,
         ref_sentemb: torch.Tensor,
-    ) -> Dict[str, torch.Tensor]:
+    ) -> Prediction:
+        """Method that takes the sentence embeddings from the Encoder and runs the
+        Estimator Feed-Forward on top.
+
+        Args:
+            src_sentemb [torch.Tensor]: Source sentence embedding
+            mt_sentemb [torch.Tensor]: Translation sentence embedding
+            ref_sentemb [torch.Tensor]: Reference sentence embedding
+
+        Return:
+            Prediction object with sentence scores.
+        """
         diff_ref = torch.abs(mt_sentemb - ref_sentemb)
         diff_src = torch.abs(mt_sentemb - src_sentemb)
 
         prod_ref = mt_sentemb * ref_sentemb
         prod_src = mt_sentemb * src_sentemb
 
         embedded_sequences = torch.cat(
             (src_sentemb, mt_sentemb, ref_sentemb, prod_ref, diff_ref, prod_src, diff_src),
             dim=1,
         )
-        return {"score": self.estimator(embedded_sequences)}
+        return Prediction(scores=self.estimator(embedded_sequences).view(-1))
 
     def forward(
         self,
         src_input_ids: torch.tensor,
         src_attention_mask: torch.tensor,
         mt_input_ids: torch.tensor,
         mt_attention_mask: torch.tensor,
         ref_input_ids: torch.tensor,
         ref_attention_mask: torch.tensor,
         **kwargs
-    ) -> Dict[str, torch.Tensor]:
+    ) -> Prediction:
+        """Regression model forward method.
+
+        Args:
+            src_input_ids [torch.tensor]: input ids from source sentences.
+            src_attention_mask [torch.tensor]: Attention mask from source sentences.
+            mt_input_ids [torch.tensor]: input ids from MT.
+            mt_attention_mask [torch.tensor]: Attention mask from MT.
+            ref_input_ids [torch.tensor]: input ids from reference translations.
+            ref_attention_mask [torch.tensor]: Attention mask from reference translations.
+
+        Return:
+            Prediction object with translation scores.
+        """
         src_sentemb = self.get_sentence_embedding(src_input_ids, src_attention_mask)
-        mt_sentemb = self.get_sentence_embedding(mt_input_ids, mt_attention_mask)
         ref_sentemb = self.get_sentence_embedding(ref_input_ids, ref_attention_mask)
+        mt_sentemb = self.get_sentence_embedding(mt_input_ids, mt_attention_mask)
         return self.estimate(src_sentemb, mt_sentemb, ref_sentemb)
 
+    def read_training_data(self, path: str) -> List[dict]:
+        """Method that reads the training data (a csv file) and returns a list of
+        samples.
+
+        Returns:
+            List[dict]: List with input samples in the form of a dict
+        """
+        raise NotImplementedError()
+        df = pd.read_csv(path)
+        df = df[["src", "mt", "ref", "score"]]
+        df["src"] = df["src"].astype(str)
+        df["mt"] = df["mt"].astype(str)
+        df["ref"] = df["ref"].astype(str)
+        df["scores"] = df["scores"].astype("float16")
+        return df.to_dict("records")
+
+    def read_validation_data(self, path: str) -> List[dict]:
+        """Method that reads the validation data (a csv file) and returns a list of
+        samples.
+
+        Returns:
+            List[dict]: List with input samples in the form of a dict
+        """
+        raise NotImplementedError()
+        df = pd.read_csv(path)
+        columns = ["src", "mt", "ref", "score"]
+        # If system in columns we will use this to calculate system-level accuracy
+        if "system" in df.columns:
+            columns.append("system")
+            df["system"] = df["system"].astype(str)
+
+        df = df[columns]
+        df["scores"] = df["scores"].astype("float16")
+        df["src"] = df["src"].astype(str)
+        df["mt"] = df["mt"].astype(str)
+        df["ref"] = df["ref"].astype(str)
+        return df.to_dict("records")
+
     def read_csv(self, path: str) -> List[dict]:
         """Reads a comma separated value file.
 
         :param path: path to a csv file.
 
         :return: List of records as dictionaries
         """
         df = pd.read_csv(path)
         df = df[["src", "mt", "ref", "score"]]
         df["src"] = df["src"].astype(str)
         df["mt"] = df["mt"].astype(str)
         df["ref"] = df["ref"].astype(str)
-        df["score"] = df["score"].astype("float16")
+        df["scores"] = df["scores"].astype("float16")
         return df.to_dict("records")
 
     def training_step(
         self,
         batch: Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]],
         batch_nb: int,
     ) -> torch.Tensor:
@@ -307,16 +373,16 @@
         batch_prediction = {'score': torch.hstack(batch_prediction)}
         new_batch_target = {'score': torch.hstack(new_batch_target)}
         loss_value = self.compute_loss(batch_prediction, new_batch_target)
         batch_target = new_batch_target
         self.log("val_loss", loss_value, on_step=True, on_epoch=True)
 
         # TODO: REMOVE if condition after torchmetrics bug fix
-        if batch_prediction["score"].view(-1).size() != torch.Size([1]):
+        if batch_prediction["scores"].view(-1).size() != torch.Size([1]):
             if dataloader_idx == 0:
                 self.train_metrics.update(
-                    batch_prediction["score"].view(-1), batch_target["score"]
+                    batch_prediction["scores"].view(-1), batch_target["scores"]
                 )
             elif dataloader_idx == 1:
                 self.val_metrics.update(
-                    batch_prediction["score"].view(-1), batch_target["score"]
+                    batch_prediction["scores"].view(-1), batch_target["scores"]
                 )
```

### Comparing `lens_metric-0.1.1/lens/modules/feedforward.py` & `lens_metric-0.2.0/lens/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `lens_metric-0.1.1/lens/modules/layerwise_attention.py` & `lens_metric-0.2.0/lens/modules/layerwise_attention.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,20 +38,27 @@
 class LayerwiseAttention(torch.nn.Module):
     def __init__(
         self,
         num_layers: int,
         layer_norm: bool = False,
         layer_weights: Optional[List[int]] = None,
         dropout: float = None,
+        layer_transformation: str = "softmax",
     ) -> None:
         super(LayerwiseAttention, self).__init__()
         self.num_layers = num_layers
         self.layer_norm = layer_norm
         self.dropout = dropout
 
+        self.transform_fn = torch.softmax
+        if layer_transformation == "sparsemax":
+            from entmax import sparsemax
+
+            self.transform_fn = sparsemax
+
         if layer_weights is None:
             layer_weights = [0.0] * num_layers
         elif len(layer_weights) != num_layers:
             raise Exception(
                 "Length of layer_weights {} differs \
                 from num_layers {}".format(
                     layer_weights, num_layers
@@ -86,22 +93,30 @@
             raise Exception(
                 "{} tensors were passed, but the module was initialized to \
                 mix {} tensors.".format(
                     len(tensors), self.num_layers
                 )
             )
 
-        def _layer_norm(tensor, broadcast_mask, num_elements_not_masked):
+        def _layer_norm(tensor, broadcast_mask, mask):
             tensor_masked = tensor * broadcast_mask
-            mean = torch.sum(tensor_masked) / num_elements_not_masked
-            variance = (
-                torch.sum(((tensor_masked - mean) * broadcast_mask) ** 2)
-                / num_elements_not_masked
+            batch_size, _, input_dim = tensors[0].size()
+
+            # mean for each sentence
+            num_elements_not_masked = mask.sum(1) * input_dim
+            mean = tensor_masked.view(batch_size, -1).sum(1)
+            mean = (mean / num_elements_not_masked).view(batch_size, 1, 1)
+
+            variance = (((tensor_masked - mean) * broadcast_mask) ** 2).view(
+                batch_size, -1
+            ).sum(1) / num_elements_not_masked
+            normalized_tensor = (tensor - mean) / torch.sqrt(variance + 1e-12).view(
+                batch_size, 1, 1
             )
-            return (tensor - mean) / torch.sqrt(variance + 1e-12)
+            return normalized_tensor
 
         # BUG: Pytorch bug fix when Parameters are not well copied across GPUs
         # https://github.com/pytorch/pytorch/issues/36035
         if len([parameter for parameter in self.scalar_parameters]) != self.num_layers:
             weights = torch.tensor(self.weights, device=tensors[0].device)
             gamma = torch.tensor(self.gamma_value, device=tensors[0].device)
         else:
@@ -109,29 +124,27 @@
             gamma = self.gamma
 
         if self.training and self.dropout:
             weights = torch.where(
                 self.dropout_mask.uniform_() > self.dropout, weights, self.dropout_fill
             )
 
-        normed_weights = torch.nn.functional.softmax(weights, dim=0)
+        normed_weights = self.transform_fn(weights, dim=0)
         normed_weights = torch.split(normed_weights, split_size_or_sections=1)
 
         if not self.layer_norm:
             pieces = []
             for weight, tensor in zip(normed_weights, tensors):
                 pieces.append(weight * tensor)
             return gamma * sum(pieces)
 
         else:
             mask_float = mask.float()
             broadcast_mask = mask_float.unsqueeze(-1)
-            input_dim = tensors[0].size(-1)
-            num_elements_not_masked = torch.sum(mask_float) * input_dim
 
             pieces = []
             for weight, tensor in zip(normed_weights, tensors):
                 pieces.append(
                     weight
-                    * _layer_norm(tensor, broadcast_mask, num_elements_not_masked)
+                    * _layer_norm(tensor, broadcast_mask, mask_float)
                 )
             return gamma * sum(pieces)
```

### Comparing `lens_metric-0.1.1/setup.py` & `lens_metric-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lens_metric',
-    version='0.1.1',
-    description='A new metric for text simplification',
+    version='0.2.0',
+    description='A learnable evaluation metric for text simplification',
     author='Mounica Maddela',
     author_email='mmaddela3@gatech.edu',
     url='https://github.com/Yao-Dou/LENS',
-    download_url='https://github.com/Yao-Dou/LENS/archive/refs/tags/v0.1.1.tar.gz',
+    download_url='https://github.com/Yao-Dou/LENS/archive/refs/tags/v0.2.0.tar.gz',
     license='Apache license',
     packages=find_packages(),
     install_requires=[
-        "sentencepiece==0.1.96",
-        "pandas==1.1.5",
-        "transformers>=4.8",
-        "pytorch-lightning==1.6.0",
-        "jsonargparse==3.13.1",
-        "torch >=1.6.0,<2",
+        "sentencepiece >= 0.1.96",
+        "pandas >= 1.5.0, < 2.0.0",
+        "transformers >= 4.8",
+        "pytorch-lightning == 2.0.9",
+        "jsonargparse == 3.13.1",
+        "torch >= 2.0.1",
         "numpy >= 1.20.0",
         "torchmetrics >= 0.7",
         "sacrebleu >= 2.0.0",
-        "scipy >=1.5.4" ],
-
+        "scipy >=1.5.4" 
+    ],
     classifiers=[
-        'Development Status :: 1 - Planning',
+        'Development Status :: 5 - Production/Stable ',
         'Intended Audience :: Science/Research',
     ],
 )
```

