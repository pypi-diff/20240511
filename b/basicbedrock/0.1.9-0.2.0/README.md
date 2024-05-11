# Comparing `tmp/basicbedrock-0.1.9.tar.gz` & `tmp/basicbedrock-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.1.9.tar", last modified: Mon Apr 29 19:41:40 2024, max compression
+gzip compressed data, was "basicbedrock-0.2.0.tar", last modified: Fri May 10 19:48:16 2024, max compression
```

## Comparing `basicbedrock-0.1.9.tar` & `basicbedrock-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.806318 basicbedrock-0.1.9/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.1.9/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-29 19:41:40.806097 basicbedrock-0.1.9/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.1.9/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-04-29 19:41:32.000000 basicbedrock-0.1.9/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-04-29 19:41:40.806373 basicbedrock-0.1.9/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.800719 basicbedrock-0.1.9/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.801654 basicbedrock-0.1.9/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      273 2024-04-29 19:41:32.000000 basicbedrock-0.1.9/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    17519 2024-04-29 19:41:32.000000 basicbedrock-0.1.9/src/basicbedrock/basicbedrock.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.804847 basicbedrock-0.1.9/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3215 2024-04-24 16:48:37.000000 basicbedrock-0.1.9/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2729 2024-04-22 21:49:02.000000 basicbedrock-0.1.9/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5028 2024-04-22 21:52:22.000000 basicbedrock-0.1.9/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     4480 2024-04-22 21:58:39.000000 basicbedrock-0.1.9/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.1.9/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3037 2024-04-22 21:52:22.000000 basicbedrock-0.1.9/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3312 2024-04-24 16:55:21.000000 basicbedrock-0.1.9/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     1559 2024-04-22 21:49:02.000000 basicbedrock-0.1.9/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.805839 basicbedrock-0.1.9/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      586 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-04-29 19:41:40.000000 basicbedrock-0.1.9/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-04-29 19:41:40.805110 basicbedrock-0.1.9/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     4526 2024-04-11 01:09:03.000000 basicbedrock-0.1.9/test/tests.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-10 19:48:16.466621 basicbedrock-0.2.0/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.2.0/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-05-10 19:48:16.466344 basicbedrock-0.2.0/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.2.0/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-05-10 19:44:46.000000 basicbedrock-0.2.0/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-05-10 19:48:16.466682 basicbedrock-0.2.0/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-10 19:48:16.461155 basicbedrock-0.2.0/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-10 19:48:16.462893 basicbedrock-0.2.0/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      330 2024-05-10 19:47:23.000000 basicbedrock-0.2.0/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    19093 2024-05-10 19:42:41.000000 basicbedrock-0.2.0/src/basicbedrock/basicbedrock.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    10079 2024-05-10 19:42:41.000000 basicbedrock-0.2.0/src/basicbedrock/guardrails.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     7632 2024-05-02 02:20:16.000000 basicbedrock-0.2.0/src/basicbedrock/guardrails_baseclasses.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-10 19:48:16.465225 basicbedrock-0.2.0/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     6371 2024-04-30 18:13:06.000000 basicbedrock-0.2.0/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2897 2024-04-30 18:26:06.000000 basicbedrock-0.2.0/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5787 2024-04-30 18:26:06.000000 basicbedrock-0.2.0/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5070 2024-04-30 18:28:26.000000 basicbedrock-0.2.0/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.2.0/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3450 2024-04-30 18:26:06.000000 basicbedrock-0.2.0/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3694 2024-04-30 18:26:06.000000 basicbedrock-0.2.0/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2353 2024-04-30 18:44:40.000000 basicbedrock-0.2.0/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-10 19:48:16.465910 basicbedrock-0.2.0/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-05-10 19:48:16.000000 basicbedrock-0.2.0/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      672 2024-05-10 19:48:16.000000 basicbedrock-0.2.0/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-05-10 19:48:16.000000 basicbedrock-0.2.0/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-05-10 19:48:16.000000 basicbedrock-0.2.0/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-05-10 19:48:16.000000 basicbedrock-0.2.0/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-10 19:48:16.465402 basicbedrock-0.2.0/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     6682 2024-05-10 19:43:58.000000 basicbedrock-0.2.0/test/test_basicbedrock.py
```

### Comparing `basicbedrock-0.1.9/LICENSE` & `basicbedrock-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.9/PKG-INFO` & `basicbedrock-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.9
+Version: 0.2.0
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3>=1.34.79
+Requires-Dist: boto3>=1.34.94
 Requires-Dist: pydantic>=2.6.4
 
 # BasicBedrock
 AWS Bedrock provides a variety of foundational models to AWS customers.  Each model family requires their own request structure, yet the underlying semantics are roughly common; there is always a field for the textual input prompt, and often there are fields to define maximum desired output, stop words, P, K and Temperature values.
 
 This package aims to abstract away all of that.
