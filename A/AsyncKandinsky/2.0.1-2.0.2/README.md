# Comparing `tmp/AsyncKandinsky-2.0.1.tar.gz` & `tmp/AsyncKandinsky-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AsyncKandinsky-2.0.1.tar", last modified: Mon Apr 15 19:05:00 2024, max compression
+gzip compressed data, was "dist/AsyncKandinsky-2.0.2.tar", last modified: Sat May 11 20:31:01 2024, max compression
```

## Comparing `AsyncKandinsky-2.0.1.tar` & `AsyncKandinsky-2.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-15 19:05:00.011260 AsyncKandinsky-2.0.1/
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-15 19:05:00.006633 AsyncKandinsky-2.0.1/AsyncKandinsky/
--rw-r--r--   0 s1rne      (503) staff       (20)     2559 2024-04-08 15:36:52.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/API_types.py
--rw-r--r--   0 s1rne      (503) staff       (20)     2804 2024-04-08 15:30:56.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/DefaultParams.py
--rw-r--r--   0 s1rne      (503) staff       (20)      944 2024-04-15 18:59:15.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/URLS.py
--rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/__init__.py
--rw-r--r--   0 s1rne      (503) staff       (20)     6470 2024-04-15 19:00:24.000000 AsyncKandinsky-2.0.1/AsyncKandinsky/api.py
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-15 19:05:00.010218 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/
--rw-r--r--   0 s1rne      (503) staff       (20)     3521 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)      349 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/SOURCES.txt
--rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/dependency_links.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/requires.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-15 19:04:59.000000 AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/top_level.txt
--rw-r--r--   0 s1rne      (503) staff       (20)     3521 2024-04-15 19:05:00.011040 AsyncKandinsky-2.0.1/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)     2883 2024-04-08 15:55:29.000000 AsyncKandinsky-2.0.1/README.md
--rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-15 19:05:00.011964 AsyncKandinsky-2.0.1/setup.cfg
--rw-r--r--   0 s1rne      (503) staff       (20)      922 2024-04-15 19:02:40.000000 AsyncKandinsky-2.0.1/setup.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-05-11 20:31:01.275492 AsyncKandinsky-2.0.2/
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-05-11 20:31:01.269636 AsyncKandinsky-2.0.2/AsyncKandinsky/
+-rw-r--r--   0 s1rne      (503) staff       (20)     2559 2024-04-08 15:36:52.000000 AsyncKandinsky-2.0.2/AsyncKandinsky/API_types.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     2976 2024-05-11 20:24:42.000000 AsyncKandinsky-2.0.2/AsyncKandinsky/DefaultParams.py
+-rw-r--r--   0 s1rne      (503) staff       (20)      944 2024-04-15 18:59:15.000000 AsyncKandinsky-2.0.2/AsyncKandinsky/URLS.py
+-rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-2.0.2/AsyncKandinsky/__init__.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     6520 2024-05-11 20:24:42.000000 AsyncKandinsky-2.0.2/AsyncKandinsky/api.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-05-11 20:31:01.274557 AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/
+-rw-r--r--   0 s1rne      (503) staff       (20)     3722 2024-05-11 20:31:01.000000 AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)      349 2024-05-11 20:31:01.000000 AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/SOURCES.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-05-11 20:31:01.000000 AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/dependency_links.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-05-11 20:31:01.000000 AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/requires.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-05-11 20:31:01.000000 AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/top_level.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)     3722 2024-05-11 20:31:01.275275 AsyncKandinsky-2.0.2/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)     3084 2024-05-11 20:28:41.000000 AsyncKandinsky-2.0.2/README.md
+-rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-05-11 20:31:01.276182 AsyncKandinsky-2.0.2/setup.cfg
+-rw-r--r--   0 s1rne      (503) staff       (20)      922 2024-05-11 20:28:41.000000 AsyncKandinsky-2.0.2/setup.py
```

### Comparing `AsyncKandinsky-2.0.1/AsyncKandinsky/API_types.py` & `AsyncKandinsky-2.0.2/AsyncKandinsky/API_types.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-2.0.1/AsyncKandinsky/DefaultParams.py` & `AsyncKandinsky-2.0.2/AsyncKandinsky/DefaultParams.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 class Text2ImageDefaultParams:
     style = "DEFAULT"
     width = 1024
     height = 1024
+    art_gpt = False
     model = "3.0"
     prompt = "Cat"
     negative_prompt = ""
 
     async def comb(
             self,
             style: str,
             width: int,
             height: int,
+            art_gpt: bool,
             model: str,
             prompt: str,
             negative_prompt: str,
     ) -> list:
         _style = self.style if style is None else style
         _width = self.width if width is None else width
         _height = self.height if height is None else height
