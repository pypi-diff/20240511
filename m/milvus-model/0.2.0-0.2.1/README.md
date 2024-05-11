# Comparing `tmp/milvus-model-0.2.0.tar.gz` & `tmp/milvus_model-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus-model-0.2.0.tar", last modified: Mon Apr  1 15:20:31 2024, max compression
+gzip compressed data, was "milvus_model-0.2.1.tar", last modified: Sat May 11 12:10:10 2024, max compression
```

## Comparing `milvus-model-0.2.0.tar` & `milvus_model-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.006065 milvus-model-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-01 15:20:24.000000 milvus-model-0.2.0/.github/workflows/publish_dev_package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-01 15:20:24.000000 milvus-model-0.2.0/.github/workflows/publish_on_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 15:20:24.000000 milvus-model-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 15:20:24.000000 milvus-model-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 15:20:31.014065 milvus-model-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-01 15:20:24.000000 milvus-model-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-01 15:20:24.000000 milvus-model-0.2.0/_version_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/dense/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/dense/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/hybrid/bge_m3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.010065 milvus-model-0.2.0/milvus_model/reranker/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/bgereranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/cross_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/reranker/voyageai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/milvus_model/sparse/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/milvus_model/sparse/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/lang.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/bm25/tokenizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-01 15:20:24.000000 milvus-model-0.2.0/milvus_model/sparse/splade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:20:31.014065 milvus-model-0.2.0/milvus_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-01 15:20:31.000000 milvus-model-0.2.0/milvus_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 15:20:30.000000 milvus-model-0.2.0/milvus_model.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-01 15:20:24.000000 milvus-model-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:20:31.014065 milvus-model-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.480344 milvus_model-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.472344 milvus_model-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.472344 milvus_model-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 12:10:04.000000 milvus_model-0.2.1/.github/workflows/publish_dev_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-11 12:10:04.000000 milvus_model-0.2.1/.github/workflows/publish_on_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-11 12:10:04.000000 milvus_model-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-11 12:10:04.000000 milvus_model-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-11 12:10:10.480344 milvus_model-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-11 12:10:04.000000 milvus_model-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-11 12:10:04.000000 milvus_model-0.2.1/_version_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.472344 milvus_model-0.2.1/milvus_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/dense/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/jinaai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/dense/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/hybrid/bge_m3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/bgereranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/cross_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/jinaai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/reranker/voyageai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.476344 milvus_model-0.2.1/milvus_model/sparse/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/lang.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/bm25/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-11 12:10:04.000000 milvus_model-0.2.1/milvus_model/sparse/splade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:10:10.480344 milvus_model-0.2.1/milvus_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 12:10:10.000000 milvus_model-0.2.1/milvus_model.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-11 12:10:04.000000 milvus_model-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:10:10.480344 milvus_model-0.2.1/setup.cfg
```

### Comparing `milvus-model-0.2.0/.github/workflows/publish_dev_package.yml` & `milvus_model-0.2.1/.github/workflows/publish_dev_package.yml`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/.github/workflows/publish_on_release.yml` & `milvus_model-0.2.1/.github/workflows/publish_on_release.yml`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/LICENSE` & `milvus_model-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/PKG-INFO` & `milvus_model-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.2.0
+Version: 0.2.1
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 Requires-Dist: FlagEmbedding>=1.2.2
 Requires-Dist: nltk
 Requires-Dist: transformers>=4.36.0
 Requires-Dist: jieba
 Requires-Dist: konlpy
 Requires-Dist: mecab-python3
 Requires-Dist: scipy>=1.10.0
-Requires-Dist: protobuf==3.20.0
+Requires-Dist: protobuf==3.20.2
 Requires-Dist: unidic-lite
 Requires-Dist: cohere
 Requires-Dist: voyageai>=0.2.0
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
@@ -44,14 +44,14 @@
 ```
 If milvus-model was initially installed as part of the PyMilvus optional components, you should also upgrade PyMilvus to ensure compatibility. This can be done with:
 ```
 pip install pymilvus[model] --upgrade
 ```
 If you need to install a specific version of milvus-model, specify the version number:
 ```bash
-pip install milvus-model==0.1.0
+pip install milvus-model==0.2.0
 ```
-This command installs version 0.1.0 of milvus-model.
+This command installs version 0.2.0 of milvus-model.
```

### Comparing `milvus-model-0.2.0/README.md` & `milvus_model-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 ```
 If milvus-model was initially installed as part of the PyMilvus optional components, you should also upgrade PyMilvus to ensure compatibility. This can be done with:
 ```
 pip install pymilvus[model] --upgrade
 ```
 If you need to install a specific version of milvus-model, specify the version number:
 ```bash
-pip install milvus-model==0.1.0
+pip install milvus-model==0.2.0
 ```
