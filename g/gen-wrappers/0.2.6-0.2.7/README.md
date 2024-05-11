# Comparing `tmp/gen_wrappers-0.2.6.tar.gz` & `tmp/gen_wrappers-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.2.6.tar", last modified: Fri May 10 20:51:41 2024, max compression
+gzip compressed data, was "gen_wrappers-0.2.7.tar", last modified: Sat May 11 14:41:11 2024, max compression
```

## Comparing `gen_wrappers-0.2.6.tar` & `gen_wrappers-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.895217 gen_wrappers-0.2.6/
--rw-rw-rw-   0        0        0      847 2024-05-10 20:51:41.893225 gen_wrappers-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.811421 gen_wrappers-0.2.6/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.6/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.822840 gen_wrappers-0.2.6/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.6/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6713 2024-05-03 20:01:50.000000 gen_wrappers-0.2.6/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.6/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.6/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.836260 gen_wrappers-0.2.6/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.6/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.6/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.6/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3028 2024-05-03 21:08:54.000000 gen_wrappers-0.2.6/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.6/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.846273 gen_wrappers-0.2.6/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.6/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9534 2024-05-10 20:51:21.000000 gen_wrappers-0.2.6/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9370 2024-05-10 20:36:48.000000 gen_wrappers-0.2.6/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.6/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.856852 gen_wrappers-0.2.6/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.6/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.6/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.6/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.6/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.891216 gen_wrappers-0.2.6/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 20:51:41.895217 gen_wrappers-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-10 20:51:31.000000 gen_wrappers-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.254916 gen_wrappers-0.2.7/
+-rw-rw-rw-   0        0        0      847 2024-05-11 14:41:11.253425 gen_wrappers-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.064329 gen_wrappers-0.2.7/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.7/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.104022 gen_wrappers-0.2.7/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.7/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6713 2024-05-03 20:01:50.000000 gen_wrappers-0.2.7/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.7/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.7/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.156855 gen_wrappers-0.2.7/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.7/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.7/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.7/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3028 2024-05-03 21:08:54.000000 gen_wrappers-0.2.7/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.7/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.182440 gen_wrappers-0.2.7/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.7/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9534 2024-05-10 20:51:21.000000 gen_wrappers-0.2.7/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     9193 2024-05-11 14:41:07.000000 gen_wrappers-0.2.7/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.7/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.218526 gen_wrappers-0.2.7/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.7/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.7/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3975 2024-05-10 20:59:44.000000 gen_wrappers-0.2.7/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.7/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-11 14:41:11.252347 gen_wrappers-0.2.7/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-11 14:41:10.000000 gen_wrappers-0.2.7/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-11 14:41:10.000000 gen_wrappers-0.2.7/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-11 14:41:10.000000 gen_wrappers-0.2.7/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-11 14:41:10.000000 gen_wrappers-0.2.7/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-11 14:41:10.000000 gen_wrappers-0.2.7/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-11 14:41:11.254916 gen_wrappers-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-11 14:41:07.000000 gen_wrappers-0.2.7/setup.py
```

### Comparing `gen_wrappers-0.2.6/PKG-INFO` & `gen_wrappers-0.2.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.2.6
+Version: 0.2.7
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.6/creator/auto/creator_auto.py` & `gen_wrappers-0.2.7/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/auto/request_auto.py` & `gen_wrappers-0.2.7/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/auto/response_auto.py` & `gen_wrappers-0.2.7/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/base/base_app.py` & `gen_wrappers-0.2.7/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/base/base_request.py` & `gen_wrappers-0.2.7/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/base/base_response.py` & `gen_wrappers-0.2.7/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.2.7/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.2.7/creator/cmfy/request_cmfy.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,99 +120,27 @@
     "class_type": "CheckpointLoaderSimple",
     "_meta": {
       "title": "Load Checkpoint"
     }
   },
   "21": {
     "inputs": {
-      "width": 832,
-      "height": 1216,
-      "batch_size": 1
+      "width": 2432,
+      "height": 1664,
+      "batch_size": 2
     },
     "class_type": "EmptyLatentImage",
     "_meta": {
       "title": "Image Size\n"
     }
   },