```

### Comparing `basicbedrock-0.1.9/README.md` & `basicbedrock-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.9/pyproject.toml` & `basicbedrock-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
@@ -15,14 +15,14 @@
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
 ]
 dependencies = [
-    "boto3>=1.34.79",
+    "boto3>=1.34.94",
     "pydantic>=2.6.4",
 ]
 
 [project.urls]
 Homepage = "https://github.com/cyberitech/BasicBedrock"
 Issues = "https://github.com/cyberitech/BasicBedrock/issues"
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.2.0/src/basicbedrock/basicbedrock.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,35 @@
 Abstracts away the need to understand any of the model-specific response or request semantics.
 Simply pick a model, and invoke it with a prompt.
 If you with to specify k, p, temp, and max_token parameters, they will be applied on a best effort basis.
 not all models support all parameters.
 """
 
 import json
-import typing
 import warnings
 
 import boto3
 import pydantic
 
 from models import *
-from src import basicbedrock
+from basicbedrock.guardrails import Guardrails
 
 
 class BasicBedrock(object):
     def __init__(self, session: boto3.session.Session = None, **kwargs):
         """
         Creates an instance of basic bedrock.
         session param is optional.  If omitted, a default session constructor will be used.
         Right now, the only kwargs supported are a param dictionary.
         Param dicts are in the format of {'top_p': float, 'top_k': int, 'temp': float, 'max_tokens': int}
         :param session: the boto3 session to use for creating the basic bedrock instance
         :param kwargs: kwargs used are in the format of {'top_p': float, 'top_k': int, 'temp': float, 'max_tokens': int}
         """
         if not session:
-            warnings.warn('No session provided, attempting to use "default" profile', category=RuntimeWarning)
+            #warnings.warn('No session provided, attempting to use "default" profile', category=RuntimeWarning)
             session = boto3.session.Session()
         self.client = session.client("bedrock-runtime")
         self._default_k = 100
         self._default_p = .5
         self._default_t = .5
         self._default_n = 150
         self._default_stop = []
@@ -43,21 +42,21 @@
         self._t = self._default_t
         self._n = self._default_n
         self._s = self._default_stop
         # set params according to kwargs
         if kwargs:
             self.set_params(kwargs)
 
-        # determine which models are enabled in AWS account and also supported by BasicBedrock
+        # We need to know what models are enabled in the aws account for this region
         _bedrock_cp = session.client("bedrock")
         r = _bedrock_cp.list_foundation_models()
         self.enabled_models = [
             e.get('modelId') for e in r['modelSummaries'] if e.get('modelLifecycle').get('status') == 'ACTIVE'
         ]
-        self.available_models = sorted(
+        self.available_models = sorted(  # calculates and sorts nodels both enabled and supported
             list(
                 set(
                     self.enabled_models
                 ).intersection(
                     set(
                         BasicBedrock.get_supported_models()
                     )
@@ -68,15 +67,14 @@
     def print_available_models(self):
         """
         Prints available models that are supported by BasicBedrock and enabled in the aws account
         :return:
         """
         print(os.linesep.join(self.available_models))
 
-
     def get_available_models(self):
         """
         Gets a list of available models that are supported by BasicBedrock and enabled in the aws account
         :return: list of models both enabled and suported
         """
         return self.available_models
 
@@ -92,114 +90,132 @@
     def get_supported_models() -> list:
         """
         returns a list of all models supported by BasicBedrock, which may not be the same models a user has enabled within their account
         :return: ["model1", "model2", "model3"...]
         """
         return sorted(model_request_mapping.keys())
 
+    @staticmethod
     def get_model_schema_dict(self, model_id: str) -> dict:
         """
         returns a dict object representing the request scheme of model_id
         :param model_id:  the chosen model id
         :return: dict object representing the base request scheme of model_id
         """
-        if model_id not in self.get_supported_models():
+        if model_id not in BasicBedrock.get_supported_models():
             raise ValueError(f"requested model {model_id} is not an available model")
         else:
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             d = json.loads(j)
             return d
 
-    def get_model_request_object(self, model_id: str) -> BaseAbstractRequest:
+    @staticmethod
+    def get_model_request_object(model_id: str) -> BaseAbstractRequest:
         """
         returns an instantiated object representing the schema for the chosen model.
         All these inherit from BaseSchemaAbstract.
         Its useful for when you want to use BaseSchemaAbstract to modify prompts and produce json or dicts manually
         :param model_id: the chosen model ID
         :return: the schema class object for the chosen model, it will be a subclass of a BaseAbstractRequest
         """
-        if model_id not in self.get_supported_models():
-            raise ValueError(f"requested model {model_id} is not an available model")
+        if model_id not in BasicBedrock.get_supported_models():
+            raise ValueError(f"requested model {model_id} is not an available model in BasicBedrock")
         _inst = model_request_mapping.get(model_id)()
         return _inst
 
-    def get_model_request_json(self, model_id: str) -> str:
+    @staticmethod
+    def get_model_request_json(model_id: str) -> str:
         """
         returns a string object representing the request scheme of model_id in json format
         :param model_id:  the chosen model id
         :return: a json string
         """
-        if model_id not in self.get_supported_models():
-            raise ValueError(f"requested model {model_id} is not an available model")
+        if model_id not in BasicBedrock.get_supported_models():
+            raise ValueError(f"requested model {model_id} is not an available model in BasicBedrock")
         else:
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             return j
 
-    def print_model_schema(self, model_id: str, indent: int = None) -> None:
+
+    @staticmethod
+    def print_model_schema(model_id: str, indent: int = None) -> None:
         """
         prints the request scheme of model_id in a pretty format.
         if indent is not None, indent the lines when printing
         :param model_id: the chosen model id
         :param indent: how many spaces to indent, default=4
         :return: None
         """
-        if model_id not in self.get_supported_models():
-            raise ValueError(f"requested model {model_id} is not an available model")
+        if model_id not in BasicBedrock.get_supported_models():
+            raise ValueError(f"requested model {model_id} is not an available model in BasicBedrock")
         else:
             model = model_request_mapping.get(model_id)
             _inst = model()
             j = _inst.json()
             if indent:
                 j = json.dumps(json.loads(j), indent=indent)
         print(j)
 
-    def get_boto3_body(self, model_id: str, prompt: str) -> str:
+    @staticmethod
+    def get_boto3_body(model_id: str, prompt: str) -> str:
         """
         given a model_id and a prompt, this will construct the boto3 'body' parameter using the specified prompt and params,
         but it will not invoke bedrock or pass it to boto3, it will simply return the boto3 'body' param as a string.
         Internally, this calls the update_prompt() function, not update_prompt_raw(), which means that it will take into account
         the expected calling convention of the underlying model by inserting things such as 'Human:' or '<s>[INST]' as appropriate
         :param model_id: the model to construct a boto3 body for
         :param prompt: the prompt to pass the model.
         :return: a string, representing the equivalent boto3 'body' parameter.
         """
-        if model_id not in self.get_supported_models():
-            raise ValueError(f"requested model {model_id} is not an available model")
+        if model_id not in BasicBedrock.get_supported_models():
+            raise ValueError(f"requested model {model_id} is not an available model in BasicBedrock")
         if not isinstance(prompt, str):
             raise ValueError(f"prompt must be a string, but got {type(prompt)}")
         schema = model_request_mapping.get(model_id)
         schema_inst: BaseAbstractRequest = schema()
         schema_inst.set_prompt(prompt)
         schema_inst.set_params(self.params)
         j = schema_inst.json()
         return j
 
     def invoke(self, model_id: str, request: typing.Union[str, dict],
-               show_request: bool = False) -> BaseAbstractResponse:
+              show_request: bool = False, guardrail: Guardrails = None) -> BaseAbstractResponse:
         """
         invokes a model_id and returns the response.  Non-streaming only.
         request may by one of: a prompt, a json string represent the request schema, or a dict representing the request schema
         invoking with a request of a string containing valid json data, if it is not a valid json schema for the model
         it will be interpreted as a prompt string and a runtime warning will be raised
         :param model_id: the model id you wish to invoke
         :param request: a string or dict representing either a prompt or a model request schema
