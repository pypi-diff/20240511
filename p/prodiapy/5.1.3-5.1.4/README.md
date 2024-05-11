# Comparing `tmp/prodiapy-5.1.3.tar.gz` & `tmp/prodiapy-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-5.1.3.tar", max compression
+gzip compressed data, was "prodiapy-5.1.4.tar", max compression
```

## Comparing `prodiapy-5.1.3.tar` & `prodiapy-5.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1070 2024-05-09 20:03:10.895299 prodiapy-5.1.3/LICENSE
--rw-r--r--   0        0        0      605 2024-05-09 20:03:10.895299 prodiapy-5.1.3/README.md
--rw-r--r--   0        0        0      183 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/__init__.py
--rw-r--r--   0        0        0     1629 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/_client.py
--rw-r--r--   0        0        0      466 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/_exceptions.py
--rw-r--r--   0        0        0     1703 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/aio.py
--rw-r--r--   0        0        0      180 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__init__.py
--rw-r--r--   0        0        0      542 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3539 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     3055 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/engine.cpython-310.pyc
--rw-r--r--   0        0        0     1357 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc
--rw-r--r--   0        0        0     2883 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/general.cpython-310.pyc
--rw-r--r--   0        0        0      212 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0      799 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     7010 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc
--rw-r--r--   0        0        0     5509 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc
--rw-r--r--   0        0        0     1606 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/upscale.cpython-310.pyc
--rw-r--r--   0        0        0      387 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      159 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/constants.py
--rw-r--r--   0        0        0     1608 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/engine.py
--rw-r--r--   0        0        0     1766 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/facerestore.py
--rw-r--r--   0        0        0     1792 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/faceswap.py
--rw-r--r--   0        0        0     6279 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/general.py
--rw-r--r--   0        0        0       58 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/logger.py
--rw-r--r--   0        0        0     2755 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/photomaker.py
--rw-r--r--   0        0        0      482 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/response.py
--rw-r--r--   0        0        0      116 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/__init__.py
--rw-r--r--   0        0        0     4595 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/sd15.py
--rw-r--r--   0        0        0      641 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/sdxl.py
--rw-r--r--   0        0        0    14541 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/stablediffusion/template.py
--rw-r--r--   0        0        0     2020 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/upscale.py
--rw-r--r--   0        0        0      469 2024-05-09 20:03:10.895299 prodiapy-5.1.3/prodiapy/resources/utils.py
--rw-r--r--   0        0        0      401 2024-05-09 20:03:10.895299 prodiapy-5.1.3/pyproject.toml
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 prodiapy-5.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-10 06:08:44.630330 prodiapy-5.1.4/LICENSE
+-rw-r--r--   0        0        0      605 2024-05-10 06:08:44.630330 prodiapy-5.1.4/README.md
+-rw-r--r--   0        0        0      183 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/__init__.py
+-rw-r--r--   0        0        0     1629 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/_client.py
+-rw-r--r--   0        0        0      466 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/_exceptions.py
+-rw-r--r--   0        0        0     1703 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/aio.py
+-rw-r--r--   0        0        0      180 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__init__.py
+-rw-r--r--   0        0        0      542 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3539 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     3055 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/engine.cpython-310.pyc
+-rw-r--r--   0        0        0     1357 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc
+-rw-r--r--   0        0        0     2883 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/general.cpython-310.pyc
+-rw-r--r--   0        0        0      212 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0      799 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/response.cpython-310.pyc
+-rw-r--r--   0        0        0     7010 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc
+-rw-r--r--   0        0        0     5509 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/upscale.cpython-310.pyc
+-rw-r--r--   0        0        0      387 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/constants.py
+-rw-r--r--   0        0        0     1608 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/engine.py
+-rw-r--r--   0        0        0     1766 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/facerestore.py
+-rw-r--r--   0        0        0     1792 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/faceswap.py
+-rw-r--r--   0        0        0     6289 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/general.py
+-rw-r--r--   0        0        0       58 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/logger.py
+-rw-r--r--   0        0        0     2758 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/photomaker.py
+-rw-r--r--   0        0        0      482 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/response.py
+-rw-r--r--   0        0        0      116 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/__init__.py
+-rw-r--r--   0        0        0     4597 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/sd15.py
+-rw-r--r--   0        0        0      643 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/sdxl.py
+-rw-r--r--   0        0        0    14542 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/template.py
+-rw-r--r--   0        0        0     2020 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/upscale.py
+-rw-r--r--   0        0        0      469 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/utils.py
+-rw-r--r--   0        0        0      401 2024-05-10 06:08:44.634330 prodiapy-5.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 prodiapy-5.1.4/PKG-INFO
```

### Comparing `prodiapy-5.1.3/LICENSE` & `prodiapy-5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/README.md` & `prodiapy-5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/_client.py` & `prodiapy-5.1.4/prodiapy/_client.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/aio.py` & `prodiapy-5.1.4/prodiapy/aio.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/__init__.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/constants.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/engine.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/general.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/response.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/__pycache__/upscale.cpython-310.pyc` & `prodiapy-5.1.4/prodiapy/resources/__pycache__/upscale.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/engine.py` & `prodiapy-5.1.4/prodiapy/resources/engine.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/facerestore.py` & `prodiapy-5.1.4/prodiapy/resources/facerestore.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/faceswap.py` & `prodiapy-5.1.4/prodiapy/resources/faceswap.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/prodiapy/resources/general.py` & `prodiapy-5.1.4/prodiapy/resources/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 class General(APIResource):
     facerestore: FaceRestore.facerestore
     faceswap: FaceSwap.faceswap
     upscale: Upscale.upscale
 
     def __init__(self, client: SyncAPIClient) -> None:
         super().__init__(client)
