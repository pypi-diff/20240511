# Comparing `tmp/semantic_router-0.0.8.tar.gz` & `tmp/semantic_router-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_router-0.0.8.tar", max compression
+gzip compressed data, was "semantic_router-0.0.9.tar", max compression
```

## Comparing `semantic_router-0.0.8.tar` & `semantic_router-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2023-12-14 09:19:43.201526 semantic_router-0.0.8/LICENSE
--rw-r--r--   0        0        0     4147 2023-12-14 09:19:43.201526 semantic_router-0.0.8/README.md
--rw-r--r--   0        0        0      941 2023-12-14 09:19:43.205525 semantic_router-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      119 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/__init__.py
--rw-r--r--   0        0        0      204 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/encoders/__init__.py
--rw-r--r--   0        0        0      273 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/encoders/base.py
--rw-r--r--   0        0        0     1682 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/encoders/bm25.py
--rw-r--r--   0        0        0     1091 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/encoders/cohere.py
--rw-r--r--   0        0        0     1917 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/encoders/openai.py
--rw-r--r--   0        0        0     5569 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/hybrid_layer.py
--rw-r--r--   0        0        0     4626 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/layer.py
--rw-r--r--   0        0        0      792 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/linear.py
--rw-r--r--   0        0        0     1222 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/schema.py
--rw-r--r--   0        0        0        0 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/utils/__init__.py
--rw-r--r--   0        0        0     1162 2023-12-14 09:19:43.205525 semantic_router-0.0.8/semantic_router/utils/logger.py
--rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 semantic_router-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-12-15 13:44:00.805233 semantic_router-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4132 2023-12-15 13:44:00.805233 semantic_router-0.0.9/README.md
+-rw-r--r--   0        0        0      940 2023-12-15 13:44:00.809233 semantic_router-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      119 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/__init__.py
+-rw-r--r--   0        0        0      204 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/encoders/__init__.py
+-rw-r--r--   0        0        0      273 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/encoders/base.py
+-rw-r--r--   0        0        0     1682 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/encoders/bm25.py
+-rw-r--r--   0        0        0     1098 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/encoders/cohere.py
+-rw-r--r--   0        0        0     1917 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/encoders/openai.py
+-rw-r--r--   0        0        0     5569 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/hybrid_layer.py
+-rw-r--r--   0        0        0     4626 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/layer.py
+-rw-r--r--   0        0        0      792 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/linear.py
+-rw-r--r--   0        0        0     1222 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/schema.py
+-rw-r--r--   0        0        0        0 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/utils/__init__.py
+-rw-r--r--   0        0        0     1162 2023-12-15 13:44:00.809233 semantic_router-0.0.9/semantic_router/utils/logger.py
+-rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 semantic_router-0.0.9/PKG-INFO
```

### Comparing `semantic_router-0.0.8/LICENSE` & `semantic_router-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/README.md` & `semantic_router-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,31 +20,31 @@
 ```
 pip install -qU semantic-router
 ```
 
 We begin by defining a set of `Decision` objects. These are the decision paths that the semantic router can decide to use, let's try two simple decisions for now — one for talk on _politics_ and another for _chitchat_:
 
 ```python
-from semantic_router.schema import Decision
+from semantic_router.schema import Route
 
 # we could use this as a guide for our chatbot to avoid political conversations
-politics = Decision(
+politics = Route(
     name="politics",
     utterances=[
         "isn't politics the best thing ever",
         "why don't you tell me about your political opinions",
         "don't you just love the president" "don't you just hate the president",
         "they're going to destroy this country!",
         "they will save the country!",
     ],
 )
 
 # this could be used as an indicator to our chatbot to switch to a more
 # conversational prompt
-chitchat = Decision(
+chitchat = Route(
     name="chitchat",
     utterances=[
         "how's the weather today?",
         "how are things going?",
         "lovely weather today",
         "the weather is horrendous",
         "let's go to the chippy",
@@ -69,17 +69,17 @@
 os.environ["OPENAI_API_KEY"] = "<YOUR_API_KEY>"
 encoder = OpenAIEncoder()
 ```
 
 With our `decisions` and `encoder` defined we now create a `DecisionLayer`. The decision layer handles our semantic decision making.
 
 ```python
-from semantic_router.layer import DecisionLayer
+from semantic_router.layer import RouteLayer
 
-dl = DecisionLayer(encoder=encoder, decisions=decisions)
+dl = RouteLayer(encoder=encoder, decisions=decisions)
 ```
 
 We can now use our decision layer to make super fast decisions based on user queries. Let's try with two queries that should trigger our decisions:
 
 ```python
 dl("don't you love politics?")
 ```