+        :param: guardrail: Optional instance of a basicbedrock.guardrails.Guardrails class. If present, it will utilize the guardrail within it.
         :param show_request: prints the request blob before invoking
         :return: the response to the request, as a subclass of a model.BaseAbstractResponse
         """
-
+        if model_id not in BasicBedrock.get_supported_models():
+            raise ValueError(f"requested model {model_id} is not an available model in BasicBedrock")
         if not isinstance(request, dict) and not isinstance(request, str):
             raise TypeError(f"request must be a string, or a json dict representing the request schema for the model, "
                             f"found: {type(request)}")
         schema_obj: BaseAbstractRequest = model_request_mapping.get(model_id)
         if schema_obj is None:
             raise ValueError(f"requested model {model_id} is not an available model")
+        if guardrail is not None and not isinstance(guardrail, Guardrails):
+            raise ValueError(f"object provided for guardrail parameter is a {type(guardrail)} but expected is a Guardrail or None")
+        if guardrail is not None:
+            if not guardrail.content_configuration and not guardrail.topic_configuration:
+                warnings.warn(f"Empty guardrails provided for invoking model {model_id}, ignoring it")
+                guardrail = None
+            if not guardrail.guardrail_id:
+                warnings.warn(f"Passed a guardrail to invoke() but guardrails not yet installed.  "
+                              f"Installing now (remember to call uninstall_guardrails() afterwards to remove the guardrail from your account")
+                guardrail.install_guardrails()
         schema_inst = None
         if isinstance(request, dict):
             # infer if the request is valid
             try:
                 schema_inst = schema_obj.parse_obj(request)
             except pydantic.ValidationError:
                 schema_inst = schema_obj()
@@ -226,14 +242,19 @@
             schema_inst.set_prompt(request)
         schema_inst.set_params(self.params)
         body = schema_inst.json()
         full_request = {
             "modelId": model_id,
             "body": body
         }
+        if guardrail is not None:
+            full_request.update({
+                "guardrailIdentifier": guardrail.guardrail_id,
+                "guardrailVersion": guardrail.guardrail_version,
+            })
         if show_request:
             print(json.dumps(full_request))
         r = self.client.invoke_model(**full_request)
         if r['ResponseMetadata']['HTTPStatusCode'] != 200:
             error = r.get('Error')
             code = error.get('Code')
             message = error.get('Message')
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock/models/ai21.py` & `basicbedrock-0.2.0/src/basicbedrock/models/ai21.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from .baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
+AI21_JURASSIC2_CONTEXT_WINDOW = 8_000
+AI21_JURASSIC2_MAX_OUTPUT = 8_191
 
 class AI21Jurassic2BaseRequest(BaseAbstractRequest):
     """
     AI21 Jurassic 2 request format.
     This model supports max_token, temperature and top_p, stop_sequences, count_penalty, presence_penalty and frequncy_penalty
     it does not support top_k
     as of right now there is no BasicBedrock support for penalty parameters