+        _art_gpt = self.art_gpt if art_gpt in None else art_gpt
         _model = self.model
         _prompt = self.prompt if prompt is None else prompt
         _negative_prompt = self.negative_prompt if negative_prompt is None else negative_prompt
 
         return [
             {
                 "type": "GENERATE",
                 "style": _style,
                 "width": _width,
                 "height": _height,
+                "censor": {"useGigaBeautificator": art_gpt},
                 "generateParams": {"query": _prompt},
                 "negativePromptDecoder": _negative_prompt
             },
             _model
         ]
```

### Comparing `AsyncKandinsky-2.0.1/AsyncKandinsky/URLS.py` & `AsyncKandinsky-2.0.2/AsyncKandinsky/URLS.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-2.0.1/AsyncKandinsky/api.py` & `AsyncKandinsky-2.0.2/AsyncKandinsky/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,21 @@
     async def text2image(
             self,
             prompt: str,
             negative_prompt: str | None = None,
             style: str | None = None,
             width: int | None = None,
             height: int | None = None,
-            model: str | None = None,  # don`t touch (only 3.0)
+            art_gpt: bool | None = None,
+            model: str | None = None,  # don`t touch (only 3.1)
 
             max_time: int = 2 * 60  # max time generation on seconds (after return error)
     ) -> dict:
         params, model = await self.api.text2image_default_params.comb(
-            style, width, height, model, prompt, negative_prompt
+            style, width, height, art_gpt, model, prompt, negative_prompt
         )
 
         data = aiohttp.FormData()
         data.add_field("params",
                        json.dumps(params),
                        content_type="application/json",
                        )
```

### Comparing `AsyncKandinsky-2.0.1/AsyncKandinsky.egg-info/PKG-INFO` & `AsyncKandinsky-2.0.2/AsyncKandinsky.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 2.0.1
+Version: 2.0.2
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp>=3.8.4
 
 # **kandinsky-api-requests**
 
-**Асинхронное** api для использования kandinsky 3.0 в своих проектах
+**Асинхронное** api для использования kandinsky 3.1 в своих проектах
 
 ## **Как использовать:**
 ##### Установка: 
 ```
 pip install AsyncKandinsky
 ```
 
@@ -44,14 +44,15 @@
 ###### *Полные примеры можно посмотреть в tests.py (GitHub)*
 
 
 ### 1. text2image
 ```
 async def generate():
     result = await model.text2image("котик", style="ANIME")
+    # новый параметр art_gpt - это инструмент для автоматического улучшения промпта => улучшение качества картинки 
     if result["error"]:
         print("Error:")
         print(result["data"])
     else:
         with open("cat_anime_img.png", "wb") as f:
             f.write(result["data"].getvalue())
         print("Done!")
```

### Comparing `AsyncKandinsky-2.0.1/PKG-INFO` & `AsyncKandinsky-2.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 2.0.1
+Version: 2.0.2
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp>=3.8.4
 
 # **kandinsky-api-requests**
 
-**Асинхронное** api для использования kandinsky 3.0 в своих проектах
+**Асинхронное** api для использования kandinsky 3.1 в своих проектах
 
 ## **Как использовать:**
 ##### Установка: 
 ```
 pip install AsyncKandinsky
 ```
 
@@ -44,14 +44,15 @@
 ###### *Полные примеры можно посмотреть в tests.py (GitHub)*
 
 
 ### 1. text2image
 ```
 async def generate():
     result = await model.text2image("котик", style="ANIME")
+    # новый параметр art_gpt - это инструмент для автоматического улучшения промпта => улучшение качества картинки 
     if result["error"]:
         print("Error:")
         print(result["data"])
     else:
         with open("cat_anime_img.png", "wb") as f:
             f.write(result["data"].getvalue())
         print("Done!")
```

### Comparing `AsyncKandinsky-2.0.1/README.md` & `AsyncKandinsky-2.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # **kandinsky-api-requests**
 
-**Асинхронное** api для использования kandinsky 3.0 в своих проектах
+**Асинхронное** api для использования kandinsky 3.1 в своих проектах
 
 ## **Как использовать:**
 ##### Установка: 
 ```
 pip install AsyncKandinsky
 ```
 
@@ -28,14 +28,15 @@
 ###### *Полные примеры можно посмотреть в tests.py (GitHub)*
 
 
 ### 1. text2image
 ```
 async def generate():
     result = await model.text2image("котик", style="ANIME")
+    # новый параметр art_gpt - это инструмент для автоматического улучшения промпта => улучшение качества картинки 
     if result["error"]:
         print("Error:")
         print(result["data"])
     else:
         with open("cat_anime_img.png", "wb") as f:
             f.write(result["data"].getvalue())
         print("Done!")
```

### Comparing `AsyncKandinsky-2.0.1/setup.py` & `AsyncKandinsky-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='AsyncKandinsky',
-    version='2.0.1',
+    version='2.0.2',
     author='s1rne',
     author_email='s.simaranov8@gmail.com',
     description='This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/s1rne/kandinsky-async-api',
     packages=find_packages(),
```

