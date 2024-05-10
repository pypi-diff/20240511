# Comparing `tmp/indexify-extractor-sdk-0.0.8.tar.gz` & `tmp/indexify-extractor-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexify-extractor-sdk-0.0.8.tar", last modified: Wed Jan 17 20:13:11 2024, max compression
+gzip compressed data, was "indexify-extractor-sdk-0.0.9.tar", last modified: Tue Jan 23 22:39:33 2024, max compression
```

## Comparing `indexify-extractor-sdk-0.0.8.tar` & `indexify-extractor-sdk-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-17 20:13:11.966523 indexify-extractor-sdk-0.0.8/
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)    11351 2023-12-19 00:14:46.000000 indexify-extractor-sdk-0.0.8/LICENSE
--rw-r--r--   0 diptanuc  (1000) diptanuc  (1000)     1605 2024-01-17 20:13:11.966523 indexify-extractor-sdk-0.0.8/PKG-INFO
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     1609 2024-01-17 20:07:03.000000 indexify-extractor-sdk-0.0.8/README.md
-drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-17 20:13:11.966523 indexify-extractor-sdk-0.0.8/extractors_sdk_tests/
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)        0 2023-12-02 00:17:00.000000 indexify-extractor-sdk-0.0.8/extractors_sdk_tests/__init__.py
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     1276 2023-12-02 00:17:00.000000 indexify-extractor-sdk-0.0.8/extractors_sdk_tests/test_mock_extractor.py
-drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-17 20:13:11.966523 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)      298 2023-11-16 09:21:02.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/__init__.py
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     2275 2023-12-02 00:17:00.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/base_embedding.py
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     3845 2024-01-17 20:07:03.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/base_extractor.py
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     2031 2023-12-29 01:36:28.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/mock_extractor.py
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     2686 2023-10-16 00:24:28.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/sentence_transformer.py
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)       22 2024-01-17 20:07:03.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/version.py
-drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-17 20:13:11.966523 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/
--rw-r--r--   0 diptanuc  (1000) diptanuc  (1000)     1605 2024-01-17 20:13:11.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)      571 2024-01-17 20:13:11.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)        1 2024-01-17 20:13:11.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)      327 2024-01-17 20:13:11.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/requires.txt
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)       44 2024-01-17 20:13:11.000000 indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/top_level.txt
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)       38 2024-01-17 20:13:11.966523 indexify-extractor-sdk-0.0.8/setup.cfg
--rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     3744 2024-01-17 20:13:09.000000 indexify-extractor-sdk-0.0.8/setup.py
+drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-23 22:39:33.560487 indexify-extractor-sdk-0.0.9/
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)    11351 2023-12-19 00:14:46.000000 indexify-extractor-sdk-0.0.9/LICENSE
+-rw-r--r--   0 diptanuc  (1000) diptanuc  (1000)     1605 2024-01-23 22:39:33.560487 indexify-extractor-sdk-0.0.9/PKG-INFO
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     1609 2024-01-17 20:07:03.000000 indexify-extractor-sdk-0.0.9/README.md
+drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-23 22:39:33.560487 indexify-extractor-sdk-0.0.9/extractors_sdk_tests/
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)        0 2023-12-02 00:17:00.000000 indexify-extractor-sdk-0.0.9/extractors_sdk_tests/__init__.py
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     1276 2023-12-02 00:17:00.000000 indexify-extractor-sdk-0.0.9/extractors_sdk_tests/test_mock_extractor.py
+drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-23 22:39:33.560487 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)      258 2024-01-23 21:28:07.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/__init__.py
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     2138 2024-01-23 21:33:15.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/base_embedding.py
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     4454 2024-01-23 22:27:48.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/base_extractor.py
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     1637 2024-01-23 22:34:01.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/mock_extractor.py
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     2686 2023-10-16 00:24:28.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/sentence_transformer.py
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)       22 2024-01-22 21:34:16.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/version.py
+drwxrwxr-x   0 diptanuc  (1000) diptanuc  (1000)        0 2024-01-23 22:39:33.560487 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/
+-rw-r--r--   0 diptanuc  (1000) diptanuc  (1000)     1605 2024-01-23 22:39:33.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)      571 2024-01-23 22:39:33.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)        1 2024-01-23 22:39:33.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)      327 2024-01-23 22:39:33.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/requires.txt
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)       44 2024-01-23 22:39:33.000000 indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)       38 2024-01-23 22:39:33.560487 indexify-extractor-sdk-0.0.9/setup.cfg
+-rw-rw-r--   0 diptanuc  (1000) diptanuc  (1000)     3744 2024-01-22 23:51:57.000000 indexify-extractor-sdk-0.0.9/setup.py
```

### Comparing `indexify-extractor-sdk-0.0.8/LICENSE` & `indexify-extractor-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `indexify-extractor-sdk-0.0.8/PKG-INFO` & `indexify-extractor-sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexify-extractor-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Content Extractor SDK for Indexify
 Home-page: https://github.com/tensorlakeai/indexify
 Author: Diptanu Choudhury
 Author-email: diptanuc@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indexify-extractor-sdk-0.0.8/README.md` & `indexify-extractor-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `indexify-extractor-sdk-0.0.8/extractors_sdk_tests/test_mock_extractor.py` & `indexify-extractor-sdk-0.0.9/extractors_sdk_tests/test_mock_extractor.py`

 * *Files identical despite different names*

### Comparing `indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/base_embedding.py` & `indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/base_embedding.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,40 +14,36 @@
 class EmbeddingInputParams(BaseModel):
     overlap: int = 0
     chunk_size: int = 0
     text_splitter: Literal["char", "recursive"] = "recursive"
 
 
 class BaseEmbeddingExtractor(Extractor):
