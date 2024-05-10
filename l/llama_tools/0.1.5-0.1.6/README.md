# Comparing `tmp/llama_tools-0.1.5.tar.gz` & `tmp/llama_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_tools-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "llama_tools-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `llama_tools-0.1.5.tar` & `llama_tools-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.5/.gitignore
--rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.5/README.md
--rw-r--r--   0        0        0      314 2024-05-10 00:48:36.154726 llama_tools-0.1.5/llama_tools/__init__.py
--rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.5/llama_tools/postprocess.py
--rw-r--r--   0        0        0    10968 2024-05-10 00:45:15.623041 llama_tools-0.1.5/llama_tools/preprocess.py
--rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 20:31:22.641082 llama_tools-0.1.6/.gitignore
+-rw-r--r--   0        0        0      441 2024-05-06 23:27:31.029032 llama_tools-0.1.6/README.md
+-rw-r--r--   0        0        0      314 2024-05-10 20:18:09.248130 llama_tools-0.1.6/llama_tools/__init__.py
+-rw-r--r--   0        0        0     1722 2024-05-10 00:43:53.515042 llama_tools-0.1.6/llama_tools/postprocess.py
+-rw-r--r--   0        0        0    11231 2024-05-10 20:13:09.818817 llama_tools-0.1.6/llama_tools/preprocess.py
+-rw-r--r--   0        0        0      739 2024-05-09 00:13:36.637592 llama_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 llama_tools-0.1.6/PKG-INFO
```

### Comparing `llama_tools-0.1.5/llama_tools/postprocess.py` & `llama_tools-0.1.6/llama_tools/postprocess.py`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.5/llama_tools/preprocess.py` & `llama_tools-0.1.6/llama_tools/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
     func_name = function_schema["name"]
     description = function_schema.get("description", "")
 
     # Check if parameters is a list and convert if necessary
     parameters_info = function_schema.get("parameters", {})
     if isinstance(parameters_info, list):
         parameters_info = convert_parameters_list_to_dict(parameters_info)
+    if parameters_info is None:
+        parameters_info = {}
 
     parameters_schema = parameters_info.get("properties", {})
     required_params = parameters_info.get("required", [])
 
     args_list = []
     comments_list = []
     interfaces = []
@@ -229,12 +231,19 @@
 
     # Converting the Python dictionary to a YAML formatted string
     tool_call_str = "\n".join(tool_list)
     return tool_call_str
 
 
 if __name__ == "__main__":
-    tools = [{"type": "function","function":{"name":"calculate_distance","description":"Calculate the distance between two locations","parameters":{"type":"object","properties":{"origin":{"type":"string","description":"The starting location"},"destination":{"type":"string","description":"The destination location"},"mode":{"type":"string","description":"The mode of transportation"}},"required":["origin","destination","mode"]}}},{"type": "function","function":{"name":"generate_password","description":"Generate a random password","parameters":{"type":"object","properties":{"length":{"type":"integer","description":"The length of the password"}},"required":["length"]}}}]
+    tools = [{
+            "type": "function",
+            "function": {
+                "name": "dummy",
+                "description": "just to say hi",
+                "parameters": None,
+            }
+        },{"type": "function","function":{"name":"calculate_distance","description":"Calculate the distance between two locations","parameters":{"type":"object","properties":{"origin":{"type":"string","description":"The starting location"},"destination":{"type":"string","description":"The destination location"},"mode":{"type":"string","description":"The mode of transportation"}},"required":["origin","destination","mode"]}}},{"type": "function","function":{"name":"generate_password","description":"Generate a random password","parameters":{"type":"object","properties":{"length":{"type":"integer","description":"The length of the password"}},"required":["length"]}}}]
     msgs = [{'role': 'system', 'content': 'You are a helpful assistant.'}, {'role': 'user', 'content': 'What is the distance between San Francisco and Cupertino by driving and by air from both directions?'}, {'role': 'assistant', 'tool_calls': [{'id': '0', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San \nFrancisco","destination":"Cupertino","mode":"drive"}'}, 'type': 'function'},{'id': '1', 'function': {'name': 'calculate_distance', 'arguments': '{"origin":"San \nFrancisco","destination":"Cupertino","mode":"air"}'}, 'type': 'function'}]}, {'role': 'tool', 'tool_call_id': '0', 'name': 'calculate_distance', 'content': 'Distance is 50 miles.'}, {'role': 'tool', 'tool_call_id': '1', 'name': 'calculate_distance', 'content': 'Distance  by air is 50 miles.'}]
     new_msgs = preprocess_input(msgs, tools)
     print(json.dumps(new_msgs, indent=2))
```

### Comparing `llama_tools-0.1.5/pyproject.toml` & `llama_tools-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_tools-0.1.5/PKG-INFO` & `llama_tools-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Llama Tools: A collection of utilities for handling function calls with local llama.cpp models.
 Home-page: https://yourpackage.example.com
 License: MIT
 Keywords: llama, function-call
 Author: Yingbei Tong
 Author-email: yingbei@acorn.io
 Requires-Python: >=3.8
```