-This command installs version 0.1.0 of milvus-model.
+This command installs version 0.2.0 of milvus-model.
```

### Comparing `milvus-model-0.2.0/_version_helper.py` & `milvus_model-0.2.1/_version_helper.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/base.py` & `milvus_model-0.2.1/milvus_model/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import abstractmethod
 from typing import List
 
 
 class BaseEmbeddingFunction:
-
     @abstractmethod
     def __call__(self, texts: List[str]):
         """ """
 
     @abstractmethod
     def encode_queries(self, queries: List[str]):
         """ """
```

### Comparing `milvus-model-0.2.0/milvus_model/dense/openai.py` & `milvus_model-0.2.1/milvus_model/dense/openai.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/dense/sentence_transformer.py` & `milvus_model-0.2.1/milvus_model/dense/sentence_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
         self.model = SentenceTransformer(**_model_config)
 
     def __call__(self, texts: List[str]) -> List[np.array]:
         return self._encode(texts)
 
     def _encode(self, texts: List[str]) -> List[np.array]:
         embs = self.model.encode(
-            texts,
-            batch_size=self.batch_size,
-            show_progress_bar=False,
-            convert_to_numpy=True,
+            texts, batch_size=self.batch_size, show_progress_bar=False, convert_to_numpy=True,
         )
         return list(embs)
 
     @property
     def dim(self):
         return self.model.get_sentence_embedding_dimension()
```

### Comparing `milvus-model-0.2.0/milvus_model/dense/voyageai.py` & `milvus_model-0.2.1/milvus_model/dense/voyageai.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/hybrid/bge_m3.py` & `milvus_model-0.2.1/milvus_model/hybrid/bge_m3.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class BGEM3EmbeddingFunction(BaseEmbeddingFunction):
     def __init__(
         self,
         model_name: str = "BAAI/bge-m3",
         batch_size: int = 16,
         device: str = "",
         normalize_embeddings: bool = True,
-        use_fp16: bool = True,
+        use_fp16: bool = False,
         return_dense: bool = True,
         return_sparse: bool = True,
         return_colbert_vecs: bool = False,
         **kwargs,
     ):
         try:
             from FlagEmbedding import BGEM3FlagModel
@@ -79,15 +79,15 @@
             results["sparse"] = []
             for sparse_vec in output["lexical_weights"]:
                 indices = [int(k) for k in sparse_vec]
                 values = list(sparse_vec.values())
                 row_indices = [0] * len(indices)
                 csr = csr_array((values, (row_indices, indices)), shape=(1, sparse_dim))
                 results["sparse"].append(csr)
-            results["sparse"] = vstack(results["sparse"])
+            results["sparse"] = vstack(results["sparse"]).tocsr()
         if self._encode_config["return_colbert_vecs"] is True:
             results["colbert_vecs"] = output["colbert_vecs"]
         return results
 
     def encode_queries(self, queries: List[str]) -> Dict:
         return self._encode(queries)
```

### Comparing `milvus-model-0.2.0/milvus_model/reranker/bgereranker.py` & `milvus_model-0.2.1/milvus_model/reranker/bgereranker.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         self.normalize = normalize
         self.device = device
         self.reranker = _FlagReranker(model_name, use_fp16=use_fp16, device=device)
 
     def _batchify(self, texts: List[str], batch_size: int) -> List[List[str]]:
         return [texts[i : i + batch_size] for i in range(0, len(texts), batch_size)]
 