-  "50": {
-    "inputs": {
-      "add_noise": "enable",
-      "noise_seed": [
-        "99",
-        0
-      ],
-      "steps": 20,
-      "cfg": 5,
-      "sampler_name": "dpmpp_2m_sde",
-      "scheduler": "karras",
-      "start_at_step": 0,
-      "end_at_step": 10,
-      "return_with_leftover_noise": "enable",
-      "model": [
-        "120",
-        0
-      ],
-      "positive": [
-        "98:0",
-        0
-      ],
-      "negative": [
-        "98:1",
-        0
-      ],
-      "latent_image": [
-        "21",
-        0
-      ]
-    },
-    "class_type": "KSamplerAdvanced",
-    "_meta": {
-      "title": "KSampler Preliminary"
-    }
-  },
-  "66": {
-    "inputs": {
-      "add_noise": "disable",
-      "noise_seed": [
-        "99",
-        0
-      ],
-      "steps": 20,
-      "cfg": 4,
-      "sampler_name": "dpmpp_2m_sde",
-      "scheduler": "karras",
-      "start_at_step": 10,
-      "end_at_step": 10000,
-      "return_with_leftover_noise": "disable",
-      "model": [
-        "120",
-        0
-      ],
-      "positive": [
-        "98:0",
-        0
-      ],
-      "negative": [
-        "98:1",
-        0
-      ],
-      "latent_image": [
-        "50",
-        0
-      ]
-    },
-    "class_type": "KSamplerAdvanced",
-    "_meta": {
-      "title": "KSampler Base"
-    }
-  },
   "67": {
     "inputs": {
       "samples": [
-        "66",
+        "132",
         0
       ],
       "vae": [
         "4",
         2
       ]
     },
@@ -231,36 +159,39 @@
     "class_type": "PreviewImage",
     "_meta": {
       "title": "Output"
     }
   },
   "99": {
     "inputs": {
-      "seed": 33675281102746
+      "seed": 1042340763738557
     },
     "class_type": "CR Seed",
     "_meta": {
       "title": "🌱 CR Seed"
     }
   },
   "100": {
     "inputs": {
-      "text": "a photo of a wizard wearing silver and white robes, holding a sword, standing in the desert",
-      "seed": 3172194303,
+      "text": [
+        "114:0",
+        0
+      ],
+      "seed": 1116260329,
       "log_prompt": "No"
     },
     "class_type": "PromptExpansion",
     "_meta": {
       "title": "Prompt Expansion"
     }
   },
   "101": {
     "inputs": {
       "text": [
-        "114:0",
+        "100",
         0
       ]
     },
     "class_type": "ShowText|pysssss",
     "_meta": {
       "title": "Final Positive Prompt"
     }
@@ -289,14 +220,72 @@
       ]
     },
     "class_type": "FreeU_V2",
     "_meta": {
       "title": "FreeU_V2"
     }
   },
