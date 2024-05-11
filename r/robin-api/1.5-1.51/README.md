# Comparing `tmp/robin_api-1.5.tar.gz` & `tmp/robin_api-1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_api-1.5.tar", last modified: Fri May 10 00:48:02 2024, max compression
+gzip compressed data, was "robin_api-1.51.tar", last modified: Sat May 11 02:14:41 2024, max compression
```

## Comparing `robin_api-1.5.tar` & `robin_api-1.51.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.5/LICENSE
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.5/MANIFEST.in
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    17355 2024-05-10 00:48:02.245630 robin_api-1.5/PKG-INFO
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    16908 2024-05-10 00:44:24.000000 robin_api-1.5/README.md
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.241630 robin_api-1.5/robin_api/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-02 19:33:54.000000 robin_api-1.5/robin_api/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    12382 2024-05-07 02:08:18.000000 robin_api-1.5/robin_api/_client.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.5/robin_api/_compat.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      404 2024-04-30 23:05:14.000000 robin_api-1.5/robin_api/_constants.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.5/robin_api/_exceptions.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.5/robin_api/_models.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      951 2024-05-02 19:39:40.000000 robin_api-1.5/robin_api/_resource.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.5/robin_api/_streaming.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.5/robin_api/_types.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.241630 robin_api-1.5/robin_api/_utils/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.5/robin_api/_utils/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.5/robin_api/_utils/_utils.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/robin_api/resources/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      164 2024-05-06 00:49:45.000000 robin_api-1.5/robin_api/resources/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5050 2024-05-07 03:00:16.000000 robin_api-1.5/robin_api/resources/completions.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5855 2024-05-09 20:27:08.000000 robin_api-1.5/robin_api/resources/files.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/robin_api/types/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      902 2024-05-09 04:13:37.000000 robin_api-1.5/robin_api/types/__init__.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2025 2024-05-06 00:21:01.000000 robin_api-1.5/robin_api/types/chat_completion.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3783 2024-05-06 00:07:24.000000 robin_api-1.5/robin_api/types/chat_completion_chunk.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1241 2024-05-03 21:04:08.000000 robin_api-1.5/robin_api/types/chat_completion_message.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      866 2024-05-03 21:04:32.000000 robin_api-1.5/robin_api/types/chat_completion_message_tool_call.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.5/robin_api/types/completion.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      928 2024-05-01 17:15:49.000000 robin_api-1.5/robin_api/types/completion_choice.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.5/robin_api/types/completion_usage.py
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      529 2024-05-09 20:21:50.000000 robin_api-1.5/robin_api/types/models_robin.py
-drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-10 00:48:02.245630 robin_api-1.5/robin_api.egg-info/
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      726 2024-05-10 00:48:02.000000 robin_api-1.5/robin_api.egg-info/SOURCES.txt
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-10 00:48:02.245630 robin_api-1.5/setup.cfg
--rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      747 2024-05-10 00:47:51.000000 robin_api-1.5/setup.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-11 02:14:41.836298 robin_api-1.51/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    11337 2024-04-30 18:06:24.000000 robin_api-1.51/LICENSE
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      210 2024-05-01 19:41:22.000000 robin_api-1.51/MANIFEST.in
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18905 2024-05-11 02:14:41.836298 robin_api-1.51/PKG-INFO
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18457 2024-05-11 02:09:25.000000 robin_api-1.51/README.md
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-11 02:14:41.832298 robin_api-1.51/robin_api/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      765 2024-05-02 19:33:54.000000 robin_api-1.51/robin_api/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    12702 2024-05-11 02:11:01.000000 robin_api-1.51/robin_api/_client.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     5102 2024-04-30 23:37:44.000000 robin_api-1.51/robin_api/_compat.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      431 2024-05-10 22:23:17.000000 robin_api-1.51/robin_api/_constants.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     3573 2024-04-30 20:26:30.000000 robin_api-1.51/robin_api/_exceptions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)    18240 2024-05-01 18:18:56.000000 robin_api-1.51/robin_api/_models.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      994 2024-05-10 19:01:49.000000 robin_api-1.51/robin_api/_resource.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7217 2024-04-30 23:44:46.000000 robin_api-1.51/robin_api/_streaming.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     9696 2024-04-30 23:36:19.000000 robin_api-1.51/robin_api/_types.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-11 02:14:41.832298 robin_api-1.51/robin_api/_utils/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      219 2024-05-01 02:38:52.000000 robin_api-1.51/robin_api/_utils/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1553 2024-05-01 02:38:37.000000 robin_api-1.51/robin_api/_utils/_utils.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-11 02:14:41.832298 robin_api-1.51/robin_api/resources/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      164 2024-05-06 00:49:45.000000 robin_api-1.51/robin_api/resources/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     4551 2024-05-11 01:31:04.000000 robin_api-1.51/robin_api/resources/completions.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     7147 2024-05-11 01:28:51.000000 robin_api-1.51/robin_api/resources/files.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-11 02:14:41.836298 robin_api-1.51/robin_api/types/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1060 2024-05-11 01:24:36.000000 robin_api-1.51/robin_api/types/__init__.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     2025 2024-05-06 00:21:01.000000 robin_api-1.51/robin_api/types/chat_completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     4007 2024-05-11 01:35:29.000000 robin_api-1.51/robin_api/types/chat_completion_chunk.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1241 2024-05-03 21:04:08.000000 robin_api-1.51/robin_api/types/chat_completion_message.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      866 2024-05-03 21:04:32.000000 robin_api-1.51/robin_api/types/chat_completion_message_tool_call.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)     1139 2024-05-01 16:49:41.000000 robin_api-1.51/robin_api/types/completion.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      928 2024-05-01 17:15:49.000000 robin_api-1.51/robin_api/types/completion_choice.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      401 2024-05-01 00:30:19.000000 robin_api-1.51/robin_api/types/completion_usage.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      560 2024-05-11 00:31:31.000000 robin_api-1.51/robin_api/types/file_model.py
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      354 2024-05-11 00:24:24.000000 robin_api-1.51/robin_api/types/models_robin.py
+drwxrwxr-x   0 wgomez    (1000) wgomez    (1000)        0 2024-05-11 02:14:41.836298 robin_api-1.51/robin_api.egg-info/
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      756 2024-05-11 02:14:41.000000 robin_api-1.51/robin_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)       38 2024-05-11 02:14:41.836298 robin_api-1.51/setup.cfg
+-rw-rw-r--   0 wgomez    (1000) wgomez    (1000)      748 2024-05-11 02:14:17.000000 robin_api-1.51/setup.py
```

### Comparing `robin_api-1.5/LICENSE` & `robin_api-1.51/LICENSE`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/PKG-INFO` & `robin_api-1.51/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: robin_api
-Version: 1.5
-Summary: file
-Home-page: https://github.com/williamgomez71/RobinApi
-Author: William Gomez
-Author-email: william.gomez712@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # RobinApi Framework
 
 **Description:**  
 RobinApi Framework is a comprehensive solution designed to facilitate efficient interaction with Large Language Model (LLM) APIs and advanced vector data management. This framework provides robust tools for uploading and storing files in an optimized vector database, allowing users to fully leverage content-based search and retrieval. Users can upload documents via the API, which are then stored in a vector database, enabling them to query for the most similar phrases. Moreover, RobinApi Framework includes dedicated endpoints for complex queries, enabling users to extract valuable insights and conduct in-depth analyses of the stored data. Ideal for developers looking to integrate LLM capabilities into their applications and efficiently manage large volumes of data, RobinApi Framework stands out for its flexibility, scalability, and ease of use.
 
 **Key Features:**
 
@@ -40,26 +24,30 @@
 
 
 
 ## Example code
 
 ### Example Code
 
-**1. Creating a Stream of Responses**
+**Creating a Stream of Responses**
+
+Set an environment variable in your os:
+Linux
+export API_KEY="API_KEY"
+Windows
+setx API_KEY "YourAPIKeyHere"
 
 ```python
 from robin_api import RobinAIClient
 
