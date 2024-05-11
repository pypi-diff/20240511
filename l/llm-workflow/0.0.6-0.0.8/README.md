# Comparing `tmp/llm-workflow-0.0.6.tar.gz` & `tmp/llm-workflow-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-workflow-0.0.6.tar", last modified: Mon Oct 16 00:33:12 2023, max compression
+gzip compressed data, was "llm-workflow-0.0.8.tar", last modified: Thu Nov  9 21:57:29 2023, max compression
```

## Comparing `llm-workflow-0.0.6.tar` & `llm-workflow-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:12.548710 llm-workflow-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-workflow-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    22987 2023-10-16 00:33:12.548324 llm-workflow-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    22269 2023-10-15 18:33:43.000000 llm-workflow-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:12.526517 llm-workflow-0.0.6/llm_workflow/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-workflow-0.0.6/llm_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11103 2023-10-14 23:21:00.000000 llm-workflow-0.0.6/llm_workflow/agents.py
--rw-r--r--   0 root         (0) root         (0)    24280 2023-10-15 18:24:43.000000 llm-workflow-0.0.6/llm_workflow/base.py
--rw-r--r--   0 root         (0) root         (0)    21049 2023-10-08 23:50:42.000000 llm-workflow-0.0.6/llm_workflow/compare.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-07-12 04:20:15.000000 llm-workflow-0.0.6/llm_workflow/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8604 2023-10-15 00:27:52.000000 llm-workflow-0.0.6/llm_workflow/hugging_face.py
--rw-r--r--   0 root         (0) root         (0)     7951 2023-10-08 23:50:42.000000 llm-workflow-0.0.6/llm_workflow/indexes.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-10-04 03:32:56.000000 llm-workflow-0.0.6/llm_workflow/internal_utilities.py
--rw-r--r--   0 root         (0) root         (0)     9314 2023-10-15 23:26:28.000000 llm-workflow-0.0.6/llm_workflow/memory.py
--rw-r--r--   0 root         (0) root         (0)    11834 2023-10-15 17:16:32.000000 llm-workflow-0.0.6/llm_workflow/openai.py
--rw-r--r--   0 root         (0) root         (0)     3793 2023-07-12 04:20:15.000000 llm-workflow-0.0.6/llm_workflow/prompt_templates.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-10-14 17:07:42.000000 llm-workflow-0.0.6/llm_workflow/resources.py
--rw-r--r--   0 root         (0) root         (0)    10863 2023-10-04 03:06:15.000000 llm-workflow-0.0.6/llm_workflow/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:12.531341 llm-workflow-0.0.6/llm_workflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)    22987 2023-10-16 00:33:12.000000 llm-workflow-0.0.6/llm_workflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      873 2023-10-16 00:33:12.000000 llm-workflow-0.0.6/llm_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:33:12.000000 llm-workflow-0.0.6/llm_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-10-16 00:33:12.000000 llm-workflow-0.0.6/llm_workflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-10-16 00:33:12.000000 llm-workflow-0.0.6/llm_workflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-workflow-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      707 2023-10-16 00:33:12.549441 llm-workflow-0.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:33:12.546969 llm-workflow-0.0.6/tests/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-workflow-0.0.6/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9006 2023-10-15 18:05:20.000000 llm-workflow-0.0.6/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     9434 2023-10-14 17:22:24.000000 llm-workflow-0.0.6/tests/test_agents.py
--rw-r--r--   0 root         (0) root         (0)    28258 2023-10-15 18:24:41.000000 llm-workflow-0.0.6/tests/test_base.py
--rw-r--r--   0 root         (0) root         (0)    18682 2023-10-07 17:00:34.000000 llm-workflow-0.0.6/tests/test_compare.py
--rw-r--r--   0 root         (0) root         (0)     7803 2023-10-14 17:22:15.000000 llm-workflow-0.0.6/tests/test_history.py
--rw-r--r--   0 root         (0) root         (0)    34832 2023-10-16 00:13:09.000000 llm-workflow-0.0.6/tests/test_hugging_face.py
--rw-r--r--   0 root         (0) root         (0)    11400 2023-10-01 02:45:59.000000 llm-workflow-0.0.6/tests/test_indexes.py
--rw-r--r--   0 root         (0) root         (0)    55514 2023-10-16 00:09:24.000000 llm-workflow-0.0.6/tests/test_openai.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-07-10 04:22:19.000000 llm-workflow-0.0.6/tests/test_prompt_templates.py
--rw-r--r--   0 root         (0) root         (0)     2000 2023-10-08 23:50:42.000000 llm-workflow-0.0.6/tests/test_records.py
--rw-r--r--   0 root         (0) root         (0)     8710 2023-10-14 17:22:20.000000 llm-workflow-0.0.6/tests/test_session.py
--rw-r--r--   0 root         (0) root         (0)    25779 2023-10-04 04:07:13.000000 llm-workflow-0.0.6/tests/test_utilities.py
--rw-r--r--   0 root         (0) root         (0)    27114 2023-10-15 18:19:19.000000 llm-workflow-0.0.6/tests/test_workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 21:57:29.829142 llm-workflow-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-02-25 17:02:25.000000 llm-workflow-0.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    22955 2023-11-09 21:57:29.828602 llm-workflow-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    22215 2023-11-09 03:23:33.000000 llm-workflow-0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 21:57:29.804415 llm-workflow-0.0.8/llm_workflow/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-09 17:08:19.000000 llm-workflow-0.0.8/llm_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11143 2023-11-09 03:24:41.000000 llm-workflow-0.0.8/llm_workflow/agents.py
+-rw-r--r--   0 root         (0) root         (0)    24280 2023-10-15 18:24:43.000000 llm-workflow-0.0.8/llm_workflow/base.py
+-rw-r--r--   0 root         (0) root         (0)    21333 2023-11-09 21:26:59.000000 llm-workflow-0.0.8/llm_workflow/compare.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-07-12 04:20:15.000000 llm-workflow-0.0.8/llm_workflow/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8604 2023-10-15 00:27:52.000000 llm-workflow-0.0.8/llm_workflow/hugging_face.py
+-rw-r--r--   0 root         (0) root         (0)     7951 2023-10-08 23:50:42.000000 llm-workflow-0.0.8/llm_workflow/indexes.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-10-04 03:32:56.000000 llm-workflow-0.0.8/llm_workflow/internal_utilities.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2023-10-15 23:26:28.000000 llm-workflow-0.0.8/llm_workflow/memory.py
+-rw-r--r--   0 root         (0) root         (0)    12799 2023-11-09 21:20:55.000000 llm-workflow-0.0.8/llm_workflow/openai.py
+-rw-r--r--   0 root         (0) root         (0)     3793 2023-07-12 04:20:15.000000 llm-workflow-0.0.8/llm_workflow/prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-10-14 17:07:42.000000 llm-workflow-0.0.8/llm_workflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2023-10-04 03:06:15.000000 llm-workflow-0.0.8/llm_workflow/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 21:57:29.810198 llm-workflow-0.0.8/llm_workflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    22955 2023-11-09 21:57:29.000000 llm-workflow-0.0.8/llm_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      873 2023-11-09 21:57:29.000000 llm-workflow-0.0.8/llm_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-09 21:57:29.000000 llm-workflow-0.0.8/llm_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-11-09 21:57:29.000000 llm-workflow-0.0.8/llm_workflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-11-09 21:57:29.000000 llm-workflow-0.0.8/llm_workflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-02-25 17:02:25.000000 llm-workflow-0.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      715 2023-11-09 21:57:29.829895 llm-workflow-0.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-09 21:57:29.826917 llm-workflow-0.0.8/tests/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-10 00:17:26.000000 llm-workflow-0.0.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9006 2023-10-15 18:05:20.000000 llm-workflow-0.0.8/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     9388 2023-11-09 03:28:59.000000 llm-workflow-0.0.8/tests/test_agents.py
+-rw-r--r--   0 root         (0) root         (0)    28258 2023-10-15 18:24:41.000000 llm-workflow-0.0.8/tests/test_base.py
+-rw-r--r--   0 root         (0) root         (0)    18682 2023-10-07 17:00:34.000000 llm-workflow-0.0.8/tests/test_compare.py
+-rw-r--r--   0 root         (0) root         (0)     7803 2023-10-14 17:22:15.000000 llm-workflow-0.0.8/tests/test_history.py
+-rw-r--r--   0 root         (0) root         (0)    34832 2023-10-16 00:13:09.000000 llm-workflow-0.0.8/tests/test_hugging_face.py
+-rw-r--r--   0 root         (0) root         (0)    11400 2023-10-01 02:45:59.000000 llm-workflow-0.0.8/tests/test_indexes.py
+-rw-r--r--   0 root         (0) root         (0)    54998 2023-11-09 03:48:11.000000 llm-workflow-0.0.8/tests/test_openai.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-07-10 04:22:19.000000 llm-workflow-0.0.8/tests/test_prompt_templates.py
+-rw-r--r--   0 root         (0) root         (0)     2000 2023-10-08 23:50:42.000000 llm-workflow-0.0.8/tests/test_records.py
+-rw-r--r--   0 root         (0) root         (0)     8710 2023-10-14 17:22:20.000000 llm-workflow-0.0.8/tests/test_session.py
+-rw-r--r--   0 root         (0) root         (0)    25779 2023-10-04 04:07:13.000000 llm-workflow-0.0.8/tests/test_utilities.py
+-rw-r--r--   0 root         (0) root         (0)    27114 2023-10-15 18:19:19.000000 llm-workflow-0.0.8/tests/test_workflows.py
```

### Comparing `llm-workflow-0.0.6/LICENSE` & `llm-workflow-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/PKG-INFO` & `llm-workflow-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llm-workflow
-Version: 0.0.6
+Version: 0.0.8
 Summary: build LLM workflows
 Home-page: https://github.com/shane-kercheval/llm-workflow
 Author: Shane Kercheval
 Author-email: shane.kercheval@gmail.com
 Project-URL: Bug Tracker, https://github.com/shane-kercheval/llm-workflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: joblib
 Requires-Dist: openai
 Requires-Dist: pydantic
 Requires-Dist: tenacity
 Requires-Dist: transformers
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
@@ -130,17 +131,17 @@
 - fourth task: ignores the response from the chat model; creates a new prompt asking the chat model to extract the relevant code created in the previous response
 - fifth task: the chat model, which internally maintains the history of messages, returns only the relevant code from the previous response.
 
 ```python
 from llm_workflow.base import Workflow
 from llm_workflow.openai import OpenAIChat
 
-prompt_enhancer = OpenAIChat(model_name='gpt-3.5-turbo')
+prompt_enhancer = OpenAIChat()
 # different model/object, therefore different message history (i.e. conversation)
-chat_assistant = OpenAIChat(model_name='gpt-3.5-turbo')
+chat_assistant = OpenAIChat()
 
 def prompt_template(user_prompt: str) -> str:
     return "Improve the user's request, below, by expanding the request " \
         "to describe the relevant python best practices and documentation " \
         f"requirements that should be followed:\n\n```{user_prompt}```"
 
 def prompt_extract_code(_) -> str:
@@ -340,15 +341,15 @@
 from llm_workflow.indexes import ChromaDocumentIndex
 from llm_workflow.prompt_templates import DocSearchTemplate
 
 duckduckgo_search = DuckDuckGoSearch(top_n=3)
 embeddings_model = OpenAIEmbedding(model_name='text-embedding-ada-002')
 document_index = ChromaDocumentIndex(embeddings_model=embeddings_model, n_results=3)
 prompt_template = DocSearchTemplate(doc_index=document_index, n_docs=3)
-chat_model = OpenAIChat(model_name='gpt-3.5-turbo')
+chat_model = OpenAIChat()
 
 def scrape_urls(search_results):
     """
     For each url (i.e. `href` in `search_results`):
     - extracts text
     - replace new-lines with spaces
     - create a Document object
@@ -412,20 +413,20 @@
 from llm_workflow.openai import OpenAIChat
 from llm_workflow.hugging_face import HuggingFaceEndpointChat
 from llm_workflow.compare import CompareModels, ModelDefinition
 
 # Comparing GPT-3.5 Turbo, GPT-4, and Mistral 7B
 model_definitions = [
     ModelDefinition(
-        create=lambda: OpenAIChat(model_name='gpt-3.5-turbo'),
+        create=lambda: OpenAIChat(model_name='gpt-3.5-turbo-1106'),
         description='GPT-3.5 Turbo',
     ),
     ModelDefinition(
-        create=lambda: OpenAIChat(model_name='gpt-4'),
-        description='GPT-4',
+        create=lambda: OpenAIChat(model_name='gpt-4-1106-preview'),
+        description='GPT-4 Turbo',
     ),
     ModelDefinition(
         create=lambda: HuggingFaceEndpointChat(
             endpoint_url=os.getenv('HUGGING_FACE_ENDPOINT_MISTRAL_7B'),
         ),
         description='Mistral 7B (HF Endpoint)',
     ),
```