-    def __call__(self, query: str, documents: List[str], top_k: int = 5) -> List[float]:
+    def __call__(self, query: str, documents: List[str], top_k: int = 5) -> List[RerankResult]:
         query_document_pairs = [[query, doc] for doc in documents]
         batched_texts = self._batchify(documents, self.batch_size)
         scores = []
         for batched_text in batched_texts:
             query_document_pairs = [[query, text] for text in batched_text]
             batch_score = self.reranker.compute_score(
                 query_document_pairs, normalize=self.normalize
```

### Comparing `milvus-model-0.2.0/milvus_model/reranker/cohere.py` & `milvus_model-0.2.1/milvus_model/reranker/cohere.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/reranker/cross_encoder.py` & `milvus_model-0.2.1/milvus_model/reranker/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/reranker/voyageai.py` & `milvus_model-0.2.1/milvus_model/reranker/voyageai.py`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/sparse/bm25/bm25.py` & `milvus_model-0.2.1/milvus_model/sparse/bm25/bm25.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,23 +156,23 @@
                 rows.append(0)
                 cols.append(self.idf[term][1])
                 values.append(value)
         return csr_array((values, (rows, cols)), shape=(1, len(self.idf)))
 
     def encode_queries(self, queries: List[str]) -> csr_array:
         sparse_embs = [self._encode_query(query) for query in queries]
-        return vstack(sparse_embs)
+        return vstack(sparse_embs).tocsr()
 
     def __call__(self, texts: List[str]) -> csr_array:
         error_message = "Unsupported function called, please check the documentation of 'BM25EmbeddingFunction'."
         raise ValueError(error_message)
 
     def encode_documents(self, documents: List[str]) -> csr_array:
         sparse_embs = [self._encode_document(document) for document in documents]
-        return vstack(sparse_embs)
+        return vstack(sparse_embs).tocsr()
 
     def save(self, path: str):
         bm25_params = {}
         bm25_params["version"] = "v1"
         bm25_params["corpus_size"] = self.corpus_size
         bm25_params["avgdl"] = self.avgdl
         bm25_params["idf_word"] = [None for _ in range(len(self.idf))]
```

### Comparing `milvus-model-0.2.0/milvus_model/sparse/bm25/lang.yaml` & `milvus_model-0.2.1/milvus_model/sparse/bm25/lang.yaml`

 * *Files identical despite different names*

### Comparing `milvus-model-0.2.0/milvus_model/sparse/bm25/tokenizers.py` & `milvus_model-0.2.1/milvus_model/sparse/bm25/tokenizers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import re
 import string
 from importlib.util import find_spec
 from pathlib import Path
 from typing import Any, Dict, List, Match, Optional, Type
 
+import nltk
 import yaml
 from nltk import word_tokenize
 from nltk.corpus import stopwords
 from nltk.stem.snowball import SnowballStemmer
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
@@ -69,14 +70,19 @@
     def apply(self, tokens: List[str]):
         return [token.lower() for token in tokens]
 
 
 @register_class("StopwordFilter")
 class StopwordFilter(TextFilter):
     def __init__(self, language: str = "english", stopword_list: Optional[List[str]] = None):
+        try:
+            nltk.corpus.stopwords.words(language)
+        except LookupError:
+            nltk.download("stopwords")
+
         if stopword_list is None:
             stopword_list = []
         self.stopwords = set(stopwords.words(language) + stopword_list)
 
     def apply(self, tokens: List[str]):
         return [token for token in tokens if token not in self.stopwords]
 
@@ -172,15 +178,15 @@
 
 def build_default_analyzer(language: str = "en"):
     default_config_path = Path(__file__).parent / "lang.yaml"
     return build_analyer_from_yaml(default_config_path, language)
 
 
 def build_analyer_from_yaml(filepath: str, name: str):
-    with Path(filepath).open() as file:
+    with Path(filepath).open(encoding="utf-8") as file:
         config = yaml.safe_load(file)
 
     lang_config = config.get(name)
     if not lang_config:
         error_message = f"No configuration found {name}"
         raise ValueError(error_message)
```

### Comparing `milvus-model-0.2.0/milvus_model/sparse/splade.py` & `milvus_model-0.2.1/milvus_model/sparse/splade.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,25 +67,23 @@
         self.doc_instruction = doc_instruction
 
     def __call__(self, texts: List[str]) -> csr_array:
         return self._encode(texts, None)
 
     def encode_documents(self, documents: List[str]) -> csr_array:
         return self._encode(
-            [self.doc_instruction + document for document in documents],
-            self.k_tokens_document,
+            [self.doc_instruction + document for document in documents], self.k_tokens_document,
         )
 
     def _encode(self, texts: List[str], k_tokens: int) -> csr_array:
         return self.model.forward(texts, k_tokens=k_tokens)
 
     def encode_queries(self, queries: List[str]) -> csr_array:
         return self._encode(
-            [self.query_instruction + query for query in queries],
-            self.k_tokens_query,
+            [self.query_instruction + query for query in queries], self.k_tokens_query,
         )
 
     @property
     def dim(self) -> int:
         return len(self.model.tokenizer)
 
     def _encode_query(self, query: str) -> csr_array:
@@ -126,34 +124,34 @@
             truncation=True,
             max_length=self.tokenizer.model_max_length,
             return_tensors="pt",
             add_special_tokens=True,
             padding=True,
         )
         encoded_input = {key: val.to(self.device) for key, val in encoded_input.items()}
-        with torch.no_grad():
-            output = self.model(**encoded_input)
+        output = self.model(**encoded_input)
         return output.logits
 
     def _batchify(self, texts: List[str], batch_size: int) -> List[List[str]]:
         return [texts[i : i + batch_size] for i in range(0, len(texts), batch_size)]
 
     def forward(self, texts: List[str], k_tokens: int) -> csr_array:
-        batched_texts = self._batchify(texts, self.batch_size)
-        sparse_embs = []
-        for batch_texts in batched_texts:
-            logits = self._encode(texts=batch_texts)
-            activations = self._get_activation(logits=logits)
-            if k_tokens is None:
-                nonzero_indices = torch.nonzero(activations["sparse_activations"])
-                activations["activations"] = nonzero_indices
-            else:
-                activations = self._update_activations(**activations, k_tokens=k_tokens)
-            batch_csr = self._convert_to_csr_array(activations)
-            sparse_embs.extend(batch_csr)
+        with torch.no_grad():
+            batched_texts = self._batchify(texts, self.batch_size)
+            sparse_embs = []
+            for batch_texts in batched_texts:
+                logits = self._encode(texts=batch_texts)
+                activations = self._get_activation(logits=logits)
+                if k_tokens is None:
+                    nonzero_indices = torch.nonzero(activations["sparse_activations"])
+                    activations["activations"] = nonzero_indices
+                else:
+                    activations = self._update_activations(**activations, k_tokens=k_tokens)
+                batch_csr = self._convert_to_csr_array(activations)
+                sparse_embs.extend(batch_csr)
 
         return vstack(sparse_embs).tocsr()
 
     def _get_activation(self, logits: torch.Tensor) -> Dict[str, torch.Tensor]:
         return {"sparse_activations": torch.amax(torch.log1p(self.relu(logits)), dim=1)}
 
     def _update_activations(self, sparse_activations: torch.Tensor, k_tokens: int) -> torch.Tensor:
```

### Comparing `milvus-model-0.2.0/milvus_model.egg-info/PKG-INFO` & `milvus_model-0.2.1/milvus_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: milvus-model
-Version: 0.2.0
+Version: 0.2.1
 Summary: Model components for PyMilvus, the Python SDK for Milvus
 Author-email: Milvus Team <milvus-team@zilliz.com>
 Project-URL: repository, https://github.com/milvus-io/milvus-model
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 Requires-Dist: FlagEmbedding>=1.2.2
 Requires-Dist: nltk
 Requires-Dist: transformers>=4.36.0
 Requires-Dist: jieba
 Requires-Dist: konlpy
 Requires-Dist: mecab-python3
 Requires-Dist: scipy>=1.10.0
-Requires-Dist: protobuf==3.20.0
+Requires-Dist: protobuf==3.20.2
 Requires-Dist: unidic-lite
 Requires-Dist: cohere
 Requires-Dist: voyageai>=0.2.0
 
 # Milvus Model Lib
 
 The milvus-model library provides model components for PyMilvus, the official Python SDK for Milvus, an open-source vector database built for AI applications.
@@ -44,14 +44,14 @@
 ```
 If milvus-model was initially installed as part of the PyMilvus optional components, you should also upgrade PyMilvus to ensure compatibility. This can be done with:
 ```
 pip install pymilvus[model] --upgrade
 ```
 If you need to install a specific version of milvus-model, specify the version number:
 ```bash
-pip install milvus-model==0.1.0
+pip install milvus-model==0.2.0
 ```
-This command installs version 0.1.0 of milvus-model.
+This command installs version 0.2.0 of milvus-model.
```

### Comparing `milvus-model-0.2.0/milvus_model.egg-info/SOURCES.txt` & `milvus_model-0.2.1/milvus_model.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,25 @@
 milvus_model/base.py
 milvus_model.egg-info/PKG-INFO
 milvus_model.egg-info/SOURCES.txt
 milvus_model.egg-info/dependency_links.txt
 milvus_model.egg-info/requires.txt
 milvus_model.egg-info/top_level.txt
 milvus_model/dense/__init__.py
+milvus_model/dense/jinaai.py
 milvus_model/dense/openai.py
 milvus_model/dense/sentence_transformer.py
 milvus_model/dense/voyageai.py
 milvus_model/hybrid/__init__.py
 milvus_model/hybrid/bge_m3.py
 milvus_model/reranker/__init__.py
 milvus_model/reranker/bgereranker.py
 milvus_model/reranker/cohere.py
 milvus_model/reranker/cross_encoder.py
+milvus_model/reranker/jinaai.py
 milvus_model/reranker/voyageai.py
 milvus_model/sparse/__init__.py
 milvus_model/sparse/splade.py
 milvus_model/sparse/bm25/__init__.py
 milvus_model/sparse/bm25/bm25.py
 milvus_model/sparse/bm25/lang.yaml
 milvus_model/sparse/bm25/tokenizers.py
```

### Comparing `milvus-model-0.2.0/pyproject.toml` & `milvus_model-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "FlagEmbedding >= 1.2.2",
     "nltk",
     "transformers >= 4.36.0",
     "jieba",
     "konlpy",
     "mecab-python3",
     "scipy >= 1.10.0",
-    "protobuf==3.20.0",
+    "protobuf==3.20.2",
     "unidic-lite",
     "cohere",
     "voyageai >= 0.2.0",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

