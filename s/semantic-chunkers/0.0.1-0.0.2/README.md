# Comparing `tmp/semantic_chunkers-0.0.1.tar.gz` & `tmp/semantic_chunkers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_chunkers-0.0.1.tar", max compression
+gzip compressed data, was "semantic_chunkers-0.0.2.tar", max compression
```

## Comparing `semantic_chunkers-0.0.1.tar` & `semantic_chunkers-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-04-30 02:58:36.256336 semantic_chunkers-0.0.1/LICENSE
--rw-r--r--   0        0        0     7633 2024-04-06 02:38:05.516738 semantic_chunkers-0.0.1/README.md
--rw-r--r--   0        0        0     1931 2024-04-30 02:45:13.118508 semantic_chunkers-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       21 2024-04-30 18:32:57.943745 semantic_chunkers-0.0.1/semantic_chunkers/__init__.py
--rw-r--r--   0        0        0      410 2024-04-30 03:00:07.685599 semantic_chunkers-0.0.1/semantic_chunkers/chunkers/__init__.py
--rw-r--r--   0        0        0     1255 2024-04-30 02:57:09.571935 semantic_chunkers-0.0.1/semantic_chunkers/chunkers/base.py
--rw-r--r--   0        0        0     2288 2024-04-30 03:00:06.155452 semantic_chunkers-0.0.1/semantic_chunkers/chunkers/consecutive_sim.py
--rw-r--r--   0        0        0     3265 2024-04-30 03:00:04.790176 semantic_chunkers-0.0.1/semantic_chunkers/chunkers/cumulative_sim.py
--rw-r--r--   0        0        0    18440 2024-04-30 03:00:03.112240 semantic_chunkers-0.0.1/semantic_chunkers/chunkers/rolling_window.py
--rw-r--r--   0        0        0     2199 2024-02-25 10:15:54.641265 semantic_chunkers-0.0.1/semantic_chunkers/chunkers/utils.py
--rw-r--r--   0        0        0     2794 2024-04-30 02:57:55.199781 semantic_chunkers-0.0.1/semantic_chunkers/encoders/__init__.py
--rw-r--r--   0        0        0      378 2024-04-28 04:31:24.128404 semantic_chunkers-0.0.1/semantic_chunkers/encoders/base.py
--rw-r--r--   0        0        0     2427 2024-04-30 02:59:08.074997 semantic_chunkers-0.0.1/semantic_chunkers/encoders/bm25.py
--rw-r--r--   0        0        0     4150 2024-04-30 02:59:05.133594 semantic_chunkers-0.0.1/semantic_chunkers/encoders/clip.py
--rw-r--r--   0        0        0     1646 2024-04-30 02:59:03.676217 semantic_chunkers-0.0.1/semantic_chunkers/encoders/cohere.py
--rw-r--r--   0        0        0     1704 2024-04-30 02:59:01.856745 semantic_chunkers-0.0.1/semantic_chunkers/encoders/fastembed.py
--rw-r--r--   0        0        0     5334 2024-04-30 02:58:50.748666 semantic_chunkers-0.0.1/semantic_chunkers/encoders/google.py
--rw-r--r--   0        0        0     9882 2024-04-30 02:58:47.621516 semantic_chunkers-0.0.1/semantic_chunkers/encoders/huggingface.py
--rw-r--r--   0        0        0     2722 2024-04-30 02:58:41.593616 semantic_chunkers-0.0.1/semantic_chunkers/encoders/mistral.py
--rw-r--r--   0        0        0     5045 2024-04-30 02:58:34.140866 semantic_chunkers-0.0.1/semantic_chunkers/encoders/openai.py
--rw-r--r--   0        0        0     2841 2024-04-30 02:58:38.090497 semantic_chunkers-0.0.1/semantic_chunkers/encoders/tfidf.py
--rw-r--r--   0        0        0     3371 2024-04-30 02:58:20.797624 semantic_chunkers-0.0.1/semantic_chunkers/encoders/vit.py
--rw-r--r--   0        0        0     4405 2024-04-30 02:57:32.955170 semantic_chunkers-0.0.1/semantic_chunkers/encoders/zure.py
--rw-r--r--   0        0        0     8100 2024-04-30 02:59:11.009441 semantic_chunkers-0.0.1/semantic_chunkers/hybrid_layer.py
--rw-r--r--   0        0        0      308 2024-04-30 02:58:22.868485 semantic_chunkers-0.0.1/semantic_chunkers/index/__init__.py
--rw-r--r--   0        0        0     2204 2024-04-27 15:02:58.045060 semantic_chunkers-0.0.1/semantic_chunkers/index/base.py
--rw-r--r--   0        0        0     4570 2024-04-30 02:58:25.195476 semantic_chunkers-0.0.1/semantic_chunkers/index/local.py
--rw-r--r--   0        0        0    10482 2024-04-30 02:58:27.046105 semantic_chunkers-0.0.1/semantic_chunkers/index/pinecone.py
--rw-r--r--   0        0        0     8695 2024-04-30 02:58:29.043581 semantic_chunkers-0.0.1/semantic_chunkers/index/qdrant.py
--rw-r--r--   0        0        0    24327 2024-04-30 02:59:06.538838 semantic_chunkers-0.0.1/semantic_chunkers/layer.py
--rw-r--r--   0        0        0      792 2023-12-02 19:41:23.483409 semantic_chunkers-0.0.1/semantic_chunkers/linear.py
--rw-r--r--   0        0        0      525 2024-04-30 02:58:30.722971 semantic_chunkers-0.0.1/semantic_chunkers/llms/__init__.py
--rw-r--r--   0        0        0     3937 2024-04-30 02:58:32.606761 semantic_chunkers-0.0.1/semantic_chunkers/llms/base.py
--rw-r--r--   0        0        0     1487 2024-04-30 02:58:03.592169 semantic_chunkers-0.0.1/semantic_chunkers/llms/cohere.py
--rw-r--r--   0        0        0      595 2024-01-13 20:10:15.356328 semantic_chunkers-0.0.1/semantic_chunkers/llms/grammars/json.gbnf
--rw-r--r--   0        0        0     2625 2024-04-30 02:57:53.534530 semantic_chunkers-0.0.1/semantic_chunkers/llms/llamacpp.py
--rw-r--r--   0        0        0     2602 2024-04-30 02:57:48.922813 semantic_chunkers-0.0.1/semantic_chunkers/llms/mistral.py
--rw-r--r--   0        0        0     1918 2024-04-30 02:57:37.148901 semantic_chunkers-0.0.1/semantic_chunkers/llms/ollama.py
--rw-r--r--   0        0        0     1879 2024-04-30 02:57:17.401069 semantic_chunkers-0.0.1/semantic_chunkers/llms/openai.py
--rw-r--r--   0        0        0     2045 2024-04-30 02:57:16.117540 semantic_chunkers-0.0.1/semantic_chunkers/llms/openrouter.py
--rw-r--r--   0        0        0     2237 2024-04-30 02:57:14.331555 semantic_chunkers-0.0.1/semantic_chunkers/llms/zure.py
--rw-r--r--   0        0        0     5547 2024-04-30 02:59:09.738360 semantic_chunkers-0.0.1/semantic_chunkers/route.py
--rw-r--r--   0        0        0     1618 2024-04-28 09:32:48.161734 semantic_chunkers-0.0.1/semantic_chunkers/schema.py
--rw-r--r--   0        0        0     8908 2024-04-30 02:58:43.707247 semantic_chunkers-0.0.1/semantic_chunkers/text.py
--rw-r--r--   0        0        0        0 2023-12-14 05:05:21.140350 semantic_chunkers-0.0.1/semantic_chunkers/utils/__init__.py
--rw-r--r--   0        0        0     1172 2024-04-07 14:10:07.845509 semantic_chunkers-0.0.1/semantic_chunkers/utils/defaults.py
--rw-r--r--   0        0        0     1941 2024-04-30 02:57:13.105730 semantic_chunkers-0.0.1/semantic_chunkers/utils/function_call.py
--rw-r--r--   0        0        0     1788 2024-04-30 02:57:11.887137 semantic_chunkers-0.0.1/semantic_chunkers/utils/llm.py
--rw-r--r--   0        0        0     1008 2024-01-13 14:02:43.907490 semantic_chunkers-0.0.1/semantic_chunkers/utils/logger.py
--rw-r--r--   0        0        0     9613 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-11 12:53:58.410362 semantic_chunkers-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1391 2024-05-11 12:53:58.410362 semantic_chunkers-0.0.2/README.md
+-rw-r--r--   0        0        0     1006 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/base.py
+-rw-r--r--   0        0        0     2238 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/consecutive.py
+-rw-r--r--   0        0        0     3211 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/cumulative.py
+-rw-r--r--   0        0        0    18448 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/statistical.py
+-rw-r--r--   0        0        0      352 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/schema.py
+-rw-r--r--   0        0        0        0 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/splitters/__init__.py
+-rw-r--r--   0        0        0     2003 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/splitters/sentence.py
+-rw-r--r--   0        0        0        0 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/utils/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/utils/logger.py
+-rw-r--r--   0        0        0      192 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/utils/text.py
+-rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.2/PKG-INFO
```

### Comparing `semantic_chunkers-0.0.1/LICENSE` & `semantic_chunkers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.1/semantic_chunkers/chunkers/base.py` & `semantic_chunkers-0.0.2/semantic_chunkers/chunkers/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import List
 
 from colorama import Fore, Style
 from pydantic.v1 import BaseModel, Extra
 