@@ -26,14 +28,15 @@
         Update the prompt based on the input text.
         inserts text according to expected request conventions.
         :param text:
         :return:
         """
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
+        input_text = input_text[:AI21_JURASSIC2_CONTEXT_WINDOW]
         self.set_prompt_raw(input_text)
 
     def set_prompt_raw(self, text):
         """
         Update the prompt based on the input text without regards to expected input format
         what you insert, is inserted raw without formatting
         :param text:
@@ -79,15 +82,15 @@
 
     def set_max_tokens(self, max_tokens: int):
         """
         set the maximum tokens parameter.
         :param max_tokens:
         :return:
         """
-        self.maxTokens = max_tokens
+        self.maxTokens = min(max_tokens, AI21_JURASSIC2_MAX_OUTPUT)
 
 
 class AI21Jurassic2BaseResponse(BaseAbstractResponse):
     """
     All AI21 Jurassic 2 models use the same response format.
     """
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock/models/amazon.py` & `basicbedrock-0.2.0/src/basicbedrock/models/amazon.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 """
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 from .baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
+AMAZON_TITAN_G1_LITE_CONTEXT_WINDOW = 4_000
+AMAZON_TITAN_G1_EXPRESS_CONTEXT_WINDOW = 8_000
+AMAZON_TITAN_TEXT_MAX_OUTPUT = 8_000
 
 class AmazonTitanTextGenerationConfig(BaseModel):
     """
     Stub class for the configuration blob included as part of requests to Amazon Titan family models.
     the available hyperparameters are kept internally here and include P, temperate and max_tokens
     this model does not support K values.
     """
@@ -26,42 +29,18 @@
     This base class is used by both Amazon Titan Text G1 Express and Titan Text v1 Lite
     This model does not support top_k parameter.
     """
     inputText: str = "{PROMPT}"
     textGenerationConfig: AmazonTitanTextGenerationConfig = AmazonTitanTextGenerationConfig()
 
     def set_prompt(self, text):
-        input_text = "{PROMPT}"
-        input_text = input_text.format(PROMPT=text)
-        self.set_prompt_raw(input_text)
-
-    def set_prompt_raw(self, text):
-        self.inputText = text
-
-    def set_stop_words(self, stop_words: List[str]):
-        """
-        https://docs.aws.amazon.com/bedrock/latest/userguide/model-parameters-titan-text.html#model-parameters-titan-request-response
-        Only valid stop words are "|", "User:" or none at all
-        If no valid stop words are passed, the default of [] is used
-        If a valid stop word is present in the list, the first one will be used
-        :param stop_words:
-        :return:
-        """
-        if not stop_words:
-            self.textGenerationConfig.stopSequences = []
-        else:
-            # titan only accepts a single stop word.  and, it only accepts '| and 'User:' as a valid stop word
-            # I want to ensure that if a valid stop word is given, we use the first one.
-            # if no valid stop words are given, we wont use any
-            if '|' not in stop_words and 'User:' not in stop_words:
-                self.textGenerationConfig.stopSequences = []
-            for word in stop_words:
-                if word in ('|', 'User:'):
-                    self.textGenerationConfig.stopSequences = [word]
+        pass
 
+    def set_prompt_raw(self, input_text):
+        pass
 
     def set_k(self, top_k: int):
         """
         Top K is not supported by Amazon Titan model family.  This method does nothing.
         :param top_k: int
         :return:
         """
@@ -77,36 +56,79 @@
 
     def set_max_tokens(self, max_tokens: int):
         """
         sets max token output of Amazon Titan model family
         :param max_tokens: int
         :return:
         """
-        self.textGenerationConfig.maxTokenCount = max_tokens
+        self.textGenerationConfig.maxTokenCount = min(max_tokens,AMAZON_TITAN_TEXT_MAX_OUTPUT)
 
     def set_p(self, top_p: float):
         """
         Sets top p of Amazon Titan model family
         :param top_p: float
         :return:
         """
         self.textGenerationConfig.topP = top_p
 