```

### Comparing `semantic_router-0.0.8/pyproject.toml` & `semantic_router-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "semantic-router"
-version = "0.0.8"
+version = "0.0.9"
 description = "Super fast semantic router for AI decision making"
 authors = [
     "James Briggs <james@aurelio.ai>",
     "Siraj Aizlewood <siraj@aurelio.ai>",
     "Simonas Jakubonis <simonas@aurelio.ai>",
     "Luca Mannini <luca@aurelio.ai>",
     "Bogdan Buduroiu <bogdan@aurelio.ai>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 pydantic = "^1.8.2"
 openai = "^1.3.9"
 cohere = "^4.32"
 numpy = "^1.25.2"
 pinecone-text = "^0.7.0"
 colorlog = "^6.8.0"
 
@@ -32,11 +32,11 @@
 mypy = "^1.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff.per-file-ignores]
-"*.ipynb" = ["E402"]
+"*.ipynb" = ["ALL"]
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `semantic_router-0.0.8/semantic_router/encoders/bm25.py` & `semantic_router-0.0.9/semantic_router/encoders/bm25.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/semantic_router/encoders/cohere.py` & `semantic_router-0.0.9/semantic_router/encoders/cohere.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import cohere
 
 from semantic_router.encoders import BaseEncoder
 
 
 class CohereEncoder(BaseEncoder):
-    client: cohere.Client | None
+    client: cohere.Client | None = None
 
     def __init__(
         self,
         name: str = os.getenv("COHERE_MODEL_NAME", "embed-english-v3.0"),
         cohere_api_key: str | None = None,
     ):
         super().__init__(name=name)
```

### Comparing `semantic_router-0.0.8/semantic_router/encoders/openai.py` & `semantic_router-0.0.9/semantic_router/encoders/openai.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/semantic_router/hybrid_layer.py` & `semantic_router-0.0.9/semantic_router/hybrid_layer.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/semantic_router/layer.py` & `semantic_router-0.0.9/semantic_router/layer.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/semantic_router/linear.py` & `semantic_router-0.0.9/semantic_router/linear.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/semantic_router/schema.py` & `semantic_router-0.0.9/semantic_router/schema.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/semantic_router/utils/logger.py` & `semantic_router-0.0.9/semantic_router/utils/logger.py`

 * *Files identical despite different names*

### Comparing `semantic_router-0.0.8/PKG-INFO` & `semantic_router-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: semantic-router
-Version: 0.0.8
+Version: 0.0.9
 Summary: Super fast semantic router for AI decision making
 Author: James Briggs
 Author-email: james@aurelio.ai
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cohere (>=4.32,<5.0)
 Requires-Dist: colorlog (>=6.8.0,<7.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: openai (>=1.3.9,<2.0.0)
 Requires-Dist: pinecone-text (>=0.7.0,<0.8.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
@@ -37,31 +38,31 @@
 ```
 pip install -qU semantic-router
 ```
 
 We begin by defining a set of `Decision` objects. These are the decision paths that the semantic router can decide to use, let's try two simple decisions for now — one for talk on _politics_ and another for _chitchat_:
 
 ```python
-from semantic_router.schema import Decision
+from semantic_router.schema import Route
 
 # we could use this as a guide for our chatbot to avoid political conversations
-politics = Decision(
+politics = Route(
     name="politics",
     utterances=[
         "isn't politics the best thing ever",
         "why don't you tell me about your political opinions",
         "don't you just love the president" "don't you just hate the president",
         "they're going to destroy this country!",
         "they will save the country!",
     ],
 )
 
 # this could be used as an indicator to our chatbot to switch to a more
 # conversational prompt
-chitchat = Decision(
+chitchat = Route(
     name="chitchat",
     utterances=[
         "how's the weather today?",
         "how are things going?",
         "lovely weather today",
         "the weather is horrendous",
         "let's go to the chippy",
@@ -86,17 +87,17 @@
 os.environ["OPENAI_API_KEY"] = "<YOUR_API_KEY>"
 encoder = OpenAIEncoder()
 ```
 
 With our `decisions` and `encoder` defined we now create a `DecisionLayer`. The decision layer handles our semantic decision making.
 
 ```python
-from semantic_router.layer import DecisionLayer
+from semantic_router.layer import RouteLayer
 
-dl = DecisionLayer(encoder=encoder, decisions=decisions)
+dl = RouteLayer(encoder=encoder, decisions=decisions)
 ```
 
 We can now use our decision layer to make super fast decisions based on user queries. Let's try with two queries that should trigger our decisions:
 
 ```python
 dl("don't you love politics?")
 ```
```