-# Initialize the client with an API key
-client = RobinAIClient(api_key="API_KEY")
 
+#This step is not necesary if you set this environment variable in your os
+client = RobinAIClient(api_key="API_KEY")
 ### Example Code
 
-**1. Creating a Stream of Responses**
-
 
 from robin_api import RobinAIClient
 
 # Initialize the client with an API key
 client = RobinAIClient(api_key="API_KEY")
 
 # Create a conversation prompt
@@ -80,21 +68,29 @@
     conversation=value, 
     max_tokens=512, 
     stream=True, 
     save_response=False, 
     temperature=1
 )
 
-# Print each chunk of the streamed response
+# Print each chunk of the streamed response and the end print the metrics
+stream = client.completions.create_stream(model="ROBIN_4", 
+                            conversation = value, 
+                            max_tokens = 512, 
+                            save_response = False,
+                            temperature=1)
+
 for chunk in stream:
-    if chunk.choices[0].delta.content is not None:
+    if not chunk.choices[0].finish_reason:
         print(chunk.choices[0].delta.content, end="")
+    else:
+        print(chunk.details, end="")
 ```
 
-2. Generating a Complete Response 
+**Generating a Complete Response**
 
 
 ```python
 response = client.completions.create(
     model="ROBIN_4",
     conversation=value, 
     max_tokens=512, 
@@ -118,16 +114,15 @@
 - **save_response**: If `False`, does not store the response in persistent storage.
 
 - **temperature**: Controls the randomness of responses; values close to 1 are more diverse.
 
 
 
 
-
-3. Upload a file from a web URL
+**Upload a file from a web URL file**
 
 ```python
 
 folder_information = client.files.upload_file(url="https://arxiv.org/pdf/2302.13971.pdf")
 
 # Example response
 {
@@ -149,15 +144,98 @@
 
 **Parameters:**
 
 - **url**:  URL of the document to upload.
 
 
 
-4. Finding Similar Sentences in the Folder
+
+**Upload Web Page information Function**
+This function allows uploading information from a web page into the system, storing the relevant data in an organized structure for subsequent analysis and retrieva
+
+```python
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1
+)
+
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1,
+    folder_id="112ccd00-3814-4f1e-975d-adsflkj6l"
+)
+
+
+```
+**Parameters:**
+
+- **url**: The URL of the web page from which to extract information.
+
+- **deep_level** (optional): The depth level for data extraction. A higher value results in more exhaustive exploration.
+  - **Accepted Values**: `1`, `2`, `3`.
+  - **Default**: `1`.
+
+- **folder_id** (optional): The folder ID where the extracted information will be stored. If not specified, a new folder will be created.
+
+**Response Structure:**
+
+```python
+ApiResponse(
+    status_code=200,
+    message={
+        'folder': {
+            'apiFolderId': '112ccd00-3814-4f1e-975d-094974d2b89d',
+            'createdAt': '2024-05-09T20:26:55.000000Z'
+        },
+        'file': {
+            'url': 'https://example.com',
+            'tokens': None,
+            'documentId': None,
+            'createdAt': '2024-05-09T20:29:12.000000Z'
+        }
+    }
+)
+```
+
+
+- **folder**: Contains details about the folder where the web page data is stored.
+  - **apiFolderId**: The unique identifier of the folder created or used for storing the extracted information.
+  - **createdAt**: The timestamp indicating when the folder was created, in ISO 8601 format.
+
+- **file**: Provides information about the extracted web page.
+  - **url**: The URL of the web page that was uploaded for data extraction.
+  - **tokens**: This field will be populated once the indexing process is complete, representing the total number of tokens extracted from the web page content.
+  - **documentId**: Will be created after indexing, serving as a unique identifier for the document.
+  - **createdAt**: The timestamp indicating when the file was created, in ISO 8601 format.
+
+
+**Upload local files**
+
+```python
+folder_information = client.files.upload_local_file(file="./LICENSE", purpose="store in datalake")
+print(folder_information)
+print(folder_information.file_id) 
+```
+**Parameters:**
+
+- **file**: Path of the local file to be uploaded.
+- **purpose**: Description of the purpose for uploading the file, such as "store in datalake".
+
+
+**Index in vector database documents by Id**
+
+folder_information = client.files.upload_file(file_id="6488ea82-2688-4307-a4d7-fd97e0ac5b2a") 
+print(folder_information)
+
+**Parameters:**
+- **file_id**: The unique identifier of the file already stored in the cloud that you wish to operate on or manage.
+
+
+
+**Finding Similar Sentences in the Folder**
 
 ```python
 
 similar_sentences = client.files.get_similar_sentences( 
     query = "What are the practical implications of the findings in the document?",
     top = 15,
     api_folder_id = "83273a99-f722-4d92-8261-bf6a29735782",
@@ -203,15 +281,15 @@
     ]
 }
 ```
 
 
 
 
-5. Getting Context-Based Responses from the Folder
+**Getting Context-Based Responses from the Folder**
 
 ```python
 answer = client.files.get_response_similar_sentences(
     model="ROBIN_4",
     max_new_tokens = 200,
     top = 15,
     api_folder_id = "17206d13-594c-4e70-a627-24ad26d1c869",
@@ -262,71 +340,30 @@
         "completion_tokens": 76,
         "prompt_tokens": 2915,
         "total_tokens": 2991
     }
 }
 ```
 
-
-6. Upload Web Page information Function
-This function allows uploading information from a web page into the system, storing the relevant data in an organized structure for subsequent analysis and retrieva
+**Getting Context-Based stream response from the Folder**
 
 ```python