-from semantic_chunkers.encoders import BaseEncoder
-from semantic_chunkers.schema import DocumentSplit
+from semantic_router.encoders.base import BaseEncoder
+from semantic_chunkers.schema import ChunkSet
 
 
-class BaseSplitter(BaseModel):
+class BaseChunker(BaseModel):
     name: str
     encoder: BaseEncoder
 
     class Config:
         extra = Extra.allow
 
-    def __call__(self, docs: List[str]) -> List[DocumentSplit]:
+    def __call__(self, docs: List[str]) -> List[ChunkSet]:
         raise NotImplementedError("Subclasses must implement this method")
 
-    def print(self, document_splits: List[DocumentSplit]) -> None:
+    def print(self, document_splits: List[ChunkSet]) -> None:
         colors = [Fore.RED, Fore.GREEN, Fore.BLUE, Fore.MAGENTA]
         for i, split in enumerate(document_splits):
             color = colors[i % len(colors)]
             colored_content = f"{color}{split.content}{Style.RESET_ALL}"
             if split.is_triggered:
                 triggered = f"{split.triggered_score:.2f}"
             elif i == len(document_splits) - 1:
```

### Comparing `semantic_chunkers-0.0.1/semantic_chunkers/chunkers/consecutive_sim.py` & `semantic_chunkers-0.0.2/semantic_chunkers/chunkers/consecutive.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from typing import Any, List
 
 import numpy as np
 
