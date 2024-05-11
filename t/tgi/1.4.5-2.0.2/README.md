# Comparing `tmp/tgi-1.4.5.tar.gz` & `tmp/tgi-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgi-1.4.5.tar", max compression
+gzip compressed data, was "tgi-2.0.2.tar", max compression
```

## Comparing `tgi-1.4.5.tar` & `tgi-2.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7589 2024-03-26 09:03:37.869972 tgi-1.4.5/README.md
--rw-r--r--   0        0        0      780 2024-04-04 18:46:14.593003 tgi-1.4.5/pyproject.toml
--rw-r--r--   0        0        0      771 2024-03-26 09:33:59.622830 tgi-1.4.5/tgi/__init__.py
--rw-r--r--   0        0        0    31577 2024-03-26 09:33:59.622993 tgi-1.4.5/tgi/client.py
--rw-r--r--   0        0        0     2839 2024-03-26 09:33:59.623166 tgi-1.4.5/tgi/errors.py
--rw-r--r--   0        0        0     5579 2024-03-26 09:33:59.623307 tgi-1.4.5/tgi/inference_api.py
--rw-r--r--   0        0        0    12548 2024-03-26 09:33:59.623455 tgi-1.4.5/tgi/types.py
--rw-r--r--   0        0        0     8602 1970-01-01 00:00:00.000000 tgi-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     7589 2024-03-26 09:03:37.869972 tgi-2.0.2/README.md
+-rw-r--r--   0        0        0      780 2024-05-11 15:11:50.006499 tgi-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      771 2024-04-05 15:22:16.757115 tgi-2.0.2/tgi/__init__.py
+-rw-r--r--   0        0        0    31917 2024-05-11 15:08:02.473804 tgi-2.0.2/tgi/client.py
+-rw-r--r--   0        0        0     2839 2024-04-05 15:22:16.758057 tgi-2.0.2/tgi/errors.py
+-rw-r--r--   0        0        0     5579 2024-04-05 15:22:16.758212 tgi-2.0.2/tgi/inference_api.py
+-rw-r--r--   0        0        0    13095 2024-05-11 15:08:02.474285 tgi-2.0.2/tgi/types.py
+-rw-r--r--   0        0        0     8602 1970-01-01 00:00:00.000000 tgi-2.0.2/PKG-INFO
```

### Comparing `tgi-1.4.5/README.md` & `tgi-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tgi-1.4.5/pyproject.toml` & `tgi-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgi"
-version = "1.4.5"
+version = "2.0.2"
 description = "Nightly release of Hugging Face Text Generation Python Client"
 license = "Apache-2.0"
 authors = ["Maziyar PANAHI <maziyar.panahi@cnrs.fr>"]
 maintainers = ["Maziyar PANAHI <maziyar.panahi@cnrs.fr>"]
 readme = "README.md"
 homepage = "https://github.com/huggingface/text-generation-inference"
 repository = "https://github.com/huggingface/text-generation-inference"
```

### Comparing `tgi-1.4.5/tgi/__init__.py` & `tgi-2.0.2/tgi/__init__.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.5/tgi/client.py` & `tgi-2.0.2/tgi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         n: Optional[int] = None,
         presence_penalty: Optional[float] = None,
         stream: bool = False,
         seed: Optional[int] = None,
         temperature: Optional[float] = None,
         top_p: Optional[float] = None,
         tools: Optional[List[Tool]] = None,
