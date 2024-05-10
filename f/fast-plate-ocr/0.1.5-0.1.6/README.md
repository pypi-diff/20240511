# Comparing `tmp/fast_plate_ocr-0.1.5.tar.gz` & `tmp/fast_plate_ocr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_plate_ocr-0.1.5.tar", max compression
+gzip compressed data, was "fast_plate_ocr-0.1.6.tar", max compression
```

## Comparing `fast_plate_ocr-0.1.5.tar` & `fast_plate_ocr-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/LICENSE
--rw-r--r--   0        0        0    12612 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/README.md
--rw-r--r--   0        0        0      140 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/__init__.py
--rw-r--r--   0        0        0      802 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/cli.py
--rw-r--r--   0        0        0     2696 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/onnx_converter.py
--rw-r--r--   0        0        0     6576 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/train.py
--rw-r--r--   0        0        0     1773 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/valid.py
--rw-r--r--   0        0        0     4344 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_augmentation.py
--rw-r--r--   0        0        0     2662 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_predictions.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.967779 fast_plate_ocr-0.1.5/fast_plate_ocr/common/__init__.py
--rw-r--r--   0        0        0     1235 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/common/utils.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/__init__.py
--rw-r--r--   0        0        0     1377 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/config.py
--rw-r--r--   0        0        0     3548 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/hub.py
--rw-r--r--   0        0        0     7684 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/onnx_inference.py
--rw-r--r--   0        0        0     2726 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/process.py
--rw-r--r--   0        0        0      752 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/inference/utils.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/py.typed
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/__init__.py
--rw-r--r--   0        0        0      804 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/augmentation.py
--rw-r--r--   0        0        0     1681 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/dataset.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/__init__.py
--rw-r--r--   0        0        0     1452 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/config.py
--rw-r--r--   0        0        0     2601 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/custom.py
--rw-r--r--   0        0        0     2400 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/layer_blocks.py
--rw-r--r--   0        0        0     2709 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/models.py
--rw-r--r--   0        0        0        0 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/__init__.py
--rw-r--r--   0        0        0      900 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/backend_utils.py
--rw-r--r--   0        0        0     5345 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/utils.py
--rw-r--r--   0        0        0     3858 2024-05-01 19:47:59.971779 fast_plate_ocr-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    14904 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/LICENSE
+-rw-r--r--   0        0        0    13004 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/README.md
+-rw-r--r--   0        0        0      140 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/__init__.py
+-rw-r--r--   0        0        0      802 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/cli.py
+-rw-r--r--   0        0        0     3420 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/onnx_converter.py
+-rw-r--r--   0        0        0     6576 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/train.py
+-rw-r--r--   0        0        0     1773 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/valid.py
+-rw-r--r--   0        0        0     4344 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/visualize_augmentation.py
+-rw-r--r--   0        0        0     2731 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/cli/visualize_predictions.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/common/__init__.py
+-rw-r--r--   0        0        0     1235 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/common/utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/inference/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/inference/config.py
+-rw-r--r--   0        0        0     3842 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/inference/hub.py
+-rw-r--r--   0        0        0     7890 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/inference/onnx_inference.py
+-rw-r--r--   0        0        0     2726 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/inference/process.py
+-rw-r--r--   0        0        0      752 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/inference/utils.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/py.typed
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/data/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/data/augmentation.py
+-rw-r--r--   0        0        0     1681 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.907150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/__init__.py
+-rw-r--r--   0        0        0     1452 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/config.py
+-rw-r--r--   0        0        0     2601 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/custom.py
+-rw-r--r--   0        0        0     2400 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/layer_blocks.py
+-rw-r--r--   0        0        0     2709 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/models.py
+-rw-r--r--   0        0        0        0 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/utilities/__init__.py
+-rw-r--r--   0        0        0      900 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/utilities/backend_utils.py
+-rw-r--r--   0        0        0     5117 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/fast_plate_ocr/train/utilities/utils.py
+-rw-r--r--   0        0        0     3924 2024-05-10 22:16:32.911150 fast_plate_ocr-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    15348 1970-01-01 00:00:00.000000 fast_plate_ocr-0.1.6/PKG-INFO
```

### Comparing `fast_plate_ocr-0.1.5/LICENSE` & `fast_plate_ocr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/README.md` & `fast_plate_ocr-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,18 @@
 - **Efficient Execution**: **Lightweight** models that are cheap to run 💰
 - **ONNX Runtime Inference**: **Fast** and **optimized** inference with **[ONNX runtime](https://onnxruntime.ai/)** ⚡
 - **User-Friendly CLI**: Simplified **CLI** for **training** and **validating** OCR models 🛠️
 - **Model HUB**: Access to a collection of **pre-trained models** ready for inference 🌟
 
 ### Available Models
 
-|          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                         Dataset                                                         | Accuracy<sup>[2]</sup> |              Dataset              |
-|:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
-| argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
+|              Model Name              | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                              Dataset                                                               | Accuracy<sup>[2]</sup> |                Dataset                |
+|:------------------------------------:|:--------------------------------:|:----------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:----------------------:|:-------------------------------------:|
+|    `argentinian-plates-cnn-model`    |               2.1                |                      476                       |      [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip)       |         94.05%         |   Non-synthetic, plates up to 2020.   |
+| `argentinian-plates-cnn-synth-model` |               2.1                |                      476                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset_plus_synth.zip) |         94.19%         | Plates up to 2020 + synthetic plates. |
 
 _<sup>[1]</sup> Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
 by 5x._
 
 _<sup>[2]</sup> Accuracy is what we refer as plate_acc. See [metrics section](#model-metrics)._
 
 
@@ -45,15 +46,15 @@
   <summary>Reproduce results.</summary>
 
 * Calculate Inference Time:
 
   ```shell
   pip install fast_plate_ocr  # CPU
   # or
-  pip install fast_plate_ocr[inference_gpu]  # GPU
+  pip install fast_plate_ocr[inference-gpu]  # GPU
   ```
 
   ```python
   from fast_plate_ocr import ONNXPlateRecognizer
 
   m = ONNXPlateRecognizer("argentinian-plates-cnn-model")
   m.benchmark()
@@ -81,15 +82,15 @@
 ```shell
 pip install fast_plate_ocr
 ```
 
 For doing inference on GPU, install:
 
 ```shell
-pip install fast_plate_ocr[inference_gpu]
+pip install fast_plate_ocr[inference-gpu]
 ```
 
 #### Usage
 
 To predict from disk image:
 
 ```python
```

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/cli.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/onnx_converter.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/cli/onnx_converter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 """
 Script for converting Keras models to ONNX format.
 """
 
 import logging
 import pathlib
+import shutil
+from tempfile import NamedTemporaryFile
 
 import click
 import numpy as np
+import onnx
 import onnxruntime as rt
+import onnxsim
 import tensorflow as tf
 import tf2onnx
 from tf2onnx import constants as tf2onnx_constants
 
 from fast_plate_ocr.common.utils import log_time_taken
 from fast_plate_ocr.train.model.config import load_config_from_yaml
 from fast_plate_ocr.train.utilities.utils import load_keras_model
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
 )
 
 
+# pylint: disable=too-many-arguments,too-many-locals
+
+
 @click.command(context_settings={"max_content_width": 120})
 @click.option(
     "-m",
     "--model",
     "model_path",
     required=True,
     type=click.Path(exists=True, file_okay=True, dir_okay=False, path_type=pathlib.Path),
     help="Path to the saved .keras model.",
 )
 @click.option(
     "--output-path",
     required=True,
     type=str,
-    help="Output name for ONNX model",
+    help="Output name for ONNX model.",
+)
+@click.option(
+    "--simplify/--no-simplify",
+    default=False,
+    show_default=True,
+    help="Simplify ONNX model using onnxsim.",
 )
 @click.option(
     "--config-file",
     required=True,
     type=click.Path(exists=True, file_okay=True, path_type=pathlib.Path),
     help="Path pointing to the model license plate OCR config.",
 )
@@ -48,34 +61,44 @@
     type=click.IntRange(max=max(tf2onnx_constants.OPSET_TO_IR_VERSION)),
     show_default=True,
     help="Opset version for ONNX.",
 )
 def export_onnx(
     model_path: pathlib.Path,
     output_path: str,
+    simplify: bool,
     config_file: pathlib.Path,
     opset: int,
 ) -> None:
     """
     Export Keras models to ONNX format.
     """
     config = load_config_from_yaml(config_file)
     model = load_keras_model(
         model_path,
         vocab_size=config.vocabulary_size,
         max_plate_slots=config.max_plate_slots,
     )
     spec = (tf.TensorSpec((None, config.img_height, config.img_width, 1), tf.uint8, name="input"),)
     # Convert from Keras to ONNX using tf2onnx library
-    model_proto, _ = tf2onnx.convert.from_keras(
-        model,
-        input_signature=spec,
-        opset=opset,
-        output_path=output_path,
-    )
+    with NamedTemporaryFile(suffix=".onnx") as tmp:
+        tmp_onnx = tmp.name
+        model_proto, _ = tf2onnx.convert.from_keras(
+            model,
+            input_signature=spec,
+            opset=opset,
+            output_path=tmp_onnx,
+        )
+        if simplify:
+            logging.info("Simplifying ONNX model ...")
+            model_simp, check = onnxsim.simplify(onnx.load(tmp_onnx))
+            assert check, "Simplified ONNX model could not be validated!"
+            onnx.save(model_simp, output_path)
+        else:
+            shutil.copy(tmp_onnx, output_path)
     output_names = [n.name for n in model_proto.graph.output]
     x = np.random.randint(0, 256, size=(1, config.img_height, config.img_width, 1), dtype=np.uint8)
     # Run dummy inference and log time taken
     m = rt.InferenceSession(output_path)
     with log_time_taken("ONNX inference took:"):
         onnx_pred = m.run(output_names, {"input": x})
     # Check if ONNX and keras have the same results
```

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/train.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/cli/train.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/valid.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/cli/valid.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_augmentation.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/cli/visualize_augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/cli/visualize_predictions.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/cli/visualize_predictions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Script for displaying an image with the OCR model predictions.
 """
 
 import logging
 import pathlib
-from contextlib import nullcontext
 
 import click
 import cv2
 import keras
 import numpy as np
 
-import fast_plate_ocr.common.utils
 from fast_plate_ocr.train.model.config import load_config_from_yaml
 from fast_plate_ocr.train.utilities import utils
+from fast_plate_ocr.train.utilities.utils import postprocess_model_output
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
 )
 
 
 @click.command(context_settings={"max_content_width": 120})
@@ -39,58 +38,56 @@
     "-d",
     "--img-dir",
     required=True,
     type=click.Path(exists=True, dir_okay=True, file_okay=False, path_type=pathlib.Path),
     help="Directory containing the images to make predictions from.",
 )
 @click.option(
-    "-t",
-    "--time",
-    default=True,
-    is_flag=True,
-    help="Log time taken to run predictions.",
-)
-@click.option(
     "-l",
     "--low-conf-thresh",
     type=float,
-    default=0.2,
+    default=0.35,
     show_default=True,
     help="Threshold for displaying low confidence characters.",
 )
+@click.option(
+    "-l",
+    "--filter-conf",
+    type=float,
+    help="Display plates that any of the plate characters are below this number.",
+)
 def visualize_predictions(
     model_path: pathlib.Path,
     config_file: pathlib.Path,
     img_dir: pathlib.Path,
     low_conf_thresh: float,
-    time: bool,
+    filter_conf: float | None,
 ):
     """
     Visualize OCR model predictions on unlabeled data.
     """
     config = load_config_from_yaml(config_file)
     model = utils.load_keras_model(
         model_path, vocab_size=config.vocabulary_size, max_plate_slots=config.max_plate_slots
     )
     images = utils.load_images_from_folder(
         img_dir, width=config.img_width, height=config.img_height
     )
     for image in images:
-        with (
-            fast_plate_ocr.common.utils.log_time_taken("Prediction time") if time else nullcontext()
-        ):
-            x = np.expand_dims(image, 0)
-            prediction = model(x, training=False)
-            prediction = keras.ops.stop_gradient(prediction).numpy()
-        utils.display_predictions(
-            image=image,
+        x = np.expand_dims(image, 0)
+        prediction = model(x, training=False)
+        prediction = keras.ops.stop_gradient(prediction).numpy()
+        plate, probs = postprocess_model_output(
             prediction=prediction,
             alphabet=config.alphabet,
-            plate_slots=config.max_plate_slots,
+            max_plate_slots=config.max_plate_slots,
             vocab_size=config.vocabulary_size,
-            low_conf_thresh=low_conf_thresh,
         )
+        if not filter_conf or (filter_conf and np.any(probs < filter_conf)):
+            utils.display_predictions(
+                image=image, plate=plate, probs=probs, low_conf_thresh=low_conf_thresh
+            )
     cv2.destroyAllWindows()
 
 
 if __name__ == "__main__":
     visualize_predictions()
```

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/common/utils.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/common/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/config.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/inference/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/hub.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/inference/hub.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,33 @@
 """
 
 import logging
 import pathlib
 import shutil
 import urllib.request
 from http import HTTPStatus
+from typing import Literal
 
 from tqdm.asyncio import tqdm
 
 from fast_plate_ocr.inference.utils import safe_write
 
 BASE_URL: str = "https://github.com/ankandrew/cnn-ocr-lp/releases/download"
+OcrModel = Literal["argentinian-plates-cnn-model", "argentinian-plates-cnn-synth-model"]
 
-AVAILABLE_ONNX_MODELS: dict[str, tuple[str, str]] = {
+
+AVAILABLE_ONNX_MODELS: dict[OcrModel, tuple[str, str]] = {
     "argentinian-plates-cnn-model": (
         f"{BASE_URL}/arg-plates/arg_cnn_ocr.onnx",
         f"{BASE_URL}/arg-plates/arg_cnn_ocr_config.yaml",
-    )
+    ),
+    "argentinian-plates-cnn-synth-model": (
+        f"{BASE_URL}/arg-plates/arg_cnn_ocr_synth.onnx",
+        f"{BASE_URL}/arg-plates/arg_cnn_ocr_config.yaml",
+    ),
 }
 """Available ONNX models for doing inference."""
 
 MODEL_CACHE_DIR: pathlib.Path = pathlib.Path.home() / ".cache" / "fast-plate-ocr"
 """Default location where models will be stored."""
 
 
@@ -41,15 +48,15 @@
         desc = f"Downloading {filename.name}"
 
         with tqdm.wrapattr(out_file, "write", total=file_size, desc=desc) as f_out:
             shutil.copyfileobj(response, f_out)
 
 
 def download_model(
-    model_name: str,
+    model_name: OcrModel,
     save_directory: pathlib.Path | None = None,
     force_download: bool = False,
 ) -> tuple[pathlib.Path, pathlib.Path]:
     """
     Download an OCR model and the config to a given directory.
 
     :param model_name: Which model to download.
```

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/onnx_inference.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/inference/onnx_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import onnxruntime as ort
 from rich.console import Console
 from rich.table import Table
 
 from fast_plate_ocr.common.utils import measure_time
 from fast_plate_ocr.inference import hub
 from fast_plate_ocr.inference.config import load_config_from_yaml
+from fast_plate_ocr.inference.hub import OcrModel
 from fast_plate_ocr.inference.process import postprocess_output, preprocess_image, read_plate_image
 
 
 def _load_image_from_source(
     source: str | list[str] | npt.NDArray | list[npt.NDArray],
 ) -> npt.NDArray | list[npt.NDArray]:
     """
@@ -58,59 +59,62 @@
 class ONNXPlateRecognizer:
     """
     ONNX inference class for performing license plates OCR.
     """
 
     def __init__(
         self,
-        hub_ocr_model: Literal["argentinian-plates-cnn-model"] | None = None,
-        device: Literal["gpu", "cpu", "auto"] = "auto",
+        hub_ocr_model: OcrModel | None = None,
+        device: Literal["cuda", "cpu", "auto"] = "auto",
         sess_options: ort.SessionOptions | None = None,
         model_path: str | os.PathLike[str] | None = None,
         config_path: str | os.PathLike[str] | None = None,
+        force_download: bool = False,
     ) -> None:
         """
         Initializes the ONNXPlateRecognizer with the specified OCR model and inference device.
 
         The current OCR models available from the HUB are:
 
         - `argentinian-plates-cnn-model`: OCR for Argentinian license plates.
 
         Args:
             hub_ocr_model: Name of the OCR model to use from the HUB.
-            device: Device type for inference. Should be one of ('cpu', 'gpu', 'auto'). If
+            device: Device type for inference. Should be one of ('cpu', 'cuda', 'auto'). If
                 'auto' mode, the device will be deduced from
                 `onnxruntime.get_available_providers()`.
             sess_options: Advanced session options for ONNX Runtime.
             model_path: Path to ONNX model file to use (In case you want to use a custom one).
             config_path: Path to config file to use (In case you want to use a custom one).
-
+            force_download: Force and download the model, even if it already exists.
         Returns:
             None.
         """
         self.logger = logging.getLogger(__name__)
 
-        if device == "gpu":
+        if device == "cuda":
             self.provider = ["CUDAExecutionProvider"]
         elif device == "cpu":
             self.provider = ["CPUExecutionProvider"]
         elif device == "auto":
             self.provider = ort.get_available_providers()
         else:
-            raise ValueError(f"Device should be one of ('cpu', 'gpu', 'auto'). Got '{device}'.")
+            raise ValueError(f"Device should be one of ('cpu', 'cuda', 'auto'). Got '{device}'.")
 
         if model_path and config_path:
             model_path = pathlib.Path(model_path)
             config_path = pathlib.Path(config_path)
             if not model_path.exists() or not config_path.exists():
                 raise FileNotFoundError("Missing model/config file!")
             self.model_name = model_path.stem
         elif hub_ocr_model:
             self.model_name = hub_ocr_model
-            model_path, config_path = hub.download_model(model_name=hub_ocr_model)
+            model_path, config_path = hub.download_model(
+                model_name=hub_ocr_model, force_download=force_download
+            )
         else:
             raise ValueError(
                 "Either provide a model from the HUB or a custom model_path and config_path"
             )
 
         self.config = load_config_from_yaml(config_path)
         self.model = ort.InferenceSession(
```

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/process.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/inference/process.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/inference/utils.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/inference/utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/augmentation.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/data/dataset.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/data/dataset.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/config.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/config.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/custom.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/custom.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/layer_blocks.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/layer_blocks.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/model/models.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/model/models.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/backend_utils.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/utilities/backend_utils.py`

 * *Files identical despite different names*

### Comparing `fast_plate_ocr-0.1.5/fast_plate_ocr/train/utilities/utils.py` & `fast_plate_ocr-0.1.6/fast_plate_ocr/train/utilities/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,29 +113,21 @@
 def low_confidence_positions(probs, thresh=0.3) -> npt.NDArray:
     """Returns indices of elements in `probs` less than `thresh`, indicating low confidence."""
     return np.where(np.array(probs) < thresh)[0]
 
 
 def display_predictions(
     image: npt.NDArray,
-    prediction: npt.NDArray,
-    alphabet: str,
-    plate_slots: int,
-    vocab_size: int,
+    plate: str,
+    probs: npt.NDArray,
     low_conf_thresh: float,
 ) -> None:
     """
     Display plate and corresponding prediction.
     """
-    plate, probs = postprocess_model_output(
-        prediction=prediction,
-        alphabet=alphabet,
-        max_plate_slots=plate_slots,
-        vocab_size=vocab_size,
-    )
     plate_str = "".join(plate)
     logging.info("Plate: %s", plate_str)
     logging.info("Confidence: %s", probs)
     image_to_show = cv2.resize(image, None, fx=3, fy=3, interpolation=cv2.INTER_LINEAR)
     # Converting to BGR for color text
     image_to_show = cv2.cvtColor(image_to_show, cv2.COLOR_GRAY2RGB)
     # Average probabilities
```

### Comparing `fast_plate_ocr-0.1.5/pyproject.toml` & `fast_plate_ocr-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-plate-ocr"
-version = "0.1.5"
+version = "0.1.6"
 description = "Fast & Lightweight OCR for vehicle license plates."
 authors = ["ankandrew <61120139+ankandrew@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/ankandrew/fast-plate-ocr/"
 documentation = "https://ankandrew.github.io/fast-plate-ocr"
 keywords = ["plate-recognition", "license-plate-recognition", "license-plate-ocr"]
 license = "MIT"
@@ -48,28 +48,30 @@
 tf2onnx = { version = "*", optional = true }
 torch = { version = "*", optional = true }
 
 # Optional packages for creating the docs
 mkdocs-material = { version = "*", optional = true }
 mkdocstrings = {version = "*", extras = ["python"], optional = true}
 mike = { version = "*", optional = true }
+onnxsim = { version = ">0.4.10", optional = true }
 
 [tool.poetry.extras]
-inference_gpu = ["onnxruntime-gpu"]
+inference-gpu = ["onnxruntime-gpu"]
 train = [
     "albumentations",
     "click",
     "keras",
     "matplotlib",
     "pandas",
     "pydantic",
     "tensorboard",
     "tensorflow",
     "tf2onnx",
     "torch",
+    "onnxsim",
 ]
 docs = ["mkdocs-material", "mkdocstrings", "mike"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `fast_plate_ocr-0.1.5/PKG-INFO` & `fast_plate_ocr-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-plate-ocr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast & Lightweight OCR for vehicle license plates.
 Home-page: https://github.com/ankandrew/fast-plate-ocr/
 License: MIT
 Keywords: plate-recognition,license-plate-recognition,license-plate-ocr
 Author: ankandrew
 Author-email: 61120139+ankandrew@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
@@ -33,14 +33,15 @@
 Requires-Dist: matplotlib ; extra == "train"
 Requires-Dist: mike ; extra == "docs"
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: mkdocstrings[python] ; extra == "docs"
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: onnxruntime (>=1.4.0)
 Requires-Dist: onnxruntime-gpu (>=1.4.0) ; (sys_platform != "darwin") and (extra == "inference-gpu")
+Requires-Dist: onnxsim (>0.4.10) ; extra == "train"
 Requires-Dist: opencv-python
 Requires-Dist: pandas ; extra == "train"
 Requires-Dist: pydantic (>=2.0.0,<3.0.0) ; extra == "train"
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: rich
 Requires-Dist: tensorboard ; extra == "train"
 Requires-Dist: tensorflow ; extra == "train"
@@ -80,17 +81,18 @@
 - **Efficient Execution**: **Lightweight** models that are cheap to run 💰
 - **ONNX Runtime Inference**: **Fast** and **optimized** inference with **[ONNX runtime](https://onnxruntime.ai/)** ⚡
 - **User-Friendly CLI**: Simplified **CLI** for **training** and **validating** OCR models 🛠️
 - **Model HUB**: Access to a collection of **pre-trained models** ready for inference 🌟
 
 ### Available Models
 
-|          Model Name          | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                         Dataset                                                         | Accuracy<sup>[2]</sup> |              Dataset              |
-|:----------------------------:|:--------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------:|:----------------------:|:---------------------------------:|
-| argentinian-plates-cnn-model |              2.0964              |                      477                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip) |         94.05%         | Non-synthetic, plates up to 2020. |
+|              Model Name              | Time b=1<br/> (ms)<sup>[1]</sup> | Throughput <br/> (plates/second)<sup>[1]</sup> |                                                              Dataset                                                               | Accuracy<sup>[2]</sup> |                Dataset                |
+|:------------------------------------:|:--------------------------------:|:----------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|:----------------------:|:-------------------------------------:|
+|    `argentinian-plates-cnn-model`    |               2.1                |                      476                       |      [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset.zip)       |         94.05%         |   Non-synthetic, plates up to 2020.   |
+| `argentinian-plates-cnn-synth-model` |               2.1                |                      476                       | [arg_plate_dataset.zip](https://github.com/ankandrew/fast-plate-ocr/releases/download/arg-plates/arg_plate_dataset_plus_synth.zip) |         94.19%         | Plates up to 2020 + synthetic plates. |
 
 _<sup>[1]</sup> Inference on Mac M1 chip using CPUExecutionProvider. Utilizing CoreMLExecutionProvider accelerates speed
 by 5x._
 
 _<sup>[2]</sup> Accuracy is what we refer as plate_acc. See [metrics section](#model-metrics)._
 
 
@@ -98,15 +100,15 @@
   <summary>Reproduce results.</summary>
 
 * Calculate Inference Time:
 
   ```shell
   pip install fast_plate_ocr  # CPU
   # or
-  pip install fast_plate_ocr[inference_gpu]  # GPU
+  pip install fast_plate_ocr[inference-gpu]  # GPU
   ```
 
   ```python
   from fast_plate_ocr import ONNXPlateRecognizer
 
   m = ONNXPlateRecognizer("argentinian-plates-cnn-model")
   m.benchmark()
@@ -134,15 +136,15 @@
 ```shell
 pip install fast_plate_ocr
 ```
 
 For doing inference on GPU, install:
 
 ```shell
-pip install fast_plate_ocr[inference_gpu]
+pip install fast_plate_ocr[inference-gpu]
 ```
 
 #### Usage
 
 To predict from disk image:
 
 ```python
```

