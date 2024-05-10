# Comparing `tmp/llama_tools-0.1.7.tar.gz` & `tmp/llama_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.7.tar` & `llama_tools-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.7/.gitignore
--rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.7/README.md
--rw-r--r--   0        0        0      314 2024-05-10 23:32:46.382393 llama_tools-0.1.7/llama_tools/__init__.py
--rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.7/llama_tools/postprocess.py
--rw-r--r--   0        0        0    11383 2024-05-10 23:10:08.253217 llama_tools-0.1.7/llama_tools/preprocess.py
--rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.8/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.8/README.md
+-rw-r--r--   0        0        0      314 2024-05-10 23:43:55.565535 llama_tools-0.1.8/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.8/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    11653 2024-05-10 23:43:47.066015 llama_tools-0.1.8/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.8/PKG-INFO
```

### Comparing `llama_tools-0.1.7/llama_tools/postprocess.py` & `llama_tools-0.1.8/llama_tools/postprocess.py`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.7/llama_tools/preprocess.py` & `llama_tools-0.1.8/llama_tools/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,19 @@
     func_observation_map = {}
     processed_msg = []
 
     for i in range(len(messages)):
         if messages[i]["role"] != "tool" and len(func_observation_map) > 0:
             # Insert the observation from the tool call before the next message
             func_observation_array = list(func_observation_map.values())
+            for i,a in enumerate(func_observation_array):
+                if a == "":
+                    func_observation_array[i] = "Empty Result"
             observation_str = json.dumps(func_observation_array)
+            
             observation_call = {"role": "observation", "content": observation_str}
             processed_msg.append(observation_call)
             func_observation_map.clear()
 
         if i == 0:
             if messages[0]["role"] == "system":
                 old_content = messages[0]["content"]
@@ -209,14 +213,17 @@
 
         else:
             processed_msg.append(messages[i])
 
     if len(func_observation_map) > 0:
         # Insert the observation from the tool call before the next message
         func_observation_array = list(func_observation_map.values())
+        for i,a in enumerate(func_observation_array):
+            if a == "":
+                func_observation_array[i] = "Empty Result"
         observation_str = json.dumps(func_observation_array)
         observation_call = {"role": "observation", "content": observation_str}
         processed_msg.append(observation_call)
         func_observation_map.clear()
 
     return processed_msg
 
@@ -241,11 +248,11 @@
             "type": "function",
             "function": {
                 "name": "dummy",
                 "description": "just to say hi",
                 "parameters": None,
             }
         },{"type": "function","function":{"name":"calculate_distance","description":"Calculate the distance between two locations","parameters":{"type":"object","properties":{"origin":{"type":"string","description":"The starting location"},"destination":{"type":"string","description":"The destination location"},"mode":{"type":"string","description":"The mode of transportation"}},"required":["origin","destination","mode"]}}},{"type": "function","function":{"name":"generate_password","description":"Generate a random password","parameters":{"type":"object","properties":{"length":{"type":"integer","description":"The length of the password"}},"required":["length"]}}}]
-    msgs = [{'role': 'system', 'content': 'You are a helpful assistant.'}, {'role': 'user', 'content': 'What is the distance between San Francisco and Cupertino by driving and by air from both directions?'}, {'role': 'assistant', 'tool_calls': [{'id': '0', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San Francisco","destination":"Cupertino","mode":"drive"}'}, 'type': 'function'},{'id': '1', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San Francisco","destination":"Cupertino","mode":"air"}'}, 'type': 'function'}]}, {'role': 'tool', 'tool_call_id': '0', 'name': 'calculate_distance', 'content': 'Distance is 50 miles.'}, {'role': 'tool', 'tool_call_id': '1', 'name': 'calculate_distance', 'content': 'Distance  by air is 50 miles.'}]
+    msgs = [{'role': 'system', 'content': 'You are a helpful assistant.'}, {'role': 'user', 'content': 'What is the distance between San Francisco and Cupertino by driving and by air from both directions?'}, {'role': 'assistant', 'tool_calls': [{'id': '0', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San Francisco","destination":"Cupertino","mode":"drive"}'}, 'type': 'function'},{'id': '1', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San Francisco","destination":"Cupertino","mode":"air"}'}, 'type': 'function'}]}, {'role': 'tool', 'tool_call_id': '0', 'name': 'calculate_distance', 'content': 'Distance is 50 miles.'}, {'role': 'tool', 'tool_call_id': '1', 'name': 'calculate_distance', 'content': ''}]
     new_msgs = preprocess_input(msgs, tools)
     print(json.dumps(new_msgs, indent=2))
```

### Comparing `llama_tools-0.1.7/pyproject.toml` & `llama_tools-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.7/PKG-INFO` & `llama_tools-0.1.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Llama Tools: A collection of utilities for handling function calls with local llama.cpp models.
 Home-page: https://yourpackage.example.com
 License: MIT
 Keywords: llama, function-call
 Author: Yingbei Tong
 Author-email: yingbei@acorn.io
 Requires-Python: >=3.8
```

