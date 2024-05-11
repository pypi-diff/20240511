# Comparing `tmp/ALLMDEV-1.3.1-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 20188 bytes, number of entries: 21
+Zip file size: 21663 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
--rw-rw-rw-  2.0 fat     4454 b- defN 24-May-04 14:17 ALLMDEV/azureagentapi.py
--rw-rw-rw-  2.0 fat     2261 b- defN 24-May-05 09:44 ALLMDEV/azureagentchat.py
--rw-rw-rw-  2.0 fat     1294 b- defN 24-May-05 07:01 ALLMDEV/azurecli.py
+-rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
+-rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
 -rw-rw-rw-  2.0 fat      757 b- defN 24-May-04 08:56 ALLMDEV/cli.py
--rw-rw-rw-  2.0 fat     1945 b- defN 24-Apr-26 04:23 ALLMDEV/fasty.py
--rw-rw-rw-  2.0 fat    10334 b- defN 24-May-04 13:49 ALLMDEV/instruct.py
+-rw-rw-rw-  2.0 fat    11849 b- defN 24-May-11 11:56 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
 -rw-rw-rw-  2.0 fat     2795 b- defN 24-May-04 14:18 ALLMDEV/serve.py
+-rw-rw-rw-  2.0 fat     1927 b- defN 24-May-11 17:57 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
--rw-rw-rw-  2.0 fat     3883 b- defN 24-May-04 14:17 ALLMDEV/vertexagentapi.py
--rw-rw-rw-  2.0 fat     1851 b- defN 24-May-04 14:57 ALLMDEV/vertexagentchat.py
--rw-rw-rw-  2.0 fat     1095 b- defN 24-May-04 13:50 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     4676 b- defN 24-May-05 09:50 ALLMDEV-1.3.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 09:50 ALLMDEV-1.3.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      522 b- defN 24-May-05 09:50 ALLMDEV-1.3.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-05 09:50 ALLMDEV-1.3.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1620 b- defN 24-May-05 09:50 ALLMDEV-1.3.1.dist-info/RECORD
-21 files, 51647 bytes uncompressed, 17598 bytes compressed:  65.9%
+-rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
+-rw-rw-rw-  2.0 fat     2824 b- defN 24-May-11 13:36 ALLMDEV/vertexagentchat.py
+-rw-rw-rw-  2.0 fat     2124 b- defN 24-May-11 13:27 ALLMDEV/vertexcli.py
+-rw-rw-rw-  2.0 fat     5962 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      556 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1621 b- defN 24-May-11 18:07 ALLMDEV-1.3.2.dist-info/RECORD
+21 files, 59824 bytes uncompressed, 19071 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: ALLMDEV/azurecli.py
 Comment: 
 
 Filename: ALLMDEV/cli.py
 Comment: 
 
-Filename: ALLMDEV/fasty.py
-Comment: 
-
 Filename: ALLMDEV/instruct.py
 Comment: 
 
 Filename: ALLMDEV/newagent.py
 Comment: 
 
 Filename: ALLMDEV/serve.py
 Comment: 
 
+Filename: ALLMDEV/studio.py
+Comment: 
+
 Filename: ALLMDEV/test.py
 Comment: 
 
 Filename: ALLMDEV/updateagent.py
 Comment: 
 
 Filename: ALLMDEV/vertexagentapi.py
@@ -42,23 +42,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.1.dist-info/METADATA
+Filename: ALLMDEV-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.1.dist-info/WHEEL
+Filename: ALLMDEV-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.1.dist-info/entry_points.txt
+Filename: ALLMDEV-1.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.1.dist-info/top_level.txt
+Filename: ALLMDEV-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.1.dist-info/RECORD
+Filename: ALLMDEV-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/azureagentapi.py