+    def set_stop_words(self, stop_words: List[str]):
+        """
+        https://docs.aws.amazon.com/bedrock/latest/userguide/model-parameters-titan-text.html#model-parameters-titan-request-response
+        Only valid stop words are "|", "User:" or none at all
+        If no valid stop words are passed, the default of [] is used
+        If a valid stop word is present in the list, the first one will be used
+        :param stop_words:
+        :return:
+        """
+        if not stop_words:
+            self.textGenerationConfig.stopSequences = []
+        else:
+            # titan only accepts a single stop word.  and, it only accepts '| and 'User:' as a valid stop word
+            # I want to ensure that if a valid stop word is given, we use the first one.
+            # if no valid stop words are given, we wont use any
+            if '|' not in stop_words and 'User:' not in stop_words:
+                self.textGenerationConfig.stopSequences = []
+            for word in stop_words:
+                if word in ('|', 'User:'):
+                    self.textGenerationConfig.stopSequences = [word]
+
+
+class AmazonTitanTextG1LiteRequest(AmazonTitanTextV1Request):
+
+    def set_prompt(self, text):
+        input_text = "{PROMPT}"
+        input_text = input_text.format(PROMPT=text)
+        input_text = input_text[:AMAZON_TITAN_G1_LITE_CONTEXT_WINDOW]
+        self.set_prompt_raw(input_text)
+
+    def set_prompt_raw(self, text):
+        self.inputText = text
+
+
+class AmazonTitanTextG1ExpressRequest(AmazonTitanTextV1Request):
+
+    def set_prompt(self, text):
+        input_text = "{PROMPT}"
+        input_text = input_text.format(PROMPT=text)
+        input_text = input_text[:AMAZON_TITAN_G1_EXPRESS_CONTEXT_WINDOW]
+        self.set_prompt_raw(input_text)
+
+    def set_prompt_raw(self, text):
+        self.inputText = text
 
 
 class AmazonTitanTextV1Response(BaseAbstractResponse):
     """
     Response structure for Amazon Titan Text V1 API both Express and Lite
     """
 
     def get_answer(self) -> List[float]:
         return self.result_raw['results'][0]['outputText']
 
 
-
 class AmazonTitanEmbedTextV1Request(BaseAbstractRequest):
     """
     Request structure for Amazon Titan Embedding V1 API
     This model accepts text and returns a list of floats, representing Amazon Titan embedding vectors.
     """
     inputText: str = "{PROMPT}"
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.2.0/src/basicbedrock/models/anthropic.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from typing import List
 
 from pydantic import BaseModel
 
 from baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
+ANTHROPIC_CLAUDE_V1V2_CONTEXT_WINDOW = 100_000 - 1
+ANTHROPIC_CLAUDE_V3_CONTEXT_WINDOW = 200_000 - 1
+ANTHROPIC_CLAUDE_MAX_OUTPUT = 4_096
+
+
 class AnthropicClaudeV1V2BaseRequest(BaseAbstractRequest):
     """
     Claude V1 and V2 family models all utilize the same request/response format
     This handles all the logic for them
     this model supports temp, top_k, top_p, stop sequences and max_tokens
     """
     prompt: str = "\n\nHuman: {PROMPT}\n\nAssistant:"
@@ -20,15 +25,18 @@
     temperature: float = 0.5
     top_k: int = 125
     top_p: float = 0.5
     stop_sequences: list = ["\n\nHuman:"]
     anthropic_version: str = "bedrock-2023-05-31"
 
     def set_prompt(self, text):
-        prompt = f"\n\nHuman: {text}\n\nAssistant:"
+        prompt = "\n\nHuman: {PROMPT}\n\nAssistant:"
+        padding = len(prompt.replace("{PROMPT}",""))
+        cut_text = text[:ANTHROPIC_CLAUDE_V1V2_CONTEXT_WINDOW-padding]
+        prompt = prompt.format(PROMPT=cut_text)
         self.set_prompt_raw(prompt)
 
     def set_prompt_raw(self, text):
         self.prompt = text
 
     def set_stop_words(self, stop_sequences: List[str]):
         """
@@ -44,42 +52,44 @@
     def set_k(self, top_k: int):
         self.top_k = top_k
 
     def set_temp(self, temp: float):
         self.temperature = temp
 
     def set_max_tokens(self, max_tokens: int):
-        self.max_tokens_to_sample = max_tokens
+        self.max_tokens_to_sample = min(max_tokens, ANTHROPIC_CLAUDE_MAX_OUTPUT)
 
 
 class AnthropicClaudeV1V2BaseResponse(BaseAbstractResponse):
     """
     Claude V1 and V2 family models all utilize the same response/response format
     Every Calude V1 and V2 model response will inherit this class
     """
 
     def get_answer(self) -> List[float]:
         return self.result_raw['completion']
 
 
-
 class AntropicClaude3MessageContent(BaseModel):
     """
     Stub class for the Antropic Claude V3 message content field.
     it contains information about the content of the input (is it text or image) as well as the input itself
     """
     type: str = "text"
     text: str = '\n\nHuman: {PROMPT}\n\nAssistant:'
 
     def update_prompt(self, text):
-        text = f'\n\nHuman: {text}\n\nAssistant:'
-        self.update_prompt_raw(text)
+        prompt = "\n\nHuman: {PROMPT}\n\nAssistant:"
+        padding = len(prompt.replace("{PROMPT}",""))
+        cut_text = text[:ANTHROPIC_CLAUDE_V1V2_CONTEXT_WINDOW-padding]
+        prompt = prompt.format(PROMPT=cut_text)
+        self.update_prompt_raw(prompt)
 
     def update_prompt_raw(self, text):
-        self.text = text
+        self.text = text[:ANTHROPIC_CLAUDE_V3_CONTEXT_WINDOW]
 
 
 class AntropicClaude3Message(BaseModel):
     """
     Stub class for the Antropic Claude V3 message content field.
     this contains metadata about the request, such as the role, as well as a list of AntropicClaude3MessageContent classes
     """
@@ -127,20 +137,18 @@
     def set_k(self, top_k: int):
         self.top_k = top_k
 
     def set_temp(self, temp: float):
         self.temperature = temp
 
     def set_max_tokens(self, max_tokens: int):
-        self.max_tokens = max_tokens
+        self.max_tokens = min(max_tokens, ANTHROPIC_CLAUDE_MAX_OUTPUT)
 
 
 class AnthropicClaude3BaseResponse(BaseAbstractResponse):
     """
     This class represents the response format used by Anthropic Claude V3 family of models
     Both Haiku and Sonnet use this response format.
     """
 
     def get_answer(self) -> List[float]:
         return self.result_raw['content'][0]['text']
-
-
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.2.0/src/basicbedrock/models/baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.1.9/src/basicbedrock/models/cohere.py` & `basicbedrock-0.2.0/src/basicbedrock/models/mistral.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,81 @@
 """