-from semantic_chunkers.encoders import BaseEncoder
-from semantic_chunkers.schema import DocumentSplit
-from semantic_chunkers.chunkers.base import BaseSplitter
+from semantic_router.encoders.base import BaseEncoder
+from semantic_chunkers.schema import ChunkSet
+from semantic_chunkers.chunkers.base import BaseChunker
 
 
-class ConsecutiveSimSplitter(BaseSplitter):
+class ConsecutiveChunker(BaseChunker):
     """
-    Called "consecutive sim splitter" because we check the similarities of consecutive document embeddings (compare ith to i+1th document embedding).
+    Called "consecutive sim chunker" because we check the similarities of consecutive document embeddings (compare ith to i+1th document embedding).
     """
 
     def __init__(
         self,
         encoder: BaseEncoder,
-        name: str = "consecutive_similarity_splitter",
+        name: str = "consecutive_chunker",
         score_threshold: float = 0.45,
     ):
         super().__init__(name=name, encoder=encoder)
         encoder.score_threshold = score_threshold
         self.score_threshold = score_threshold
 
-    def __call__(self, docs: List[Any]) -> List[DocumentSplit]:
+    def __call__(self, docs: List[Any]) -> List[ChunkSet]:
         """Split documents into smaller chunks based on semantic similarity.
 
         :param docs: list of text documents to be split, if only wanted to
             split a single document, pass it as a list with a single element.
 
-        :return: list of DocumentSplit objects containing the split documents.
+        :return: list of ChunkSet objects containing the chunks.
         """
         # Check if there's only a single document
         if len(docs) == 1:
             raise ValueError(
                 "There is only one document provided; at least two are required to determine topics based on similarity."
             )
 