```diff
@@ -1,53 +1,37 @@
 from flask import Flask, request, jsonify
 from openai import AzureOpenAI
 import argparse
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import os
+import json
 
 
 persist_directory = None
 
 app = Flask(__name__)
 
-# Check if apiconfig.txt exists in the model folder
-config_file_path = os.path.join('model', 'apiconfig.txt')
-if not os.path.exists(config_file_path):
-    # Create apiconfig.txt with default values
-    with open(config_file_path, 'w') as file:
-       file.write('Host=127.0.0.1\n')
-       file.write('Port=5000\n')
-       file.write('CertFile=""\n')
-       file.write('CertKey=""\n')
-
-# Read host and port from apiconfig.txt
-if os.path.exists(config_file_path):
-    with open(config_file_path, 'r') as file:
-        for line in file:
-            key, value = line.strip().split('=')
-            if key == 'Host':
-                host = value
-            elif key == 'Port':
-                port = int(value)
-            elif key == 'CertFile':
-                cert_file = value.strip('"')
-            elif key == 'CertKey':
-                cert_key = value.strip('"')
-else:
-    print("File doesn't exist.")
-    host = '127.0.0.1'
-    port = 5000
-    cert_file = ""
-    cert_key = ""
-
-print("Host:", host)
-print("Port:", port)
-print("CertFile:", cert_file)
-print("CertKey:", cert_key)
+model_dir = "model"
+
+config = {
+    "apikey": "",
+    "version": "",
+    "endpoint": "",
+    "model": "",
+    "host": "",
+    "port": "",
+    "cert_file": "",
+    "cert_key": ""
+}
+
+file_path=os.path.join(model_dir, "azureapiconfig.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
 
 
 
 @app.route('/v1/chat/completions', methods=['POST'])
 def chat():
 
     global persist_directory
@@ -58,30 +42,32 @@
     prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query: {prompt} "
     persist_directory = os.path.join('db',agent)
 
     embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
 
     # Create ChromaDB and store document IDs
     db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
+    user_input = request.json.get("input")
 
-    while True:
-        user_input = input("\n\nUser:")
-        docs = db.similarity_search(user_input,k=1)
-        context=docs[0].page_content
-        prompt = prompt_template.format(context=context, prompt=user_input)
-        response = client.chat.completions.create(
-            model=model, # model = "deployment_name".
-            messages=[
-                {"role": "system", "content": "Assistant is a large language model trained by OpenAI."},
-                {"role": "user", "content": prompt}
-                
-            ]
-        )
-        for choice in response.choices:
-            return jsonify({"response": choice.message.content})
+    if user_input.lower() == "exit":
+        return jsonify({"response": "Exiting chat."})
+    
+    docs = db.similarity_search(user_input,k=1)
+    context=docs[0].page_content
+    prompt = prompt_template.format(context=context, prompt=user_input)
+    response = client.chat.completions.create(
+        model=model, # model = "deployment_name".
+        messages=[
+            {"role": "system", "content": "Assistant is a large language model trained by OpenAI."},
+            {"role": "user", "content": prompt}
+            
+        ]
+    )
+    for choice in response.choices:
+        return jsonify({"response": choice.message.content})
 
 def main():
         global persist_directory
         global multimodal_model
         global agent
         global client
         global model
@@ -89,24 +75,58 @@
         # parser.add_argument("--model", type=str, default="Mistral", help="Name of the model or path to the model file")
         parser.add_argument("--key", type=str, default=None, help="your azure openai key.")
         parser.add_argument("--version", type=str, default=None, help="Your azure api version.")
         parser.add_argument("--endpoint", type=str, default=None, help="Your azure endpoint")
         parser.add_argument("--model", type=str, default='gpt-35-turbo', help="Your cloud model deployed on azure.")
         parser.add_argument("--agent", type=str, default=None, help="Name of the agent to query.")
         args = parser.parse_args()
-        client = AzureOpenAI(
-            api_key = (args.key),
-            api_version = args.version,
-            azure_endpoint = (args.endpoint)
-        )
-        model=args.model
+        agent = args.agent
+        with open(file_path, "r") as json_file:
+            config = json.load(json_file)
+            key=config["apikey"]
+            version=config["version"]
+            endpoint=config["endpoint"]
+            model=config["model"]
+            host=config["host"]
+            port=config["port"]
+            cert_file=config["cert_file"]
+            cert_key=config["cert_key"]
+            # print(projectid, region, model)
+        if key != "" and version != "" and endpoint != "" and model != "":
+            client = AzureOpenAI(
+                    api_key = (key),
+                    api_version = version,
+                    azure_endpoint = (endpoint)
+                )
+            model=args.model
+
+        else:
+            client = AzureOpenAI(
+                    api_key = (args.key),
+                    api_version = args.version,
+                    azure_endpoint = (args.endpoint)
+                )
+            model=args.model
+            config = {
+                "apikey": args.key,
+                "version": args.version,
+                "endpoint": args.endpoint,
+                "model": args.model,
+                "host":"127.0.0.1",
+                "port":"5000",
+                "cert_file":"",
+                "cert_key":""
+            }
+            with open(file_path, "w") as json_file:
+                json.dump(config, json_file)
+
 
         
         if cert_file is not "" and cert_key is not "":
-            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {file_path}")
             app.run(host=host, port=port, debug=False, ssl_context=(cert_file,cert_key))
         else:
-            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {file_path}")
             app.run(host=host, port=port, debug=False)
 
 if __name__ == "__main__":
     main()
```

