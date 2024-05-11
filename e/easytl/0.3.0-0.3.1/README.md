# Comparing `tmp/easytl-0.3.0.tar.gz` & `tmp/easytl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.3.0.tar", last modified: Sun Apr 28 07:30:18 2024, max compression
+gzip compressed data, was "easytl-0.3.1.tar", last modified: Sat May 11 03:06:02 2024, max compression
```

## Comparing `easytl-0.3.0.tar` & `easytl-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.779622 easytl-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.771622 easytl-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.775622 easytl-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-28 07:28:44.000000 easytl-0.3.0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-28 07:28:44.000000 easytl-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-28 07:28:44.000000 easytl-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-28 07:30:18.779622 easytl-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-04-28 07:28:44.000000 easytl-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-28 07:28:44.000000 easytl-0.3.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-28 07:28:44.000000 easytl-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 07:30:18.779622 easytl-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.771622 easytl-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.775622 easytl-0.3.0/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10417 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    68885 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/googletl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-28 07:28:44.000000 easytl-0.3.0/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.779622 easytl-0.3.0/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 07:30:18.000000 easytl-0.3.0/src/easytl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 07:30:18.779622 easytl-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-28 07:28:44.000000 easytl-0.3.0/tests/issue_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-04-28 07:28:44.000000 easytl-0.3.0/tests/passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.672974 easytl-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.664974 easytl-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.668974 easytl-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-11 03:04:38.000000 easytl-0.3.1/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-11 03:04:38.000000 easytl-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-05-11 03:04:38.000000 easytl-0.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-11 03:06:02.672974 easytl-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-05-11 03:04:38.000000 easytl-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-11 03:04:38.000000 easytl-0.3.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 03:04:38.000000 easytl-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:06:02.672974 easytl-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.664974 easytl-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.668974 easytl-0.3.1/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71506 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14874 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/googletl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-11 03:04:38.000000 easytl-0.3.1/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.672974 easytl-0.3.1/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8229 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 03:06:02.000000 easytl-0.3.1/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:06:02.672974 easytl-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-11 03:04:38.000000 easytl-0.3.1/tests/issue_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13247 2024-05-11 03:04:38.000000 easytl-0.3.1/tests/passing.py
```

### Comparing `easytl-0.3.0/.github/workflows/workflow.yml` & `easytl-0.3.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/.gitignore` & `easytl-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/LICENSE.md` & `easytl-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/PKG-INFO` & `easytl-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `easytl-0.3.0/README.md` & `easytl-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/pyproject.toml` & `easytl-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0",
     "google-cloud-translate==3.15.3"
 ]
 
 name = "easytl"
-version = "v0.3.0"
+version = "v0.3.1"
 authors = [
   { name="Bikatr7", email="Bikatr7@proton.me" },
 ]
 description = "Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `easytl-0.3.0/src/easytl/__init__.py` & `easytl-0.3.1/src/easytl/__init__.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/src/easytl/classes.py` & `easytl-0.3.1/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/src/easytl/decorators.py` & `easytl-0.3.1/src/easytl/decorators.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/src/easytl/deepl_service.py` & `easytl-0.3.1/src/easytl/deepl_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 ## license that can be found in the LICENSE file.
 
 ## built-in libraries
 import typing
 import asyncio
 import time
 
+
 ## third-party libraries
 from deepl.translator import Translator
 
+import deepl
+
+## custom modules
 from .util import _convert_iterable_to_str
 from .decorators import _async_logging_decorator, _sync_logging_decorator
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, TextResult
 
 class DeepLService:
 
     _api_key:str = ""
@@ -86,14 +90,21 @@
 
         ## Service Attributes
 
         DeepLService._decorator_to_use = decorator
 
         DeepLService._log_directory = logging_directory
 
+        ## if a decorator is used, we want to disable retries, otherwise set it to the default value which is 5
+        if(DeepLService._decorator_to_use is not None):
+            deepl.http_client.max_network_retries = 0
+
+        else:
+            deepl.http_client.max_network_retries = 5
+
         if(semaphore is not None):
             DeepLService._semaphore_value = semaphore
             DeepLService._semaphore = asyncio.Semaphore(semaphore)
 
         DeepLService._rate_limit_delay = rate_limit_delay
 
 ##-------------------start-of-_prepare_translation_parameters()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