-File containing all of the definitions and implementations for the Cohere family of requests and responses.
+File containing all of the definitions and implementations for the Mistral family of requests and responses.
 """
 import typing
-from typing import List
 
-from baseclasses import BaseAbstractRequest, BaseAbstractResponse
+from .baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
+MISTRAL_CONTEXT_WINDOW = 32_000 - 1
+MISTRAL_7B_INSTRUCT_MAX_OUTPUT = 8_192
+MISTRAL_8X7B_INSTRUCT_MAX_OUTPUT = 4_096
+MISTRAL_LARGE_MAX_OUTPUT = 4_096  # docs claim its 8_192 but this is apparently not true, it fails boto3 validation
 
-class CohereCommandTextBaseRequest(BaseAbstractRequest):
+
+class MistralBaseRequest(BaseAbstractRequest):
     """
-    This is the base request format that all Cohere text-family models use
-    These models support top_p, top_k, max_tokens and temperature.
+    Base request for Mistral family of models.
+    this mnodel supports temperature, top_p, top_k and max_tokens
     """
-    prompt: str = "{PROMPT}"
+    prompt: str = "<s>[INST] {PROMPT} [/INST]"
     max_tokens: int = 250
     temperature: float = 0.5
-    p: float = 0.5
-    k: int = 125
-    stop_sequences: List[str] = []
+    top_p: float = 0.5
+    top_k: int = 125
+    stop: typing.List[str] = []
 
     def set_prompt(self, text):
-        input_text = "{PROMPT}"
-        input_text = input_text.format(PROMPT=text)
-        self.set_prompt_raw(input_text)
+        prompt = "<s>[INST] {PROMPT} [/INST]"
+        padding = len(prompt.replace("{PROMPT}",""))
+        cut_text = text[:MISTRAL_CONTEXT_WINDOW-padding]
+        prompt = prompt.format(PROMPT=cut_text)
+        self.set_prompt_raw(prompt)
 
     def set_prompt_raw(self, text):
         self.prompt = text
 
     def set_stop_words(self, stop_words: typing.List[str]):
         """
-        Cohere seems to accept any number of stop words
+        Mistral models seem to accept any number of stop words in any format
         :param stop_words:
         :return:
         """
-        self.stop_sequences = stop_words
+        self.stop = stop_words
 
     def set_p(self, top_p: float):
-        self.p = top_p
+        self.top_p = top_p
 
     def set_k(self, top_k: int):
-        self.k = top_k
+        self.top_k = top_k
 
     def set_temp(self, temp: float):
         self.temperature = temp
 
-    def set_max_tokens(self, max_tokens: int):
-        self.max_tokens = max_tokens
-
-
-
-class CohereCommandTextBaseResponse(BaseAbstractResponse):
-    """
-    this is the base response format used by all text-family cohere models
-    """
-
-    def get_answer(self) -> str:
-        return self.result_raw['generations'][0]['text']
-
-
-"""
-Cohere Embed English V3
-"""
+    def set_max_tokens(self, top_p: float):
+        pass
 
 
-class CohereEmbedBaseRequest(BaseAbstractRequest):
-    """
-    All cohere command models use the same request format.
-    Models support input text only.
-    """
-    texts: List[str] = ["{PROMPT}"]
-    input_type: str = "search_document"
+class Mistral7BInstructRequest(MistralBaseRequest):
 
-    def set_prompt(self, text):
-        input_text = "{PROMPT}"
-        input_text = input_text.format(PROMPT=text)
-        texts = [input_text]
-        self.set_prompt_raw(texts)
+    def set_max_tokens(self, max_tokens: int):
+        self.max_tokens = min(max_tokens, MISTRAL_7B_INSTRUCT_MAX_OUTPUT)
 
-    def set_prompt_raw(self, texts: list):
-        self.texts = texts
 
-    def set_stop_words(self, stop_words: typing.List[str]):
-        pass
+class Mistral8X7BInstructRequest(MistralBaseRequest):
 
-    def set_p(self, top_p: float):
-        """
-        Cohere Embed V3 does not support top_p
-        :param top_p:
-        :return:
-        """
-        pass
+    def set_max_tokens(self, max_tokens: int):
+        self.max_tokens = min(max_tokens, MISTRAL_8X7B_INSTRUCT_MAX_OUTPUT)
 
-    def set_k(self, top_k: int):
-        """
-        Cohere Embed V3 does not support top_k
-        :param top_k:
-        :return:
-        """
-        pass
 
-    def set_temp(self, temp: float):
-        """
-        Cohere Embed V3 does not support temperature
-        :param temp:
-        :return:
-        """
-        pass
+class MistralLargeRequest(MistralBaseRequest):
 
     def set_max_tokens(self, max_tokens: int):
-        """
-        Cohere Embed V3 does not support max_tokens
-        :param max_tokens:
-        :return:
-        """
-        pass
+        self.max_tokens = min(max_tokens, MISTRAL_LARGE_MAX_OUTPUT)
 
 
-class CohereEmbedBaseResponse(BaseAbstractResponse):
+class MistralBaseResponse(BaseAbstractResponse):
     """