## ALLMDEV/azureagentchat.py

```diff
@@ -1,12 +1,28 @@
 import os
 from openai import AzureOpenAI
 import argparse
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
+import json
+
+
+model_dir = "model"
+
+config = {
+    "apikey": "",
+    "version": "",
+    "endpoint": "",
+    "model": ""
+}
+
+file_path=os.path.join(model_dir, "azure_config.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
 
 
 def infer(model, client, agent):
     persist_directory = os.path.join('db',agent)
 
     embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
 
@@ -27,27 +43,50 @@
             ]
         )
         for choice in response.choices:
             print(choice.message.content)
 
 
 def main():
+
     parser = argparse.ArgumentParser()
-    # parser.add_argument("--model", type=str, default="Mistral", help="Name of the model or path to the model file")
     parser.add_argument("--key", type=str, default=None, help="your azure openai key.")
     parser.add_argument("--version", type=str, default=None, help="Your azure api version.")
     parser.add_argument("--endpoint", type=str, default=None, help="Your azure endpoint")
     parser.add_argument("--model", type=str, default='gpt-35-turbo', help="Your cloud model deployed on azure.")
     parser.add_argument("--agent", type=str, default=None, help="Name of the agent to query.")
     args = parser.parse_args()
 
-    client = AzureOpenAI(
-        api_key = (str(args.key)),
-        api_version = str(args.version),
-        azure_endpoint = (str(args.endpoint))
-    )
-
+    with open(file_path, "r") as json_file:
+        config = json.load(json_file)
+        key=config["apikey"]
+        version=config["version"]
+        endpoint=config["endpoint"]
+        model=config["model"]
+        # print(projectid, region, model)
+    if key != "" and version != "" and endpoint != "" and model != "":
+        client = AzureOpenAI(
+                api_key = (key),
+                api_version = version,
+                azure_endpoint = (endpoint)
+            )
+
+        infer(args.model, client, args.agent)
+    else:
+        client = AzureOpenAI(
+                api_key = (args.key),
+                api_version = args.version,
+                azure_endpoint = (args.endpoint)
+            )
+        config = {
+            "apikey": args.key,
+            "version": args.version,
+            "endpoint": args.endpoint,
+            "model": args.model
+        }
+        with open(file_path, "w") as json_file:
+            json.dump(config, json_file)
 
-    infer(args.model, client, args.agent)
+        infer(args.model, client, args.agent)
 
 if __name__=='__main__':
      main()
```

## ALLMDEV/azurecli.py

```diff
@@ -1,12 +1,27 @@
 from openai import AzureOpenAI
 import argparse
 import os
+import json
 
 
+model_dir = "model"
+
+config = {
+    "apikey": "",
+    "version": "",
+    "endpoint": "",
+    "model": ""
+}
+
+file_path=os.path.join(model_dir, "azure_config.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
+
 def infer(model, client):
     while True:
         user_input = input("\n\nUser:")
         response = client.chat.completions.create(
             model=model, # model = "deployment_name".
             messages=[
                 {"role": "system", "content": "Assistant is a large language model trained by OpenAI."},
@@ -23,18 +38,42 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("--key", type=str, default=None, help="your azure openai key.")
     parser.add_argument("--version", type=str, default=None, help="Your azure api version.")
     parser.add_argument("--endpoint", type=str, default=None, help="Your azure endpoint")
     parser.add_argument("--model", type=str, default='gpt-35-turbo', help="Your cloud model deployed on azure.")
     args = parser.parse_args()
 
-    client = AzureOpenAI(
-            api_key = (args.key),
-            api_version = args.version,
-            azure_endpoint = (args.endpoint)
-        )
+    with open(file_path, "r") as json_file:
+        config = json.load(json_file)
+        key=config["apikey"]
+        version=config["version"]
+        endpoint=config["endpoint"]
+        model=config["model"]
+        # print(projectid, region, model)
+    if key != "" and version != "" and endpoint != "" and model != "":
+        client = AzureOpenAI(
+                api_key = (key),
+                api_version = version,
+                azure_endpoint = (endpoint)
+            )
+
+        infer(args.model, client)
+    else:
+        client = AzureOpenAI(
+                api_key = (args.key),
+                api_version = args.version,
+                azure_endpoint = (args.endpoint)
+            )
+        config = {
+            "apikey": args.key,
+            "version": args.version,
+            "endpoint": args.endpoint,
+            "model": args.model
+        }
+        with open(file_path, "w") as json_file:
+            json.dump(config, json_file)
 
-    infer(args.model, client)
+        infer(args.model, client)
         
 
 if __name__=='__main__':
      main()
```

