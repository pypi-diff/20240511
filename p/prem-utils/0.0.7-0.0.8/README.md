# Comparing `tmp/prem-utils-0.0.7.tar.gz` & `tmp/prem-utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prem-utils-0.0.7.tar", last modified: Tue Feb 27 08:35:36 2024, max compression
+gzip compressed data, was "prem-utils-0.0.8.tar", last modified: Tue Feb 27 16:05:54 2024, max compression
```

## Comparing `prem-utils-0.0.7.tar` & `prem-utils-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.679776 prem-utils-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-27 08:35:28.000000 prem-utils-0.0.7/.env.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.671775 prem-utils-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.675776 prem-utils-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-27 08:35:28.000000 prem-utils-0.0.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-27 08:35:28.000000 prem-utils-0.0.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-27 08:35:28.000000 prem-utils-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-27 08:35:28.000000 prem-utils-0.0.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.675776 prem-utils-0.0.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-27 08:35:28.000000 prem-utils-0.0.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-27 08:35:28.000000 prem-utils-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-27 08:35:36.679776 prem-utils-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-27 08:35:28.000000 prem-utils-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-02-27 08:35:28.000000 prem-utils-0.0.7/e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.675776 prem-utils-0.0.7/prem_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.679776 prem-utils-0.0.7/prem_utils/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/anyscale.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/deepinfra.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/fireworksai.py
--rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/lamini.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/octoai.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/perplexity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/prem.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/replicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/together.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/connectors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    42247 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/models.json
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-27 08:35:28.000000 prem-utils-0.0.7/prem_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 08:35:36.679776 prem-utils-0.0.7/prem_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-02-27 08:35:36.000000 prem-utils-0.0.7/prem_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-27 08:35:36.000000 prem-utils-0.0.7/prem_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 08:35:36.000000 prem-utils-0.0.7/prem_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-27 08:35:36.000000 prem-utils-0.0.7/prem_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 08:35:36.000000 prem-utils-0.0.7/prem_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-27 08:35:28.000000 prem-utils-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-27 08:35:28.000000 prem-utils-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-27 08:35:36.679776 prem-utils-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.244467 prem-utils-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-27 16:05:46.000000 prem-utils-0.0.8/.env.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.232468 prem-utils-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.236467 prem-utils-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-27 16:05:46.000000 prem-utils-0.0.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-27 16:05:46.000000 prem-utils-0.0.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-27 16:05:46.000000 prem-utils-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-27 16:05:46.000000 prem-utils-0.0.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.236467 prem-utils-0.0.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-27 16:05:46.000000 prem-utils-0.0.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-27 16:05:46.000000 prem-utils-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-27 16:05:54.244467 prem-utils-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-27 16:05:46.000000 prem-utils-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-02-27 16:05:46.000000 prem-utils-0.0.8/e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.236467 prem-utils-0.0.8/prem_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.240467 prem-utils-0.0.8/prem_utils/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/anyscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/deepinfra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/fireworksai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/lamini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/octoai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/perplexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/prem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/replicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/together.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/connectors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42246 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/models.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-27 16:05:46.000000 prem-utils-0.0.8/prem_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 16:05:54.240467 prem-utils-0.0.8/prem_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-27 16:05:54.000000 prem-utils-0.0.8/prem_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-27 16:05:54.000000 prem-utils-0.0.8/prem_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 16:05:54.000000 prem-utils-0.0.8/prem_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-27 16:05:54.000000 prem-utils-0.0.8/prem_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 16:05:54.000000 prem-utils-0.0.8/prem_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-27 16:05:46.000000 prem-utils-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-27 16:05:46.000000 prem-utils-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-27 16:05:54.244467 prem-utils-0.0.8/setup.cfg
```

### Comparing `prem-utils-0.0.7/.gitignore` & `prem-utils-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/.pre-commit-config.yaml` & `prem-utils-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/.vscode/settings.json` & `prem-utils-0.0.8/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/LICENSE` & `prem-utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/PKG-INFO` & `prem-utils-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prem-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Prem generic utils to use across Prem Components.
 Author-email: Filippo Pedrazzini <filippo@premai.io>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/premAI-io/prem-utils
 Project-URL: Releases, https://github.com/premAI-io/prem-utils/tags
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -42,7 +42,27 @@
 
 prompt = "Hello, how are you?"
 response = connector.chat_completion(model="gpt-3.5-turbo", messages=[{"role": "user", "content": prompt}])
 
 message = response["choices"][0]["message"]["content"]
 print(message)
 ```
+
+## 📦 Contribute
+
+### Install the necessary dependencies
+
+```bash
+virtualenv venv -p=3.11
+source venv/bin/activate
+pip install -r requirements.txt
+```
+
+### Test all or one connector
+
+```bash
+# will run all the connectors
+python e2e.py
+
+# only one connector
+python e2e.py --name perplexity
+```
```