+    input_mimes = ["text/plain"]
     def __init__(self, max_context_length: int):
         self._model_context_length: int = max_context_length
 
     def extract(
-        self, content_list: List[Content], params: EmbeddingInputParams
-    ) -> List[List[Content]]:
+        self, content: Content, params: EmbeddingInputParams
+    ) -> List[Content]:
         if params.chunk_size == 0:
             params.chunk_size = self._model_context_length
 
         splitter: Callable[[str], List[str]] = self._create_splitter(params)
-        extracted_content = []
-        for content in content_list:
-            extracted_embeddings = []
-            if content.content_type != "text/plain":
-                continue
-            text = content.data.decode("utf-8")
-            chunks: List[str] = splitter(text)
-            embeddings_list = self.extract_embeddings(chunks)
-            for chunk, embeddings in zip(chunks, embeddings_list):
-                content = Content.from_text(
-                    text=chunk,
-                    feature=Feature.embedding(value=embeddings),
-                )
-                extracted_embeddings.append(content)
-            extracted_content.append(extracted_embeddings)
-        return extracted_content
+        extracted_embeddings = []
+        text = content.data.decode("utf-8")
+        chunks: List[str] = splitter(text)
+        embeddings_list = self.extract_embeddings(chunks)
+        for chunk, embeddings in zip(chunks, embeddings_list):
+            content = Content.from_text(
+                text=chunk,
+                feature=Feature.embedding(values=embeddings),
+            )
+            extracted_embeddings.append(content)
+        return extracted_embeddings
 
     def _create_splitter(
         self, input_params: EmbeddingInputParams
     ) -> Callable[[str], List[str]]:
         if input_params.text_splitter == "recursive":
             return text_splitter.RecursiveCharacterTextSplitter(
                 chunk_size=input_params.chunk_size,
@@ -59,7 +55,10 @@
                 chunk_overlap=input_params.overlap,
                 separator="\n\n",
             ).split_text
 
     @abstractmethod
     def extract_embeddings(self, texts: List[str]) -> List[List[float]]:
         ...
+
+    def sample_input(self) -> Content:
+        return Content.from_text("hello world")
```

### Comparing `indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/base_extractor.py` & `indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/base_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,105 +1,127 @@
 from abc import ABC, abstractmethod
-from typing import List, Type, Optional, Union
+from typing import Dict, List, Type, Optional, Union
 import json
 from importlib import import_module
 from typing import get_type_hints
 
-from pydantic import BaseModel, Json, Field
+from pydantic import BaseModel, Json
 
 class EmbeddingSchema(BaseModel):
-    distance_metric: str
     dim: int
+    distance: str
 
-class ExtractorSchema(BaseModel):
-    features: dict[str, Union[EmbeddingSchema, Json]] = Field(default_factory=dict)
+class Embedding(BaseModel):
+    values: List[float]
+    distance: str
 
 class InternalExtractorSchema(BaseModel):
     embedding_schemas: dict[str, EmbeddingSchema]
     input_params: Optional[str]
+    input_mimes: List[str]
 
 class Feature(BaseModel):
     feature_type: str
     name: str
     value: str
 
     @classmethod