-    All Cohere Embed models use the same response format.
+    Base response format for Mistral Instruct family of models.
     """
 
-    def get_answer(self) -> List[float]:
-        return self.result_raw['embeddings'][0]
+    def get_answer(self) -> str:
+        return self.result_raw['outputs'][0]['text']
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock/models/meta.py` & `basicbedrock-0.2.0/src/basicbedrock/models/meta.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 Amazon docs currently do not have request schemas for Llama 2 13b and Llama 2 70b, only the chat versions
 """
 import typing
 
 from baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 
+META_LLAMA_V2_CONTEXT_WINDOW = 4_000
+META_LLAMA_V3_CONTEXT_WINDOW = 8_000
+META_LLAMA_V2V3_MAX_OUTPUT = 2_048
+
+
 class MetaLlamaBaseRequest(BaseAbstractRequest):
     """
     This model supports max_token, temperature and top_p.
     It does not support top_k
     """
+
     max_gen_len: int = 250
     temperature: float = 0.5
     top_p: float = 0.5
 
 
-    def set_prompt_raw(self, text):
-        """
-        Update the prompt based on the input text without regards to expected input format
-        what you insert, is inserted raw without formatting
-        :param text:
-        :return:
-        """
-        self.prompt = text
-
     def set_stop_words(self, stop_words: typing.List[str]):
         """
         Meta Llama 2 models dont support stop words
         :param stop_words:
         :return:
         """
         pass
@@ -60,15 +57,21 @@
 
     def set_max_tokens(self, max_tokens: int):
         """
         set the maximum tokens parameter.
         :param max_tokens:
         :return:
         """
-        self.max_gen_len = max_tokens
+        self.max_gen_len = min(max_tokens, META_LLAMA_V2V3_MAX_OUTPUT)
+
+    def set_prompt(self, text: str):
+        pass
+
+    def set_prompt_raw(self, text: str):
+        pass
 
 
 class MetaLlamaV2V3BaseResponse(BaseAbstractResponse):
     """
     Response format of Meta Llama 2 V1 family chat response.
     """
 
@@ -78,43 +81,53 @@
 
 class MetaLlamaV2BaseRequest(MetaLlamaBaseRequest):
     """
     Specifies the expected Llama 2 V1 family chat request format using the [INST] tags
     """
     prompt: str = "<s>[INST]{PROMPT}[/INST]"
 
-
     def set_prompt(self, text):
+        prompt = "<s>[INST]{PROMPT}[/INST]"
+        padding = len(prompt.replace("{PROMPT}",""))
+        cut_text = text[:META_LLAMA_V2_CONTEXT_WINDOW-padding]
+        prompt = prompt.format(PROMPT=cut_text)
+        self.set_prompt_raw(prompt)
+
+
+    def set_prompt_raw(self, text):
         """
-        Update the prompt based on the input text.
-        inserts text according to expected request conventions.
+        Update the prompt based on the input text without regards to expected input format
+        what you insert, is inserted raw without formatting
         :param text:
         :return:
         """
-        input_text = "<s>[INST]{PROMPT}[/INST]"
-        input_text = input_text.format(PROMPT=text)
-        self.set_prompt_raw(input_text)
+        self.prompt = text
 
 class MetaLlamaV3BaseRequest(MetaLlamaBaseRequest):
     """
     Specifies the expected Llama 2 V1 family chat request format using the expected header format
     """
     prompt: str = (
         '<|begin_of_text|><|start_header_id|>user<|end_header_id|>\n'
         '\n'
         '{PROMPT}<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n'
     )
 
     def set_prompt(self, text):