+  "132": {
+    "inputs": {
+      "add_noise": True,
+      "noise_seed": [
+        "99",
+        0
+      ],
+      "steps": 20,
+      "cfg": 5,
+      "sampler_name": "dpmpp_2m",
+      "scheduler": "AYS SDXL",
+      "start_at_step": 0,
+      "end_at_step": 10000,
+      "noise_mode": "GPU(=A1111)",
+      "return_with_leftover_noise": False,
+      "batch_seed_mode": "incremental",
+      "variation_seed": 0,
+      "variation_strength": 0,
+      "model": [
+        "134",
+        0
+      ],
+      "positive": [
+        "98:0",
+        0
+      ],
+      "negative": [
+        "98:1",
+        0
+      ],
+      "latent_image": [
+        "21",
+        0
+      ]
+    },
+    "class_type": "KSamplerAdvanced //Inspire",
+    "_meta": {
+      "title": "KSamplerAdvanced (inspire)"
+    }
+  },
+  "134": {
+    "inputs": {
+      "ds_depth_1": 3,
+      "ds_depth_2": 3,
+      "ds_timestep_1": 900,
+      "ds_timestep_2": 650,
+      "resize_scale_1": 2,
+      "resize_scale_2": 2,
+      "model": [
+        "120",
+        0
+      ]
+    },
+    "class_type": "Hires",
+    "_meta": {
+      "title": "Apply Kohya's HiresFix"
+    }
+  },
   "119:0": {
     "inputs": {
       "text_positive": "",
       "text_negative": "",
       "style": "Fooocus Photograph",
       "log_prompt": True,
       "style_positive": True,
@@ -307,15 +296,15 @@
       "title": "SDXL Prompt Styler"
     }
   },
   "119:1": {
     "inputs": {
       "text_positive": "",
       "text_negative": "",
-      "style": "Fooocus Masterpiece",
+      "style": "Fooocus Enhance",
       "log_prompt": True,
       "style_positive": True,
       "style_negative": True
     },
     "class_type": "SDXLPromptStyler",
     "_meta": {
       "title": "SDXL Prompt Styler"
@@ -331,46 +320,43 @@
       "style_negative": True
     },
     "class_type": "SDXLPromptStyler",
     "_meta": {
       "title": "SDXL Prompt Styler"
     }
   },
-  "113:0": {
+  "133:0": {
     "inputs": {
-      "text1": [
-        "100",
-        0
-      ],
+      "text1": "a close-up shot of a soldier running on the battlefield, world war 2, gritty, dust, explosions",
       "text2": [
         "119:0",
         0
       ],
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Positive"
     }
   },
-  "113:1": {
+  "133:1": {
     "inputs": {
-      "text1": "blurry eyes, zombie eyes, bad face, glowing sword, lightsaber",
+      "text1": "blurry eyes, zombie eyes, bad face, too many fingers",
       "text2": [
         "119:0",
         1
       ],
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Negative"
     }
   },
-  "113:2": {
+  "133:2": {
     "inputs": {
       "text1": [
         "119:1",
         0
       ],
       "text2": [
         "119:2",
@@ -379,15 +365,15 @@
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Positive"
     }
   },
-  "113:3": {
+  "133:3": {
     "inputs": {
       "text1": [
         "119:1",
         1
       ],
       "text2": [
         "119:2",
@@ -399,36 +385,36 @@
     "_meta": {
       "title": "Concat Negative"
     }
   },
   "114:0": {
     "inputs": {
       "text1": [
-        "113:0",
+        "133:0",
         0
       ],
       "text2": [
-        "113:2",
+        "133:2",
         0
       ],
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Positive"
     }
   },
   "114:1": {
     "inputs": {
       "text1": [
-        "113:1",
+        "133:1",
         0
       ],
       "text2": [
-        "113:3",
+        "133:3",
         0
       ],
       "separator": ", "
     },
     "class_type": "CR Text Concatenate",
     "_meta": {
       "title": "Concat Negative"
```

### Comparing `gen_wrappers-0.2.6/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.2.7/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.2.7/creator/fcus_api/request_fcus_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                                         examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = "Speed"
     aspect_ratios_selection: str = "1152*896"
     image_number: int = 2
     image_seed: int = -1
     sharpness: float = 0.0
     guidance_scale: float = 7.5
-    base_model_name: str = "RunDiffusion-XL-Photo.safetensors"
+    base_model_name: str = "Juggernaut-XI-Prototype.safetensors"
     refiner_model_name: str = "None"
     refiner_switch: float = 0.1
     loras: List[Lora] = Field(default_factory=list, examples=[[Lora()]])
     advanced_params: Optional[FcusAdvancedParams] = Field(default=None, examples=[FcusAdvancedParams()])
     require_base64: bool = True
     async_process: bool = True
```

### Comparing `gen_wrappers-0.2.6/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.2.7/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.2.7/gen_wrappers.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.2.6
+Version: 0.2.7
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.6/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.2.7/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.6/setup.py` & `gen_wrappers-0.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.2.6',
+    version='0.2.7',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