### Comparing `llm-workflow-0.0.6/README.md` & `llm-workflow-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,17 @@
 - fourth task: ignores the response from the chat model; creates a new prompt asking the chat model to extract the relevant code created in the previous response
 - fifth task: the chat model, which internally maintains the history of messages, returns only the relevant code from the previous response.
 
 ```python
 from llm_workflow.base import Workflow
 from llm_workflow.openai import OpenAIChat
 
-prompt_enhancer = OpenAIChat(model_name='gpt-3.5-turbo')
+prompt_enhancer = OpenAIChat()
 # different model/object, therefore different message history (i.e. conversation)
-chat_assistant = OpenAIChat(model_name='gpt-3.5-turbo')
+chat_assistant = OpenAIChat()
 
 def prompt_template(user_prompt: str) -> str:
     return "Improve the user's request, below, by expanding the request " \
         "to describe the relevant python best practices and documentation " \
         f"requirements that should be followed:\n\n```{user_prompt}```"
 
 def prompt_extract_code(_) -> str:
@@ -317,15 +317,15 @@
 from llm_workflow.indexes import ChromaDocumentIndex
 from llm_workflow.prompt_templates import DocSearchTemplate
 
 duckduckgo_search = DuckDuckGoSearch(top_n=3)
 embeddings_model = OpenAIEmbedding(model_name='text-embedding-ada-002')
 document_index = ChromaDocumentIndex(embeddings_model=embeddings_model, n_results=3)
 prompt_template = DocSearchTemplate(doc_index=document_index, n_docs=3)
-chat_model = OpenAIChat(model_name='gpt-3.5-turbo')
+chat_model = OpenAIChat()
 
 def scrape_urls(search_results):
     """
     For each url (i.e. `href` in `search_results`):
     - extracts text
     - replace new-lines with spaces
     - create a Document object
@@ -389,20 +389,20 @@
 from llm_workflow.openai import OpenAIChat
 from llm_workflow.hugging_face import HuggingFaceEndpointChat
 from llm_workflow.compare import CompareModels, ModelDefinition
 
 # Comparing GPT-3.5 Turbo, GPT-4, and Mistral 7B
 model_definitions = [
     ModelDefinition(
-        create=lambda: OpenAIChat(model_name='gpt-3.5-turbo'),
+        create=lambda: OpenAIChat(model_name='gpt-3.5-turbo-1106'),
         description='GPT-3.5 Turbo',
     ),
     ModelDefinition(
-        create=lambda: OpenAIChat(model_name='gpt-4'),
-        description='GPT-4',
+        create=lambda: OpenAIChat(model_name='gpt-4-1106-preview'),
+        description='GPT-4 Turbo',
     ),
     ModelDefinition(
         create=lambda: HuggingFaceEndpointChat(
             endpoint_url=os.getenv('HUGGING_FACE_ENDPOINT_MISTRAL_7B'),
         ),
         description='Mistral 7B (HF Endpoint)',
     ),
```

### Comparing `llm-workflow-0.0.6/llm_workflow/agents.py` & `llm-workflow-0.0.8/llm_workflow/agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,23 +183,23 @@
     The response from the tool is retuned by the agent object.
 
     See this notebooks for an example: https://github.com/shane-kercheval/llm-workflow/blob/main/examples/agents.ipynb
     """
 
     def __init__(
             self,
-            model_name: str,
             tools: list[Tool],
+            model_name: str = 'gpt-3.5-turbo-1106',
             system_message: str = "Decide which function to use. Only use the functions you have been provided with. Don't make assumptions about what values to plug into functions.",  # noqa
             timeout: int = 10,
         ) -> dict | None:
         """
         Args:
             model_name:
-                e.g. 'gpt-3.5-turbo'
+                e.g. 'gpt-3.5-turbo-1106'
             tools:
                 a list of Tool objects (created with the `Tool` class or `tool` decorator).
             system_message:
                 The content of the message associated with the "system" `role`.
             timeout:
                 timeout value passed to OpenAI model.
         """
@@ -213,50 +213,51 @@
 
     def __call__(self, prompt: object) -> object:
         """
         Uses the OpenAI "functions" api to decide which tool to call based on the `prompt`. The
         selected tool (which is a callable) is called and passed the arguments determined by
         OpenAI. The response from the tool is retuned by the agent object.
         """
-        import openai
+        from openai import OpenAI
         messages = [
             {"role": "system", "content": self._system_message},
             {"role": "user", "content": prompt},
         ]
         # we want to track to track costs/etc.; but we don't need the history to build up memory
         # essentially, for now, this class won't have any memory/context of previous questions;
         # it's only used to decide which tools/functions to call
+        client = OpenAI()
         response = retry_handler()(
-                openai.ChatCompletion.create,
+                client.chat.completions.create,
                 model=self.model_name,
                 messages=messages,
                 functions=[x.to_dict() for x in self._tools],
                 temperature=0,
                 # max_tokens=self.max_tokens,
                 timeout=self.timeout,
             )
-        input_tokens = response['usage'].prompt_tokens
-        completion_tokens = response['usage'].completion_tokens
-        total_tokens = response['usage'].total_tokens
+        input_tokens = response.usage.prompt_tokens
+        completion_tokens = response.usage.completion_tokens
+        total_tokens = response.usage.total_tokens
         cost = (input_tokens * self.cost_per_token['input']) + \
             (completion_tokens * self.cost_per_token['output'])
         record = ExchangeRecord(
             prompt=prompt,
             response='',
             metadata={'model_name': self.model_name},
             input_tokens=input_tokens,
             response_tokens=completion_tokens,
             total_tokens=total_tokens,
             cost=cost,
         )
         self._history.append(record)
-        function_call = response["choices"][0]["message"].get('function_call')
+        function_call = response.choices[0].message.function_call
         if function_call:
-            function_name = function_call['name']
-            function_args = json.loads(function_call['arguments'])
+            function_name = function_call.name
+            function_args = json.loads(function_call.arguments)
             record.response = f"tool: '{function_name}' - {function_args}"
             record.metadata['tool_name'] = function_name
             record.metadata['tool_args'] = function_args
             for tool in self._tools:
                 if function_name == tool.name:
                     return tool(**function_args)
         return None
```

### Comparing `llm-workflow-0.0.6/llm_workflow/base.py` & `llm-workflow-0.0.8/llm_workflow/base.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow/compare.py` & `llm-workflow-0.0.8/llm_workflow/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utilities to compare the responses and performance of different models."""
 
 from typing import TypeVar
 from collections.abc import Callable
 import time
 import textwrap
+from joblib import Parallel, delayed
 from pydantic import BaseModel
 import markdown
 from llm_workflow.internal_utilities import execute_code_blocks, extract_code_blocks
 from pygments.formatters import HtmlFormatter
 
 
 Model = TypeVar('Model', bound=Callable[[str], str])
@@ -181,29 +182,35 @@
         # ensure no model descriptions are duplicated
         model_descriptions = [model_creation.description for model_creation in model_definitions]
         if len(model_descriptions) != len(set(model_descriptions)):
             raise ValueError("Model descriptions must be unique.")
 
         self.prompts = prompts
         self._model_definitions = model_definitions
+        self.scenarios = []
 
     def __call__(self):
-        """Runs the prompts/scenarios."""
+        """Runs each scenarios against all models."""
         self.scenarios = []
-        for prompts in self.prompts:
-            runs = []
-            for create_model in self._model_definitions:
-                scenario = Scenario(
-                    model=create_model.create(),  # create a new model for each run
-                    description=create_model.description,
-                )
-                scenario(prompts=prompts)
-                runs.append(scenario)
+        for scenario_prompts in self.prompts:
+            # Use joblib's Parallel and delayed functions to run in parallel
+            runs = Parallel(n_jobs=-1)(
+                delayed(self._run_scenario)(create_model, scenario_prompts)
+                for create_model in self._model_definitions
+            )
             self.scenarios.append(runs)
-        assert len(self.scenarios) == len(self.prompts)
+
+    def _run_scenario(self, create_model: Callable, prompts: list[str]) -> Scenario:
+        """Runs a single scenario for a model and set of prompts."""
+        scenario = Scenario(
+            model=create_model.create(),
+            description=create_model.description,
+        )
+        scenario(prompts=prompts)
+        return scenario
 
     @property
     def num_scenarios(self) -> int:
         """
         The number of scenarios. self.scenarios is a list of lists (of prompts). The outer list
         represents the scenarios. The inner list represents the prompts for a single scenario.
         `num_scenarios` is the number of outer lists.
@@ -455,15 +462,15 @@
 
         num_prompts = len(comparison.prompts)
         for i in range(num_prompts):
             # create a row for the prompt
             rows_html += '<tr>'
             rows_html += f'<td colspan="{len(model_scenarios)}" style="vertical-align: top; text-align: center;" >'  # noqa
             rows_html += '<h3>Prompt</h3><br>'
-            rows_html += f'{scenario.prompts[0]}<br><br>'
+            rows_html += f'{scenario.prompts[i]}<br><br>'
             rows_html += '</td>'
             rows_html += '</tr>'
             # create a row for the response
             rows_html += '<tr>'
             for scenario in model_scenarios:
                 rows_html += '<td style="vertical-align: top;">'
                 rows_html += '<h3>Response</h3><br>'
```

### Comparing `llm-workflow-0.0.6/llm_workflow/hugging_face.py` & `llm-workflow-0.0.8/llm_workflow/hugging_face.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow/indexes.py` & `llm-workflow-0.0.8/llm_workflow/indexes.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow/internal_utilities.py` & `llm-workflow-0.0.8/llm_workflow/internal_utilities.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow/memory.py` & `llm-workflow-0.0.8/llm_workflow/memory.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow/openai.py` & `llm-workflow-0.0.8/llm_workflow/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,40 @@
     ExchangeRecord,
     MemoryManager,
     StreamingEvent,
 )
 
 
 MODEL_COST_PER_TOKEN = {
+    # "Prices are per 1,000 tokens. You can think of tokens as pieces of words, where 1,000 tokens
+    # is about 750 words. This paragraph is 35 tokens."
+    # https://openai.com/pricing
+    # https://platform.openai.com/docs/models
+    ####
+    # Embedding models
+    ####
     'text-embedding-ada-002': 0.0001 / 1_000,
-    'gpt-4': {'input': 0.03 / 1_000, 'output': 0.06 / 1_000},
-    'gpt-4-32k': {'input': 0.06 / 1_000, 'output': 0.12 / 1_000},
-    'gpt-3.5-turbo': {'input': 0.0015 / 1_000, 'output': 0.002 / 1_000},
-    'gpt-3.5-turbo-16k': {'input': 0.003 / 1_000, 'output': 0.004 / 1_000},
+    ####
+    # Chat Models
+    ####
+    # GPT-4-Turbo 128K
+    'gpt-4-1106-preview': {'input': 0.01 / 1_000, 'output': 0.03 / 1_000},
+    # GPT-3.5-Turbo 16K
+    'gpt-3.5-turbo-1106': {'input': 0.001 / 1_000, 'output': 0.002 / 1_000},
+    ####
+    # legacy models
+    ####
+    # GPT-4
+    'gpt-4-0613': {'input': 0.03 / 1_000, 'output': 0.06 / 1_000},
+    # GPT-4- 32K
+    # 'gpt-4-32k-0613': {'input': 0.06 / 1_000, 'output': 0.12 / 1_000},
+    # GPT-3.5-Turbo 4K
+    'gpt-3.5-turbo-0613': {'input': 0.0015 / 1_000, 'output': 0.002 / 1_000},
+    # GPT-3.5-Turbo 16K
+    'gpt-3.5-turbo-16k-0613': {'input': 0.003 / 1_000, 'output': 0.004 / 1_000},
 }
 
 
 @cache
 def _get_encoding_for_model(model_name: str) -> Encoding:
     """Gets the encoding for a given model so that we can calculate the number of tokens."""
     return tiktoken.encoding_for_model(model_name)
@@ -45,27 +66,30 @@
     if model_name in {
         "gpt-3.5-turbo-0613",
         "gpt-3.5-turbo-16k-0613",
         "gpt-4-0314",
         "gpt-4-32k-0314",
         "gpt-4-0613",
         "gpt-4-32k-0613",
+        # todo: verify once .ipynb is updated
+        "gpt-4-1106-preview",
+        "gpt-3.5-turbo-1106",
         }:
         tokens_per_message = 3
         tokens_per_name = 1
     elif model_name == "gpt-3.5-turbo-0301":
         tokens_per_message = 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
         tokens_per_name = -1  # if there's a name, the role is omitted
     elif "gpt-3.5-turbo" in model_name:
         # Warning: gpt-3.5-turbo may update over time.
         # Returning num tokens assuming gpt-3.5-turbo-0613
-        return num_tokens_from_messages(model_name="gpt-3.5-turbo-0613", messages=messages)
+        return num_tokens_from_messages(model_name="gpt-3.5-turbo-1106", messages=messages)
     elif "gpt-4" in model_name:
         # Warning: gpt-4 may update over time. Returning num tokens assuming gpt-4-0613.
-        return num_tokens_from_messages(model_name="gpt-4-0613", messages=messages)
+        return num_tokens_from_messages(model_name="gpt-4-1106-preview", messages=messages)
     else:
         raise NotImplementedError(f"""num_tokens_from_messages() is not implemented for model {model_name}. See https://github.com/openai/openai-python/blob/main/chatml.md for information on how messages are converted to tokens.""")  # noqa
     num_tokens = 0
     for message in messages:
         num_tokens += tokens_per_message
         for key, value in message.items():
             num_tokens += len(_get_encoding_for_model(model_name=model_name).encode(value))