+        tool_prompt: Optional[str] = None,
         tool_choice: Optional[str] = None,
     ):
         """
         Given a list of messages, generate a response asynchronously
 
         Args:
             messages (`List[Message]`):
@@ -115,14 +116,16 @@
             temperature (`float`):
                 The value used to module the logits distribution.
             top_p (`float`):
                 If set to < 1, only the smallest set of most probable tokens with probabilities that add up to `top_p` or
                 higher are kept for generation
             tools (`List[Tool]`):
                 List of tools to use
+            tool_prompt (`str`):
+                A prompt to be appended before the tools
             tool_choice (`str`):
                 The tool to use
 
         """
         request = ChatRequest(
             model="tgi",
             messages=messages,
@@ -135,14 +138,15 @@
             n=n,
             presence_penalty=presence_penalty,
             stream=stream,
             seed=seed,
             temperature=temperature,
             top_p=top_p,
             tools=tools,
+            tool_prompt=tool_prompt,
             tool_choice=tool_choice,
         )
         if not stream:
             resp = requests.post(
                 f"{self.base_url}/v1/chat/completions",
                 json=request.dict(),
                 headers=self.headers,
@@ -462,14 +466,15 @@
         n: Optional[int] = None,
         presence_penalty: Optional[float] = None,
         stream: bool = False,
         seed: Optional[int] = None,
         temperature: Optional[float] = None,
         top_p: Optional[float] = None,
         tools: Optional[List[Tool]] = None,
+        tool_prompt: Optional[str] = None,
         tool_choice: Optional[str] = None,
     ) -> Union[ChatComplete, AsyncIterator[ChatCompletionChunk]]:
         """
         Given a list of messages, generate a response asynchronously
 
         Args:
             messages (`List[Message]`):
@@ -501,14 +506,16 @@
             temperature (`float`):
                 The value used to module the logits distribution.
             top_p (`float`):
                 If set to < 1, only the smallest set of most probable tokens with probabilities that add up to `top_p` or
                 higher are kept for generation
             tools (`List[Tool]`):
                 List of tools to use
+            tool_prompt (`str`):
+                A prompt to be appended before the tools
             tool_choice (`str`):
                 The tool to use
 
         """
         request = ChatRequest(
             model="tgi",
             messages=messages,
@@ -521,14 +528,15 @@
             n=n,
             presence_penalty=presence_penalty,
             stream=stream,
             seed=seed,
             temperature=temperature,
             top_p=top_p,
             tools=tools,
+            tool_prompt=tool_prompt,
             tool_choice=tool_choice,
         )
         if not stream:
             return await self._chat_single_response(request)
         else:
             return self._chat_stream_response(request)
```

### Comparing `tgi-1.4.5/tgi/errors.py` & `tgi-2.0.2/tgi/errors.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.5/tgi/inference_api.py` & `tgi-2.0.2/tgi/inference_api.py`

 * *Files identical despite different names*

### Comparing `tgi-1.4.5/tgi/types.py` & `tgi-2.0.2/tgi/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,25 @@
     logprobs: Optional[Any]
     # Reason for completion
     finish_reason: str
     # Usage details of the chat completion
     usage: Optional[Any] = None
 
 
+class CompletionComplete(BaseModel):
+    # Index of the chat completion
+    index: int
+    # Message associated with the chat completion
+    text: str
+    # Log probabilities for the chat completion
+    logprobs: Optional[Any]
+    # Reason for completion
+    finish_reason: str
+
+
 class Function(BaseModel):
     name: Optional[str]
     arguments: str
 
 
 class ChoiceDeltaToolCall(BaseModel):
     index: int
@@ -100,14 +111,24 @@
     created: int
     model: str
     system_fingerprint: str
     choices: List[ChatCompletionComplete]
     usage: Any
 
 
+class Completion(BaseModel):
+    # Completion details
+    id: str
+    object: str
+    created: int
+    model: str
+    system_fingerprint: str
+    choices: List[CompletionComplete]
+
+
 class ChatRequest(BaseModel):
     # Model identifier
     model: str
     # List of messages in the conversation
     messages: List[Message]
     # The parameter for repetition penalty. 1.0 means no penalty.
     # See [this paper](https://arxiv.org/pdf/1909.05858.pdf) for more details.
@@ -134,14 +155,16 @@
     seed: Optional[int] = None
     # Sampling temperature
     temperature: Optional[float] = None
     # Top-p value for nucleus sampling
     top_p: Optional[float] = None
     # List of tools to be used
     tools: Optional[List[Tool]] = None
+    # A prompt to be appended before the tools
+    tool_prompt: Optional[str] = None
     # Choice of tool to be used
     tool_choice: Optional[str] = None
 
 
 class Parameters(BaseModel):
     # Activate logits sampling
     do_sample: bool = False
```

### Comparing `tgi-1.4.5/PKG-INFO` & `tgi-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgi
-Version: 1.4.5
+Version: 2.0.2
 Summary: Nightly release of Hugging Face Text Generation Python Client
 Home-page: https://github.com/huggingface/text-generation-inference
 License: Apache-2.0
 Author: Maziyar PANAHI
 Author-email: maziyar.panahi@cnrs.fr
 Maintainer: Maziyar PANAHI
 Maintainer-email: maziyar.panahi@cnrs.fr
```