@@ -44,17 +44,17 @@
         curr_split_start_idx = 0
         curr_split_num = 1
 
         for idx in range(1, total_docs):
             curr_sim_score = sim_matrix[idx - 1][idx]
             if idx < len(sim_matrix) and curr_sim_score < self.score_threshold:
                 splits.append(
-                    DocumentSplit(
+                    ChunkSet(
                         docs=list(docs[curr_split_start_idx:idx]),
                         is_triggered=True,
                         triggered_score=curr_sim_score,
                     )
                 )
                 curr_split_start_idx = idx
                 curr_split_num += 1
-        splits.append(DocumentSplit(docs=list(docs[curr_split_start_idx:])))
+        splits.append(ChunkSet(docs=list(docs[curr_split_start_idx:])))
         return splits
```

### Comparing `semantic_chunkers-0.0.1/semantic_chunkers/chunkers/rolling_window.py` & `semantic_chunkers-0.0.2/semantic_chunkers/chunkers/statistical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,108 @@
 from dataclasses import dataclass
 from typing import List
 
 import numpy as np
 
-from semantic_chunkers.encoders.base import BaseEncoder
-from semantic_chunkers.schema import DocumentSplit
-from semantic_chunkers.chunkers.base import BaseSplitter
-from semantic_chunkers.chunkers.utils import split_to_sentences, tiktoken_length
+from semantic_router.encoders.base import BaseEncoder
+from semantic_chunkers.schema import ChunkSet
+from semantic_chunkers.chunkers.base import BaseChunker
+from semantic_chunkers.splitters import sentence
+from semantic_chunkers.utils.text import tiktoken_length
 from semantic_chunkers.utils.logger import logger
 
 
 @dataclass
-class SplitStatistics:
+class ChunkStatistics:
     total_documents: int
-    total_splits: int
-    splits_by_threshold: int
-    splits_by_max_chunk_size: int
-    splits_by_last_split: int
+    total_chunks: int
+    chunks_by_threshold: int
+    chunks_by_max_chunk_size: int
+    chunks_by_last_split: int
     min_token_size: int
     max_token_size: int
-    splits_by_similarity_ratio: float
+    chunks_by_similarity_ratio: float
 
     def __str__(self):
         return (
-            f"Splitting Statistics:\n"
+            f"Chunking Statistics:\n"
             f"  - Total Documents: {self.total_documents}\n"
-            f"  - Total Splits: {self.total_splits}\n"
-            f"  - Splits by Threshold: {self.splits_by_threshold}\n"
-            f"  - Splits by Max Chunk Size: {self.splits_by_max_chunk_size}\n"
-            f"  - Last Split: {self.splits_by_last_split}\n"
-            f"  - Minimum Token Size of Split: {self.min_token_size}\n"
-            f"  - Maximum Token Size of Split: {self.max_token_size}\n"
-            f"  - Similarity Split Ratio: {self.splits_by_similarity_ratio:.2f}"
+            f"  - Total Chunks: {self.total_chunks}\n"
+            f"  - Chunks by Threshold: {self.chunks_by_threshold}\n"
+            f"  - Chunks by Max Chunk Size: {self.chunks_by_max_chunk_size}\n"
+            f"  - Last Chunk: {self.chunks_by_last_split}\n"
+            f"  - Minimum Token Size of Chunk: {self.min_token_size}\n"
+            f"  - Maximum Token Size of Chunk: {self.max_token_size}\n"
+            f"  - Similarity Chunk Ratio: {self.chunks_by_similarity_ratio:.2f}"
         )
 
 
-class RollingWindowSplitter(BaseSplitter):
+class StatisticalChunker(BaseChunker):
     def __init__(
         self,
         encoder: BaseEncoder,
-        name="rolling_window_splitter",
+        name="statistical_chunker",
         threshold_adjustment=0.01,
         dynamic_threshold: bool = True,
         window_size=5,
         min_split_tokens=100,
         max_split_tokens=300,
         split_tokens_tolerance=10,
-        plot_splits=False,
+        plot_chunks=False,
         enable_statistics=False,
     ):
         super().__init__(name=name, encoder=encoder)
         self.calculated_threshold: float
         self.encoder = encoder
         self.threshold_adjustment = threshold_adjustment
         self.dynamic_threshold = dynamic_threshold
         self.window_size = window_size
-        self.plot_splits = plot_splits
+        self.plot_chunks = plot_chunks
         self.min_split_tokens = min_split_tokens
         self.max_split_tokens = max_split_tokens
         self.split_tokens_tolerance = split_tokens_tolerance
         self.enable_statistics = enable_statistics
-        self.statistics: SplitStatistics
+        self.statistics: ChunkStatistics
 
-    def __call__(self, docs: List[str]) -> List[DocumentSplit]:
-        """Split documents into smaller chunks based on semantic similarity.
+    def __call__(self, docs: List[str]) -> List[ChunkSet]:
+        """Chunk documents into smaller chunks based on semantic similarity.
 
         :param docs: list of text documents to be split, if only wanted to
             split a single document, pass it as a list with a single element.
 
-        :return: list of DocumentSplit objects containing the split documents.
+        :return: list of DocumentChunk objects containing the split documents.
         """
         if not docs:
             raise ValueError("At least one document is required for splitting.")
 
         if len(docs) == 1:
             token_count = tiktoken_length(docs[0])
             if token_count > self.max_split_tokens:
                 logger.info(
                     f"Single document exceeds the maximum token limit "
                     f"of {self.max_split_tokens}. "
-                    "Splitting to sentences before semantically splitting."
+                    "Splitting to sentences before semantically merging."
                 )
-            docs = split_to_sentences(docs[0])
+            docs = sentence.regex_splitter(docs[0])
         encoded_docs = self._encode_documents(docs)
         similarities = self._calculate_similarity_scores(encoded_docs)
         if self.dynamic_threshold:
             self._find_optimal_threshold(docs, similarities)
         else:
             self.calculated_threshold = self.encoder.score_threshold
         split_indices = self._find_split_indices(similarities=similarities)
-        splits = self._split_documents(docs, split_indices, similarities)
+        chunks = self._split_documents(docs, split_indices, similarities)
 
-        if self.plot_splits:
-            self.plot_similarity_scores(similarities, split_indices, splits)
+        if self.plot_chunks:
+            self.plot_similarity_scores(similarities, split_indices, chunks)
 
         if self.enable_statistics:
             print(self.statistics)
 
-        return splits
+        return chunks
 
     def _encode_documents(self, docs: List[str]) -> np.ndarray:
         """
         Encodes a list of documents into embeddings. If the number of documents exceeds 2000,
         the documents are split into batches to avoid overloading the encoder. OpenAI has a
         limit of len(array) < 2048.
 
@@ -139,15 +140,15 @@
         for idx, score in enumerate(similarities):
             logger.debug(f"Similarity score at index {idx}: {score}")
             if score < self.calculated_threshold:
                 logger.debug(
                     f"Adding to split_indices due to score < threshold: "
                     f"{score} < {self.calculated_threshold}"
                 )
-                # Split after the document at idx
+                # Chunk after the document at idx
                 split_indices.append(idx + 1)
         return split_indices
 
     def _find_optimal_threshold(self, docs: List[str], similarity_scores: List[float]):
         token_counts = [tiktoken_length(doc) for doc in docs]
         cumulative_token_counts = np.cumsum([0] + token_counts)
 
@@ -172,15 +173,15 @@
             split_token_counts = [
                 cumulative_token_counts[end] - cumulative_token_counts[start]
                 for start, end in zip(
                     [0] + split_indices, split_indices + [len(token_counts)]
                 )
             ]
 
-            # Calculate the median token count for the splits
+            # Calculate the median token count for the chunks
             median_tokens = np.median(split_token_counts)
             logger.debug(
                 f"Iteration {iteration}: Median tokens per split: {median_tokens}"
             )
             if (
                 self.min_split_tokens - self.split_tokens_tolerance
                 <= median_tokens
@@ -202,31 +203,31 @@
             f"({self.min_split_tokens}-{self.max_split_tokens})."
         )
 
         return self.calculated_threshold
 
     def _split_documents(
         self, docs: List[str], split_indices: List[int], similarities: List[float]
-    ) -> List[DocumentSplit]:
+    ) -> List[ChunkSet]:
         """
         This method iterates through each document, appending it to the current split
         until it either reaches a split point (determined by split_indices) or exceeds
         the maximum token limit for a split (self.max_split_tokens).
         When a document causes the current token count to exceed this limit,
         or when a split point is reached and the minimum token requirement is met,
-        the current split is finalized and added to the List of splits.
+        the current split is finalized and added to the List of chunks.
         """
         token_counts = [tiktoken_length(doc) for doc in docs]