-folder_information = client.files.upload_web_page_information(
-    url="https://web.com/example",
-    deep_level=1
-)
-
-folder_information = client.files.upload_web_page_information(
-    url="https://web.com/example",
-    deep_level=1,
-    folder_id="112ccd00-3814-4f1e-975d-adsflkj6l"
-)
-
-
-```
-**Parameters:**
-
-- **url**: The URL of the web page from which to extract information.
-
-- **deep_level** (optional): The depth level for data extraction. A higher value results in more exhaustive exploration.
-  - **Accepted Values**: `1`, `2`, `3`.
-  - **Default**: `1`.
-
-- **folder_id** (optional): The folder ID where the extracted information will be stored. If not specified, a new folder will be created.
-
-**Response Structure:**
+stream = client.files.get_response_similar_sentences_stream(
+    model="ROBIN_4",
+    max_new_tokens = 200,
+    top = 1,
+    api_folder_id = "17206d13-594c-4e70-a627-24asdfas",
+    similarity_threshold = 0.4,
+    conversation=value,
+    only_with_context = True)
 
-```python
-ApiResponse(
-    status_code=200,
-    message={
-        'folder': {
-            'apiFolderId': '112ccd00-3814-4f1e-975d-094974d2b89d',
-            'createdAt': '2024-05-09T20:26:55.000000Z'
-        },
-        'file': {
-            'url': 'https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset',
-            'tokens': None,
-            'documentId': None,
-            'createdAt': '2024-05-09T20:29:12.000000Z'
-        }
-    }
-)
+for chunk in stream:
+    if not chunk.choices[0].finish_reason:
+        print(chunk.choices[0].delta.content, end="")
+    else:
+        print(chunk.details, end="")
 ```
 
 
-- **folder**: Contains details about the folder where the web page data is stored.
-  - **apiFolderId**: The unique identifier of the folder created or used for storing the extracted information.
-  - **createdAt**: The timestamp indicating when the folder was created, in ISO 8601 format.
-
-- **file**: Provides information about the extracted web page.
-  - **url**: The URL of the web page that was uploaded for data extraction.
-  - **tokens**: This field will be populated once the indexing process is complete, representing the total number of tokens extracted from the web page content.
-  - **documentId**: Will be created after indexing, serving as a unique identifier for the document.
-  - **createdAt**: The timestamp indicating when the file was created, in ISO 8601 format.
-
-
-
```