@@ -145,27 +156,25 @@
         text (string) : The text to translate.
 
         Returns:
         translation (TextResult or list of TextResult) : The translation result.
 
         """
 
+
+        ## decorators need to be applied outside of the function, for reasons detailed in easytl.py
+
         if(DeepLService._rate_limit_delay is not None):
             time.sleep(DeepLService._rate_limit_delay)
 
         params = DeepLService._prepare_translation_parameters(text)
 
         try:
 
-            if(DeepLService._decorator_to_use is None):
-                return DeepLService._translator.translate_text(**params)
-            
-            else:
-                decorated_function = DeepLService._decorator_to_use(DeepLService._translate_text)
-                return decorated_function(**params)
+            return DeepLService._translator.translate_text(**params)
             
         except Exception as _e:
             raise _e
         
 ##-------------------start-of-_translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
@@ -180,30 +189,28 @@
         text (string) : The text to translate.
 
         Returns:
         translation (TextResult or list of TextResult) : The translation result.
 
         """
 
+        ## decorators need to be applied outside of the function, for reasons detailed in easytl.py
+
         async with DeepLService._semaphore:
 
             if(DeepLService._rate_limit_delay is not None):
                 await asyncio.sleep(DeepLService._rate_limit_delay)
 
             params = DeepLService._prepare_translation_parameters(text)
 
             try:
-                if(DeepLService._decorator_to_use is None):
-                    loop = asyncio.get_running_loop()
-                    return await loop.run_in_executor(None, lambda: DeepLService._translator.translate_text(**params))
-                
-                else:
-                    decorated_function = DeepLService._decorator_to_use(DeepLService._translate_text_async)
-                    return await decorated_function(**params)
-                
+
+                loop = asyncio.get_running_loop()
+                return await loop.run_in_executor(None, lambda: DeepLService._translator.translate_text(**params))
+                                
             except Exception as _e:
                 raise _e
 
 ##-------------------start-of-_set_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     def _set_api_key(api_key:str) -> None:
```

### Comparing `easytl-0.3.0/src/easytl/easytl.py` & `easytl-0.3.1/src/easytl/easytl.py`

 * *Files 6% similar despite different names*

```diff
@@ -227,24 +227,36 @@
                                             format=format, 
                                             source_language=source_lang, 
                                             decorator=decorator, 
                                             logging_directory=logging_directory, 
                                             semaphore=None, 
                                             rate_limit_delay=translation_delay)
             
+        ## This section may seem overly complex, but it is necessary to apply the decorator outside of the function call to avoid infinite recursion.
+        ## Attempting to dynamically apply the decorator within the function leads to unexpected behavior, where this function's arguments are passed to the function instead of the intended translation function.
+
+        def translate(text):
+            return GoogleTLService._translate_text(text)
+        
+        if(decorator is not None):
+            translate = GoogleTLService._decorator_to_use(GoogleTLService._translate_text) ## type: ignore
+
+        else:
+            translate = GoogleTLService._translate_text
+            
         if(isinstance(text, str)):
-            result = GoogleTLService._translate_text(text)
+            result = translate(text)
         
             assert not isinstance(result, list), EasyTLException("Malformed response received. Please try again.")
 
             result = result if response_type == "raw" else result["translatedText"]
         
         elif(_is_iterable_of_strings(text)):
 
-            results = [GoogleTLService._translate_text(t) for t in text]
+            results = [translate(t) for t in text]
 
             assert isinstance(results, list), EasyTLException("Malformed response received. Please try again.")
 
             result = [r["translatedText"] for r in results] if response_type == "text" else results # type: ignore
             
         else:
             raise InvalidTextInputException("text must be a string or an iterable of strings.")
@@ -309,23 +321,34 @@
                                             format=format, 
                                             source_language=source_lang, 
                                             decorator=decorator, 
                                             logging_directory=logging_directory, 
                                             semaphore=semaphore, 
                                             rate_limit_delay=translation_delay)
             
