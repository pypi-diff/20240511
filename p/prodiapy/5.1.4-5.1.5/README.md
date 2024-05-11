# Comparing `tmp/prodiapy-5.1.4.tar.gz` & `tmp/prodiapy-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-5.1.4.tar", max compression
+gzip compressed data, was "prodiapy-5.1.5.tar", max compression
```

## Comparing `prodiapy-5.1.4.tar` & `prodiapy-5.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1070 2024-05-10 06:08:44.630330 prodiapy-5.1.4/LICENSE
--rw-r--r--   0        0        0      605 2024-05-10 06:08:44.630330 prodiapy-5.1.4/README.md
--rw-r--r--   0        0        0      183 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/__init__.py
--rw-r--r--   0        0        0     1629 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/_client.py
--rw-r--r--   0        0        0      466 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/_exceptions.py
--rw-r--r--   0        0        0     1703 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/aio.py
--rw-r--r--   0        0        0      180 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__init__.py
--rw-r--r--   0        0        0      542 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3539 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/constants.cpython-310.pyc
--rw-r--r--   0        0        0     3055 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/engine.cpython-310.pyc
--rw-r--r--   0        0        0     1357 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc
--rw-r--r--   0        0        0     2883 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/general.cpython-310.pyc
--rw-r--r--   0        0        0      212 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/logger.cpython-310.pyc
--rw-r--r--   0        0        0      799 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/response.cpython-310.pyc
--rw-r--r--   0        0        0     7010 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc
--rw-r--r--   0        0        0     5509 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc
--rw-r--r--   0        0        0     1606 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/upscale.cpython-310.pyc
--rw-r--r--   0        0        0      387 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0      159 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/constants.py
--rw-r--r--   0        0        0     1608 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/engine.py
--rw-r--r--   0        0        0     1766 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/facerestore.py
--rw-r--r--   0        0        0     1792 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/faceswap.py
--rw-r--r--   0        0        0     6289 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/general.py
--rw-r--r--   0        0        0       58 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/logger.py
--rw-r--r--   0        0        0     2758 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/photomaker.py
--rw-r--r--   0        0        0      482 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/response.py
--rw-r--r--   0        0        0      116 2024-05-10 06:08:44.630330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/__init__.py
--rw-r--r--   0        0        0     4597 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/sd15.py
--rw-r--r--   0        0        0      643 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/sdxl.py
--rw-r--r--   0        0        0    14542 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/stablediffusion/template.py
--rw-r--r--   0        0        0     2020 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/upscale.py
--rw-r--r--   0        0        0      469 2024-05-10 06:08:44.634330 prodiapy-5.1.4/prodiapy/resources/utils.py
--rw-r--r--   0        0        0      401 2024-05-10 06:08:44.634330 prodiapy-5.1.4/pyproject.toml
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 prodiapy-5.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-11 03:40:50.176770 prodiapy-5.1.5/LICENSE
+-rw-r--r--   0        0        0      605 2024-05-11 03:40:50.176770 prodiapy-5.1.5/README.md
+-rw-r--r--   0        0        0      183 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/__init__.py
+-rw-r--r--   0        0        0     1676 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/_client.py
+-rw-r--r--   0        0        0      466 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/_exceptions.py
+-rw-r--r--   0        0        0     1750 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/aio.py
+-rw-r--r--   0        0        0      180 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__init__.py
+-rw-r--r--   0        0        0      542 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3539 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/constants.cpython-310.pyc
+-rw-r--r--   0        0        0     3055 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/engine.cpython-310.pyc
+-rw-r--r--   0        0        0     1357 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc
+-rw-r--r--   0        0        0     2883 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/general.cpython-310.pyc
+-rw-r--r--   0        0        0      212 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/logger.cpython-310.pyc
+-rw-r--r--   0        0        0      799 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/response.cpython-310.pyc
+-rw-r--r--   0        0        0     7010 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc
+-rw-r--r--   0        0        0     5509 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc
+-rw-r--r--   0        0        0     1606 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/upscale.cpython-310.pyc
+-rw-r--r--   0        0        0      387 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/constants.py
+-rw-r--r--   0        0        0     1608 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/engine.py
+-rw-r--r--   0        0        0     1766 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/facerestore.py
+-rw-r--r--   0        0        0     1792 2024-05-11 03:40:50.176770 prodiapy-5.1.5/prodiapy/resources/faceswap.py
+-rw-r--r--   0        0        0     6289 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/general.py
+-rw-r--r--   0        0        0       58 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/logger.py
+-rw-r--r--   0        0        0     2758 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/photomaker.py
+-rw-r--r--   0        0        0      482 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/response.py
+-rw-r--r--   0        0        0      116 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/stablediffusion/__init__.py
+-rw-r--r--   0        0        0     4597 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/stablediffusion/sd15.py
+-rw-r--r--   0        0        0      642 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/stablediffusion/sdxl.py
+-rw-r--r--   0        0        0    14542 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/stablediffusion/template.py
+-rw-r--r--   0        0        0     2020 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/upscale.py
+-rw-r--r--   0        0        0      469 2024-05-11 03:40:50.180770 prodiapy-5.1.5/prodiapy/resources/utils.py
+-rw-r--r--   0        0        0      401 2024-05-11 03:40:50.180770 prodiapy-5.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 prodiapy-5.1.5/PKG-INFO
```

### Comparing `prodiapy-5.1.4/LICENSE` & `prodiapy-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/README.md` & `prodiapy-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/_client.py` & `prodiapy-5.1.5/prodiapy/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
         self.sd = resources.StableDiffusion(self)
         self.sdxl = resources.StableDiffusionXL(self)
 
         general = resources.General(self)
 
         self.photomaker = general.photomaker