### Comparing `robin_api-1.5/README.md` & `robin_api-1.51/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: robin_api
+Version: 1.51
+Summary: file
+Home-page: https://github.com/williamgomez71/RobinApi
+Author: William Gomez
+Author-email: william.gomez712@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # RobinApi Framework
 
 **Description:**  
 RobinApi Framework is a comprehensive solution designed to facilitate efficient interaction with Large Language Model (LLM) APIs and advanced vector data management. This framework provides robust tools for uploading and storing files in an optimized vector database, allowing users to fully leverage content-based search and retrieval. Users can upload documents via the API, which are then stored in a vector database, enabling them to query for the most similar phrases. Moreover, RobinApi Framework includes dedicated endpoints for complex queries, enabling users to extract valuable insights and conduct in-depth analyses of the stored data. Ideal for developers looking to integrate LLM capabilities into their applications and efficiently manage large volumes of data, RobinApi Framework stands out for its flexibility, scalability, and ease of use.
 
 **Key Features:**
 
@@ -24,26 +40,30 @@
 
 
 
 ## Example code
 
 ### Example Code
 
-**1. Creating a Stream of Responses**
+**Creating a Stream of Responses**
+
+Set an environment variable in your os:
+Linux
+export API_KEY="API_KEY"
+Windows
+setx API_KEY "YourAPIKeyHere"
 
 ```python
 from robin_api import RobinAIClient
 
-# Initialize the client with an API key
-client = RobinAIClient(api_key="API_KEY")
 
+#This step is not necesary if you set this environment variable in your os
+client = RobinAIClient(api_key="API_KEY")
 ### Example Code
 
-**1. Creating a Stream of Responses**
-
 
 from robin_api import RobinAIClient
 
 # Initialize the client with an API key
 client = RobinAIClient(api_key="API_KEY")
 
 # Create a conversation prompt
@@ -64,21 +84,29 @@
     conversation=value, 
     max_tokens=512, 
     stream=True, 
     save_response=False, 
     temperature=1
 )
 
-# Print each chunk of the streamed response
+# Print each chunk of the streamed response and the end print the metrics
+stream = client.completions.create_stream(model="ROBIN_4", 
+                            conversation = value, 
+                            max_tokens = 512, 
+                            save_response = False,
+                            temperature=1)
+
 for chunk in stream:
-    if chunk.choices[0].delta.content is not None:
+    if not chunk.choices[0].finish_reason:
         print(chunk.choices[0].delta.content, end="")
+    else:
+        print(chunk.details, end="")
 ```
 