### Comparing `prem-utils-0.0.7/e2e.py` & `prem-utils-0.0.8/e2e.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,63 +21,48 @@
     perplexity,
     prem,
     replicate,
     together,
 )
 
 logger = logging.getLogger(__name__)
+
 load_dotenv()
 
 
 def load_models_file():
     try:
         return json.loads(pathlib.Path("./prem_utils/models.json").read_text())
     except FileNotFoundError:
         logger.error("models.json file not found.")
         return None
     except json.JSONDecodeError:
         logger.error("models.json file contains invalid JSON.")
         return None
 
 
-def get_provider_blob(provider_name: str) -> dict:
-    try:
-        with open("./prem_utils/models.json") as file:
-            data = json.load(file)
-            for connector in data["connectors"]:
-                if connector["provider"] == provider_name:
-                    return connector
-            print(f"No data found for provider: {provider_name}")
-            return None
-    except FileNotFoundError:
-        print("JSON file not found.")
-        return None
-    except json.JSONDecodeError:
-        print("Invalid JSON format.")
-        return None
-
-
 def run_single_connector(connector_name: str) -> None:
     connectors_mapping = load_models_file()["connectors"]
-    all_connectors = [connector["provider"] for connector in connectors_mapping]
-    assert connector_name in all_connectors, ValueError(f"Connector: {connector_name} does not exist")
-    connector = get_provider_blob(provider_name=connector_name)
+
+    for conn in connectors_mapping:
+        if conn["provider"] == connector_name:
+            connector = conn
 
     connector_class_mapping = {
         "anthropic": (anthropic.AnthropicConnector, "ANTHROPIC_API_KEY"),
         "azure": (azure.AzureOpenAIConnector, "AZURE_OPENAI_API_KEY"),
         "cohere": (cohere.CohereConnector, "COHERE_API_KEY"),
         "fireworksai": (fireworksai.FireworksAIConnector, "FIREWORKS_AI_API_KEY"),
         "octoai": (octoai.OctoAIConnector, "OCTO_AI_API_KEY"),
         "openai": (openai.OpenAIConnector, "OPENAI_API_KEY"),
         "replicate": (replicate.ReplicateConnector, "REPLICATE_API_KEY"),
         "together": (together.TogetherConnector, "TOGETHER_AI_API_KEY"),
         "cloudflare": (cloudflare.CloudflareConnector, "CLOUDFLARE_API_KEY"),
         "mistralai": (mistral.MistralConnector, "MISTRAL_AI_API_KEY"),
-        "prem": (prem.PremConnector, "PREMAI_BEARER_TOKEN"),
+        "prem": (prem.PremConnector, "PREM_AI_API_KEY"),
         "deepinfra": (deepinfra.DeepInfraConnector, "DEEP_INFRA_API_KEY"),
         "perplexity": (perplexity.PerplexityAIConnector, "PERPLEXITY_API_KEY"),
         "anyscale": (anyscale.AnyscaleEndpointsConnector, "ANYSCALE_API_KEY"),
         "openrouter": (openrouter.OpenRouterConnector, "OPENROUTER_API_KEY"),
     }
 
     if connector_name == "cloudflare":
@@ -137,41 +122,31 @@
         input = "Hello, how is it going?"
         print(f"Testing model {model_object['slug']} from {connector['provider']} connector")
         response = connector_object.embeddings(model=model_object["slug"], input=input)
         print(f"Embeddings: {len(response['data'][0])}")
         print(f"Model {model_object['slug']} succeeed 🚀 \n\n\n")
 
 
-def run_all_connectors(connector_name_list: list[str] | None = None) -> None:
-    if connector_name_list is None:
-        connectors_mapping = load_models_file()["connectors"]
-        connector_name_list = [connector["provider"] for connector in connectors_mapping]
-
-    for connector in connector_name_list:
-        try:
-            print("=" * 20, f"Running for Connector: {connector}", "=" * 20)
-            run_single_connector(connector_name=connector)
-        except Exception as e:
-            print(f"Error: {e}")
-            continue
-
-
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Testing different providers from prem-utils package")
 
     parser.add_argument(
         "--name",
-        nargs="+",
         help=(
             "The following providers are supported:\n"
             "openai, azure, anthropic, cloudflare, cohere, fireworksai, lamini, mistral, ocotoai, deepinfra, prem, replicate, together\n"  # noqa: E501
             "You can choose any one of them to test it out. Please note: you should include the provider's API key in the .env file. You can check .env.template for your reference. if you put 'all' then all the providers will be used at once"  # noqa: E501
         ),
-        default=["all"],
+        default="all",
     )
 
     args = parser.parse_args()
 