-    def embedding(cls, value: List[float], name: str="embedding"):
-        return cls(feature_type="embedding", name=name, value=json.dumps(value))
-    
-    @classmethod
-    def ner(cls, entity: str, value: str, score: float, name: str="ner"):
-        return cls(feature_type="ner", name=name, value=json.dumps({"entity": entity, "value": value, "score": score}))
+    def embedding(cls, values: List[float], name: str="embedding", distance="cosine"):
+        embedding = Embedding(values=values, distance=distance)
+        return cls(feature_type="embedding", name=name, value=embedding.model_dump_json())
     
     @classmethod
     def metadata(cls, value: Json, name: str="metadata"):
         return cls(feature_type="metadata", name=name, value=json.dumps(value))
 
 class Content(BaseModel):
     content_type: Optional[str]
-    data: bytes 
-    feature:Optional[Feature] = None
+    data: bytes
+    feature: Optional[Feature] = None
+    labels: Optional[Dict[str, str]] = None
+
+    @classmethod
+    def from_text(
+        cls, text: str, feature: Feature = None, labels: Dict[str, str] = None
+    ):
+
+        return cls(
+            content_type="text/plain",
+            data=bytes(text, "utf-8"),
+            feature=feature,
+            labels=labels,
+        )
+    
 
     @classmethod
-    def from_text(cls, text: str, feature: Feature=None):
-        return cls(content_type="text/plain", data=bytes(text, "utf-8"), feature=feature)
+    def from_file(cls, path: str):
+        import mimetypes
+        m = mimetypes.guess_extension(path)
+        with open(path, "rb") as f:
+            return cls(content_type=m, data=f.read())
+
     
 class Extractor(ABC):
 
+    system_dependencies: List[str] = []
+
+    python_dependencies: List[str] = []
+
+    description: str = ""
+
+    input_mimes = ["text/plain"]
+
     @abstractmethod
     def extract(
-        self, content: List[Content], params: Type[BaseModel]=None) -> List[List[Content]]:
+        self, content: Content, params: Type[BaseModel]=None) -> List[Content]:
         """
         Extracts information from the content.
         """
         pass
 
-
-    @classmethod
     @abstractmethod
-    def schemas(cls) -> ExtractorSchema:
-        """
-        Returns a list of options for indexing.
-        """
-        return NotImplemented
+    def sample_input(self) -> Content:
+        pass
+    
+    def run_sample_input(self) -> List[Content]:
+        return self.extract(self.sample_input())
 
 class ExtractorWrapper:
 
     def __init__(self, module_name: str, class_name: str):
         self._module = import_module(module_name)
         self._cls = getattr(self._module, class_name)
         self._param_cls = get_type_hints(self._cls.extract).get("params", None)
-        self._instance = self._cls()
+        self._instance: Extractor = self._cls()
 
     def extract(self, content: List[Content], params: Json) -> List[List[Content]]:
         params_dict = json.loads(params)
         param_instance = self._param_cls.model_validate(params_dict) if self._param_cls else None
-        content_list = []
-        for c in content:
-            content_list.append(Content(content_type=c.content_type, data=bytes(c.data)))
-        return self._instance.extract(content_list, param_instance)
 
-    def schemas(self) -> InternalExtractorSchema:
-        schema: ExtractorSchema = self._cls.schemas()
+        # This is because the rust side does batching and on python we don't batch 
+        out = []
+        for c in content:
+            extracted_data = self._instance.extract(Content(content_type=c.content_type, data=bytes(c.data)), param_instance)
+            out.append(extracted_data)
+        return out
+    
+    def schema(self, input_params: Type[BaseModel] = None) -> InternalExtractorSchema:
+        s_input = self._instance.sample_input()
+        input_mimes = self._instance.input_mimes
+        # Come back to this when we can support schemas based on user defined input params
+        if input_params is None:
+            input_params = self._param_cls() if self._param_cls else None
+        out_c: List[Content] = self._instance.extract(s_input, input_params)
         embedding_schemas = {}
-        for k,v in schema.features.items():
-            if isinstance(v, EmbeddingSchema):
-                embedding_schemas[k] = v
-                continue
+        metadata_schemas = {}
         json_schema = self._param_cls.model_json_schema() if self._param_cls else {}
         json_schema['additionalProperties'] = False