+        self.facerestore = general.facerestore
         self.faceswap = general.faceswap
         self.upscale = general.upscale
         self.create = general.create
         self.job = general.job
         self.constants = general.constants
         self.wait = general.wait
```

### Comparing `prodiapy-5.1.4/prodiapy/aio.py` & `prodiapy-5.1.5/prodiapy/aio.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
         self.sd = resources.AsyncStableDiffusion(self)
         self.sdxl = resources.AsyncStableDiffusionXL(self)
 
         general = resources.AsyncGeneral(self)
 
         self.photomaker = general.photomaker
+        self.facerestore = general.facerestore
         self.faceswap = general.faceswap
         self.upscale = general.upscale
         self.create = general.create
         self.job = general.job
         self.constants = general.constants
         self.wait = general.wait
```

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/__init__.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/constants.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/constants.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/engine.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/faceswap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/general.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/general.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/response.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/response.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/stablediffusion.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/stablediffusionxl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/__pycache__/upscale.cpython-310.pyc` & `prodiapy-5.1.5/prodiapy/resources/__pycache__/upscale.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/engine.py` & `prodiapy-5.1.5/prodiapy/resources/engine.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/facerestore.py` & `prodiapy-5.1.5/prodiapy/resources/facerestore.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/faceswap.py` & `prodiapy-5.1.5/prodiapy/resources/faceswap.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/general.py` & `prodiapy-5.1.5/prodiapy/resources/general.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/photomaker.py` & `prodiapy-5.1.5/prodiapy/resources/photomaker.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/stablediffusion/sd15.py` & `prodiapy-5.1.5/prodiapy/resources/stablediffusion/sd15.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/stablediffusion/sdxl.py` & `prodiapy-5.1.5/prodiapy/resources/stablediffusion/sdxl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from prodiapy.resources.stablediffusion.template import StableDiffusionTemplate, AsyncStableDiffusionGeneral
 
 
 class StableDiffusionXL(StableDiffusionTemplate):
     """
     class related to /sdxl endpoints, source: https://docs.prodia.com/reference/sdxl-generate
     """
```

### Comparing `prodiapy-5.1.4/prodiapy/resources/stablediffusion/template.py` & `prodiapy-5.1.5/prodiapy/resources/stablediffusion/template.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/prodiapy/resources/upscale.py` & `prodiapy-5.1.5/prodiapy/resources/upscale.py`

 * *Files identical despite different names*

### Comparing `prodiapy-5.1.4/PKG-INFO` & `prodiapy-5.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 5.1.4
+Version: 5.1.5
 Summary: Package for using Prodia API
 Author: zenafey
 Author-email: zenafey@eugw.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

