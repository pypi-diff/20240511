# Comparing `tmp/docprompt-0.4.4.tar.gz` & `tmp/docprompt-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docprompt-0.4.4.tar", max compression
+gzip compressed data, was "docprompt-0.4.5.tar", last modified: Sat May 11 02:46:12 2024, max compression
```

## Comparing `docprompt-0.4.4.tar` & `docprompt-0.4.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.4/LICENSE
--rw-r--r--   0        0        0     4917 2024-03-19 03:22:18.145677 docprompt-0.4.4/README.md
--rw-r--r--   0        0        0      752 2024-05-07 01:31:13.350643 docprompt-0.4.4/docprompt/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.4/docprompt/_exec/__init__.py
--rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.4/docprompt/_exec/ghostscript.py
--rw-r--r--   0        0        0     1541 2024-05-07 01:14:14.543427 docprompt-0.4.4/docprompt/_pdfium.py
--rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.4/docprompt/provenance/__init__.py
--rw-r--r--   0        0        0     9850 2024-03-19 01:27:56.655646 docprompt-0.4.4/docprompt/provenance/search.py
--rw-r--r--   0        0        0     1357 2024-03-19 01:25:52.543395 docprompt-0.4.4/docprompt/provenance/source.py
--rw-r--r--   0        0        0     6054 2024-03-19 01:25:52.543395 docprompt-0.4.4/docprompt/provenance/util.py
--rw-r--r--   0        0        0     7097 2024-05-07 00:41:50.085452 docprompt-0.4.4/docprompt/rasterize.py
--rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.4/docprompt/schema/__init__.py
--rw-r--r--   0        0        0     9402 2024-05-07 01:14:14.547427 docprompt-0.4.4/docprompt/schema/document.py
--rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.4/docprompt/schema/layout.py
--rw-r--r--   0        0        0    12026 2024-05-07 01:27:16.164027 docprompt-0.4.4/docprompt/schema/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.4/docprompt/tasks/__init__.py
--rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.4/docprompt/tasks/base.py
--rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.4/docprompt/tasks/classification/__init__.py
--rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.4/docprompt/tasks/message.py
--rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.4/docprompt/tasks/ocr/__init__.py
--rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.4/docprompt/tasks/ocr/gcp.py
--rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.4/docprompt/tasks/ocr/result.py
--rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.4/docprompt/tasks/table_extraction/__init__.py
--rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.4/docprompt/tasks/table_extraction/base.py
--rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.4/docprompt/tasks/table_extraction/providers/__init__.py
--rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.4/docprompt/tasks/table_extraction/providers/claude.py
--rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.4/docprompt/tasks/table_extraction/result.py
--rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.4/docprompt/utils/__init__.py
--rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.4/docprompt/utils/compressor.py
--rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.4/docprompt/utils/date_extraction.py
--rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.4/docprompt/utils/masking/__init__.py
--rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.4/docprompt/utils/masking/image.py
--rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.4.4/docprompt/utils/splitter.py
--rw-r--r--   0        0        0     4088 2024-05-06 23:51:36.485689 docprompt-0.4.4/docprompt/utils/util.py
--rw-r--r--   0        0        0     4177 2024-05-07 01:31:06.306565 docprompt-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.4/tests/fixtures/1.pdf
--rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.4/tests/fixtures/1_ocr.json
--rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.4/tests/fixtures.py
--rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.4/tests/test_date_extraction.py
--rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.4/tests/test_document.py
--rw-r--r--   0        0        0     1813 2024-05-07 01:14:14.543427 docprompt-0.4.4/tests/test_documentnode.py
--rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.4/tests/test_layout_models.py
--rw-r--r--   0        0        0     2517 2024-05-06 01:04:51.295282 docprompt-0.4.4/tests/test_search.py
--rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.4/tests/test_threadpool.py
--rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.4/tests/util.py
--rw-r--r--   0        0        0     7726 1970-01-01 00:00:00.000000 docprompt-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      585 2023-10-19 02:11:11.194822 docprompt-0.4.5/LICENSE
+-rw-r--r--   0        0        0     5174 2024-05-10 05:55:50.188361 docprompt-0.4.5/README.md
+-rw-r--r--   0        0        0      752 2024-05-11 02:46:08.414792 docprompt-0.4.5/docprompt/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:11:05.761315 docprompt-0.4.5/docprompt/_exec/__init__.py
+-rw-r--r--   0        0        0     2395 2024-03-19 02:54:19.707704 docprompt-0.4.5/docprompt/_exec/ghostscript.py
+-rw-r--r--   0        0        0     1541 2024-05-07 01:14:14.543427 docprompt-0.4.5/docprompt/_pdfium.py
+-rw-r--r--   0        0        0      107 2024-05-06 05:10:23.648879 docprompt-0.4.5/docprompt/provenance/__init__.py
+-rw-r--r--   0        0        0     9861 2024-05-10 22:04:25.589467 docprompt-0.4.5/docprompt/provenance/search.py
+-rw-r--r--   0        0        0     1425 2024-05-10 22:19:31.977780 docprompt-0.4.5/docprompt/provenance/source.py
+-rw-r--r--   0        0        0     5771 2024-05-10 22:19:31.977780 docprompt-0.4.5/docprompt/provenance/util.py
+-rw-r--r--   0        0        0     7097 2024-05-07 00:41:50.085452 docprompt-0.4.5/docprompt/rasterize.py
+-rw-r--r--   0        0        0        0 2024-01-07 23:02:33.076362 docprompt-0.4.5/docprompt/schema/__init__.py
+-rw-r--r--   0        0        0     9402 2024-05-07 01:14:14.547427 docprompt-0.4.5/docprompt/schema/document.py
+-rw-r--r--   0        0        0     6649 2024-04-13 03:18:18.370507 docprompt-0.4.5/docprompt/schema/layout.py
+-rw-r--r--   0        0        0    12026 2024-05-07 01:27:16.164027 docprompt-0.4.5/docprompt/schema/pipeline.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:38:52.149979 docprompt-0.4.5/docprompt/tasks/__init__.py
+-rw-r--r--   0        0        0     5103 2024-04-05 21:43:53.078902 docprompt-0.4.5/docprompt/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-03-12 20:43:10.168189 docprompt-0.4.5/docprompt/tasks/classification/__init__.py
+-rw-r--r--   0        0        0     2522 2024-04-05 21:40:07.216964 docprompt-0.4.5/docprompt/tasks/message.py
+-rw-r--r--   0        0        0        0 2024-03-14 22:11:01.166853 docprompt-0.4.5/docprompt/tasks/ocr/__init__.py
+-rw-r--r--   0        0        0    18558 2024-04-13 03:18:18.370507 docprompt-0.4.5/docprompt/tasks/ocr/gcp.py
+-rw-r--r--   0        0        0     1170 2024-04-05 21:40:16.917047 docprompt-0.4.5/docprompt/tasks/ocr/result.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:03:50.676445 docprompt-0.4.5/docprompt/tasks/table_extraction/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-05 21:43:47.746856 docprompt-0.4.5/docprompt/tasks/table_extraction/base.py
+-rw-r--r--   0        0        0        0 2024-03-17 06:15:55.636068 docprompt-0.4.5/docprompt/tasks/table_extraction/providers/__init__.py
+-rw-r--r--   0        0        0     3420 2024-04-05 21:53:59.072160 docprompt-0.4.5/docprompt/tasks/table_extraction/providers/claude.py
+-rw-r--r--   0        0        0      783 2024-04-05 21:40:26.277127 docprompt-0.4.5/docprompt/tasks/table_extraction/result.py
+-rw-r--r--   0        0        0      375 2024-05-04 01:28:27.264357 docprompt-0.4.5/docprompt/utils/__init__.py
+-rw-r--r--   0        0        0      421 2023-10-19 04:28:21.331934 docprompt-0.4.5/docprompt/utils/compressor.py
+-rw-r--r--   0        0        0     4915 2024-04-05 21:45:37.323801 docprompt-0.4.5/docprompt/utils/date_extraction.py
+-rw-r--r--   0        0        0        0 2024-04-16 21:31:16.273985 docprompt-0.4.5/docprompt/utils/masking/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-17 06:27:28.658476 docprompt-0.4.5/docprompt/utils/masking/image.py
+-rw-r--r--   0        0        0     3577 2024-05-06 23:51:36.501689 docprompt-0.4.5/docprompt/utils/splitter.py
+-rw-r--r--   0        0        0     4088 2024-05-06 23:51:36.485689 docprompt-0.4.5/docprompt/utils/util.py
+-rw-r--r--   0        0        0     2717 2024-05-11 02:46:12.886829 docprompt-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-10-19 02:11:11.222822 docprompt-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0      202 2024-03-19 01:25:52.543395 docprompt-0.4.5/tests/fixtures.py
+-rw-r--r--   0        0        0   123638 2024-03-18 16:06:46.485527 docprompt-0.4.5/tests/fixtures/1.pdf
+-rw-r--r--   0        0        0  2788655 2024-03-19 01:25:52.543395 docprompt-0.4.5/tests/fixtures/1_ocr.json
+-rw-r--r--   0        0        0      830 2024-04-05 21:43:39.530785 docprompt-0.4.5/tests/test_date_extraction.py
+-rw-r--r--   0        0        0     5225 2024-05-04 01:28:27.264357 docprompt-0.4.5/tests/test_document.py
+-rw-r--r--   0        0        0     1813 2024-05-07 01:14:14.543427 docprompt-0.4.5/tests/test_documentnode.py
+-rw-r--r--   0        0        0     1361 2024-04-13 03:17:35.662168 docprompt-0.4.5/tests/test_layout_models.py
+-rw-r--r--   0        0        0     2868 2024-05-10 22:19:31.977780 docprompt-0.4.5/tests/test_search.py
+-rw-r--r--   0        0        0      878 2024-04-10 19:57:12.041828 docprompt-0.4.5/tests/test_threadpool.py
+-rw-r--r--   0        0        0     1003 2024-03-19 01:25:52.547395 docprompt-0.4.5/tests/util.py
+-rw-r--r--   0        0        0     6689 1970-01-01 00:00:00.000000 docprompt-0.4.5/PKG-INFO
```

### Comparing `docprompt-0.4.4/LICENSE` & `docprompt-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/README.md` & `docprompt-0.4.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://pypi.org/project/docprompt/)
 [![python](https://img.shields.io/pypi/pyversions/docprompt.svg)](https://pypi.org/project/docprompt/)
 [![Build Status](https://github.com/Page-Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://github.com/Page-Leaf/docprompt/actions/workflows/dev.yml)
 [![codecov](https://codecov.io/gh/Page-Leaf/Docprompt/branch/main/graphs/badge.svg)](https://codecov.io/github/Page-Leaf/Docprompt)
-
+[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm-project.org)
 
 <br />
 <div align="center">
   <a href="https://github.com/Page-Leaf/Docprompt">
     <img src="docs/docprompt/static/img/logo.png" alt="Logo" width="120" height="120">
   </a>
 
@@ -150,7 +150,11 @@
 # With OCR results available, we can now instantiate a locator and search through documents.
 
 document_node.locator.search("John Doe") # This will return a list of all terms across the document that contain "John Doe"
 document_node.locator.search("Jane Doe", page_number=4) # Just return results a list of matching results from page 4
 ```
 
 This functionality uses a combination of `rtree` and the Rust library `tantivy`, allowing you to perform thousands of searches in **seconds** :fire: :rocket:
+
+<a href="https://trackgit.com">
+<img src="https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lw098gfpjhrd7b2ev4rl" alt="trackgit-views" />
+</a>
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 [![pypi](https://img.shields.io/pypi/v/docprompt.svg)](https://pypi.org/
 project/docprompt/) [![python](https://img.shields.io/pypi/pyversions/
 docprompt.svg)](https://pypi.org/project/docprompt/) [![Build Status](https://
 github.com/Page-Leaf/Docprompt/actions/workflows/dev.yml/badge.svg)](https://
 github.com/Page-Leaf/docprompt/actions/workflows/dev.yml) [![codecov](https://
 codecov.io/gh/Page-Leaf/Docprompt/branch/main/graphs/badge.svg)](https://
-codecov.io/github/Page-Leaf/Docprompt)
+codecov.io/github/Page-Leaf/Docprompt) [![pdm-managed](https://img.shields.io/
+badge/pdm-managed-blueviolet)](https://pdm-project.org)
                                     _[_L_o_g_o_]
                               ******** DDooccpprroommpptt ********
                         Document AI, powered by LLM's
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                        Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 # About Docprompt is a library for Document AI. It aims to make enterprise-
@@ -59,8 +60,8 @@
 provider.process_document_node(document_node) # Caches results on the
 document_node # With OCR results available, we can now instantiate a locator
 and search through documents. document_node.locator.search("John Doe") # This
 will return a list of all terms across the document that contain "John Doe"
 document_node.locator.search("Jane Doe", page_number=4) # Just return results a
 list of matching results from page 4 ``` This functionality uses a combination
 of `rtree` and the Rust library `tantivy`, allowing you to perform thousands of
-searches in **seconds** :fire: :rocket:
+searches in **seconds** :fire: :rocket:_[_t_r_a_c_k_g_i_t_-_v_i_e_w_s_]
```

### Comparing `docprompt-0.4.4/docprompt/__init__.py` & `docprompt-0.4.5/docprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Docprompt."""
 
 __author__ = """Frankie Colson"""
 __email__ = "frank@pageleaf.io"
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 from docprompt.schema.document import Document, PdfDocument  # noqa
 from docprompt.schema.layout import NormBBox, TextBlock  # noqa
 from docprompt.schema.pipeline import DocumentCollection, DocumentNode, PageNode  # noqa
 from docprompt.utils import load_document, load_documents, hash_from_bytes  # noqa
 from docprompt.rasterize import ProviderResizeRatios
```

### Comparing `docprompt-0.4.4/docprompt/_exec/ghostscript.py` & `docprompt-0.4.5/docprompt/_exec/ghostscript.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/_pdfium.py` & `docprompt-0.4.5/docprompt/_pdfium.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/provenance/search.py` & `docprompt-0.4.5/docprompt/provenance/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,14 +212,15 @@
 
         return refine_result
 
     def search(
         self,
         query: str,
         page_number: Optional[int] = None,
+        *,
         refine_to_word: bool = True,
         require_exact_match: bool = True,
     ) -> List[ProvenanceSource]:
         """
         Search for a piece of text in the document and return the source of it
 
         Args:
```

### Comparing `docprompt-0.4.4/docprompt/provenance/source.py` & `docprompt-0.4.5/docprompt/provenance/source.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,25 +22,26 @@
     """
     Bundled with some data, specifies exactly where a piece of verbatim text came from
     in a document.
     """
 
     document_name: str
     page_number: PositiveInt
-    text_location: PageTextLocation
+    text_location: Optional[PageTextLocation] = None
 
     @computed_field  # type: ignore
     @property
     def source_block(self) -> Optional[TextBlock]:
-        if self.text_location.merged_source_block:
-            return self.text_location.merged_source_block
-        if self.text_location.source_blocks:
-            return self.text_location.source_blocks[0]
+        if self.text_location:
+            if self.text_location.merged_source_block:
+                return self.text_location.merged_source_block
+            if self.text_location.source_blocks:
+                return self.text_location.source_blocks[0]
 
-        return None
+            return None
 
     @property
     def text(self) -> str:
         if self.text_location:
             return "\n".join([block.text for block in self.text_location.source_blocks])
 
         return ""
```

### Comparing `docprompt-0.4.4/docprompt/provenance/util.py` & `docprompt-0.4.5/docprompt/provenance/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 import re
 from docprompt.schema.layout import NormBBox, TextBlock
 from typing import Any, Iterable, List, Optional
 from rapidfuzz import fuzz
+from rapidfuzz.utils import default_process
 
 try:
     import tantivy
 except ImportError:
     raise ImportError("Could not import tantivy. Install with `docprompt[search]`")
 
 try:
@@ -33,36 +34,14 @@
     text = text.strip()
 
     text = text.replace('"', "")
 
     return text
 
 
-def fuzzify_token(
-    token: str,
-    lowercase: bool = True,
-    strip_punct: bool = True,
-    strip_whitespace: bool = True,
-) -> str:
-    """
-    Convert a token into a form that is suitable for fuzzy matching.
-    """
-    if strip_whitespace:
-        token = token.strip()
-
-    if strip_punct:
-        token = token.strip(".")
-        token = token.strip(",")
-
-    if lowercase:
-        token = token.lower()
-
-    return token
-
-
 def word_tokenize(text: str) -> List[str]:
     """
     Tokenize a string into words.
     """
     return re.split(r"\s+", text)
 
 
@@ -120,30 +99,34 @@
     intersecting_word_level_blocks.sort(
         key=lambda x: (x.bounding_box.top, x.bounding_box.x0)
     )
 
     tokenized_query = word_tokenize(query)
 
     if len(tokenized_query) == 1:
-        fuzzified = fuzzify_token(tokenized_query[0])
+        fuzzified = default_process(tokenized_query[0])
         for word_level_block in intersecting_word_level_blocks:
-            if fuzz.ratio(fuzzified, fuzzify_token(word_level_block.text)) > 87.5:
+            if fuzz.ratio(fuzzified, default_process(word_level_block.text)) > 87.5:
                 return word_level_block, [word_level_block]
     else:
+        fuzzified_word_level_texts = [
+            default_process(word_level_block.text)
+            for word_level_block in intersecting_word_level_blocks
+        ]
+
         # Populate the block mapping
         token_block_mapping = defaultdict(set)
 
         first_word = tokenized_query[0]
         last_word = tokenized_query[-1]
 
         for token in tokenized_query:
-            fuzzified_token = fuzzify_token(token)
+            fuzzified_token = default_process(token)
             for i, word_level_block in enumerate(intersecting_word_level_blocks):
-                fuzzified_block_text = fuzzify_token(word_level_block.text)
-                if fuzz.ratio(fuzzified_token, fuzzified_block_text) > 87.5:
+                if fuzz.ratio(fuzzified_token, fuzzified_word_level_texts[i]) > 87.5:
                     token_block_mapping[token].add(i)
 
         graph = networkx.DiGraph()
         prev = tokenized_query[0]
 
         for i in token_block_mapping[prev]:
             graph.add_node(i)
```

### Comparing `docprompt-0.4.4/docprompt/rasterize.py` & `docprompt-0.4.5/docprompt/rasterize.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/schema/document.py` & `docprompt-0.4.5/docprompt/schema/document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/schema/layout.py` & `docprompt-0.4.5/docprompt/schema/layout.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/schema/pipeline.py` & `docprompt-0.4.5/docprompt/schema/pipeline.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/base.py` & `docprompt-0.4.5/docprompt/tasks/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/message.py` & `docprompt-0.4.5/docprompt/tasks/message.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/ocr/gcp.py` & `docprompt-0.4.5/docprompt/tasks/ocr/gcp.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/ocr/result.py` & `docprompt-0.4.5/docprompt/tasks/ocr/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/table_extraction/base.py` & `docprompt-0.4.5/docprompt/tasks/table_extraction/base.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/table_extraction/providers/claude.py` & `docprompt-0.4.5/docprompt/tasks/table_extraction/providers/claude.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/tasks/table_extraction/result.py` & `docprompt-0.4.5/docprompt/tasks/table_extraction/result.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/utils/date_extraction.py` & `docprompt-0.4.5/docprompt/utils/date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/utils/masking/image.py` & `docprompt-0.4.5/docprompt/utils/masking/image.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/utils/splitter.py` & `docprompt-0.4.5/docprompt/utils/splitter.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/docprompt/utils/util.py` & `docprompt-0.4.5/docprompt/utils/util.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/fixtures/1.pdf` & `docprompt-0.4.5/tests/fixtures/1.pdf`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/fixtures/1_ocr.json` & `docprompt-0.4.5/tests/fixtures/1_ocr.json`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/test_date_extraction.py` & `docprompt-0.4.5/tests/test_date_extraction.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/test_document.py` & `docprompt-0.4.5/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/test_documentnode.py` & `docprompt-0.4.5/tests/test_documentnode.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/test_layout_models.py` & `docprompt-0.4.5/tests/test_layout_models.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/test_search.py` & `docprompt-0.4.5/tests/test_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,28 @@
 
     assert len(result_page_1) == 1
 
     result_multiple_words = locator.search("MMAX2 system", page_number=1)
 
     assert len(result_multiple_words) == 1
 
+    sources = result_multiple_words[0].text_location.source_blocks
+
+    assert len(sources) == 2
+
+    result_multiple_words = locator.search(
+        "MMAX2 system", page_number=1, refine_to_word=False
+    )
+
+    assert len(result_multiple_words) == 1
+
+    sources = result_multiple_words[0].text_location.source_blocks
+
+    assert len(sources) == 1
+
     n_best = locator.search_n_best("and", n=3)
 
     assert len(n_best) == 3
 
     raw_search = locator.search_raw('content:"rooted"')
 
     assert len(raw_search) == 1
```

### Comparing `docprompt-0.4.4/tests/test_threadpool.py` & `docprompt-0.4.5/tests/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `docprompt-0.4.4/tests/util.py` & `docprompt-0.4.5/tests/util.py`

 * *Files identical despite different names*