-        return InternalExtractorSchema(embedding_schemas=embedding_schemas, input_params=json.dumps(json_schema))
-    
-def extractor_schema(module_name: str, class_name: str) -> InternalExtractorSchema:
-    module = import_module(module_name)
-    cls = getattr(module, class_name)
-    param_cls = get_type_hints(cls.extract).get("params", None)
-    schema: ExtractorSchema = cls.schemas()
-    embedding_schemas = {}
-    if schema is not None:
-        for k,v in schema.features.items():
-            if isinstance(v, EmbeddingSchema):
-                embedding_schemas[k] = v
-                continue
-    json_schema = param_cls.model_json_schema() if param_cls else {}
-    json_schema['additionalProperties'] = False
-    return InternalExtractorSchema(embedding_schemas=embedding_schemas, input_params=json.dumps(json_schema))
+        for content in out_c:
+            if content.feature is not None:
+                if content.feature.feature_type == "embedding":
+                    embedding_value: Embedding = Embedding.parse_raw(content.feature.value)
+                    embedding_schema = EmbeddingSchema(dim=len(embedding_value.values), distance=embedding_value.distance)
+                    embedding_schemas[content.feature.name] = embedding_schema
+                elif content.feature.feature_type == "metadata":
+                    metadata_schemas[content.feature.name] = json.loads(content.feature.value)
+
+        return InternalExtractorSchema(embedding_schemas=embedding_schemas, input_mimes=input_mimes, input_params=json.dumps(json_schema))
```

### Comparing `indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/mock_extractor.py` & `indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/mock_extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,53 @@
-from .base_extractor import Extractor, Content, Feature, EmbeddingSchema, ExtractorSchema
+from .base_extractor import Extractor, Content, Feature
 
 from typing import List
 
 from pydantic import BaseModel
 
+import json
+
 class InputParams(BaseModel):
     a: int = 0
     b: str = ""
 
 class MockExtractor(Extractor):
+    input_mimes = ["text/plain", "application/pdf", "image/jpeg"]
     def __init__(self):
         super().__init__()
 
     def extract(
-        self, content: List[Content], params: InputParams
-    ) -> List[List[Content]]:
+        self, content: Content, params: InputParams
+    ) -> List[Content]:
         return [
-            [
                 Content.from_text(
-                    text="Hello World", feature=Feature.embedding(value=[1, 2, 3])
+                    text="Hello World", feature=Feature.embedding(values=[1, 2, 3])
                 ),
                 Content.from_text(
-                    text="Pipe Baz", feature=Feature.embedding(value=[1, 2, 3])
+                    text="Pipe Baz", feature=Feature.embedding(values=[1, 2, 3])
                 ),
                 Content.from_text(
                     text="Hello World",
-                    feature=Feature.ner(entity="Kevin Durant", value="PER", score=0.9),
+                    feature=Feature.metadata(json.loads('{"a": 1, "b": "foo"}')),
+                    labels={"label1": "val1", "label2": "val2"}
                 ),
             ]
-        ]
     
-
-    def extract_query_embeddings(self, query: str) -> List[float]:
-        return [1, 2, 3]
-
-    @classmethod
-    def schemas(cls) -> ExtractorSchema:
-        """
-        Returns a list of options for indexing.
-        """
-        return ExtractorSchema(
-            features={"embedding": EmbeddingSchema(distance_metric="cosine", dim=3)},
-        )
-
-
+    def sample_input(self) -> Content:
+        return Content.from_text("hello world")
+    
 class MockExtractorNoInputParams(Extractor):
     def __init__(self):
         super().__init__()
 
-    def extract(self, content: List[Content], params=None) -> List[List[Content]]:
+    def extract(self, content: Content, params=None) -> List[Content]:
         return [
-            [
                 Content.from_text(
-                    text="Hello World", feature=Feature.embedding(value=[1, 2, 3])
+                    text="Hello World", feature=Feature.embedding(values=[1, 2, 3])
                 ),
                 Content.from_text(
-                    text="Pipe Baz", feature=Feature.embedding(value=[1, 2, 3])
+                    text="Pipe Baz", feature=Feature.embedding(values=[1, 2, 3])
                 ),
             ]
-        ]
-
-    @classmethod
-    def schemas(cls) -> ExtractorSchema:
-        """
-        Returns a list of options for indexing.
-        """
-        return ExtractorSchema(
-            features={"embedding": EmbeddingSchema(distance_metric="cosine", dim=3)},
-        )
+    
+    def sample_input(self) -> Content:
+        return Content.from_text("hello world")
```

### Comparing `indexify-extractor-sdk-0.0.8/indexify_extractor_sdk/sentence_transformer.py` & `indexify-extractor-sdk-0.0.9/indexify_extractor_sdk/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/PKG-INFO` & `indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexify-extractor-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Content Extractor SDK for Indexify
 Home-page: https://github.com/tensorlakeai/indexify
 Author: Diptanu Choudhury
 Author-email: diptanuc@gmail.com
 License: Apache 2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `indexify-extractor-sdk-0.0.8/indexify_extractor_sdk.egg-info/SOURCES.txt` & `indexify-extractor-sdk-0.0.9/indexify_extractor_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `indexify-extractor-sdk-0.0.8/setup.py` & `indexify-extractor-sdk-0.0.9/setup.py`

 * *Files identical despite different names*