+        ## This section may seem overly complex, but it is necessary to apply the decorator outside of the function call to avoid infinite recursion.
+        ## Attempting to dynamically apply the decorator within the function leads to unexpected behavior, where this function's arguments are passed to the function instead of the intended translation function.
+        def translate(text):
+            return GoogleTLService._translate_text_async(text)
+        
+        if(decorator is not None):
+            translate = GoogleTLService._decorator_to_use(GoogleTLService._translate_text_async) ## type: ignore
+
+        else:
+            translate = GoogleTLService._translate_text_async
+            
         if(isinstance(text, str)):
-            _result = await GoogleTLService._translate_text_async(text)
+            _result = await translate(text)
 
             assert not isinstance(_result, list), EasyTLException("Malformed response received. Please try again.")
 
             result = _result if response_type == "raw" else _result["translatedText"]
             
         elif(_is_iterable_of_strings(text)):
-            _tasks = [GoogleTLService._translate_text_async(t) for t in text]
+            _tasks = [translate(t) for t in text]
             _results = await asyncio.gather(*_tasks)
             
             assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
 
             result = [_r["translatedText"] for _r in _results] if response_type == "text" else _results # type: ignore
                 
         else:
@@ -357,23 +380,21 @@
         
         """
 
         Translates the given text to the target language using DeepL.
 
         This function assumes that the API key has already been set.
 
-        DeepL has backoff retrying implemented by default.
-
         Due to how DeepL's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
 
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
-        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this parameter is None, DeepL will retry your request 5 times before failing. Otherwise, the given decorator will be used.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         source_lang (string or Language or None) : The source language to translate from.
         context (string or None) : Additional information for the translator to be considered when translating. Not translated itself. This is a DeepL alpha feature and may be removed at any time.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
         preserve_formatting (bool or None) : Whether to preserve formatting.
@@ -408,33 +429,44 @@
                                         splitting_tags = splitting_tags, 
                                         ignore_tags = ignore_tags,
                                         decorator=decorator,
                                         logging_directory=logging_directory,
                                         semaphore=None,
                                         rate_limit_delay=translation_delay)
             
+        ## This section may seem overly complex, but it is necessary to apply the decorator outside of the function call to avoid infinite recursion.
+        ## Attempting to dynamically apply the decorator within the function leads to unexpected behavior, where this function's arguments are passed to the function instead of the intended translation function.
+        def translate(text):
+            return DeepLService._translate_text(text)
+        
+        if(decorator is not None):
+            translate = DeepLService._decorator_to_use(DeepLService._translate_text) ## type: ignore
+
+        else:
+            translate = DeepLService._translate_text
+
         if(isinstance(text, str)):
-            result = DeepLService._translate_text(text)
+            result = translate(text)
         
             assert not isinstance(result, list), EasyTLException("Malformed response received. Please try again.")
 
             result = result if response_type == "raw" else result.text
         
         elif(_is_iterable_of_strings(text)):
 
-            results = [DeepLService._translate_text(t) for t in text]
+            results = [translate(t) for t in text]
 
             assert isinstance(results, list), EasyTLException("Malformed response received. Please try again.")
 
             result = [_r.text for _r in results] if response_type == "text" else results # type: ignore    
             
         else:
             raise InvalidTextInputException("text must be a string or an iterable of strings.")
         
-        return result
+        return result  ## type: ignore
         
 ##-------------------start-of-deepl_translate_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
     @staticmethod
     async def deepl_translate_async(text:typing.Union[str, typing.Iterable[str]],
                             target_lang:str | Language = "EN-US",
                             override_previous_settings:bool = True,
@@ -460,23 +492,21 @@
         Asynchronous version of deepl_translate().
         
         Translates the given text to the target language using DeepL.
         Will generally be faster for iterables. Order is preserved.
 
         This function assumes that the API key has already been set.
 
-        DeepL has backoff retrying implemented by default.
-
         Due to how DeepL's API works, the translation delay and semaphore are not as important as they are for other services. As they process iterables directly.
         
         Parameters:
         text (string or iterable) : The text to translate.
         target_lang (string or Language) : The target language to translate to.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to a DeepL translation function.
-        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this parameter is None, DeepL will retry your request 5 times before failing. Otherwise, the given decorator will be used.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a TextResult object.
         semaphore (int) : The number of concurrent requests to make. Default is 30.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         source_lang (string or Language or None) : The source language to translate from.
         context (string or None) : Additional information for the translator to be considered when translating. Not translated itself. This is a DeepL alpha feature and may be removed at any time.
         split_sentences (literal or SplitSentences or None) : How to split sentences.
@@ -511,23 +541,35 @@
                                         non_splitting_tags=non_splitting_tags, 
                                         splitting_tags=splitting_tags, 
                                         ignore_tags=ignore_tags,
                                         decorator=decorator,
                                         logging_directory=logging_directory,
                                         semaphore=semaphore,
                                         rate_limit_delay=translation_delay)
+            
+        ## This section may seem overly complex, but it is necessary to apply the decorator outside of the function call to avoid infinite recursion.
+        ## Attempting to dynamically apply the decorator within the function leads to unexpected behavior, where this function's arguments are passed to the function instead of the intended translation function.
+        def translate(text):
+            return DeepLService._translate_text_async(text)
+        
+        if(decorator is not None):
+            translate = DeepLService._decorator_to_use(DeepLService._translate_text_async) ## type: ignore
+
+        else:
+            translate = DeepLService._translate_text_async
+
         if(isinstance(text, str)):
-            _result = await DeepLService._translate_text_async(text)
+            _result = await translate(text)
 
             assert not isinstance(_result, list), EasyTLException("Malformed response received. Please try again.")
 
             result = _result if response_type == "raw" else _result.text
             
         elif(_is_iterable_of_strings(text)):
-            _tasks = [DeepLService._translate_text_async(t) for t in text]
+            _tasks = [translate(t) for t in text]
             _results = await asyncio.gather(*_tasks)
             
             assert isinstance(_results, list), EasyTLException("Malformed response received. Please try again.")
 
             result = [_r.text for _r in _results] if response_type == "text" else _results # type: ignore
                 
         else:
@@ -763,20 +805,18 @@
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
-        OpenAI has it's backoff retrying disabled by EasyTL, in favor of the user implementing their own retrying mechanism via the decorator.
-
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
-        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, OpenAI will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
         top_p (float) : The nucleus sampling probability. The higher the value, the more words are considered for the next token. Generally, alter this or temperature, not both.
         stop (list or None) : The sequences to stop at.
@@ -872,20 +912,18 @@
 
         This function assumes that the API key has already been set.
 
         Translation instructions default to translating the text to English. To change this, specify the instructions.
 
         This function is not for use for real-time translation, nor for generating multiple translation candidates. Another function may be implemented for this given demand.
 
-        OpenAI has it's backoff retrying disabled by EasyTL.
-
         Parameters:
         text (string or iterable) : The text to translate.
         override_previous_settings (bool) : Whether to override the previous settings that were used during the last call to an OpenAI translation function.
-        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying.
+        decorator (callable or None) : The decorator to use when translating. Typically for exponential backoff retrying. If this is None, OpenAI will retry the request twice if it fails.
         logging_directory (string or None) : The directory to log to. If None, no logging is done. This'll append the text result and some function information to a file in the specified directory. File is created if it doesn't exist.
         response_type (literal["text", "raw", "json"]) : The type of response to return. 'text' returns the translated text, 'raw' returns the raw response, a ChatCompletion object, 'json' returns a json-parseable string.
         semaphore (int) : The number of concurrent requests to make. Default is 5.
         translation_delay (float or None) : If text is an iterable, the delay between each translation. Default is none. This is more important for asynchronous translations where a semaphore alone may not be sufficient.
         translation_instructions (string or SystemTranslationMessage or None) : The translation instructions to use. If None, the default system message is used. If you plan on using the json response type, you must specify that you want a json output and it's format in the instructions. The default system message will ask for a generic json if the response type is json.
         model (string) : The model to use.
         temperature (float) : The temperature to use. The higher the temperature, the more creative the output. Lower temperatures are typically better for translation.
```

### Comparing `easytl-0.3.0/src/easytl/exceptions.py` & `easytl-0.3.1/src/easytl/exceptions.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/src/easytl/gemini_service.py` & `easytl-0.3.1/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/src/easytl/googletl_service.py` & `easytl-0.3.1/src/easytl/googletl_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -166,28 +166,25 @@
         text (string) : The text to translate.
 
         Returns:
         translation (TextResult or list of TextResult) : The translation result.
 
         """
 