## ALLMDEV/instruct.py

```diff
@@ -23,15 +23,34 @@
                                     # # else:
                                     # print("Using existing mistral GGUF file")
                                     model_path = os.path.join(model_dir, model_files[0])
                                 else:
                                         model_id = "TheBloke/Mistral-7B-v0.1-GGUF"
                                         filename = hf_hub_download(repo_id=model_id, filename="mistral-7b-v0.1.Q8_0.gguf")
                                         shutil.move(filename,model_dir)
-                                        model_path = os.path.join(model_dir, filename) 
+                                        model_path = os.path.join(model_dir, filename)
+
+                        elif model=='llama3' or model=='Llama3':
+                            for file in model_files:
+                                if 'llama3' in file.lower():
+                                    # print("A mistral model already exists")
+                                    # # download_again = input("Do you want to download mistral model again? (yes/y to download): ")
+                                    # # if download_again.lower() in ['yes', 'y']:
+                                    # #     model_id = "TheBloke/Mistral-7B-v0.1-GGUF"
+                                    # #     filename = hf_hub_download(repo_id=model_id, filename="mistral-7b-v0.1.Q8_0.gguf")
+                                    # #     shutil.move(filename,model_dir)
+                                    # #     model_path = os.path.join(model_dir, filename)
+                                    # # else:
+                                    # print("Using existing mistral GGUF file")
+                                    model_path = os.path.join(model_dir, model_files[0])
+                                else:
+                                        model_id = "crusoeai/Llama-3-8B-Instruct-262k-GGUF"
+                                        filename = hf_hub_download(repo_id=model_id, filename="llama-3-8b-instruct-262k.Q8_0.gguf")
+                                        shutil.move(filename,model_dir)
+                                        model_path = os.path.join(model_dir, filename)  
                             
 
                         elif model=='Mistral_instruct' or model=='mistral_instruct':
                             for file in model_files:
                                 if 'mistral-7b-instruct' in file.lower():
                                     # print("A mistral instruct model already exists")
                                     # # download_again = input("Do you want to download mistral instruct model again? (yes/y to download): ")
@@ -148,15 +167,15 @@
             verbose=False,
         )
 
         # Start the chat loop
         while True:
             try:
                 # Prompt user for input
-                user_input = input("User: ")
+                user_input = input("\n\nUser: ")
                 
                 # Exit loop if user types "exit"
                 if user_input.lower() == "exit":
                     print("Exiting chat.")
                     break
                 
                 # Construct prompt with user input
```

## ALLMDEV/vertexagentapi.py