@@ -99,15 +123,15 @@
 
 
 class OpenAIEmbedding(EmbeddingModel):
     """A wrapper around the OpenAI Embedding model that tracks token usage and costs."""
 
     def __init__(
             self,
-            model_name: str,
+            model_name: str = 'text-embedding-ada-002',
             doc_prep: Callable[[str], str] = lambda x: x.strip().replace('\n', ' '),
             timeout: int = 10,
             ) -> None:
         """
         Args:
             model_name:
                 e.g. 'text-embedding-ada-002'
@@ -118,24 +142,25 @@
         """
         super().__init__()
         self.model_name = model_name
         self.doc_prep = doc_prep
         self.timeout = timeout
 
     def _run(self, docs: list[Document]) -> tuple[list[list[float]], EmbeddingRecord]:
-        import openai
+        from openai import OpenAI
         texts = [self.doc_prep(x.content) for x in docs]
+        client = OpenAI()
         response = retry_handler()(
-            openai.Embedding.create,
+            client.embeddings.create,
             input = texts,
             model=self.model_name,
             timeout=self.timeout,
         )
-        total_tokens = response['usage']['total_tokens']
-        embedding = [x['embedding'] for x in response['data']]
+        total_tokens = response.usage.total_tokens
+        embedding = [x.embedding for x in response.data]
         metadata = EmbeddingRecord(
             metadata={'model_name': self.model_name},
             total_tokens=total_tokens,
             cost=self.cost_per_token * total_tokens,
         )
         return embedding, metadata
 
@@ -158,26 +183,27 @@
     messages previously sent to the model in subsequent requests. Therefore, each object created
     represents a single conversation. The number of messages sent to the model can be controlled
     via `memory_manager`.
     """
 
     def __init__(
             self,
-            model_name: str,
+            model_name: str = 'gpt-3.5-turbo-1106',
             temperature: float = 0,
             max_tokens: int = 2000,
             system_message: str = 'You are a helpful assistant.',
             streaming_callback: Callable[[StreamingEvent], None] | None = None,
             memory_manager: MemoryManager | None = None,
-            timeout: int = 10,
+            timeout: int = 30,
+            seed: int | None = None,
             ) -> None:
         """
         Args:
             model_name:
-                e.g. 'gpt-3.5-turbo'
+                e.g. 'gpt-3.5-turbo-1106'
             temperature:
                 "What sampling temperature to use, between 0 and 2. Higher values like 0.8 will
                 make the output more random, while lower values like 0.2 will make it more focused
                 and deterministic."
             max_tokens:
                 The maximum number of tokens to generate in the chat completion.
                 The total length of input tokens and generated tokens is limited by the model's
@@ -189,14 +215,16 @@
                 the `response` property and perhaps other metadata.
             memory_manager:
                 MemoryManager object (or callable that takes a list of ExchangeRecord objects and
                 returns a list of ExchangeRecord objects. The underlying logic should return the
                 messages sent to the OpenAI model.
             timeout:
                 timeout value passed to OpenAI model.
+            seed:
+                seed value passed to OpenAI model.
         """
         def cost_calculator(input_tokens: int, response_tokens: int) -> float:
             model_costs = MODEL_COST_PER_TOKEN[self.model_name]
             return (input_tokens * model_costs['input']) + \
                 (response_tokens * model_costs['output'])
 
         def token_calculator(messages: str | list[dict]) -> int:
@@ -214,61 +242,62 @@
             memory_manager=memory_manager,
         )
         self.model_name = model_name
         self.temperature = temperature
         self.max_tokens = max_tokens
         self.streaming_callback = streaming_callback
         self.timeout = timeout
+        self.seed = seed
 
     def _run(self, messages: list[dict]) -> tuple[str, dict]:
         """
-        `openai.ChatCompletion.create` expects a list of messages with various roles (i.e. system,
-        user, assistant). This function builds the list of messages based on the history of
+        `client.chat.completions.create` expects a list of messages with various roles (i.e.
+        system, user, assistant). This function builds the list of messages based on the history of
         messages and based on an optional 'memory_manager' that filters the history based on
         it's own logic. The `system_message` is always the first message regardless if a
         `memory_manager` is passed in.
 
         The use of a streaming callback does not change the output returned from calling the object
         (i.e. a ExchangeRecord object).
         """
-        import openai
+        from openai import OpenAI
+        client = OpenAI()
         if self.streaming_callback:
             response = retry_handler()(
-                openai.ChatCompletion.create,
+                client.chat.completions.create,
                 model=self.model_name,
                 messages=messages,
                 temperature=self.temperature,
                 max_tokens=self.max_tokens,
                 timeout=self.timeout,
                 stream=True,
+                seed=self.seed,
             )
             # extract the content/token from the streaming response and send to the callback
             # build up the message so that we can calculate usage/costs and send back the same
             # ExchangeRecord response that we would return if we weren't streaming
             def get_delta(chunk):  # noqa
-                delta = chunk['choices'][0]['delta']
-                if 'content' in delta:
-                    return delta['content']
-                return None
+                return chunk.choices[0].delta.content
             response_message = ''
             for chunk in response:
                 delta = get_delta(chunk)
                 if delta:
                     self.streaming_callback(StreamingEvent(response=delta))
                     response_message += delta
         else:
             response = retry_handler()(
-                openai.ChatCompletion.create,
+                client.chat.completions.create,
                 model=self.model_name,
                 messages=messages,
                 temperature=self.temperature,
                 max_tokens=self.max_tokens,
                 timeout=self.timeout,
+                seed=self.seed,
             )
-            response_message = response['choices'][0]['message'].content
+            response_message = response.choices[0].message.content
 
         metadata = {
             'model_name': self.model_name,
             'temperature': self.temperature,
             'max_tokens': self.max_tokens,
             'timeout': self.timeout,
         }
```

### Comparing `llm-workflow-0.0.6/llm_workflow/prompt_templates.py` & `llm-workflow-0.0.8/llm_workflow/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow/utilities.py` & `llm-workflow-0.0.8/llm_workflow/utilities.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/llm_workflow.egg-info/PKG-INFO` & `llm-workflow-0.0.8/llm_workflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llm-workflow
-Version: 0.0.6
+Version: 0.0.8
 Summary: build LLM workflows
 Home-page: https://github.com/shane-kercheval/llm-workflow
 Author: Shane Kercheval
 Author-email: shane.kercheval@gmail.com
 Project-URL: Bug Tracker, https://github.com/shane-kercheval/llm-workflow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: joblib
 Requires-Dist: openai
 Requires-Dist: pydantic
 Requires-Dist: tenacity
 Requires-Dist: transformers
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
@@ -130,17 +131,17 @@
 - fourth task: ignores the response from the chat model; creates a new prompt asking the chat model to extract the relevant code created in the previous response
 - fifth task: the chat model, which internally maintains the history of messages, returns only the relevant code from the previous response.
 
 ```python
 from llm_workflow.base import Workflow
 from llm_workflow.openai import OpenAIChat
 
-prompt_enhancer = OpenAIChat(model_name='gpt-3.5-turbo')
+prompt_enhancer = OpenAIChat()
 # different model/object, therefore different message history (i.e. conversation)
-chat_assistant = OpenAIChat(model_name='gpt-3.5-turbo')
+chat_assistant = OpenAIChat()
 
 def prompt_template(user_prompt: str) -> str:
     return "Improve the user's request, below, by expanding the request " \
         "to describe the relevant python best practices and documentation " \
         f"requirements that should be followed:\n\n```{user_prompt}```"
 
 def prompt_extract_code(_) -> str:
@@ -340,15 +341,15 @@
 from llm_workflow.indexes import ChromaDocumentIndex
 from llm_workflow.prompt_templates import DocSearchTemplate
 
 duckduckgo_search = DuckDuckGoSearch(top_n=3)
 embeddings_model = OpenAIEmbedding(model_name='text-embedding-ada-002')
 document_index = ChromaDocumentIndex(embeddings_model=embeddings_model, n_results=3)
 prompt_template = DocSearchTemplate(doc_index=document_index, n_docs=3)
-chat_model = OpenAIChat(model_name='gpt-3.5-turbo')
+chat_model = OpenAIChat()
 
 def scrape_urls(search_results):
     """
     For each url (i.e. `href` in `search_results`):
     - extracts text
     - replace new-lines with spaces
     - create a Document object
@@ -412,20 +413,20 @@
 from llm_workflow.openai import OpenAIChat
 from llm_workflow.hugging_face import HuggingFaceEndpointChat
 from llm_workflow.compare import CompareModels, ModelDefinition
 
 # Comparing GPT-3.5 Turbo, GPT-4, and Mistral 7B
 model_definitions = [
     ModelDefinition(
-        create=lambda: OpenAIChat(model_name='gpt-3.5-turbo'),
+        create=lambda: OpenAIChat(model_name='gpt-3.5-turbo-1106'),
         description='GPT-3.5 Turbo',
     ),
     ModelDefinition(
-        create=lambda: OpenAIChat(model_name='gpt-4'),
-        description='GPT-4',
+        create=lambda: OpenAIChat(model_name='gpt-4-1106-preview'),
+        description='GPT-4 Turbo',
     ),
     ModelDefinition(
         create=lambda: HuggingFaceEndpointChat(
             endpoint_url=os.getenv('HUGGING_FACE_ENDPOINT_MISTRAL_7B'),
         ),
         description='Mistral 7B (HF Endpoint)',
     ),
```

### Comparing `llm-workflow-0.0.6/llm_workflow.egg-info/SOURCES.txt` & `llm-workflow-0.0.8/llm_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/setup.cfg` & `llm-workflow-0.0.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = llm-workflow
-version = 0.0.6
+version = 0.0.8
 author = Shane Kercheval
 author_email = shane.kercheval@gmail.com
 description = build LLM workflows
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/shane-kercheval/llm-workflow
 project_urls = 
@@ -15,14 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 packages = find:
 python_requires = >=3.10
 install_requires = 
+	joblib
 	openai
 	pydantic
 	tenacity
 	transformers
 	torch
 	torchvision
 	torchaudio
```

### Comparing `llm-workflow-0.0.6/tests/conftest.py` & `llm-workflow-0.0.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_agents.py` & `llm-workflow-0.0.8/tests/test_agents.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,18 +63,15 @@
                 'type': 'string',
                 'description': "The stock symbol, e.g. 'AAPL'",
             },
         },
         required= ['symbol'],
     )
 
