# Comparing `tmp/denoisers-0.1.7.tar.gz` & `tmp/denoisers-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoisers-0.1.7.tar", last modified: Wed Mar 13 10:54:31 2024, max compression
+gzip compressed data, was "denoisers-0.1.8.tar", last modified: Sat May 11 16:42:00 2024, max compression
```

## Comparing `denoisers-0.1.7.tar` & `denoisers-0.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 10:54:26.000000 denoisers-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-13 10:54:31.108456 denoisers-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-13 10:54:26.000000 denoisers-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.104456 denoisers-0.1.7/denoisers/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.104456 denoisers-0.1.7/denoisers/datamodules/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/datamodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/datamodules/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/datamodules/unet1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/datamodules/waveunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/modeling/unet/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/unet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/unet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/modeling/unet1d/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/unet1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/unet1d/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/unet1d/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/unet1d/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/modeling/waveunet/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/waveunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/waveunet/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/modeling/waveunet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/scripts/train/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/scripts/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/scripts/train/unet1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/scripts/train/waveunet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-13 10:54:26.000000 denoisers-0.1.7/denoisers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/denoisers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-13 10:54:31.000000 denoisers-0.1.7/denoisers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-13 10:54:31.000000 denoisers-0.1.7/denoisers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:54:31.000000 denoisers-0.1.7/denoisers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-13 10:54:31.000000 denoisers-0.1.7/denoisers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-13 10:54:26.000000 denoisers-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 10:54:31.108456 denoisers-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-13 10:54:26.000000 denoisers-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:54:31.108456 denoisers-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-13 10:54:26.000000 denoisers-0.1.7/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-13 10:54:26.000000 denoisers-0.1.7/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 16:41:56.000000 denoisers-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-11 16:42:00.436685 denoisers-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-11 16:41:56.000000 denoisers-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.432685 denoisers-0.1.8/denoisers/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.432685 denoisers-0.1.8/denoisers/datamodules/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/datamodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/datamodules/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/datamodules/unet1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/datamodules/waveunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.432685 denoisers-0.1.8/denoisers/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.432685 denoisers-0.1.8/denoisers/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.432685 denoisers-0.1.8/denoisers/modeling/unet/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/unet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/unet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/denoisers/modeling/unet1d/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/unet1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/unet1d/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/unet1d/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/unet1d/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/denoisers/modeling/waveunet/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/waveunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/waveunet/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7748 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/modeling/waveunet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/denoisers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/denoisers/scripts/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/scripts/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/scripts/train/unet1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/scripts/train/waveunet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/denoisers/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-11 16:41:56.000000 denoisers-0.1.8/denoisers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/denoisers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-11 16:42:00.000000 denoisers-0.1.8/denoisers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-11 16:42:00.000000 denoisers-0.1.8/denoisers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 16:42:00.000000 denoisers-0.1.8/denoisers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-11 16:42:00.000000 denoisers-0.1.8/denoisers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-11 16:41:56.000000 denoisers-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 16:42:00.436685 denoisers-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-11 16:41:56.000000 denoisers-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 16:42:00.436685 denoisers-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-11 16:41:56.000000 denoisers-0.1.8/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-11 16:41:56.000000 denoisers-0.1.8/tests/test_transforms.py
```

### Comparing `denoisers-0.1.7/LICENSE` & `denoisers-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/PKG-INFO` & `denoisers-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: denoisers
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for training audio denoisers
 Author-email: Will Rice <wrice20@gmail.com>
 Project-URL: Homepage, https://github.com/will-rice/denoisers
 Project-URL: Bug Tracker, https://github.com/will-rice/denoisers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Denoisers
 