```diff
@@ -1,54 +1,37 @@
 from flask import Flask, request, jsonify
 import vertexai
 from vertexai.generative_models import GenerativeModel
 import argparse
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import os
+import json
 
 
 persist_directory = None
 
 app = Flask(__name__)
 
-# Check if apiconfig.txt exists in the model folder
-config_file_path = os.path.join('model', 'apiconfig.txt')
-if not os.path.exists(config_file_path):
-    # Create apiconfig.txt with default values
-    with open(config_file_path, 'w') as file:
-       file.write('Host=127.0.0.1\n')
-       file.write('Port=5000\n')
-       file.write('CertFile=""\n')
-       file.write('CertKey=""\n')
-
-# Read host and port from apiconfig.txt
-if os.path.exists(config_file_path):
-    with open(config_file_path, 'r') as file:
-        for line in file:
-            key, value = line.strip().split('=')
-            if key == 'Host':
-                host = value
-            elif key == 'Port':
-                port = int(value)
-            elif key == 'CertFile':
-                cert_file = value.strip('"')
-            elif key == 'CertKey':
-                cert_key = value.strip('"')
-else:
-    print("File doesn't exist.")
-    host = '127.0.0.1'
-    port = 5000
-    cert_file = ""
-    cert_key = ""
-
-print("Host:", host)
-print("Port:", port)
-print("CertFile:", cert_file)
-print("CertKey:", cert_key)
+model_dir = "model"
+
+config = {
+    "project_id": "",
+    "region": "",
+    "model": "",
+    "host": "",
+    "port": "",
+    "cert_file": "",
+    "cert_key": ""
+}
+
+file_path=os.path.join(model_dir, "vertexapiconfig.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
 
 
 
 @app.route('/v1/chat/completions', methods=['POST'])
 def chat():
 
     global persist_directory
@@ -58,39 +41,71 @@
     persist_directory = os.path.join('db',agent)
 
     embeddings = SentenceTransformerEmbeddings(model_name="all-MiniLM-L6-v2")
 
     # Create ChromaDB and store document IDs
     db = Chroma(embedding_function=embeddings, persist_directory=persist_directory)
 
-    while True:
-        user_input = input("\n\nUser:")
-        docs = db.similarity_search(user_input,k=1)
-        context=docs[0].page_content
-        prompt = prompt_template.format(context=context, prompt=user_input)
-        response = multimodal_model.generate_content(prompt)
-        return jsonify({"response": response})
+    user_input = request.json.get("input")
+
+    if user_input.lower() == "exit":
+        return jsonify({"response": "Exiting chat."})
+
+    prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query:<s>[INST] {prompt} [/INST]"
+    docs = db.similarity_search(user_input,k=1)
+    context=docs[0].page_content
+    prompt = prompt_template.format(context=context,prompt=user_input)
+    response = multimodal_model.generate_content(prompt)
+    return jsonify({"response": response.text})
 
 def main():
         global persist_directory
         global multimodal_model
         global agent
         parser = argparse.ArgumentParser()
         parser.add_argument("--projectid", type=str, default=None, help="Id of your GCP project.")
-        parser.add_argument("--region", type=str, default=0.5, help="Your cloud provider region.")
+        parser.add_argument("--region", type=str, default=None, help="Your cloud provider region.")
         parser.add_argument("--agent", type=str, help="Name of the agent to query.")
-        parser.add_argument("--model", type=str, default=0.5, help="Your cloud model on VertexAI.")
+        parser.add_argument("--model", type=str, default="gemini-1.0-pro-002", help="Your cloud model on VertexAI.")
         args = parser.parse_args()
         agent=args.agent
         persist_directory = os.path.join('db', agent)
-        vertexai.init(project=args.projectid, location=args.region)
-        # Load the model
-        multimodal_model = GenerativeModel(model_name=args.model)
+        with open(file_path, "r") as json_file:
+            config = json.load(json_file)
+            projectid=config["project_id"]
+            region=config["region"]
+            model=config["model"]
+            host=config["host"]
+            port=config["port"]
+            cert_file=config["cert_file"]
+            cert_key=config["cert_key"]
+            # print(projectid, region, model)
+        if projectid != "" and region != "" and model != "":
+        # Initialize Vertex AI
+            vertexai.init(project=projectid, location=region)
+            # Load the model
+            multimodal_model = GenerativeModel(model_name=model)
+        else:
+            vertexai.init(project=args.projectid, location=args.region)
+            # Load the model
+            multimodal_model = GenerativeModel(model_name=args.model)
+            config = {
+                "project_id": args.projectid,
+                "region": args.region,
+                "model": args.model,
+                "host":"127.0.0.1",
+                "port":"5000",
+                "cert_file":"",
+                "cert_key":""
+            }
+            with open(file_path, "w") as json_file:
+                json.dump(config, json_file)
+        
         if cert_file is not "" and cert_key is not "":
-            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            print(f"Inference is working on https://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the vertexapiconfig.json file available at {file_path}")
             app.run(host=host, port=port, debug=False, ssl_context=(cert_file,cert_key))
         else:
-            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the apiconfig.txt file available at {config_file_path}")
+            print(f"Inference is working on http://{host}:{port}/v1/chat/completions. You can configure custom host IP and port, and ssl certificate via the vertexapiconfig.json file available at {file_path}")
             app.run(host=host, port=port, debug=False)
 
 if __name__ == "__main__":
     main()
```