-        splits, current_split = [], []
+        chunks, current_split = [], []
         current_tokens_count = 0
 
         # Statistics
-        splits_by_threshold = 0
-        splits_by_max_chunk_size = 0
-        splits_by_last_split = 0
+        chunks_by_threshold = 0
+        chunks_by_max_chunk_size = 0
+        chunks_by_last_split = 0
 
         for doc_idx, doc in enumerate(docs):
             doc_token_count = token_counts[doc_idx]
             logger.debug(f"Accumulative token count: {current_tokens_count} tokens")
             logger.debug(f"Document token count: {doc_token_count} tokens")
             # Check if current index is a split point based on similarity
             if doc_idx + 1 in split_indices:
@@ -239,112 +240,112 @@
                     # if it doesn't exceed the max limit
                     current_split.append(doc)
                     current_tokens_count += doc_token_count
 
                     triggered_score = (
                         similarities[doc_idx] if doc_idx < len(similarities) else None
                     )
-                    splits.append(
-                        DocumentSplit(
+                    chunks.append(
+                        ChunkSet(
                             docs=current_split.copy(),
                             is_triggered=True,
                             triggered_score=triggered_score,
                             token_count=current_tokens_count,
                         )
                     )
                     logger.debug(
-                        f"Split finalized with {current_tokens_count} tokens due to "
+                        f"Chunk finalized with {current_tokens_count} tokens due to "
                         f"threshold {self.calculated_threshold}."
                     )
                     current_split, current_tokens_count = [], 0
-                    splits_by_threshold += 1
+                    chunks_by_threshold += 1
                     continue  # Move to the next document after splitting
 
             # Check if adding the current document exceeds the max token limit
             if current_tokens_count + doc_token_count > self.max_split_tokens:
                 if current_tokens_count >= self.min_split_tokens:
-                    splits.append(
-                        DocumentSplit(
+                    chunks.append(
+                        ChunkSet(
                             docs=current_split.copy(),
                             is_triggered=False,
                             triggered_score=None,
                             token_count=current_tokens_count,
                         )
                     )
-                    splits_by_max_chunk_size += 1
+                    chunks_by_max_chunk_size += 1
                     logger.debug(
-                        f"Split finalized with {current_tokens_count} tokens due to "
+                        f"Chink finalized with {current_tokens_count} tokens due to "
                         f"exceeding token limit of {self.max_split_tokens}."
                     )
                     current_split, current_tokens_count = [], 0
 
             current_split.append(doc)
             current_tokens_count += doc_token_count
 
         # Handle the last split
         if current_split:
-            splits.append(
-                DocumentSplit(
+            chunks.append(
+                ChunkSet(
                     docs=current_split.copy(),
                     is_triggered=False,
                     triggered_score=None,
                     token_count=current_tokens_count,
                 )
             )
-            splits_by_last_split += 1
+            chunks_by_last_split += 1
             logger.debug(
                 f"Final split added with {current_tokens_count} "
                 "tokens due to remaining documents."
             )
 
         # Validation to ensure no tokens are lost during the split
         original_token_count = sum(token_counts)
         split_token_count = sum(
-            [tiktoken_length(doc) for split in splits for doc in split.docs]
+            [tiktoken_length(doc) for split in chunks for doc in split.docs]
         )
         if original_token_count != split_token_count:
             logger.error(
                 f"Token count mismatch: {original_token_count} != {split_token_count}"
             )
             raise ValueError(
                 f"Token count mismatch: {original_token_count} != {split_token_count}"
             )
 
         # Statistics
-        total_splits = len(splits)
-        splits_by_similarity_ratio = (
-            splits_by_threshold / total_splits if total_splits else 0
+        total_chunks = len(chunks)
+        chunks_by_similarity_ratio = (
+            chunks_by_threshold / total_chunks if total_chunks else 0
         )
         min_token_size = max_token_size = 0
-        if splits:
+        if chunks:
             token_counts = [
-                split.token_count for split in splits if split.token_count is not None
+                split.token_count for split in chunks if split.token_count is not None
             ]
             min_token_size, max_token_size = min(token_counts, default=0), max(
                 token_counts, default=0
             )
 
-        self.statistics = SplitStatistics(
+        self.statistics = ChunkStatistics(
             total_documents=len(docs),
-            total_splits=total_splits,
-            splits_by_threshold=splits_by_threshold,
-            splits_by_max_chunk_size=splits_by_max_chunk_size,
-            splits_by_last_split=splits_by_last_split,
+            total_chunks=total_chunks,
+            chunks_by_threshold=chunks_by_threshold,
+            chunks_by_max_chunk_size=chunks_by_max_chunk_size,
+            chunks_by_last_split=chunks_by_last_split,
             min_token_size=min_token_size,
             max_token_size=max_token_size,
-            splits_by_similarity_ratio=splits_by_similarity_ratio,
+            chunks_by_similarity_ratio=chunks_by_similarity_ratio,
         )
 
-        return splits
+        return chunks
 
     def plot_similarity_scores(
         self,
         similarities: List[float],
         split_indices: List[int],
-        splits: list[DocumentSplit],
+        chunks: list[ChunkSet],
     ):
         try:
             from matplotlib import pyplot as plt
         except ImportError:
             logger.warning(
                 "Plotting is disabled. Please `pip install "
                 "semantic-router[processing]`."
@@ -356,15 +357,15 @@
         # Plot 1: Similarity Scores
         axs[0].plot(similarities, label="Similarity Scores", marker="o")
         for split_index in split_indices:
             axs[0].axvline(
                 x=split_index - 1,
                 color="r",
                 linestyle="--",
-                label="Split" if split_index == split_indices[0] else "",
+                label="Chunk" if split_index == split_indices[0] else "",
             )
         axs[0].axhline(
             y=self.calculated_threshold,
             color="g",
             linestyle="-.",
             label="Threshold Similarity Score",
         )
@@ -385,19 +386,19 @@
             f"Threshold: {self.calculated_threshold} |"
             f" Window Size: {self.window_size}",
             loc="right",
             fontsize=10,
         )
         axs[0].legend()
 
-        # Plot 2: Split Token Size Distribution
-        token_counts = [split.token_count for split in splits]
+        # Plot 2: Chunk Token Size Distribution
+        token_counts = [split.token_count for split in chunks]
         axs[1].bar(range(len(token_counts)), token_counts, color="lightblue")
-        axs[1].set_title("Split Token Sizes")
-        axs[1].set_xlabel("Split Index")
+        axs[1].set_title("Chunk Token Sizes")
+        axs[1].set_xlabel("Chunk Index")
         axs[1].set_ylabel("Token Count")
         axs[1].set_xticks(range(len(token_counts)))
         axs[1].set_xticklabels([str(i) for i in range(len(token_counts))])
         axs[1].grid(True)
 
         # Annotate each bar with the token size
         for idx, token_count in enumerate(token_counts):
@@ -421,15 +422,17 @@
         """
         Computes similarity scores between the average of the last
         'window_size' sentences and the next one,
         plots a graph of these similarity scores, and prints the first
         sentence after a similarity score below
         a specified threshold.
         """
-        sentences = [sentence for doc in docs for sentence in split_to_sentences(doc)]
+        sentences = [
+            sentence for doc in docs for sentence in sentence.regex_splitter(doc)
+        ]
         encoded_sentences = self._encode_documents(sentences)
         similarity_scores = []
 
         for i in range(window_size, len(encoded_sentences)):
             window_avg_encoding = np.mean(
                 encoded_sentences[i - window_size : i], axis=0
             )
```

### Comparing `semantic_chunkers-0.0.1/semantic_chunkers/chunkers/utils.py` & `semantic_chunkers-0.0.2/semantic_chunkers/splitters/sentence.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import regex
-import tiktoken
 
 
-def split_to_sentences(text: str) -> list[str]:
+def regex_splitter(text: str) -> list[str]:
     """
     Enhanced regex pattern to split a given text into sentences more accurately.
 
     The enhanced regex pattern includes handling for:
     - Direct speech and quotations.
     - Abbreviations, initials, and acronyms.
     - Decimal numbers and dates.
@@ -51,13 +50,7 @@
         |
         # Matches and removes control characters and format characters
         [\p{Cc}\p{Cf}]+
     """
     sentences = regex.split(regex_pattern, text, flags=regex.VERBOSE)
     sentences = [sentence.strip() for sentence in sentences if sentence.strip()]
     return sentences
-
-
-def tiktoken_length(text: str) -> int:
-    tokenizer = tiktoken.get_encoding("cl100k_base")
-    tokens = tokenizer.encode(text, disallowed_special=())
-    return len(tokens)
```

### Comparing `semantic_chunkers-0.0.1/semantic_chunkers/utils/logger.py` & `semantic_chunkers-0.0.2/semantic_chunkers/utils/logger.py`

 * *Files identical despite different names*