-    if args.name == ["all"]:
-        run_all_connectors()
+    if args.name == "all":
+        connectors_mapping = load_models_file()["connectors"]
+        connector_name_list = [connector["provider"] for connector in connectors_mapping]
+
+        for connector in connector_name_list:
+            logger.info("=" * 20, f"Running for Connector: {connector}", "=" * 20)
+            run_single_connector(connector_name=connector)
     else:
-        run_all_connectors(connector_name_list=args.name)
+        run_single_connector(connector_name=args.name)
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/anthropic.py` & `prem-utils-0.0.8/prem_utils/connectors/anthropic.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/anyscale.py` & `prem-utils-0.0.8/prem_utils/connectors/anyscale.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,34 +9,30 @@
         self, api_key: str, base_url: str = "https://api.endpoints.anyscale.com/v1", prompt_template: str = None
     ) -> None:
         super().__init__(prompt_template=prompt_template, base_url=base_url, api_key=api_key)
 
     def chat_completion(
         self,
         model: str,
-        messages: list[dict[str, Any]],
-        max_tokens: int = 512,
-        frequency_penalty: float = 0.1,
+        messages: list[dict[str]],
+        max_tokens: int = None,
+        frequency_penalty: float = 0,
         presence_penalty: float = 0,
         seed: int | None = None,
         stop: str | list[str] = None,
         stream: bool = False,
         temperature: float = 1,
         top_p: float = 1,
-        tools: list[dict[str, Any]] = None,
-        tool_choice: dict = None,
     ):
         if "anyscale" in model:
             model = model.replace("anyscale/", "", 1)
 
         return super().chat_completion(
             model=model,
             messages=messages,
-            tools=tools,
-            tool_choice=tool_choice,
             stream=stream,
             max_tokens=max_tokens,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             seed=seed,
             stop=stop,
             temperature=temperature,
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/azure.py` & `prem-utils-0.0.8/prem_utils/connectors/azure.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/base.py` & `prem-utils-0.0.8/prem_utils/connectors/base.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/cloudflare.py` & `prem-utils-0.0.8/prem_utils/connectors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/cohere.py` & `prem-utils-0.0.8/prem_utils/connectors/cohere.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/deepinfra.py` & `prem-utils-0.0.8/prem_utils/connectors/openrouter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 from collections.abc import Sequence
 from typing import Any
 
 from prem_utils.connectors.openai import OpenAIConnector
 
 
-class DeepInfraConnector(OpenAIConnector):
+class OpenRouterConnector(OpenAIConnector):
     def __init__(
-        self, api_key: str, base_url: str = "https://api.deepinfra.com/v1/openai", prompt_template: str = None
+        self, api_key: str, base_url: str = "https://openrouter.ai/api/v1/", prompt_template: str = None
     ) -> None:
         super().__init__(prompt_template=prompt_template, base_url=base_url, api_key=api_key)
 
     def chat_completion(
         self,
         model: str,
-        messages: list[dict[str, Any]],
-        max_tokens: int = 512,
-        frequency_penalty: float = 0.1,
+        messages: list[dict[str]],
+        max_tokens: int = None,
+        frequency_penalty: float = 0,
         presence_penalty: float = 0,
         seed: int | None = None,
         stop: str | list[str] = None,
         stream: bool = False,
         temperature: float = 1,
         top_p: float = 1,
-        tools: list[dict[str, Any]] = None,
-        tool_choice: dict = None,
     ):
-        if "deepinfra" in model:
-            model = model.replace("deepinfra/", "", 1)
+        if "openrouter" in model:
+            model = model.replace("openrouter/", "", 1)
 
         return super().chat_completion(
-            model,
-            messages,
-            max_tokens,
-            frequency_penalty,
-            presence_penalty,
-            seed,
-            stop,
-            stream,
-            temperature,
-            top_p,
-            tools,
-            tool_choice,
+            model=model,
+            messages=messages,
+            stream=stream,
+            max_tokens=max_tokens,
+            frequency_penalty=frequency_penalty,
+            presence_penalty=presence_penalty,
+            seed=seed,
+            stop=stop,
+            temperature=temperature,
+            top_p=top_p,
         )
 
     def embeddings(
         self,
         model: str,
         input: str | Sequence[str] | Sequence[int] | Sequence[Sequence[int]],
         encoding_format: str = "float",
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/fireworksai.py` & `prem-utils-0.0.8/prem_utils/connectors/fireworksai.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/lamini.py` & `prem-utils-0.0.8/prem_utils/connectors/lamini.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/mistral.py` & `prem-utils-0.0.8/prem_utils/connectors/mistral.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/octoai.py` & `prem-utils-0.0.8/prem_utils/connectors/octoai.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/openai.py` & `prem-utils-0.0.8/prem_utils/connectors/openai.py`

 * *Files 26% similar despite different names*

```diff
@@ -72,53 +72,30 @@
         frequency_penalty: float = 0,
         presence_penalty: float = 0,
         seed: int | None = None,
         stop: str | list[str] = None,
         stream: bool = False,
         temperature: float = 1,
         top_p: float = 1,
-        tools: list[dict[str]] = None,
-        tool_choice: dict = None,
-        logit_bias: dict = None,
-        logprobs: bool = None,
-        top_logprobs: int = None,
     ):
         if self.prompt_template is not None:
             messages = self.apply_prompt_template(messages)
 
-        # NOTE custom logic for providers who don't have
-        # their sdk, but they use direclty OpenAI python client.
-
-        other_parameters = {}
-        if tools is not None and tool_choice is not None:
-            other_parameters["tools"] = tools
-            other_parameters["tool_choice"] = tool_choice
-
-        if logit_bias is not None:
-            other_parameters["logit_bias"] = logit_bias
-
-        if logprobs is not None:
-            other_parameters["logprobs"] = logprobs
-
-        if top_logprobs is not None:
-            other_parameters["top_logprobs"] = top_logprobs
-
         try:
             response = self.client.chat.completions.create(
                 model=model,
                 messages=messages,
                 stream=stream,
                 max_tokens=max_tokens,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
                 seed=seed,
                 stop=stop,
                 temperature=temperature,
                 top_p=top_p,
-                **other_parameters,
             )
         except (
             NotFoundError,
             APIResponseValidationError,
             ConflictError,
             APIStatusError,
             APITimeoutError,
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/openrouter.py` & `prem-utils-0.0.8/prem_utils/connectors/deepinfra.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,37 @@
 from collections.abc import Sequence
 from typing import Any
 
 from prem_utils.connectors.openai import OpenAIConnector
 
 
-class OpenRouterConnector(OpenAIConnector):
+class DeepInfraConnector(OpenAIConnector):
     def __init__(
-        self, api_key: str, base_url: str = "https://openrouter.ai/api/v1/", prompt_template: str = None
+        self, api_key: str, base_url: str = "https://api.deepinfra.com/v1/openai", prompt_template: str = None
     ) -> None:
         super().__init__(prompt_template=prompt_template, base_url=base_url, api_key=api_key)
 
     def chat_completion(
         self,
         model: str,
-        messages: list[dict[str, Any]],
-        max_tokens: int = 512,
-        frequency_penalty: float = 0.1,
+        messages: list[dict[str]],
+        max_tokens: int = None,
+        frequency_penalty: float = 0,
         presence_penalty: float = 0,
         seed: int | None = None,
         stop: str | list[str] = None,
         stream: bool = False,
         temperature: float = 1,
         top_p: float = 1,
-        tools: list[dict[str, Any]] = None,
-        tool_choice: dict = None,
     ):
-        model = model.replace("openrouter/", "", 1)
+        if "deepinfra" in model:
+            model = model.replace("deepinfra/", "", 1)
 
         return super().chat_completion(
-            model=model,
-            messages=messages,
-            tools=tools,
-            tool_choice=tool_choice,
-            stream=stream,
-            max_tokens=max_tokens,
-            frequency_penalty=frequency_penalty,
-            presence_penalty=presence_penalty,
-            seed=seed,
-            stop=stop,
-            temperature=temperature,
-            top_p=top_p,
+            model, messages, max_tokens, frequency_penalty, presence_penalty, seed, stop, stream, temperature, top_p
         )
 
     def embeddings(
         self,
         model: str,
         input: str | Sequence[str] | Sequence[int] | Sequence[Sequence[int]],
         encoding_format: str = "float",
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/perplexity.py` & `prem-utils-0.0.8/prem_utils/connectors/perplexity.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,46 +7,32 @@
 class PerplexityAIConnector(OpenAIConnector):
     def __init__(self, api_key: str, base_url: str = "https://api.perplexity.ai", prompt_template: str = None) -> None:
         super().__init__(prompt_template=prompt_template, base_url=base_url, api_key=api_key)
 
     def chat_completion(
         self,
         model: str,
-        messages: list[dict[str, Any]],
+        messages: list[dict[str]],
         max_tokens: int = None,
-        frequency_penalty: float = 0.1,
-        log_probs: int = None,
-        logit_bias: dict[str, float] = None,
+        frequency_penalty: float = 0,
         presence_penalty: float = 0,
         seed: int | None = None,
         stop: str | list[str] = None,
         stream: bool = False,
         temperature: float = 1,
         top_p: float = 1,
-        tools: list[dict[str, Any]] = None,
-        tool_choice: dict = None,
     ):
+        if frequency_penalty == 0:
+            frequency_penalty = 0.1
+
         if "perplexity" in model:
             model = model.replace("perplexity/", "", 1)
 
         return super().chat_completion(
-            model,
-            messages,
-            max_tokens,
-            frequency_penalty,
-            log_probs,
-            logit_bias,
-            presence_penalty,
-            seed,
-            stop,
-            stream,
-            temperature,
-            top_p,
-            tools,
-            tool_choice,
+            model, messages, max_tokens, frequency_penalty, presence_penalty, seed, stop, stream, temperature, top_p
         )
 
     def embeddings(
         self,
         model: str,
         input: str | Sequence[str] | Sequence[int] | Sequence[Sequence[int]],
         encoding_format: str = "float",
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/prem.py` & `prem-utils-0.0.8/prem_utils/connectors/prem.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,17 +111,21 @@
         return responses
 
     def chat_completion(
         self,
         model: str,
         messages: list[dict[str]],
         max_tokens: int | None = 128,
-        temperature: float | None = 1.0,
-        top_p: float | None = 0.95,
-        stream: bool | None = False,
+        frequency_penalty: float = 0,
+        presence_penalty: float = 0,
+        seed: int | None = None,
+        stop: str | list[str] = None,
+        stream: bool = False,
+        temperature: float = 1,
+        top_p: float = 1,
     ) -> str | Generator[str, None, None]:
         try:
             if stream:
                 return self._chat_completion_stream(
                     model=model,
                     messages=messages,
                     max_tokens=max_tokens,
```

### Comparing `prem-utils-0.0.7/prem_utils/connectors/replicate.py` & `prem-utils-0.0.8/prem_utils/connectors/replicate.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/together.py` & `prem-utils-0.0.8/prem_utils/connectors/together.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/connectors/utils.py` & `prem-utils-0.0.8/prem_utils/connectors/utils.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/errors.py` & `prem-utils-0.0.8/prem_utils/errors.py`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/prem_utils/models.json` & `prem-utils-0.0.8/prem_utils/models.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999537037037037%*

 * *Differences: {"'connectors'": "{11: {'models': {5: {'slug': 'gemma', delete: ['gemma']}}}}"}*

```diff
@@ -579,16 +579,16 @@
                 {
                     "context_window": 2048,
                     "model_type": "text2text",
                     "slug": "stable_lm2"
                 },
                 {
                     "context_window": 2048,
-                    "gemma": "gemma",
-                    "model_type": "text2text"
+                    "model_type": "text2text",
+                    "slug": "gemma"
                 },
                 {
                     "coming_soon": true,
                     "model_type": "text2text",
                     "slug": "prem-1b-chat"
                 },
                 {
```

### Comparing `prem-utils-0.0.7/prem_utils.egg-info/PKG-INFO` & `prem-utils-0.0.8/prem_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prem-utils
-Version: 0.0.7
+Version: 0.0.8
 Summary: Prem generic utils to use across Prem Components.
 Author-email: Filippo Pedrazzini <filippo@premai.io>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/premAI-io/prem-utils
 Project-URL: Releases, https://github.com/premAI-io/prem-utils/tags
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -42,7 +42,27 @@
 
 prompt = "Hello, how are you?"
 response = connector.chat_completion(model="gpt-3.5-turbo", messages=[{"role": "user", "content": prompt}])
 
 message = response["choices"][0]["message"]["content"]
 print(message)
 ```
+
+## 📦 Contribute
+
+### Install the necessary dependencies
+
+```bash
+virtualenv venv -p=3.11
+source venv/bin/activate
+pip install -r requirements.txt
+```
+
+### Test all or one connector
+
+```bash
+# will run all the connectors
+python e2e.py
+
+# only one connector
+python e2e.py --name perplexity
+```
```

### Comparing `prem-utils-0.0.7/prem_utils.egg-info/SOURCES.txt` & `prem-utils-0.0.8/prem_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prem-utils-0.0.7/pyproject.toml` & `prem-utils-0.0.8/pyproject.toml`

 * *Files identical despite different names*

