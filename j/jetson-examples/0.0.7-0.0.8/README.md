# Comparing `tmp/jetson_examples-0.0.7.tar.gz` & `tmp/jetson_examples-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetson_examples-0.0.7.tar", last modified: Fri Apr 19 06:18:16 2024, max compression
+gzip compressed data, was "jetson_examples-0.0.8.tar", last modified: Sat May 11 08:42:04 2024, max compression
```

## Comparing `jetson_examples-0.0.7.tar` & `jetson_examples-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.705111 jetson_examples-0.0.7/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1066 2024-04-16 06:52:15.000000 jetson_examples-0.0.7/LICENSE
--rw-r--r--   0 seeed     (1000) seeed     (1000)     4598 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/PKG-INFO
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     3948 2024-04-19 03:00:30.000000 jetson_examples-0.0.7/README.md
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/jetson_examples.egg-info/
--rw-r--r--   0 seeed     (1000) seeed     (1000)     4598 2024-04-19 06:18:16.000000 jetson_examples-0.0.7/jetson_examples.egg-info/PKG-INFO
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      865 2024-04-19 06:18:16.000000 jetson_examples-0.0.7/jetson_examples.egg-info/SOURCES.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)        1 2024-04-19 06:18:16.000000 jetson_examples-0.0.7/jetson_examples.egg-info/dependency_links.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       58 2024-04-19 06:18:16.000000 jetson_examples-0.0.7/jetson_examples.egg-info/entry_points.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       27 2024-04-19 06:18:16.000000 jetson_examples-0.0.7/jetson_examples.egg-info/top_level.txt
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1081 2024-04-19 06:17:41.000000 jetson_examples-0.0.7/pyproject.toml
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.697111 jetson_examples-0.0.7/reComputer/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       22 2024-04-19 06:17:34.000000 jetson_examples-0.0.7/reComputer/__init__.py
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1821 2024-04-17 12:03:58.000000 jetson_examples-0.0.7/reComputer/main.py
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      134 2024-04-16 09:51:17.000000 jetson_examples-0.0.7/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      127 2024-04-16 09:45:34.000000 jetson_examples-0.0.7/reComputer/scripts/check.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/live-llava/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)    10137 2024-04-16 09:45:34.000000 jetson_examples-0.0.7/reComputer/scripts/live-llava/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/llama3/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      226 2024-04-19 02:35:03.000000 jetson_examples-0.0.7/reComputer/scripts/llama3/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/llava/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      148 2024-04-16 09:49:26.000000 jetson_examples-0.0.7/reComputer/scripts/llava/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/llava-v1.5-7b/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      147 2024-04-16 09:50:12.000000 jetson_examples-0.0.7/reComputer/scripts/llava-v1.5-7b/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/llava-v1.6-vicuna-7b/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      165 2024-04-16 09:50:51.000000 jetson_examples-0.0.7/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/nanodb/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      247 2024-04-16 10:00:31.000000 jetson_examples-0.0.7/reComputer/scripts/nanodb/readme.md
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     2571 2024-04-19 06:12:37.000000 jetson_examples-0.0.7/reComputer/scripts/nanodb/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/nanoowl/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      161 2024-04-16 09:53:17.000000 jetson_examples-0.0.7/reComputer/scripts/nanoowl/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/ollama/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      143 2024-04-19 02:27:31.000000 jetson_examples-0.0.7/reComputer/scripts/ollama/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)     1370 2024-04-19 06:13:07.000000 jetson_examples-0.0.7/reComputer/scripts/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/stable-diffusion-webui/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       57 2024-04-16 09:52:42.000000 jetson_examples-0.0.7/reComputer/scripts/stable-diffusion-webui/run.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/text-generation-webui/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      304 2024-04-16 09:52:01.000000 jetson_examples-0.0.7/reComputer/scripts/text-generation-webui/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)      900 2024-04-17 12:02:17.000000 jetson_examples-0.0.7/reComputer/scripts/update.sh
-drwxrwxr-x   0 seeed     (1000) seeed     (1000)        0 2024-04-19 06:18:16.701111 jetson_examples-0.0.7/reComputer/scripts/whisper/
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       43 2024-04-16 09:53:47.000000 jetson_examples-0.0.7/reComputer/scripts/whisper/run.sh
--rw-rw-r--   0 seeed     (1000) seeed     (1000)       38 2024-04-19 06:18:16.705111 jetson_examples-0.0.7/setup.cfg
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1066 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/LICENSE
+-rw-r--r--   0 nvidia    (1001) nvidia    (1001)     4731 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/PKG-INFO
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     4081 2024-05-11 03:18:46.000000 jetson_examples-0.0.8/README.md
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/jetson_examples.egg-info/
+-rw-r--r--   0 nvidia    (1001) nvidia    (1001)     4731 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/PKG-INFO
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      950 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/SOURCES.txt
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)        1 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/dependency_links.txt
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       58 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/entry_points.txt
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       27 2024-05-11 08:42:04.000000 jetson_examples-0.0.8/jetson_examples.egg-info/top_level.txt
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1081 2024-05-11 08:38:00.000000 jetson_examples-0.0.8/pyproject.toml
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       22 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/__init__.py
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1821 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/main.py
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      134 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/Sheared-LLaMA-2.7B-ShareGPT/run.sh
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      127 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/check.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/live-llava/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)    10137 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/live-llava/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llama3/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      226 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llama3/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llava/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      148 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llava/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llava-v1.5-7b/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      147 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llava-v1.5-7b/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/llava-v1.6-vicuna-7b/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      165 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/nanodb/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      247 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/nanodb/readme.md
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     2571 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/nanodb/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.865776 jetson_examples-0.0.8/reComputer/scripts/nanoowl/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      161 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/nanoowl/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/ollama/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      143 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/ollama/run.sh
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1370 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/stable-diffusion-webui/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       57 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/stable-diffusion-webui/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/text-generation-webui/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      304 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/text-generation-webui/run.sh
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      900 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/update.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/whisper/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       43 2024-05-10 08:20:22.000000 jetson_examples-0.0.8/reComputer/scripts/whisper/run.sh
+drwxrwxr-x   0 nvidia    (1001) nvidia    (1001)        0 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/reComputer/scripts/yolov8-counter/
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)     1500 2024-05-11 03:18:28.000000 jetson_examples-0.0.8/reComputer/scripts/yolov8-counter/readme.md
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)      817 2024-05-11 02:05:15.000000 jetson_examples-0.0.8/reComputer/scripts/yolov8-counter/run.sh
+-rw-rw-r--   0 nvidia    (1001) nvidia    (1001)       38 2024-05-11 08:42:04.869776 jetson_examples-0.0.8/setup.cfg
```

### Comparing `jetson_examples-0.0.7/LICENSE` & `jetson_examples-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.7/PKG-INFO` & `jetson_examples-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.7
+Version: 0.0.8
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-
+| [yolov8-counter](/reComputer/scripts/yolov8-counter/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8_counter`  |
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
 
 ## TODO List
```

### Comparing `jetson_examples-0.0.7/README.md` & `jetson_examples-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-
+| [yolov8-counter](/reComputer/scripts/yolov8-counter/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8_counter`  |
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
 
 ## TODO List
```

### Comparing `jetson_examples-0.0.7/jetson_examples.egg-info/PKG-INFO` & `jetson_examples-0.0.8/jetson_examples.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetson-examples
-Version: 0.0.7
+Version: 0.0.8
 Summary: Running Gen AI models and applications on NVIDIA Jetson devices with one-line command
 Author-email: luozhixin <zhixin.luo@seeed.cc>
 Project-URL: Homepage, https://github.com/Seeed-Projects/jetson-examples
 Project-URL: Issues, https://github.com/Seeed-Projects/jetson-examples/issues
 Keywords: llama,llava,gpt,llm,nvidia,jetson,multimodal,jetson orin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,15 +55,15 @@
 | 🆕 [ollama](https://github.com/ollama/ollama)     | Inference Server         | *               | 10.5GB     | `reComputer run ollama`                 |
 | LLaVA                                            | Text + Vision (VLM)      | 13GB            | 14.4GB     | `reComputer run llava`                  |
 | Live LLaVA                                       | Text + Vision (VLM)      | 13GB            | 20.3GB     | `reComputer run live-llava`             |
 | stable-diffusion-webui                           | Image Generation         | 3.97G           | 7.3GB      | `reComputer run stable-diffusion-webui` |
 | nanoowl                                          | Vision Transformers(ViT) | 613MB           | 15.1GB     | `reComputer run nanoowl`                |
 | [nanodb](../reComputer/scripts/nanodb/readme.md) | Vector Database          | 76GB            | 7.0GB      | `reComputer run nanodb`                 |
 | whisper                                          | Audio                    | 1.5GB           | 6.0GB      | `reComputer run whisper`                |
-
+| [yolov8-counter](/reComputer/scripts/yolov8-counter/readme.md) |Computer Vision | 6M | 13.8GB  | `reComputer run yolov8_counter`  |
 > Note: You should have enough space to run example, like `LLaVA`, at least `27.4GB` totally
 
 More Examples can be found [examples.md](./docs/examples.md)
 
 Want to add a Example by yourself? Check this [develop.md](./docs/develop.md)
 
 ## TODO List
```

### Comparing `jetson_examples-0.0.7/jetson_examples.egg-info/SOURCES.txt` & `jetson_examples-0.0.8/jetson_examples.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 reComputer/scripts/llava-v1.6-vicuna-7b/run.sh
 reComputer/scripts/nanodb/readme.md
 reComputer/scripts/nanodb/run.sh
 reComputer/scripts/nanoowl/run.sh
 reComputer/scripts/ollama/run.sh
 reComputer/scripts/stable-diffusion-webui/run.sh
 reComputer/scripts/text-generation-webui/run.sh
-reComputer/scripts/whisper/run.sh
+reComputer/scripts/whisper/run.sh
+reComputer/scripts/yolov8-counter/readme.md
+reComputer/scripts/yolov8-counter/run.sh
```

### Comparing `jetson_examples-0.0.7/pyproject.toml` & `jetson_examples-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jetson-examples"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{ name = "luozhixin", email = "zhixin.luo@seeed.cc" }]
 description = "Running Gen AI models and applications on NVIDIA Jetson devices with one-line command"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `jetson_examples-0.0.7/reComputer/main.py` & `jetson_examples-0.0.8/reComputer/main.py`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.7/reComputer/scripts/live-llava/run.sh` & `jetson_examples-0.0.8/reComputer/scripts/live-llava/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.7/reComputer/scripts/nanodb/run.sh` & `jetson_examples-0.0.8/reComputer/scripts/nanodb/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.7/reComputer/scripts/run.sh` & `jetson_examples-0.0.8/reComputer/scripts/run.sh`

 * *Files identical despite different names*

### Comparing `jetson_examples-0.0.7/reComputer/scripts/update.sh` & `jetson_examples-0.0.8/reComputer/scripts/update.sh`

 * *Files identical despite different names*

