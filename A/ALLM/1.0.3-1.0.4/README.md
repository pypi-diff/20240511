# Comparing `tmp/ALLM-1.0.3-py3-none-any.whl.zip` & `tmp/ALLM-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3972 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     7005 b- defN 24-May-05 10:18 ALLM-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 10:18 ALLM-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      522 b- defN 24-May-05 10:17 ALLM-1.0.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 24-May-05 10:17 ALLM-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      378 b- defN 24-May-05 10:18 ALLM-1.0.3.dist-info/RECORD
-5 files, 7998 bytes uncompressed, 3264 bytes compressed:  59.2%
+Zip file size: 4081 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     7664 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      556 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        1 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      378 b- defN 24-May-11 18:27 ALLM-1.0.4.dist-info/RECORD
+5 files, 8691 bytes uncompressed, 3373 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: ALLM-1.0.3.dist-info/METADATA
+Filename: ALLM-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ALLM-1.0.3.dist-info/WHEEL
+Filename: ALLM-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ALLM-1.0.3.dist-info/entry_points.txt
+Filename: ALLM-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLM-1.0.3.dist-info/top_level.txt
+Filename: ALLM-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLM-1.0.3.dist-info/RECORD
+Filename: ALLM-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ALLM-1.0.3.dist-info/METADATA` & `ALLM-1.0.4.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ALLM
-Version: 1.0.3
-Summary: A simple and efficient python library for fast inference of LLMs.
+Version: 1.0.4
+Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
-Maintainer: Abdul Mannan Khan
-Maintainer-email: abdulmannan.khan@allaai.com
+Maintainer: All Advance AI
+Maintainer-email: allmdev@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
 Requires-Dist: Flask
 Requires-Dist: click
 Requires-Dist: llama-index
 Requires-Dist: llama-cpp-python
 Requires-Dist: aiohttp
@@ -137,35 +137,73 @@
 ALLM supports all types of Generative LLMs on AzureOpenAI & VertexAI, including GPT(s) & Geminipro models. You can start local inference of cloud based models using the following command:
  
 ### 2.1 VertixAI Generic Prompt 
 ```bash
 allm-run-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server
 ```
 
+or 
+
+```bash
+allm-run-vertex
+```
+
 ### 2.2 AzureOpneAI Generic Prompt
 ```bash
 allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name
 ```
+
+or 
+
+```bash
+allm-run-azure
+```
  
-You can also have a custom agent working with your cloud deployed model using the following command. It is important to note that before this step, agent should be created using section: **1.1 New Agent Creation**.
+You can also have a custom agent working with your cloud deployed model using the following command. It is important to note that before this step, agent should be created using section: **1.1 New Agent Creation**. 
 
 ### 2.3 VertixAI AgentChat 
 ```bash
 allm-agentchat-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server --agent agent_name
 ```
 
-### 2.3 AzureOpenAI AgentChat 
+model\vertex-config.json needs to be configured to use below command, this will ensure projectid, region are captured.
+
+```bash
+allm-agentchat-vertex --agent agent_name
+```
+
+### 2.4 AzureOpenAI AgentChat 
+
 ```bash
-allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name --agent agentname
+allm-agentchat-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name --agent agentname
 ```
+
+model\azure-config.json needs to be configured to use below command, this will ensure endpoint, modelname etc are captured.
+
+```bash
+allm-agentchat-azure --agent agentname
+```
+
 model_name is an optional parameter in both vertex and azure, if not mentioned, inference will work on gemini-1.0-pro-002 for vertex and gpt-35-turbo for OpenAI by default.
 
+### 2.5 AzureOpenAI AgentChat API 
+
+```bash
+allm-agentapi-azure --agent agentname
+```
+
+### 2.6 AzureOpenAI AgentChat API 
+
+```bash
+allm-agentapi-vertex --agent agent_name
+```
 
 ## Supported Model names.
 
+- Llama3
 - Llama2
 - Llama
 - Llama2_chat
 - Llama_chat
 - Mistral
 - Mistral_instruct
```

## Comparing `ALLM-1.0.3.dist-info/entry_points.txt` & `ALLM-1.0.4.dist-info/entry_points.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 allm-agentchat-azure = ALLMDEV.azureagentchat:main
 allm-agentchat-vertex = ALLMDEV.vertexagentchat:main
 allm-newagent = ALLMDEV.newagent:main
 allm-run = ALLMDEV.cli:main
 allm-run-azure = ALLMDEV.azurecli:main
 allm-run-vertex = ALLMDEV.vertexcli:main
 allm-serve = ALLMDEV.serve:main
+allm-studio = ALLMDEV.studio:main
 allm-updateagent = ALLMDEV.updateagent:main
```