-2. Generating a Complete Response 
+**Generating a Complete Response**
 
 
 ```python
 response = client.completions.create(
     model="ROBIN_4",
     conversation=value, 
     max_tokens=512, 
@@ -102,16 +130,15 @@
 - **save_response**: If `False`, does not store the response in persistent storage.
 
 - **temperature**: Controls the randomness of responses; values close to 1 are more diverse.
 
 
 
 
-
-3. Upload a file from a web URL
+**Upload a file from a web URL file**
 
 ```python
 
 folder_information = client.files.upload_file(url="https://arxiv.org/pdf/2302.13971.pdf")
 
 # Example response
 {
@@ -133,15 +160,98 @@
 
 **Parameters:**
 
 - **url**:  URL of the document to upload.
 
 
 
-4. Finding Similar Sentences in the Folder
+
+**Upload Web Page information Function**
+This function allows uploading information from a web page into the system, storing the relevant data in an organized structure for subsequent analysis and retrieva
+
+```python
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1
+)
+
+folder_information = client.files.upload_web_page_information(
+    url="https://web.com/example",
+    deep_level=1,
+    folder_id="112ccd00-3814-4f1e-975d-adsflkj6l"
+)
+
+
+```
+**Parameters:**
+
+- **url**: The URL of the web page from which to extract information.
+
+- **deep_level** (optional): The depth level for data extraction. A higher value results in more exhaustive exploration.
+  - **Accepted Values**: `1`, `2`, `3`.
+  - **Default**: `1`.
+
+- **folder_id** (optional): The folder ID where the extracted information will be stored. If not specified, a new folder will be created.
+
+**Response Structure:**
+
+```python
+ApiResponse(
+    status_code=200,
+    message={
+        'folder': {
+            'apiFolderId': '112ccd00-3814-4f1e-975d-094974d2b89d',
+            'createdAt': '2024-05-09T20:26:55.000000Z'
+        },
+        'file': {
+            'url': 'https://example.com',
+            'tokens': None,
+            'documentId': None,
+            'createdAt': '2024-05-09T20:29:12.000000Z'
+        }
+    }
+)
+```
+
+
+- **folder**: Contains details about the folder where the web page data is stored.
+  - **apiFolderId**: The unique identifier of the folder created or used for storing the extracted information.
+  - **createdAt**: The timestamp indicating when the folder was created, in ISO 8601 format.
+
+- **file**: Provides information about the extracted web page.
+  - **url**: The URL of the web page that was uploaded for data extraction.
+  - **tokens**: This field will be populated once the indexing process is complete, representing the total number of tokens extracted from the web page content.
+  - **documentId**: Will be created after indexing, serving as a unique identifier for the document.
+  - **createdAt**: The timestamp indicating when the file was created, in ISO 8601 format.
+
+
+**Upload local files**
+
+```python
+folder_information = client.files.upload_local_file(file="./LICENSE", purpose="store in datalake")
+print(folder_information)
+print(folder_information.file_id) 
+```
+**Parameters:**
+
+- **file**: Path of the local file to be uploaded.
+- **purpose**: Description of the purpose for uploading the file, such as "store in datalake".
+
+
+**Index in vector database documents by Id**
+
+folder_information = client.files.upload_file(file_id="6488ea82-2688-4307-a4d7-fd97e0ac5b2a") 
+print(folder_information)
+
+**Parameters:**
+- **file_id**: The unique identifier of the file already stored in the cloud that you wish to operate on or manage.
+
+
+
+**Finding Similar Sentences in the Folder**
 
 ```python
 
 similar_sentences = client.files.get_similar_sentences( 
     query = "What are the practical implications of the findings in the document?",
     top = 15,
     api_folder_id = "83273a99-f722-4d92-8261-bf6a29735782",
@@ -187,15 +297,15 @@
     ]
 }
 ```
 
 
 
 
-5. Getting Context-Based Responses from the Folder
+**Getting Context-Based Responses from the Folder**
 
 ```python
 answer = client.files.get_response_similar_sentences(
     model="ROBIN_4",
     max_new_tokens = 200,
     top = 15,
     api_folder_id = "17206d13-594c-4e70-a627-24ad26d1c869",
@@ -246,69 +356,32 @@
         "completion_tokens": 76,
         "prompt_tokens": 2915,
         "total_tokens": 2991
     }
 }
 ```
 
-
-6. Upload Web Page information Function
-This function allows uploading information from a web page into the system, storing the relevant data in an organized structure for subsequent analysis and retrieva
+**Getting Context-Based stream response from the Folder**
 
 ```python
-folder_information = client.files.upload_web_page_information(
-    url="https://web.com/example",
-    deep_level=1
-)
-
-folder_information = client.files.upload_web_page_information(
-    url="https://web.com/example",
-    deep_level=1,
-    folder_id="112ccd00-3814-4f1e-975d-adsflkj6l"
-)
-
-
-```
-**Parameters:**
-
-- **url**: The URL of the web page from which to extract information.
-
-- **deep_level** (optional): The depth level for data extraction. A higher value results in more exhaustive exploration.
-  - **Accepted Values**: `1`, `2`, `3`.
-  - **Default**: `1`.
-
-- **folder_id** (optional): The folder ID where the extracted information will be stored. If not specified, a new folder will be created.
-
-**Response Structure:**
+stream = client.files.get_response_similar_sentences_stream(
+    model="ROBIN_4",
+    max_new_tokens = 200,
+    top = 1,
+    api_folder_id = "17206d13-594c-4e70-a627-24asdfas",
+    similarity_threshold = 0.4,
+    conversation=value,
+    only_with_context = True)
 
-```python
-ApiResponse(
-    status_code=200,
-    message={
-        'folder': {
-            'apiFolderId': '112ccd00-3814-4f1e-975d-094974d2b89d',
-            'createdAt': '2024-05-09T20:26:55.000000Z'
-        },
-        'file': {
-            'url': 'https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset',
-            'tokens': None,
-            'documentId': None,
-            'createdAt': '2024-05-09T20:29:12.000000Z'
-        }
-    }
-)
+for chunk in stream:
+    if not chunk.choices[0].finish_reason:
+        print(chunk.choices[0].delta.content, end="")
+    else:
+        print(chunk.details, end="")
 ```
 
 
-- **folder**: Contains details about the folder where the web page data is stored.
-  - **apiFolderId**: The unique identifier of the folder created or used for storing the extracted information.
-  - **createdAt**: The timestamp indicating when the folder was created, in ISO 8601 format.
 
-- **file**: Provides information about the extracted web page.
-  - **url**: The URL of the web page that was uploaded for data extraction.
-  - **tokens**: This field will be populated once the indexing process is complete, representing the total number of tokens extracted from the web page content.
-  - **documentId**: Will be created after indexing, serving as a unique identifier for the document.
-  - **createdAt**: The timestamp indicating when the file was created, in ISO 8601 format.
```

### Comparing `robin_api-1.5/robin_api/__init__.py` & `robin_api-1.51/robin_api/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/_client.py` & `robin_api-1.51/robin_api/_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 from ._exceptions import RobinError
 import json
 from .types import ApiResponse 
 __all__ = [
     "RobinAIClient",
 ]
 
+""" import logging
+logging.basicConfig(level=logging.DEBUG)
+logger = logging.getLogger("httpx")
+logger.setLevel(logging.DEBUG) """
+
 
 def _merge_mappings(
     obj1,
     obj2,
 ):
     """Merge two mappings of the same type, removing any values that are instances of `Omit`.
     In cases with duplicate keys the second mapping takes precedence.
@@ -243,92 +248,98 @@
 
         self.api_key = api_key
 
         if base_url is None:
             self.base_url = f"https://robin-ai.xyz:8443/api/api-response-service/"
 
         self._default_stream_cls = Stream
-        headers = self._build_headers()
+        self.headers = self._build_headers()
+        proxies = {
+        "http://": "http://localhost:8080",
+        "https://": "http://localhost:8080"
+        }
         self.http_client = http_client or httpx.Client(
             base_url=self.base_url,
-            # cast to a valid type because mypy doesn't understand our type narrowing
             timeout=timeout,
             verify=False,
-            headers=headers
+            headers=self.headers,
+            #proxies= proxies
         )
 
         self.completions = resources.Completions(self)
         self.files = resources.Files(self)
          
         #self.completions_based_text: resources.Completions
         #self.upload_file: resources.Completions
         #self.models: resources.Models
         #self.fine_tuning: resources.FineTuning
 
 
     def _build_headers(self) -> httpx.Headers:
         headers_dict = _merge_mappings(self.default_headers, self.auth_headers)
         headers_dict = _merge_mappings(headers_dict, self.platform_headers())
-        headers = httpx.Headers(headers_dict)
-        return headers
+        #headers = httpx.Headers(headers_dict)
+        return headers_dict
     
     def platform_headers(self) -> Dict[str, str]:
         return {
             "X-Stainless-Lang": "python",
             #"X-Stainless-Package-Version": self._version,
             "X-Stainless-OS": str(get_platform()),
             "X-Stainless-Arch": str(get_architecture()),
             "X-Stainless-Runtime": platform.python_implementation(),
             "X-Stainless-Runtime-Version": platform.python_version(),
         }
     
     def stream(self, end_point: str, body: json, method: str="POST"):
         self.create_new_client()
-        print(self.http_client.is_closed)
-        
-        print(self.http_client.is_closed)
-        print(self.http_client.is_closed)
-        print(self.http_client._state)
-        print(self.http_client._state)
         with self.http_client.stream(
             url = end_point,
             #url = "https://localhost:8443/api/api-response-service/get-response",
             method=method,
             json= body,
             ) as response:
             if response.status_code == 200:
-                print(response.status_code)
                 for data in response.iter_bytes():
                     json_part = data.decode('utf-8').split("data: ", 1)[1]
                     if json_part.startswith("DONE"):
                         break
                     objeto = json.loads(json_part)
                     yield objeto                   
             else:
                 err = self._make_status_error_from_response(response)
-                print(err)
                 return err
 
             
     def post(self, end_point: str, body: json):
         self.create_new_client()
         with self.http_client as client:
             response = client.post(
             url = end_point,
-            #url = "https://localhost:8443/api/api-response-service/get-response",
             json = body,
             )
             if response.status_code == 200:
                 return ApiResponse (message=response.json(), status_code=200)
             else:
                 err = self._make_status_error_from_response(response)
-                print(err)
+                return err
+            
+    def post_form(self, end_point: str, file):
+        self.create_new_client()
+        with self.http_client as client:
+            response = client.post(
+                url = self.base_url + end_point,
+                files = file,
+                )
+            if response.status_code == 200:
+                return ApiResponse (message=response.json(), status_code=200)
+            else:
+                err = self._make_status_error_from_response(response)
                 return err
     
-
     def _make_status_error_from_response(
         self,
         response: httpx.Response,
     ) -> ApiResponse:
         if hasattr(response, 'read') and callable(getattr(response, 'read')):
             err_text = str(response.read().decode('utf-8'))
         else:
```

### Comparing `robin_api-1.5/robin_api/_compat.py` & `robin_api-1.51/robin_api/_compat.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/_exceptions.py` & `robin_api-1.51/robin_api/_exceptions.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/_models.py` & `robin_api-1.51/robin_api/_models.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/_resource.py` & `robin_api-1.51/robin_api/_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class SyncAPIResource:
     _client: RobinAIClient
 
     def __init__(self, client: RobinAIClient) -> None:
         self._client = client
         self._stream = client.stream
         self._post = client.post
+        self._post_form = client.post_form
 
     def _sleep(self, seconds: float) -> None:
         time.sleep(seconds)
 
 #TODO
 class AsyncAPIResource:
     _client: AsyncRobinAIClient
```

### Comparing `robin_api-1.5/robin_api/_streaming.py` & `robin_api-1.51/robin_api/_streaming.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/_types.py` & `robin_api-1.51/robin_api/_types.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/_utils/_utils.py` & `robin_api-1.51/robin_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/resources/completions.py` & `robin_api-1.51/robin_api/resources/completions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 
 from typing import TYPE_CHECKING, List, Union, Optional, Iterator
-from ..types import Completion, ChatCompletionChunk, ChatCompletion, ApiResponse, Models
+from ..types import Completion, ChatCompletionChunk, ChatCompletion, ApiResponse, Models, MetricsChunk
 from .._streaming import Stream
 from typing_extensions import Literal
 import httpx
 from .._types import NOT_GIVEN, NotGiven
 from .._resource import SyncAPIResource
 from .._models import construct_type, construct_type_v2
 
@@ -36,15 +36,15 @@
         model: Models,
         conversation: Union[str, List[str], List[int], List[List[int]], None],
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
         save_response: Optional[Literal[False]] | Literal[True] | NotGiven = NOT_GIVEN,
         temperature: Optional[float] | NotGiven = NOT_GIVEN,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
 
-    ) -> Completion | Stream[Completion] | Iterator[Stream[Completion]]:
+    ) -> Completion | Stream[Completion] | Iterator[ChatCompletionChunk] | Iterator[MetricsChunk]:
 
         body_request= {
                     "model": model,
                     "conversation": conversation,
                     "max_new_tokens": max_tokens,
                     "stream": True,
                     "temperature": temperature,
@@ -52,16 +52,20 @@
                 }
         response = self._stream(
             end_point = "get-response",
             body= body_request,
             )
         for data in response:
             ensure_list(data, 'choices')
-            completion_obj = construct_type_v2(type_=ChatCompletionChunk, value=data)
-            yield completion_obj
+            if not ('details' in data.keys()):
+                completion_obj = construct_type_v2(type_=ChatCompletionChunk, value=data)
+                yield completion_obj
+            else:
+                completion_obj = construct_type_v2(type_=MetricsChunk, value=data)
+                yield completion_obj
 
     def create(
         self,
         *,
         model: Models,
         conversation: Union[str, List[str], List[int], List[List[int]], None],
         max_tokens: Optional[int] | NotGiven = NOT_GIVEN,
@@ -80,38 +84,15 @@
                     }
 
         value : ApiResponse = self._post(
                 end_point = "get-response",
                 body= body_request,
                 ) 
         if value.status_code == 200:
-            value2 = {
-            "choices": [
-                {
-                "finish_reason": "stop",
-                "index": 0,
-                "message": {
-                    "content": "The 2020 World Series was played in Texas at Globe Life Field in Arlington.",
-                    "role": "assistant"
-                },
-                "logprobs": None
-                }
-            ],
-            "created": 1677664795,
-            "id": "chatcmpl-7QyqpwdfhqwajicIEznoc6Q47XAyW",
-            "model": "Robin-4",
-            "object": "chat.completion",
-            "usage": {
-                "completion_tokens": 17,
-                "prompt_tokens": 57,
-                "total_tokens": 74
-            }
-            }
             ensure_list(value.message, 'choices')
-
             completion_obj = construct_type_v2(type_=ChatCompletion, value=value.message)
 
             return completion_obj
         else:
             return value
```

### Comparing `robin_api-1.5/robin_api/resources/files.py` & `robin_api-1.51/robin_api/resources/files.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,88 @@
 
 
 
 from typing import TYPE_CHECKING
-from ..types import Models, DeepLevel
 from .._resource import SyncAPIResource
 from .._models import construct_type_v2
 from ..types import ApiResponse
-from typing import TYPE_CHECKING, Dict, List, Union, Optional, overload, Iterator
-from ..types import  ChatCompletionChunk, ChatCompletion
+from typing import TYPE_CHECKING, Iterator
+from ..types import  ChatCompletionChunk, ChatCompletion, FilesModel, Models, DeepLevel, IndexFile, MetricsChunk
 import validators
 from typing_extensions import Literal
-
+from .._models import BaseModel
+from typing import  Optional
 
 if TYPE_CHECKING:
     from .._client import RobinAIClient
 
 __all__ = ["Files"]
 
 
 def ensure_list(value, key):
     if key in value and not isinstance(value[key], list):
         value[key] = [value[key]]
 
 
 
+class CLIFileCreateArgs(BaseModel):
+    file: str
+    purpose: str
+
+
 class Files(SyncAPIResource):
     #from .._client import RobinAIClient
     def __init__(self, client) -> None:
         super().__init__(client)
 
     #def upload_web_page_information(self, args: DeepLevel):
 
-    def _upload_file(self, args: DeepLevel):
-
-
-        args = DeepLevel(args)    
-        if not validators.url(args.url):
-            raise ValueError("url is not valid")
+    def upload_file(self, *, url: Optional[str] = None, file_id: Optional[str] = None, folder_id: Optional[str] = None):
+        # Verifica que 'url' y 'file_id' no existan ambos al mismo tiempo
+        if url and file_id:
+            raise ValueError("Only 'url' or 'file_id' but no both.")
+ 
+        if not url and not file_id:
+            raise ValueError("You must provide either 'url' or 'file_id'. At least one is required.")
+    
+        args = IndexFile(url=url,file_id=file_id,folder_id=folder_id)
+        body_request = {}
+        if args.url != None:
+            if not validators.url(args.url):
+                raise ValueError("url is not valid")
+            body_request = {"fileUrl": args.url}
+        else:
+            body_request = {"fileId": args.file_id}
 
-        if args.folder_id == None:
-            body_request= {
-                            "fileUrl": args.url
-                        }
-        else:
-            body_request= {
-                            "fileUrl": args.url,
-                            "apiFolderId": args.folder_id
-                        }
+        if args.folder_id is not None:
+            body_request["apiFolderId"]= args.folder_id
         
         value : ApiResponse = self._post(
                 end_point = "folders",
                 body= body_request,
                 ) 
         if value.status_code == 200:
             return value
         else:
             return value
+      
+    def upload_local_file(self, file:str, purpose:str) -> FilesModel | ApiResponse:
+        args = CLIFileCreateArgs(file=file,purpose=purpose)
+        with open(args.file, 'rb') as file:
+            files = {'file': (args.file, file)}
+            value : ApiResponse = self._post_form(
+                    end_point = "upload-file",
+                    file= files,
+                    ) 
+            if value.status_code == 200:
+                return construct_type_v2(type_=FilesModel, value=value.message)
+            else:
+                return value
     
+
     def upload_web_page_information(self, *, url: str, deep_level: Literal[1, 2, 3] = 1 , folder_id=None):
         args = DeepLevel(url=url, deep_level=deep_level, folder_id=folder_id)  
         #if not isinstance(deep_level, DeepLevel):
         #    raise ValueError("deep_level must have values between 1 and 3")
 
         if not validators.url(url):
             raise ValueError("url is not valid")
@@ -140,15 +162,15 @@
                                        api_folder_id:str, 
                                        model:Models,
                                        only_with_context: bool, 
                                        top: int = 10, 
                                        similarity_threshold: 
                                        float = 0.4, 
                                        max_new_tokens: 512,
-                                       save_response: bool = False) -> Iterator[ChatCompletion]:
+                                       save_response: bool = False) -> Iterator[ChatCompletion] | Iterator[MetricsChunk]:
         body_request= { 
             "max_new_tokens": max_new_tokens,
             "stream" : True,
             "model" : model,
             "conversation" : conversation,
             "top": top,
             "folder_id": api_folder_id,
@@ -159,16 +181,22 @@
 
         response = self._stream(
         end_point = "get-response",
         body= body_request,
         )
         for data in response:
             ensure_list(data, 'choices')
-            completion_obj = construct_type_v2(type_=ChatCompletionChunk, value=data)
-            yield completion_obj
+            if not ('details' in data.keys()):
+                completion_obj = construct_type_v2(type_=ChatCompletionChunk, value=data)
+                yield completion_obj
+            else:
+                completion_obj = construct_type_v2(type_=MetricsChunk, value=data)
+                yield completion_obj
+
+
```

### Comparing `robin_api-1.5/robin_api/types/chat_completion.py` & `robin_api-1.51/robin_api/types/chat_completion.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/types/chat_completion_chunk.py` & `robin_api-1.51/robin_api/types/chat_completion_chunk.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 __all__ = [
     "ChatCompletionChunk",
     "Choice",
     "ChoiceDelta",
     "ChoiceDeltaFunctionCall",
     "ChoiceDeltaToolCall",
     "ChoiceDeltaToolCallFunction",
+    "Metrics",
+    "MetricsChunk",
 ]
 
 
 class ChoiceDeltaFunctionCall(BaseModel):
     arguments: Optional[str] = None
     """
     The arguments to call the function with, as generated by the model in JSON
@@ -67,15 +69,15 @@
     role: Optional[Literal["system", "user", "assistant", "tool"]] = None
     """The role of the author of this message."""
 
     tool_calls: Optional[List[ChoiceDeltaToolCall]] = None
 
 
 class Choice(BaseModel):
-    delta: ChoiceDelta
+    delta: Optional[ChoiceDelta] = None
     """A chat completion delta generated by streamed model responses."""
 
     finish_reason: Optional[Literal["stop", "length", "tool_calls", "content_filter", "function_call", False, "false", True, "true"]]
     """The reason the model stopped generating tokens.
 
     This will be `stop` if the model hit a natural stop point or a provided stop
     sequence, `length` if the maximum number of tokens specified in the request was
@@ -113,8 +115,16 @@
     system_fingerprint: Optional[str] = None
     """
     This fingerprint represents the backend configuration that the model runs with.
     Can be used in conjunction with the `seed` request parameter to understand when
     backend changes have been made that might impact determinism.
     """
 
-
+class Metrics(BaseModel):
+    cost: float
+    tokens_generated: int
+    tokens_input: int
+    
+
+class MetricsChunk(BaseModel):
+    details: Metrics
+    choices: List[Choice]
```

### Comparing `robin_api-1.5/robin_api/types/chat_completion_message.py` & `robin_api-1.51/robin_api/types/chat_completion_message.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/types/chat_completion_message_tool_call.py` & `robin_api-1.51/robin_api/types/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/types/completion.py` & `robin_api-1.51/robin_api/types/completion.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/types/completion_choice.py` & `robin_api-1.51/robin_api/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `robin_api-1.5/robin_api/types/models_robin.py` & `robin_api-1.51/robin_api/types/file_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
 
 from .._models import BaseModel
 from typing import  Union
 from typing_extensions import Literal
 from typing import Any, Optional, cast
 
-__all__ = ["Models", "DeepLevel"]
+__all__ = ["FilesModel" , "IndexFile", "DeepLevel"]
+
+        
+class FilesModel(BaseModel):
+        file_id: str
+
+
+class IndexFile(BaseModel):
+        url: Optional[str]
+        folder_id: Optional[Any]=None
+        file_id: Optional[str]
 
-class Models(BaseModel):
-        model: Union[
-            str,
-            Literal[
-                "ROBIN_4",
-                "ROBIN_3",
-            ],
-        ]
 
 class DeepLevel(BaseModel):
         url: str
         folder_id: Optional[Any]=None
         deep_level:  Literal[
                 1,
                 2,
                 3
-            ]
-        
+            ]
```

### Comparing `robin_api-1.5/robin_api.egg-info/SOURCES.txt` & `robin_api-1.51/robin_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 robin_api/types/chat_completion.py
 robin_api/types/chat_completion_chunk.py
 robin_api/types/chat_completion_message.py
 robin_api/types/chat_completion_message_tool_call.py
 robin_api/types/completion.py
 robin_api/types/completion_choice.py
 robin_api/types/completion_usage.py
+robin_api/types/file_model.py
 robin_api/types/models_robin.py
```

### Comparing `robin_api-1.5/setup.py` & `robin_api-1.51/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 #packages=find_packages()
 #packages=['robin_api'],
 setup(
     name='robin_api',
-    version='1.5',
+    version='1.51',
     packages=find_packages(),
     description="file",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'httpx',
         'pydantic',
```