-        """
-        Update the prompt based on the input text.
-        inserts text according to expected request conventions.
-        :param text:
-        :return:
-        """
-        input_text = str(
+        prompt = str(
             "<|begin_of_text|><|start_header_id|>user<|end_header_id|>\n"
             "\n"
             "{PROMPT}<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n"
         )
-        input_text = input_text.format(PROMPT=text)
-        self.set_prompt_raw(input_text)
+        padding = len(prompt.replace("{PROMPT}",""))
+        cut_text = text[:META_LLAMA_V3_CONTEXT_WINDOW-padding]
+        prompt = prompt.format(PROMPT=cut_text)
+        self.set_prompt_raw(prompt)
+
+    def set_prompt_raw(self, text):
+        """
+        Update the prompt based on the input text without regards to expected input format
+        what you insert, is inserted raw without formatting
+        :param text:
+        :return:
+        """
+        self.prompt = text
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.2.0/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.1.9
+Version: 0.2.0
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -18,15 +18,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3>=1.34.79
+Requires-Dist: boto3>=1.34.94
 Requires-Dist: pydantic>=2.6.4
 
 # BasicBedrock
 AWS Bedrock provides a variety of foundational models to AWS customers.  Each model family requires their own request structure, yet the underlying semantics are roughly common; there is always a field for the textual input prompt, and often there are fields to define maximum desired output, stop words, P, K and Temperature values.
 
 This package aims to abstract away all of that.
```

### Comparing `basicbedrock-0.1.9/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.2.0/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 README.md
 pyproject.toml
 src/basicbedrock/__init__.py
 src/basicbedrock/basicbedrock.py
+src/basicbedrock/guardrails.py
+src/basicbedrock/guardrails_baseclasses.py
 src/basicbedrock.egg-info/PKG-INFO
 src/basicbedrock.egg-info/SOURCES.txt
 src/basicbedrock.egg-info/dependency_links.txt
 src/basicbedrock.egg-info/requires.txt
 src/basicbedrock.egg-info/top_level.txt
 src/basicbedrock/models/__init__.py
 src/basicbedrock/models/ai21.py
 src/basicbedrock/models/amazon.py
 src/basicbedrock/models/anthropic.py
 src/basicbedrock/models/baseclasses.py
 src/basicbedrock/models/cohere.py
 src/basicbedrock/models/meta.py
 src/basicbedrock/models/mistral.py
-test/tests.py
+test/test_basicbedrock.py
```

### Comparing `basicbedrock-0.1.9/test/tests.py` & `basicbedrock-0.2.0/test/test_basicbedrock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,44 @@
-import sys
-import os
+from random import choice
 import json
 import boto3
 
-sys.path.append(os.path.abspath('../src/basicbedrock'))
-from basicbedrock import BasicBedrock
+from basicbedrock import *
+
+
+def test_content_policy():
+    gr = Guardrails()
+    gr.add_content_filter("SEXUAL","HIGH","HIGH")
+    gr.install_guardrails()
+    model = choice([model for model in bb.get_available_models() if "embed" not in model])
+    r = bb.invoke(model,"write a lewd story",guardrail=gr)
+    print(r.get_answer())
+    gr.uninstall_guardrails()
+
+
+def test_filter_policy(bb: BasicBedrock):
+    gr = Guardrails()
+    gr.add_topic_filter(definition="Conversation related to politics", examples=[
+        "Jane Doe is a great president!",
+        "Randy Randolph is the better presidential candidate ",
+        "the House of Lords and the House of Commons ",
+        "This election season will be a great match up between political parties"
+    ])
+    gr.install_guardrails()
+    model = choice([model for model in bb.get_available_models() if "embed" not in model])
+    r = bb.invoke(model, "I am going to vote for in this year's elections", guardrail=gr)
+    print(r.get_answer())
+    gr.uninstall_guardrails()
+
+
+def test_no_guardrail(bb: BasicBedrock):
+    bb = BasicBedrock()
+    model = choice([model for model in bb.get_available_models() if "embed" not in model])
+    r = bb.invoke(model, "simple test", guardrail=None)
+    print(r.get_answer())
 
 
 def test_invoke_with_string(bb, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with string")
@@ -106,20 +136,48 @@
     prompt = "Hittem hard with dem params doe"
     for model in bb.get_available_models():
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
 
 
+def test_context_window_limits(bb, verbose=False):
+    for model_id,ctxt in model_request_context_windows.items():
+        if not ctxt:  # embeds have no max
+            continue
+        print(f"now testing {model_id} test_context_window_limits")
+        prompt = "My name is the real slim shady" * ctxt
+        r = bb.invoke(model_id, prompt, show_request=verbose)
+
+
+def test_max_tokens(bb, verbose=False):
+    for model_id,max_token in model_request_max_outputs.items():
+        if not max_token:  # embeds have no max
+            continue
+        print(f"now testing {model_id} test_max_tokens")
+        params = {
+            "max_tokens": max_token,
+        }
+        print(params)
+        prompt = "this is a test"
+        bb.params = params
+        r = bb.invoke(model_id, prompt, show_request=verbose)
+
+
 if __name__ == "__main__":
-    verbose = True
+    verbose = False
     session = boto3.session.Session(profile_name='default')
     bb = BasicBedrock(session=session)
     single_run(bb, verbose)
+    test_no_guardrail()
+    test_content_policy()
+    test_filter_policy()
     test_invoke_with_string(bb, verbose=verbose)
     test_get_boto3_body(bb, sess=session, verbose=verbose)
     test_set_params(bb, verbose=verbose)
     test_invoke_with_invalid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_dict(bb, verbose=verbose)
     test_invoke_with_invalid_dict(bb, verbose=verbose)
+    test_context_window_limits(bb,verbose=verbose)
+    test_max_tokens(bb,verbose=verbose)
     print("All tests successful")
```