+        ## decorators need to be applied outside of the function for reasons detailed in easytl.py
+
         if(GoogleTLService._rate_limit_delay is not None):
             time.sleep(GoogleTLService._rate_limit_delay)
 
         params = GoogleTLService._prepare_translation_parameters(text)
 
         try:
 
-            if(GoogleTLService._decorator_to_use is None):
-                return GoogleTLService._translator.translate(**params)
-            
-            else:
-                decorated_function = GoogleTLService._decorator_to_use(GoogleTLService._translate_text)
-                return decorated_function(**params)
-            
+            return GoogleTLService._translator.translate(**params)
+                        
         except Exception as _e:
             raise _e
         
 ##-------------------start-of-_translate_text_async()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
         
     @staticmethod
     @_async_logging_decorator
@@ -201,29 +198,27 @@
         text (string) : The text to translate.
 
         Returns:
         translation (TextResult or list of TextResult) : The translation result.
 
         """
 
+        ## decorators need to be applied outside of the function for reasons detailed in easytl.py
+
         async with GoogleTLService._semaphore:
 
             if(GoogleTLService._rate_limit_delay is not None):
                 await asyncio.sleep(GoogleTLService._rate_limit_delay)
 
             params = GoogleTLService._prepare_translation_parameters(text)
 
             try:
-                if(GoogleTLService._decorator_to_use is None):
-                    loop = asyncio.get_running_loop()
-                    return await loop.run_in_executor(None, lambda: GoogleTLService._translator.translate(**params))
                 
-                else:
-                    decorated_function = GoogleTLService._decorator_to_use(GoogleTLService._translate_text_async)
-                    return await decorated_function(**params)
+                loop = asyncio.get_running_loop()
+                return await loop.run_in_executor(None, lambda: GoogleTLService._translator.translate(**params))
                 
             except Exception as _e:
                 raise _e
     
 ##-------------------start-of-_test_credentials()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
     
     @staticmethod
```

### Comparing `easytl-0.3.0/src/easytl/openai_service.py` & `easytl-0.3.1/src/easytl/openai_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     _max_tokens:int | None = None
     _presence_penalty:float = 0.0
     _frequency_penalty:float = 0.0
 
     _semaphore_value:int = 5
     _semaphore:asyncio.Semaphore = asyncio.Semaphore(_semaphore_value)
 
-    _sync_client = OpenAI(max_retries=0, api_key="DummyKey")
-    _async_client = AsyncOpenAI(max_retries=0, api_key="DummyKey")
+    _sync_client = OpenAI(api_key="DummyKey")
+    _async_client = AsyncOpenAI(api_key="DummyKey")
 
     _rate_limit_delay:float | None = None
 
     _decorator_to_use:typing.Union[typing.Callable, None] = None
 
     _log_directory:str | None = None
 
@@ -105,14 +105,21 @@
 
             OpenAIService._log_directory = logging_directory
 
             OpenAIService._rate_limit_delay = rate_limit_delay
 
             OpenAIService._json_mode = json_mode
 
+            ## if a decorator is used, we want to disable retries, otherwise set it to the default value which is 2
+            if(OpenAIService._decorator_to_use is not None):
+                OpenAIService._sync_client.max_retries = 0
+                OpenAIService._async_client.max_retries = 0
+            else:
+                OpenAIService._sync_client.max_retries = 2
+                OpenAIService._async_client.max_retries = 2
             
             if(semaphore is not None):
                 OpenAIService._semaphore_value = semaphore
                 OpenAIService._semaphore = asyncio.Semaphore(OpenAIService._semaphore_value)
 
             if(OpenAIService._json_mode and OpenAIService._model in VALID_JSON_OPENAI_MODELS):
                 OpenAIService._default_translation_instructions = SystemTranslationMessage("Please translate the following text into English. Make sure to return the translated text in JSON format.")
```

### Comparing `easytl-0.3.0/src/easytl/util.py` & `easytl-0.3.1/src/easytl/util.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/src/easytl.egg-info/PKG-INFO` & `easytl-0.3.1/src/easytl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Seamless Multi-API Translation: Simplifying Language Barriers with DeepL, OpenAI, Gemini and Google Translate.
 Author-email: Bikatr7 <Bikatr7@proton.me>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `easytl-0.3.0/src/easytl.egg-info/SOURCES.txt` & `easytl-0.3.1/src/easytl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/tests/issue_template.py` & `easytl-0.3.1/tests/issue_template.py`

 * *Files identical despite different names*

### Comparing `easytl-0.3.0/tests/passing.py` & `easytl-0.3.1/tests/passing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from easytl import EasyTL
 
 import asyncio
 import os
 import time
+import logging
+
+import backoff
+
+from easytl.exceptions import DeepLException, GoogleAPIError, OpenAIError
 
 ##-------------------start-of-read_api_key()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 def read_api_key(filename):
     try:
         with open(filename, 'r') as file:
             return file.read().strip()
@@ -59,30 +64,32 @@
 
 ##-------------------start-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
 async def main():
 
     gemini_time_delay, logging_directory = setup_preconditions()
 
+    decorator = backoff.on_exception(backoff.expo, exception=(DeepLException, GoogleAPIError, OpenAIError), logger=logging.getLogger())
+
     print("------------------------------------------------Deepl------------------------------------------------")
 
     print("------------------------------------------------Text response------------------------------------------------")
 
-    print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", logging_directory=logging_directory))
-    print(await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", logging_directory=logging_directory))
-    
-    print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory).text) # type: ignore
-    result = await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory)
+    print(EasyTL.deepl_translate(text="Hello, world!", target_lang="DE", logging_directory=logging_directory, decorator=decorator))
+    print(await EasyTL.deepl_translate_async(text="Hello, world!", target_lang="DE", logging_directory=logging_directory,decorator=decorator))
+
+    print(EasyTL.deepl_translate("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator).text) # type: ignore
+    result = await EasyTL.deepl_translate_async("Hello, world!", target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator)
 
     print(result.text) # type: ignore
 
     print("------------------------------------------------Raw response------------------------------------------------")
 
-    results = EasyTL.deepl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory)
-    async_results = await EasyTL.deepl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory)
+    results = EasyTL.deepl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator)
+    async_results = await EasyTL.deepl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="DE", response_type="raw", logging_directory=logging_directory, decorator=decorator)
 
     for result in results: # type: ignore
         print(result.text) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.text)
 
@@ -92,107 +99,121 @@
 
     print(f"Characters: {characters}, Cost: {cost}, Model: {model}")
 
     print("------------------------------------------------Google Translate------------------------------------------------")
 
     print("------------------------------------------------Text response------------------------------------------------")
 
-    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", logging_directory=logging_directory))
-    print(await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", logging_directory=logging_directory))
+    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator))
+    print(await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory)["translatedText"]) # type: ignore
-    result = await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory)
+    print(EasyTL.googletl_translate("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)["translatedText"]) # type: ignore
+    result = await EasyTL.googletl_translate_async("Hello, world!", target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)
 
     print(result["translatedText"]) # type: ignore
 
     print("------------------------------------------------Raw response------------------------------------------------")
 
-    results = EasyTL.googletl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory)
-    async_results = await EasyTL.googletl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory)
+    results = EasyTL.googletl_translate(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)
+    async_results = await EasyTL.googletl_translate_async(text=["Hello, world!", "Goodbye, world!"], target_lang="de", response_type="raw", logging_directory=logging_directory, decorator=decorator)
 
     for result in results: # type: ignore
         print(result["translatedText"]) # type: ignore
 
     for result in async_results: # type: ignore
         print(result["translatedText"]) # type: ignore
-
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     characters, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="google translate", model=None, translation_instructions=None)
 
     print(f"Characters: {characters}, Cost: {cost}, Model: {model}")
 
     print("------------------------------------------------Gemini------------------------------------------------")
 
     print("-----------------------------------------------Text response-----------------------------------------------")
 
-    print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory))
-    print(await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory))
+    print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
+    print(await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory).text) # type: ignore
-    result = await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
+    print(EasyTL.gemini_translate("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator).text) # type: ignore
+    result = await EasyTL.gemini_translate_async("Hello, world!", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
 
     print(result.text) # type: ignore
 
     print("-----------------------------------------------Raw response-----------------------------------------------")
 
-    results = EasyTL.gemini_translate(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
-    async_results = await EasyTL.gemini_translate_async(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory, translation_delay=5)
+    results = EasyTL.gemini_translate(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
+    async_results = await EasyTL.gemini_translate_async(text=["Hello, world!", "Goodbye, world!"], translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory, translation_delay=5,decorator=decorator)
 
     for result in results: # type: ignore
         print(result.text) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.text)
 
     print("-----------------------------------------------JSON response-----------------------------------------------")
 
-    print(EasyTL.gemini_translate("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Translate this to German. Format the response as JSON.", response_type="json", logging_directory=logging_directory))
+    print(EasyTL.gemini_translate("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Translate this to German. Format the response as JSON.", response_type="json", logging_directory=logging_directory,decorator=decorator))
     
     time.sleep(gemini_time_delay)
     
-    print(await EasyTL.gemini_translate_async("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory))
+    print(await EasyTL.gemini_translate_async("Hello, world!", model="gemini-1.5-pro-latest", translation_instructions="Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory,decorator=decorator))
 
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="gemini", model="gemini-pro", translation_instructions="Translate this to German.")
 
     print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
 
     print("------------------------------------------------OpenAI------------------------------------------------")
 
     print("-----------------------------------------------Text response-----------------------------------------------")
 
-    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory))
-    print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory))
+    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
+    print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", logging_directory=logging_directory, decorator=decorator))
 
-    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory).choices[0].message.content) # type: ignore
-    result = await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
+    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator).choices[0].message.content) # type: ignore
+    result = await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
 
     print(result.choices[0].message.content) # type: ignore
 
     print("-----------------------------------------------Raw response-----------------------------------------------")
 
-    results = EasyTL.openai_translate(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
-    async_results = await EasyTL.openai_translate_async(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory)
+    results = EasyTL.openai_translate(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
+    async_results = await EasyTL.openai_translate_async(text=["Hello, world!", "Goodbye, world!"], model="gpt-3.5-turbo", translation_instructions="Translate this to German.", response_type="raw", logging_directory=logging_directory,decorator=decorator)
 
     for result in results: # type: ignore
         print(result.choices[0].message.content) # type: ignore
 
     for result in async_results: # type: ignore
         print(result.choices[0].message.content ) # type: ignore
 
     print("-----------------------------------------------JSON response-----------------------------------------------")
 
-    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German. Format the response as JSON parseable string.", response_type="json", logging_directory=logging_directory))
-    print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German. Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory))
+    print(EasyTL.openai_translate("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German. Format the response as JSON parseable string.", response_type="json", logging_directory=logging_directory,decorator=decorator))
+    print(await EasyTL.openai_translate_async("Hello, world!", model="gpt-3.5-turbo-0125", translation_instructions="Translate this to German. Format the response as JSON parseable string. It should have 2 keys, one for input titled input, and one called output, which is the translation.", response_type="json", logging_directory=logging_directory,decorator=decorator))
 
     print("------------------------------------------------Cost calculation------------------------------------------------")
 
     tokens, cost, model = EasyTL.calculate_cost(text="Hello, world!", service="openai", model="gpt-3.5-turbo", translation_instructions="Translate this to German.")
 
     print(f"Tokens: {tokens}, Cost: {cost}, Model: {model}")
 
 ##-------------------end-of-main()---------------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
+
+
 if(__name__ == "__main__"):
-    asyncio.run(main())
+    ## setup logging
+    logging.basicConfig(level=logging.DEBUG, 
+                        filename='passing.log',
+                        filemode='w', 
+                        format='[%(asctime)s] [%(levelname)s] [%(filename)s] %(message)s', 
+                        datefmt='%Y-%m-%d %H:%M:%S')
+
+    console = logging.StreamHandler()
+    console.setLevel(logging.INFO)
+    formatter = logging.Formatter('[%(asctime)s] [%(levelname)s] [%(filename)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
+    console.setFormatter(formatter)
+    logging.getLogger('').addHandler(console)
+
+    asyncio.run(main())
```