## ALLMDEV/vertexagentchat.py

```diff
@@ -1,13 +1,28 @@
 import vertexai
 from vertexai.generative_models import GenerativeModel
 import argparse
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import os
+import json
+
+
+model_dir = "model"
+
+config = {
+    "project_id": "",
+    "region": "",
+    "model": ""
+}
+
+file_path=os.path.join(model_dir, "vertex_config.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
 
 
 # Query the model
 def infer(multimodal_model, agent):
     prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query: {prompt} "
     persist_directory = os.path.join('db',agent)
 
@@ -30,16 +45,34 @@
 def main():
     parser = argparse.ArgumentParser()
     # parser.add_argument("--model", type=str, default="Mistral", help="Name of the model or path to the model file")
     parser.add_argument("--projectid", type=str, default=None, help="Id of your GCP project.")
     parser.add_argument("--region", type=str, default=0.5, help="Your cloud provider region.")
     parser.add_argument("--agent", type=str, default=None, help="Name of the agent to query.")
     args = parser.parse_args()
+    with open(file_path, "r") as json_file:
+        config = json.load(json_file)
+        projectid=config["project_id"]
+        region=config["region"]
+        model=config["model"] 
+        print(projectid, region, model)
+    if projectid != "" and region != "" and model != "":
     # Initialize Vertex AI
-    vertexai.init(project=args.projectid, location=args.region)
-    # Load the model
-    multimodal_model = GenerativeModel(model_name="gemini-1.0-pro-002")
+        vertexai.init(project=projectid, location=region)
+        # Load the model
+        multimodal_model = GenerativeModel(model_name=model)
+    else:
+        vertexai.init(project=args.projectid, location=args.region)
+        # Load the model
+        multimodal_model = GenerativeModel(model_name=args.model)
+        config = {
+            "project_id": args.projectid,
+            "region": args.region,
+            "model": args.model
+        }
+        with open(file_path, "w") as json_file:
+            json.dump(config, json_file)
 
     infer(multimodal_model, args.agent)
 
 if __name__=='__main__':
      main()
```

## ALLMDEV/vertexcli.py

```diff
@@ -1,11 +1,25 @@
 import vertexai
 from vertexai.generative_models import GenerativeModel
 import argparse
+import json
+import os
 
+model_dir = "model"
+
+config = {
+    "project_id": "",
+    "region": "",
+    "model": ""
+}
+
+file_path=os.path.join(model_dir, "vertex_config.json")
+if not os.path.exists(file_path):
+    with open(file_path, "w") as json_file:
+        json.dump(config, json_file)
 
 # Query the model
 def infer(multimodal_model):
     while True:
         user_input = input("\n\nUser:")
         response = multimodal_model.generate_content(user_input)
         print(response.text)
@@ -16,16 +30,36 @@
 def main():
     parser = argparse.ArgumentParser()
     # parser.add_argument("--model", type=str, default="Mistral", help="Name of the model or path to the model file")
     parser.add_argument("--projectid", type=str, default=None, help="Id of your GCP project.")
     parser.add_argument("--region", type=str, default=None, help="Your cloud provider region.")
     parser.add_argument("--model", type=str, default='gemini-1.0-pro-002', help="Your cloud model deployed on VertexAI.")
     args = parser.parse_args()
+
+    # if os.path.exists(file_path):
+    with open(file_path, "r") as json_file:
+        config = json.load(json_file)
+        projectid=config["project_id"]
+        region=config["region"]
+        model=config["model"] 
+        print(projectid, region, model)
+    if projectid != "" and region != "" and model != "":
     # Initialize Vertex AI
-    vertexai.init(project=args.projectid, location=args.region)
-    # Load the model
-    multimodal_model = GenerativeModel(model_name=args.model)
+        vertexai.init(project=projectid, location=region)
+        # Load the model
+        multimodal_model = GenerativeModel(model_name=model)
+    else:
+        vertexai.init(project=args.projectid, location=args.region)
+        # Load the model
+        multimodal_model = GenerativeModel(model_name=args.model)
+        config = {
+            "project_id": args.projectid,
+            "region": args.region,
+            "model": args.model
+        }
+        with open(file_path, "w") as json_file:
+            json.dump(config, json_file)
 
     infer(multimodal_model)
 
 if __name__=='__main__':
      main()
```