+        
         self.photomaker = PhotoMaker(client).photomaker
         self.facerestore = FaceRestore(client).facerestore
         self.faceswap = FaceSwap(client).faceswap
         self.upscale = Upscale(client).upscale
 
     def create(
             self,
@@ -104,14 +105,15 @@
 class AsyncGeneral(APIResource):
     facerestore: AsyncFaceRestore.facerestore
     faceswap: AsyncFaceSwap.faceswap
     upscale: AsyncUpscale.upscale
 
     def __init__(self, client: AsyncAPIClient) -> None:
         super().__init__(client)
+
         self.photomaker = AsyncPhotoMaker(client).photomaker
         self.facerestore = AsyncFaceRestore(client).facerestore
         self.faceswap = AsyncFaceSwap(client).faceswap
         self.upscale = AsyncUpscale(client).upscale
 
     async def create(
             self,
```

### Comparing `prodiapy-5.1.3/prodiapy/resources/photomaker.py` & `prodiapy-5.1.4/prodiapy/resources/photomaker.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         """
         Generate images with character consistency, source: https://docs.prodia.com/reference/photomaker
 
         Returns:
             Python dictionary containing job id
         """
         return await self._post(
-            "/upscale",
+            "/photomaker",
             body=form_body(
                 dict_parameters=dict_parameters,
                 imageUrls=image_urls,
                 imageData=image_data,
                 prompt=prompt,
                 negative_prompt=negative_prompt,
                 style_preset=style_preset,
```

### Comparing `prodiapy-5.1.3/prodiapy/resources/stablediffusion/sd15.py` & `prodiapy-5.1.4/prodiapy/resources/stablediffusion/sd15.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import Union, Optional, Literal
-from prodiapy.resources.stablediffusion.template import StableDiffusionGeneral, AsyncStableDiffusionGeneral
+from prodiapy.resources.stablediffusion.template import StableDiffusionTemplate, AsyncStableDiffusionGeneral
 from prodiapy.resources.engine import SyncAPIClient, AsyncAPIClient
 from prodiapy.resources.utils import form_body
 
 
-class StableDiffusion(StableDiffusionGeneral):
+class StableDiffusion(StableDiffusionTemplate):
     """class related to /sd endpoints, source: https://docs.prodia.com/reference/generate"""
     def __init__(self, client: SyncAPIClient) -> None:
         super().__init__(client, model_architecture="sd")
 
     def controlnet(
             self,
             image_url: Optional[str] = None,
```

### Comparing `prodiapy-5.1.3/prodiapy/resources/stablediffusion/template.py` & `prodiapy-5.1.4/prodiapy/resources/stablediffusion/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from prodiapy.resources.engine import APIResource
 from typing import Union, Optional, Literal
 from prodiapy.resources.utils import form_body
 
 
-class StableDiffusionGeneral(APIResource):
+class StableDiffusionTemplate(APIResource):
     def __init__(self, client, model_architecture="sd") -> None:
         super().__init__(client)
         self.model_architecture = model_architecture
 
     def generate(
             self,
             model: Optional[str] = None,
```

### Comparing `prodiapy-5.1.3/prodiapy/resources/upscale.py` & `prodiapy-5.1.4/prodiapy/resources/upscale.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.3/PKG-INFO` & `prodiapy-5.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 5.1.3
+Version: 5.1.4
 Summary: Package for using Prodia API
 Author: zenafey
 Author-email: zenafey@eugw.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