-Denoisers is a denoising library for audio with a focus on simplicity and ease of use. There are two major types of architectures available. WaveUNet for waveform denoising and UNet for spectrogram denoising.
+Denoisers is a denoising library for audio with a focus on simplicity and ease of use. There are two major architectures available for waveforms: WaveUNet which follows the [paper](https://arxiv.org/abs/1806.03185) and a custom UNet1D architecture similar to what you would see in diffusion models.
 
 ## Demo
 
-Gradio demo [here](https://wrice-denoisers.hf.space)
+[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/wrice/denoisers)
+
 
 ## Usage/Examples
 
 ```sh
 pip install denoisers
 ```
```

### Comparing `denoisers-0.1.7/denoisers/datamodules/unet.py` & `denoisers-0.1.8/denoisers/datamodules/unet.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/datamodules/unet1d.py` & `denoisers-0.1.8/denoisers/datamodules/unet1d.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/datamodules/waveunet.py` & `denoisers-0.1.8/denoisers/datamodules/waveunet.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/datasets/audio.py` & `denoisers-0.1.8/denoisers/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/metrics.py` & `denoisers-0.1.8/denoisers/metrics.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/modeling/modules.py` & `denoisers-0.1.8/denoisers/modeling/modules.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/modeling/unet/model.py` & `denoisers-0.1.8/denoisers/modeling/unet/model.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/modeling/unet1d/config.py` & `denoisers-0.1.8/denoisers/modeling/unet1d/config.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/modeling/unet1d/model.py` & `denoisers-0.1.8/denoisers/modeling/unet1d/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,13 +241,13 @@
         for layer in self.encoder_layers:
             out = layer(out)
             skips.append(out)
 
         out = self.middle(out)
 
         for skip, layer in zip(reversed(skips), self.decoder_layers):
-            out = layer(out + skip)
+            out = layer(out[..., : skip.size(-1)] + skip)
 
         out = torch.concat([out, inputs], dim=1)
         out = self.out_conv(out)
 
         return out.float()
```

### Comparing `denoisers-0.1.7/denoisers/modeling/unet1d/modules.py` & `denoisers-0.1.8/denoisers/modeling/unet1d/modules.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/modeling/waveunet/config.py` & `denoisers-0.1.8/denoisers/modeling/waveunet/config.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/modeling/waveunet/model.py` & `denoisers-0.1.8/denoisers/modeling/waveunet/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,14 +243,14 @@
         for layer in self.encoder_layers:
             out = layer(out)
             skips.append(out)
 
         out = self.middle(out)
 
         for skip, layer in zip(reversed(skips), self.decoder_layers):
-            out = torch.concat([out, skip], dim=1)
+            out = torch.concat([out[..., : skip.size(-1)], skip], dim=1)
             out = layer(out)
 
         out = torch.concat([out, inputs], dim=1)
         out = self.out_conv(out)
 
         return out.float()
```

### Comparing `denoisers-0.1.7/denoisers/scripts/train/unet1d.py` & `denoisers-0.1.8/denoisers/scripts/train/unet1d.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/scripts/train/waveunet.py` & `denoisers-0.1.8/denoisers/scripts/train/waveunet.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/testing/__init__.py` & `denoisers-0.1.8/denoisers/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/transforms.py` & `denoisers-0.1.8/denoisers/transforms.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers/utils.py` & `denoisers-0.1.8/denoisers/utils.py`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/denoisers.egg-info/PKG-INFO` & `denoisers-0.1.8/denoisers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: denoisers
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for training audio denoisers
 Author-email: Will Rice <wrice20@gmail.com>
 Project-URL: Homepage, https://github.com/will-rice/denoisers
 Project-URL: Bug Tracker, https://github.com/will-rice/denoisers/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Denoisers
 
-Denoisers is a denoising library for audio with a focus on simplicity and ease of use. There are two major types of architectures available. WaveUNet for waveform denoising and UNet for spectrogram denoising.
+Denoisers is a denoising library for audio with a focus on simplicity and ease of use. There are two major architectures available for waveforms: WaveUNet which follows the [paper](https://arxiv.org/abs/1806.03185) and a custom UNet1D architecture similar to what you would see in diffusion models.
 
 ## Demo
 
-Gradio demo [here](https://wrice-denoisers.hf.space)
+[![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/wrice/denoisers)
+
 
 ## Usage/Examples
 
 ```sh
 pip install denoisers
 ```
```

### Comparing `denoisers-0.1.7/denoisers.egg-info/SOURCES.txt` & `denoisers-0.1.8/denoisers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoisers-0.1.7/pyproject.toml` & `denoisers-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "denoisers"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Will Rice", email="wrice20@gmail.com" },
 ]
 description = "A package for training audio denoisers"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `denoisers-0.1.7/tests/test_transforms.py` & `denoisers-0.1.8/tests/test_transforms.py`

 * *Files identical despite different names*