## Comparing `ALLMDEV/fasty.py` & `ALLMDEV/studio.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 prompt_template = "<s>[INST] {prompt} [/INST]"
 
 executor = ThreadPoolExecutor(max_workers=1)
 
 @app.route('/')
 def index():
-    return render_template('indexy.html')
+    return render_template('index.html')
 
 @app.route('/send_message', methods=['POST'])
 @app.route('/send_message', methods=['POST'])
 def send_message():
     data = request.json
     prompt = data['userInput']
     modelPath = data['filePath']
@@ -45,21 +45,21 @@
         verbose=False,
     )
 
     # Perform inference and stream the generated tokens
     response_iter = llm.stream_complete(formatted_prompt)
     prev_token = ''
     for response in response_iter:
-        token = response.text
-        new_token = token.replace(prev_token, token)
-        if new_token:
-            print(new_token, end='')
-            socketio.emit('response', new_token)
-            prev_token = token
-        time.sleep(0.01)
+        token = response.delta
+        # new_token = token.replace(prev_token, token)
+        # if new_token:
+        print(token, end='')
+        socketio.emit('response', token)
+        # prev_token = token
+    time.sleep(0.01)
 
 
     return None
 
 
 
 if __name__ == '__main__':
```

## Comparing `ALLMDEV-1.3.1.dist-info/METADATA` & `ALLMDEV-1.3.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -94,32 +94,77 @@
 
 ```bash
 allm-updateagent --doc "document path" --agent agentname
 ```
 
 ##Supported Cloud models.
 
-As of now, ALLM supports the Generative LLMs on VertexAI, including Gemini-1.5 pro and AzureOpenAi models. You can start local inference of cloud based models using the following command:
+ALLM supports the Generative LLMs on VertexAI, including Gemini-1.5 pro and AzureOpenAi models. You can start local inference of cloud based models using the following command:
 
 ```bash
 allm-run-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server
 ```
+
 or
+
 ```bash
 allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name
 ```
 
+ALLM supports the local config based inference of Generative LLMs on VertexAI, including Gemini-1.5 pro and AzureOpenAi models. You can manually create a json confi file or ALLM will create one for you and start local inference of cloud based models using the following command:
+
+```bash
+allm-run-vertex
+```
+Note that for the above command to work, config file needs to have all the necessary parameters set. This can be achieved by running thr full command including CLI arguments once, and then using the shortened command
+
+Same procedure can be followed for azure.
+
+```bash
+allm-run-azure
+```
+
+
 You can also have a custom agent working with your cloud deployed model using the following command. It is important to note that before this step, agent should be created using the commands in the AGENTS section above.
 
 ```bash
 allm-agentchat-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server --agent agent_name
 ```
 or
 ```bash
 allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name --agent agentname
 ```
 model_name is an optional parameter in both vertex and azure, if not mentioned, inference will work on gemini-1.0-pro-002 for vertex and gpt-35-turbo for OpenAI by default.
 
+Also, have an api config file ready, the following commands can be used:
+
+```bash
+allm-agentchat-vertex --agent agent_name
+```
+and
+```bash
+allm-agentchat-azure --agent agent_name
+```
+
+ALLM also supports inferencing of cloud model based agents on API
+
+```bash
+allm-agentapi-vertex --projectid Id_of_your_GCP_project --region location_of_your_cloud_server --agent agent_name
+```
+or
+```bash
+allm-agentapi-vertex --agent agent_name
+```
+
+For Azure,
+
+```bash
+allm-run-azure --key key --version version --endpoint https://{your_endpoint}.openai.azure.com --model model_name --agent agentname
+```
+or
+```bash
+allm-agentapi-vertex --agent agent_name
+```
 
 ## Supported Model names
-Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
+Llama3, Llama2, llama, llama2_chat, Llama_chat, Mistral, Mistral_instruct
```

## Comparing `ALLMDEV-1.3.1.dist-info/entry_points.txt` & `ALLMDEV-1.3.2.dist-info/entry_points.txt`

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

## Comparing `ALLMDEV-1.3.1.dist-info/RECORD` & `ALLMDEV-1.3.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
 ALLMDEV/agentapi.py,sha256=vnkpCaviW0w5EQTE99els4Nb8QABv0TgNoP2FdFsWVQ,3706
 ALLMDEV/agentchat.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