-    agent = OpenAIFunctionAgent(
-        model_name='gpt-3.5-turbo',
-        tools=[fake_weather_tool, fake_stock_tool],
-    )
+    agent = OpenAIFunctionAgent(tools=[fake_weather_tool, fake_stock_tool])
 
     question = "What is the temperature in Seattle WA."
     response = agent(question)
     assert 'Seattle' in response
     assert 'degrees' in response
     # assert 'fahrenheit' in response  # model does not correctly infer fahrenheight
     assert len(fake_weather_tool.history()) == 1
@@ -167,15 +164,15 @@
     def fake_stock(symbol: str) -> str:
             return f"The stock price of {symbol} is $1000."
 
     assert isinstance(fake_weather, Tool)
     assert isinstance(fake_stock, Tool)
 
     agent = OpenAIFunctionAgent(
-        model_name='gpt-3.5-turbo',
+        model_name='gpt-3.5-turbo-0613',
         tools=[fake_weather, fake_stock],
     )
 
     question = "What is the temperature in Seattle WA."
     response = agent(question)
     assert 'Seattle' in response
     assert 'degrees' in response
```

### Comparing `llm-workflow-0.0.6/tests/test_base.py` & `llm-workflow-0.0.8/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_compare.py` & `llm-workflow-0.0.8/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_history.py` & `llm-workflow-0.0.8/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_hugging_face.py` & `llm-workflow-0.0.8/tests/test_hugging_face.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_indexes.py` & `llm-workflow-0.0.8/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_openai.py` & `llm-workflow-0.0.8/tests/test_openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test the OpenAI Model classes."""
 
-import openai
+from openai import OpenAI
 import pytest
 from llm_workflow.base import Document, EmbeddingRecord, ExchangeRecord, StreamingEvent
 from llm_workflow.memory import (
     LastNExchangesManager,
     LastNTokensMemoryManager,
     MessageSummaryMemoryManager,
 )
@@ -15,15 +15,15 @@
     num_tokens,
     num_tokens_from_messages,
     MODEL_COST_PER_TOKEN,
 )
 
 
 def test_num_tokens():  # noqa
-    assert num_tokens(model_name='gpt-3.5-turbo', value="This should be six tokens.") == 6
+    assert num_tokens(model_name='gpt-3.5-turbo-0613', value="This should be six tokens.") == 6
 
 def test_num_tokens_from_messages():  # noqa
     # copied from https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     example_messages = [
         {
             "role": "system",
             "content": "You are a helpful, pattern-following assistant that translates corporate jargon into plain English.",  # noqa
@@ -49,29 +49,30 @@
             "content": "Let's talk later when we're less busy about how to do better.",
         },
         {
             "role": "user",
             "content": "This late pivot means we don't have time to boil the ocean for the client deliverable.",  # noqa
         },
     ]
-    model_name = 'gpt-3.5-turbo'
-    response = openai.ChatCompletion.create(
+    model_name = 'gpt-3.5-turbo-0613'
+    client = OpenAI()
+    response = client.chat.completions.create(
         model=model_name,
         messages=example_messages,
         temperature=0,
         max_tokens=1,  # we're only counting input tokens here, so let's not waste tokens on output
     )
-    expected_value = response["usage"]["prompt_tokens"]
+    expected_value = response.usage.prompt_tokens
     actual_value = num_tokens_from_messages(model_name=model_name, messages=example_messages)
     assert expected_value == actual_value
 
     # above we checked that the numbers match exactly from what OpenAI returns;
     # here, let's just check that the other models run and return >0 to avoid API calls
     assert num_tokens_from_messages(model_name='gpt-3.5-turbo-0301', messages=example_messages) > 0
-    assert num_tokens_from_messages(model_name='gpt-4', messages=example_messages) > 0
+    assert num_tokens_from_messages(model_name='gpt-4-1106-preview', messages=example_messages) > 0
     assert num_tokens_from_messages(model_name='gpt-4-0314', messages=example_messages) > 0
     with pytest.raises(NotImplementedError):
         num_tokens_from_messages(model_name='<not implemented>', messages=example_messages)
 
 def test_message_formatter():  # noqa
     assert message_formatter(None, None, None) == []
     messages = message_formatter('System message', None, None)
@@ -88,16 +89,15 @@
     assert messages == [
         {'role': 'system', 'content': 'System message'},
         {'role': 'user', 'content': 'prompt'}, {'role': 'assistant', 'content': 'response'},
         {'role': 'user', 'content': 'New Prompt.'},
     ]
 
 def test_OpenAIChat():  # noqa
-    model_name = 'gpt-3.5-turbo'
-    model = OpenAIChat(model_name=model_name)
+    model = OpenAIChat()
     assert len(model.history()) == 0
     assert model.previous_record() is None
     assert model.previous_prompt is None
     assert model.previous_response is None
     assert model.cost == 0
     assert model.total_tokens == 0
     assert model.input_tokens == 0
@@ -123,30 +123,30 @@
     assert model.chat_history[0].prompt == prompt
     assert model.chat_history[0].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == message.cost
     assert model.total_tokens == message.total_tokens
     assert model.input_tokens == message.input_tokens
     assert model.response_tokens == message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
@@ -182,45 +182,44 @@
     assert model.chat_history[1].prompt == prompt
     assert model.chat_history[1].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.uuid != previous_message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == previous_cost + message.cost
     assert model.total_tokens == previous_total_tokens + message.total_tokens
     assert model.input_tokens == previous_input_tokens + message.input_tokens
     assert model.response_tokens == previous_response_tokens + message.response_tokens
 
 def test_OpenAIChat_streaming():  # noqa
     """Test the same thing as above but for streaming. All usage and history should be the same."""
     callback_response = ''
     def streaming_callback(record: StreamingEvent) -> None:
         nonlocal callback_response
         callback_response += record.response
 
-    model_name = 'gpt-3.5-turbo'
-    model = OpenAIChat(model_name=model_name, streaming_callback=streaming_callback)
+    model = OpenAIChat(streaming_callback=streaming_callback)
     assert model.previous_record() is None
     assert model.previous_prompt is None
     assert model.previous_response is None
     assert model.cost == 0
     assert model.total_tokens == 0
     assert model.input_tokens == 0
     assert model.response_tokens == 0
@@ -246,30 +245,30 @@
     assert model.chat_history[0].prompt == prompt
     assert model.chat_history[0].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == message.cost
     assert model.total_tokens == message.total_tokens
     assert model.input_tokens == message.input_tokens
     assert model.response_tokens == message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
@@ -307,388 +306,368 @@
     assert model.chat_history[1].prompt == prompt
     assert model.chat_history[1].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.uuid != previous_message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == previous_cost + message.cost
     assert model.total_tokens == previous_total_tokens + message.total_tokens
     assert model.input_tokens == previous_input_tokens + message.input_tokens
     assert model.response_tokens == previous_response_tokens + message.response_tokens
 
 def test_OpenAIChat_streaming_response_matches_non_streaming():  # noqa
     """
     Test that we get the same final response and usage data when streaming vs not streaming.
     Additionally test that the response we get in the streaming callback matches the overall
     response.
     """
-    question = "Explain what a large language model is in a single sentence."
-    model_name = 'gpt-3.5-turbo'
-    non_streaming_chat = OpenAIChat(
-        model_name=model_name,
-        temperature=0,
-        )
+    question = "What is the capital of France?"
+    non_streaming_chat = OpenAIChat(seed=42)
     non_streaming_response = non_streaming_chat(question)
 
     callback_response = ''
     def streaming_callback(record: StreamingEvent) -> None:
         nonlocal callback_response
         callback_response += record.response
 
-    streaming_chat = OpenAIChat(
-        model_name=model_name,
-        temperature=0,
-        streaming_callback=streaming_callback,
-    )
+    streaming_chat = OpenAIChat(streaming_callback=streaming_callback, seed=42)
     streaming_response  = streaming_chat(question)
     assert non_streaming_response == streaming_response
     assert non_streaming_response == callback_response
     assert non_streaming_chat.input_tokens == streaming_chat.input_tokens
     assert non_streaming_chat.response_tokens == streaming_chat.response_tokens
     assert non_streaming_chat.total_tokens == streaming_chat.total_tokens
     assert non_streaming_chat.cost == streaming_chat.cost
 
 def test_OpenAIChat__LastNExchangesManager0():  # noqa
-    model_name = 'gpt-3.5-turbo'
-    openai_llm = OpenAIChat(
-        model_name=model_name,
-        memory_manager=LastNExchangesManager(last_n_exchanges=0),
-    )
-    assert openai_llm.previous_record() is None
-    assert openai_llm.previous_prompt is None
-    assert openai_llm.previous_response is None
-    assert openai_llm.cost == 0
-    assert openai_llm.total_tokens == 0
-    assert openai_llm.input_tokens == 0
-    assert openai_llm.response_tokens == 0
+    model = OpenAIChat(memory_manager=LastNExchangesManager(last_n_exchanges=0))
+    assert model.previous_record() is None
+    assert model.previous_prompt is None
+    assert model.previous_response is None
+    assert model.cost == 0
+    assert model.total_tokens == 0
+    assert model.input_tokens == 0
+    assert model.response_tokens == 0
 
     ####
     # first interaction
     # this shouldn't be any different
     ####
     prompt = "Hi my name is shane. What is my name?"
-    response = openai_llm(prompt)
+    response = model(prompt)
     assert 'shane' in response.lower()
     assert isinstance(response, str)
     assert len(response) > 1
 
     # previous memory is the input to ChatGPT
-    assert openai_llm._previous_messages[0]['role'] == 'system'
-    assert openai_llm._previous_messages[-1]['role'] == 'user'
-    assert openai_llm._previous_messages[-1]['content'] == prompt
-
-    assert len(openai_llm.history()) == 1
-    assert len(openai_llm.chat_history) == 1
-    assert openai_llm.history() == openai_llm.chat_history
-    assert openai_llm.chat_history[0].prompt == prompt
-    assert openai_llm.chat_history[0].response == response
+    assert model._previous_messages[0]['role'] == 'system'
+    assert model._previous_messages[-1]['role'] == 'user'
+    assert model._previous_messages[-1]['content'] == prompt
 
-    message = openai_llm.previous_record()
+    assert len(model.history()) == 1
+    assert len(model.chat_history) == 1
+    assert model.history() == model.chat_history
+    assert model.chat_history[0].prompt == prompt
+    assert model.chat_history[0].response == response
+
+    message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
-        messages=openai_llm._previous_messages,
+        model_name=model.model_name,
+        messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
 
-    assert openai_llm.previous_prompt == prompt
-    assert openai_llm.previous_response == response
-    assert openai_llm.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
-    assert openai_llm.cost == message.cost
-    assert openai_llm.total_tokens == message.total_tokens
-    assert openai_llm.input_tokens == message.input_tokens
-    assert openai_llm.response_tokens == message.response_tokens
+    assert model.previous_prompt == prompt
+    assert model.previous_response == response
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
+    assert model.cost == message.cost
+    assert model.total_tokens == message.total_tokens
+    assert model.input_tokens == message.input_tokens
+    assert model.response_tokens == message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
     previous_cost = message.cost
     previous_total_tokens = message.total_tokens
     previous_input_tokens = message.input_tokens
     previous_response_tokens = message.response_tokens
 
     ####
     # second interaction
     # this shouldn't be any different
     ####
     prompt = "What is my name?"
-    response = openai_llm(prompt)
+    response = model(prompt)
     assert 'shane' not in response.lower()
     assert isinstance(response, str)
     assert len(response) > 1
 
     # previous memory is the input to ChatGPT
-    assert len(openai_llm._previous_messages) == 2  # system/user
-    assert openai_llm._previous_messages[0]['role'] == 'system'
-    assert openai_llm._previous_messages[0]['content'] == 'You are a helpful assistant.'
-    assert openai_llm._previous_messages[1]['role'] == 'user'
-    assert openai_llm._previous_messages[1]['content'] == prompt
-
-    assert len(openai_llm.history()) == 2
-    assert len(openai_llm.chat_history) == 2
-    assert openai_llm.history() == openai_llm.chat_history
-    assert openai_llm.chat_history[0].prompt == previous_prompt
-    assert openai_llm.chat_history[0].response == previous_response
-    assert openai_llm.chat_history[1].prompt == prompt
-    assert openai_llm.chat_history[1].response == response
+    assert len(model._previous_messages) == 2  # system/user
+    assert model._previous_messages[0]['role'] == 'system'
+    assert model._previous_messages[0]['content'] == 'You are a helpful assistant.'
+    assert model._previous_messages[1]['role'] == 'user'
+    assert model._previous_messages[1]['content'] == prompt
 
-    message = openai_llm.previous_record()
+    assert len(model.history()) == 2
+    assert len(model.chat_history) == 2
+    assert model.history() == model.chat_history
+    assert model.chat_history[0].prompt == previous_prompt
+    assert model.chat_history[0].response == previous_response
+    assert model.chat_history[1].prompt == prompt
+    assert model.chat_history[1].response == response
+
+    message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
-        messages=openai_llm._previous_messages,
+        model_name=model.model_name,
+        messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
-    assert openai_llm.previous_prompt == prompt
-    assert openai_llm.previous_response == response
-    assert openai_llm.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
-    assert openai_llm.cost == previous_cost + message.cost
-    assert openai_llm.total_tokens == previous_total_tokens + message.total_tokens
-    assert openai_llm.input_tokens == previous_input_tokens + message.input_tokens
-    assert openai_llm.response_tokens == previous_response_tokens + message.response_tokens
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
+    assert model.previous_prompt == prompt
+    assert model.previous_response == response
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
+    assert model.cost == previous_cost + message.cost
+    assert model.total_tokens == previous_total_tokens + message.total_tokens
+    assert model.input_tokens == previous_input_tokens + message.input_tokens
+    assert model.response_tokens == previous_response_tokens + message.response_tokens
 
 def test_OpenAIChat__LastNExchangesManager1():  # noqa
-    model_name = 'gpt-3.5-turbo'
-    openai_llm = OpenAIChat(
-        model_name=model_name,
-        memory_manager=LastNExchangesManager(last_n_exchanges=1),
-    )
-    assert openai_llm.previous_record() is None
-    assert openai_llm.previous_prompt is None
-    assert openai_llm.previous_response is None
-    assert openai_llm.cost == 0
-    assert openai_llm.total_tokens == 0
-    assert openai_llm.input_tokens == 0
-    assert openai_llm.response_tokens == 0
+    model = OpenAIChat(memory_manager=LastNExchangesManager(last_n_exchanges=1))
+    assert model.previous_record() is None
+    assert model.previous_prompt is None
+    assert model.previous_response is None
+    assert model.cost == 0
+    assert model.total_tokens == 0
+    assert model.input_tokens == 0
+    assert model.response_tokens == 0
 
     ####
     # first interaction
     # this shouldn't be any different
     ####
     prompt = "Hi my name is shane. What is my name?"
-    response = openai_llm(prompt)
+    response = model(prompt)
     assert 'shane' in response.lower()
     assert isinstance(response, str)
     assert len(response) > 1
 
     # previous memory is the input to ChatGPT
-    assert openai_llm._previous_messages[0]['role'] == 'system'
-    assert openai_llm._previous_messages[-1]['role'] == 'user'
-    assert openai_llm._previous_messages[-1]['content'] == prompt
-
-    assert len(openai_llm.history()) == 1
-    assert len(openai_llm.chat_history) == 1
-    assert openai_llm.history() == openai_llm.chat_history
-    assert openai_llm.chat_history[0].prompt == prompt
-    assert openai_llm.chat_history[0].response == response
+    assert model._previous_messages[0]['role'] == 'system'
+    assert model._previous_messages[-1]['role'] == 'user'
+    assert model._previous_messages[-1]['content'] == prompt
+
+    assert len(model.history()) == 1
+    assert len(model.chat_history) == 1
+    assert model.history() == model.chat_history
+    assert model.chat_history[0].prompt == prompt
+    assert model.chat_history[0].response == response
 
-    message = openai_llm.previous_record()
+    message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
-        messages=openai_llm._previous_messages,
+        model_name=model.model_name,
+        messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
 
-    assert openai_llm.previous_prompt == prompt
-    assert openai_llm.previous_response == response
-    assert openai_llm.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
-    assert openai_llm.cost == message.cost
-    assert openai_llm.total_tokens == message.total_tokens
-    assert openai_llm.input_tokens == message.input_tokens
-    assert openai_llm.response_tokens == message.response_tokens
+    assert model.previous_prompt == prompt
+    assert model.previous_response == response
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
+    assert model.cost == message.cost
+    assert model.total_tokens == message.total_tokens
+    assert model.input_tokens == message.input_tokens
+    assert model.response_tokens == message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
     previous_cost = message.cost
     previous_total_tokens = message.total_tokens
     previous_input_tokens = message.input_tokens
     previous_response_tokens = message.response_tokens
 
     ####
     # second interaction
     # this shouldn't be any different
     ####
     prompt = "What is my name?"
-    response = openai_llm(prompt)
+    response = model(prompt)
     assert 'shane' in response.lower()
     assert isinstance(response, str)
     assert len(response) > 1
 
     # previous memory is the input to ChatGPT
-    assert openai_llm._previous_messages[0]['role'] == 'system'
-    assert openai_llm._previous_messages[0]['content'] == 'You are a helpful assistant.'
-    assert openai_llm._previous_messages[1]['role'] == 'user'
-    assert openai_llm._previous_messages[1]['content'] == previous_prompt
-    assert openai_llm._previous_messages[2]['role'] == 'assistant'
-    assert openai_llm._previous_messages[2]['content'] == previous_response
-    assert openai_llm._previous_messages[3]['role'] == 'user'
-    assert openai_llm._previous_messages[3]['content'] == prompt
-
-    assert len(openai_llm.history()) == 2
-    assert len(openai_llm.chat_history) == 2
-    assert openai_llm.history() == openai_llm.chat_history
-    assert openai_llm.chat_history[0].prompt == previous_prompt
-    assert openai_llm.chat_history[0].response == previous_response
-    assert openai_llm.chat_history[1].prompt == prompt
-    assert openai_llm.chat_history[1].response == response
+    assert model._previous_messages[0]['role'] == 'system'
+    assert model._previous_messages[0]['content'] == 'You are a helpful assistant.'
+    assert model._previous_messages[1]['role'] == 'user'
+    assert model._previous_messages[1]['content'] == previous_prompt
+    assert model._previous_messages[2]['role'] == 'assistant'
+    assert model._previous_messages[2]['content'] == previous_response
+    assert model._previous_messages[3]['role'] == 'user'
+    assert model._previous_messages[3]['content'] == prompt
+
+    assert len(model.history()) == 2
+    assert len(model.chat_history) == 2
+    assert model.history() == model.chat_history
+    assert model.chat_history[0].prompt == previous_prompt
+    assert model.chat_history[0].response == previous_response
+    assert model.chat_history[1].prompt == prompt
+    assert model.chat_history[1].response == response
 
-    message = openai_llm.previous_record()
+    message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
-        messages=openai_llm._previous_messages,
+        model_name=model.model_name,
+        messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
 
-    assert openai_llm.previous_prompt == prompt
-    assert openai_llm.previous_response == response
-    assert openai_llm.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
-    assert openai_llm.cost == previous_cost + message.cost
-    assert openai_llm.total_tokens == previous_total_tokens + message.total_tokens
-    assert openai_llm.input_tokens == previous_input_tokens + message.input_tokens
-    assert openai_llm.response_tokens == previous_response_tokens + message.response_tokens
+    assert model.previous_prompt == prompt
+    assert model.previous_response == response
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
+    assert model.cost == previous_cost + message.cost
+    assert model.total_tokens == previous_total_tokens + message.total_tokens
+    assert model.input_tokens == previous_input_tokens + message.input_tokens
+    assert model.response_tokens == previous_response_tokens + message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
 
     ####
     # third interaction
     # this shouldn't be any different
     ####
     prompt = "What is today's date?"
-    response = openai_llm(prompt)
+    response = model(prompt)
     assert 'shane' not in response.lower()
     assert isinstance(response, str)
     assert len(response) > 1
 
     # previous memory is the input to ChatGPT
     # The last message should contain shane, but not this one
-    assert openai_llm._previous_messages[0]['role'] == 'system'
-    assert openai_llm._previous_messages[0]['content'] == 'You are a helpful assistant.'
-    assert openai_llm._previous_messages[1]['role'] == 'user'
-    assert openai_llm._previous_messages[1]['content'] == previous_prompt
-    assert openai_llm._previous_messages[2]['role'] == 'assistant'
-    assert openai_llm._previous_messages[2]['content'] == previous_response
-    assert 'shane' in openai_llm._previous_messages[2]['content'].lower()
-    assert openai_llm._previous_messages[3]['role'] == 'user'
-    assert openai_llm._previous_messages[3]['content'] == prompt
-    assert len(openai_llm._previous_messages) == 4
+    assert model._previous_messages[0]['role'] == 'system'
+    assert model._previous_messages[0]['content'] == 'You are a helpful assistant.'
+    assert model._previous_messages[1]['role'] == 'user'
+    assert model._previous_messages[1]['content'] == previous_prompt
+    assert model._previous_messages[2]['role'] == 'assistant'
+    assert model._previous_messages[2]['content'] == previous_response
+    assert 'shane' in model._previous_messages[2]['content'].lower()
+    assert model._previous_messages[3]['role'] == 'user'
+    assert model._previous_messages[3]['content'] == prompt
+    assert len(model._previous_messages) == 4
 
-    assert len(openai_llm.history()) == 3
-    message = openai_llm.previous_record()
+    assert len(model.history()) == 3
+    message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
-        messages=openai_llm._previous_messages,
+        model_name=model.model_name,
+        messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
 
-    assert openai_llm.previous_prompt == prompt
-    assert openai_llm.previous_response == response
-    assert openai_llm.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.previous_prompt == prompt
+    assert model.previous_response == response
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
 
     previous_prompt = prompt
     previous_response = response
 
     ####
     # 4th interaction
     # this shouldn't contain the name shane because the last interaction was the first that didn't
     ####
     prompt = "What is today's date?"
-    response = openai_llm(prompt)
+    response = model(prompt)
     assert 'shane' not in response.lower()
     assert isinstance(response, str)
     assert len(response) > 1
 
     # previous memory is the input to ChatGPT
-    assert openai_llm._previous_messages[0]['role'] == 'system'
-    assert openai_llm._previous_messages[0]['content'] == 'You are a helpful assistant.'
-    assert openai_llm._previous_messages[1]['role'] == 'user'
-    assert openai_llm._previous_messages[1]['content'] == previous_prompt
-    assert openai_llm._previous_messages[2]['role'] == 'assistant'
-    assert openai_llm._previous_messages[2]['content'] == previous_response
-    assert openai_llm._previous_messages[3]['role'] == 'user'
-    assert openai_llm._previous_messages[3]['content'] == prompt
+    assert model._previous_messages[0]['role'] == 'system'
+    assert model._previous_messages[0]['content'] == 'You are a helpful assistant.'
+    assert model._previous_messages[1]['role'] == 'user'
+    assert model._previous_messages[1]['content'] == previous_prompt
+    assert model._previous_messages[2]['role'] == 'assistant'
+    assert model._previous_messages[2]['content'] == previous_response
+    assert model._previous_messages[3]['role'] == 'user'
+    assert model._previous_messages[3]['content'] == prompt
     # still 4 because we are only keeping 1 message
     # (1)system + (2)previous question + (3)previous answer + (4)new question
-    assert len(openai_llm._previous_messages) == 4
+    assert len(model._previous_messages) == 4
 
-    assert len(openai_llm.history()) == 4
-    message = openai_llm.previous_record()
+    assert len(model.history()) == 4
+    message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
-        messages=openai_llm._previous_messages,
+        model_name=model.model_name,
+        messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
 
-    assert openai_llm.previous_prompt == prompt
-    assert openai_llm.previous_response == response
-    assert openai_llm.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.previous_prompt == prompt
+    assert model.previous_response == response
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
 
 def test_OpenAIChat_with_LastNTokensMemoryManager_1000_tokens():  # noqa
-    model_name = 'gpt-3.5-turbo'
-    model = OpenAIChat(
-        model_name=model_name,
-        memory_manager=LastNTokensMemoryManager(last_n_tokens=1000),
-    )
+    model = OpenAIChat(memory_manager=LastNTokensMemoryManager(last_n_tokens=1000))
     assert len(model.history()) == 0
     assert model.previous_record() is None
     assert model.previous_prompt is None
     assert model.previous_response is None
     assert model.cost == 0
     assert model.total_tokens == 0
     assert model.input_tokens == 0
@@ -714,30 +693,30 @@
     assert model.chat_history[0].prompt == prompt
     assert model.chat_history[0].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == message.cost
     assert model.total_tokens == message.total_tokens
     assert model.input_tokens == message.input_tokens
     assert model.response_tokens == message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
@@ -773,42 +752,38 @@
     assert model.chat_history[1].prompt == prompt
     assert model.chat_history[1].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.uuid != previous_message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == previous_cost + message.cost
     assert model.total_tokens == previous_total_tokens + message.total_tokens
     assert model.input_tokens == previous_input_tokens + message.input_tokens
     assert model.response_tokens == previous_response_tokens + message.response_tokens
 
 def test_OpenAIChat_with_LastNTokensMemoryManager_75_tokens():  # noqa
-    model_name = 'gpt-3.5-turbo'
-    model = OpenAIChat(
-        model_name=model_name,
-        memory_manager=LastNTokensMemoryManager(last_n_tokens=45),
-    )
+    model = OpenAIChat(memory_manager=LastNTokensMemoryManager(last_n_tokens=45))
     assert len(model.history()) == 0
     assert model.previous_record() is None
     assert model.previous_prompt is None
     assert model.previous_response is None
     assert model.cost == 0
     assert model.total_tokens == 0
     assert model.input_tokens == 0
@@ -834,30 +809,30 @@
     assert model.chat_history[0].prompt == prompt
     assert model.chat_history[0].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == message.cost
     assert model.total_tokens == message.total_tokens
     assert model.input_tokens == message.input_tokens
     assert model.response_tokens == message.response_tokens
 
     previous_prompt = prompt
     previous_response = response
@@ -895,52 +870,47 @@
     assert model.chat_history[1].prompt == prompt
     assert model.chat_history[1].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.uuid != previous_message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == previous_cost + message.cost
     assert model.total_tokens == previous_total_tokens + message.total_tokens
     assert model.input_tokens == previous_input_tokens + message.input_tokens
     assert model.response_tokens == previous_response_tokens + message.response_tokens
 
 def test_OpenAIChat_with_LastNTokensMemoryManager__1_tokens():  # noqa
-    model = OpenAIChat(
-        model_name='gpt-3.5-turbo',
-        memory_manager=LastNTokensMemoryManager(last_n_tokens=1),
-    )
+    model = OpenAIChat(memory_manager=LastNTokensMemoryManager(last_n_tokens=1))
     prompt = "My name is Shane and my favorite color is blue. What's your name?"
     with pytest.raises(AssertionError):
         _ = model(prompt)
 
 def test_OpenAIChat_with_MessageSummaryMemoryManager():  # noqa
-    model_name = 'gpt-3.5-turbo'
     summarize_instruction = 'Summarize the following while retaining the important information.'
     model = OpenAIChat(
-        model_name=model_name,
         memory_manager=MessageSummaryMemoryManager(
-            model=OpenAIChat(model_name=model_name),
+            model=OpenAIChat(),
             summarize_instruction=summarize_instruction,
         ),
     )
     assert len(model.history()) == 0
     assert model.previous_record() is None
     assert model.previous_prompt is None
     assert model.previous_response is None
@@ -973,30 +943,30 @@
     assert model.chat_history[0].prompt == prompt
     assert model.chat_history[0].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
     assert message.total_tokens == message.input_tokens + message.response_tokens
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     assert model.cost == message.cost
     assert model.total_tokens == message.total_tokens
     assert model.input_tokens == message.input_tokens
     assert model.response_tokens == message.response_tokens
 
     previous_prompt_0 = prompt
     previous_response_0 = response
@@ -1043,31 +1013,31 @@
     assert model.chat_history[1].prompt == prompt
     assert model.chat_history[1].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.uuid != previous_message_0.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     summarization_cost = sum(record.cost for record in model._memory_manager.history())
     summarization_input_tokens = sum(record.input_tokens for record in model._memory_manager.history())  # noqa
     summarization_response_tokens = sum(record.response_tokens for record in model._memory_manager.history())  # noqa
     assert model.input_tokens == previous_input_tokens_0 + message.input_tokens + summarization_input_tokens  # noqa
     assert model.response_tokens == previous_response_tokens_0 + message.response_tokens + summarization_response_tokens  # noqa
     assert model.total_tokens == previous_total_tokens_0 + message.total_tokens + summarization_input_tokens + summarization_response_tokens  # noqa
     assert round(model.cost, 5) == round(previous_cost_0 + message.cost + summarization_cost, 5)
@@ -1124,31 +1094,31 @@
     assert model.chat_history[2].prompt == prompt
     assert model.chat_history[2].response == response
 
     message = model.previous_record()
     assert isinstance(message, ExchangeRecord)
     assert message.prompt == prompt
     assert message.response == response
-    assert message.metadata['model_name'] == model_name
+    assert message.metadata['model_name'] == model.model_name
     assert message.metadata['messages'] == model._previous_messages
     assert message.input_tokens == num_tokens_from_messages(
-        model_name=model_name,
+        model_name=model.model_name,
         messages=model._previous_messages,
     )
-    assert message.response_tokens == num_tokens(model_name=model_name, value=response)
-    assert message.cost == (MODEL_COST_PER_TOKEN[model_name]['input'] * message.input_tokens) + \
-        (MODEL_COST_PER_TOKEN[model_name]['output'] * message.response_tokens)
+    assert message.response_tokens == num_tokens(model_name=model.model_name, value=response)
+    assert message.cost == (MODEL_COST_PER_TOKEN[model.model_name]['input'] * message.input_tokens) + \
+        (MODEL_COST_PER_TOKEN[model.model_name]['output'] * message.response_tokens)  # noqa: E501
     assert message.total_tokens == message.input_tokens + message.response_tokens
     assert message.uuid
     assert message.uuid != previous_message_0.uuid
     assert message.timestamp
 
     assert model.previous_prompt == prompt
     assert model.previous_response == response
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model_name]
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
     summarization_cost = sum(record.cost for record in model._memory_manager.history())
     summarization_input_tokens = sum(record.input_tokens for record in model._memory_manager.history())  # noqa
     summarization_response_tokens = sum(record.response_tokens for record in model._memory_manager.history())  # noqa
     assert model.input_tokens == previous_input_tokens_0 + previous_input_tokens_1 + message.input_tokens + summarization_input_tokens  # noqa
     assert model.response_tokens == previous_response_tokens_0 + previous_response_tokens_1 + message.response_tokens + summarization_response_tokens  # noqa
     assert model.total_tokens == previous_total_tokens_0 + previous_total_tokens_1 + message.total_tokens + summarization_input_tokens + summarization_response_tokens  # noqa
     assert round(model.cost, 5) == round(previous_cost_0 + previous_cost_1 + message.cost + summarization_cost, 5)  # noqa
@@ -1229,16 +1199,16 @@
     assert previous_record.metadata['model_name'] == 'text-embedding-ada-002'
 
     assert model.total_tokens == previous_tokens + previous_record.total_tokens
     assert model.cost == previous_cost + expected_cost
 
 def test_bug_where_costs_are_incorrect_after_changing_model_name_after_creation():  # noqa
     """We can't set cost_per_token during object creation, because the model might change."""
-    model = OpenAIChat(model_name='gpt-3.5-turbo')
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN['gpt-3.5-turbo']
-    model.model_name = 'gpt-4'
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN['gpt-4']
-
-    model = OpenAIEmbedding(model_name='gpt-3.5-turbo')
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN['gpt-3.5-turbo']
-    model.model_name = 'gpt-4'
-    assert model.cost_per_token == MODEL_COST_PER_TOKEN['gpt-4']
+    model = OpenAIChat()
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
+    model.model_name = 'gpt-4-1106-preview'
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN['gpt-4-1106-preview']
+
+    model = OpenAIEmbedding()
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN[model.model_name]
+    model.model_name = 'gpt-4-1106-preview'
+    assert model.cost_per_token == MODEL_COST_PER_TOKEN['gpt-4-1106-preview']
```

### Comparing `llm-workflow-0.0.6/tests/test_prompt_templates.py` & `llm-workflow-0.0.8/tests/test_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_records.py` & `llm-workflow-0.0.8/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_session.py` & `llm-workflow-0.0.8/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_utilities.py` & `llm-workflow-0.0.8/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `llm-workflow-0.0.6/tests/test_workflows.py` & `llm-workflow-0.0.8/tests/test_workflows.py`

 * *Files identical despite different names*