-ALLMDEV/azureagentapi.py,sha256=GEY_byQWMHlZPWLz1shNo8q2PtmRw9v8GGUaPqp-tuo,4454
-ALLMDEV/azureagentchat.py,sha256=fhmUVUlVAzRNEeSoRR8Nd8QeT4A9WwRr9bBqEKMYpz4,2261
-ALLMDEV/azurecli.py,sha256=XxVYv4cwJBtt9K066HsC9Re5SD-pdW4KgxhM3GN_x1o,1294
+ALLMDEV/azureagentapi.py,sha256=dzMwkJHfRBqRxYAwpe_aQRgASqnsNBaEzT9jsc791QQ,4986
+ALLMDEV/azureagentchat.py,sha256=6L9m2B6dfe9LUWdd_Vj6_TT1n1GBXxVvqOeA-yTuV_Q,3298
+ALLMDEV/azurecli.py,sha256=nLoSVPpxWwIJWhiddB0_qzNw53hrAE6ijK0diDlaGYs,2435
 ALLMDEV/cli.py,sha256=wWOt7Uv_DmQKT821rEIaEVh9MFJVz0n19BXgwTHsdDY,757
-ALLMDEV/fasty.py,sha256=9YSkUcPnZUW2B2JrkHZaH75FcNYLZL5JNJI9ZmqkBCw,1945
-ALLMDEV/instruct.py,sha256=9cjx7CnIc-C-LXxVl2THdlrNX3WXcZ0rXKXWVpZ0BXY,10334
+ALLMDEV/instruct.py,sha256=qFO727_ehoI5Luj07D1ptomdwtRg0MByR1hr1bcA8as,11849
 ALLMDEV/newagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/serve.py,sha256=SWs9Afph4glJjCcX46rYNA0N0xQZiXmBv0H_DXNCxnU,2795
+ALLMDEV/studio.py,sha256=bI4_O3Ed6T3ngPBTVqhJS3U6i9DvSuSDgh8h88hjAOc,1927
 ALLMDEV/test.py,sha256=CxP_WW9ZXEiLCJh_9MLdieFU-yfNMwWlXrcrs7gtXx8,683
 ALLMDEV/updateagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
-ALLMDEV/vertexagentapi.py,sha256=dAnfVE8VhFqWtdFtqcIPA2GqjbJtaToa9UTKnctpQ6M,3883
-ALLMDEV/vertexagentchat.py,sha256=fSfkhdaS8emPk0a2bILIeAMN3zIijQLQpu7YJ2XqNPQ,1851
-ALLMDEV/vertexcli.py,sha256=JyWDSHqx65Xfhhj2-_t33yqvN8DDlLwSuoLkv6TxdK4,1095
-ALLMDEV-1.3.1.dist-info/METADATA,sha256=mFSPqbFVJSTHico1N9MOckBfxx-P3TeDqcuJtSHSzjQ,4676
-ALLMDEV-1.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.3.1.dist-info/entry_points.txt,sha256=JNVr0vn9WZHCesyd6_opoW_UpSgh_UheMv5Le5wvWh4,522
-ALLMDEV-1.3.1.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.3.1.dist-info/RECORD,,
+ALLMDEV/vertexagentapi.py,sha256=fPbLJoy8Wirh7wPc31EzlgLSqfF2e4PkEwYCO9h4yqk,4530
+ALLMDEV/vertexagentchat.py,sha256=k15s16rOtQYNBQnGWI4cXYd4ywOcT2lSaHx_34Qb6DQ,2824
+ALLMDEV/vertexcli.py,sha256=48piq7FW15eRJoQCKR8x3ke_gvsBhJsKVfMLHJX8auw,2124
+ALLMDEV-1.3.2.dist-info/METADATA,sha256=q0_65qktCeZVhVN83uRUyurldNvwou3urdU04cTv1T8,5962
+ALLMDEV-1.3.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.3.2.dist-info/entry_points.txt,sha256=ba3jURsRqh2LaBbetX9AiRLtq9rPzVNR36GOhAa_3N4,556
+ALLMDEV-1.3.2.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.3.2.dist-info/RECORD,,
```

