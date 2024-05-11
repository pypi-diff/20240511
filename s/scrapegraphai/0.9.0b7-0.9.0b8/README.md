# Comparing `tmp/scrapegraphai-0.9.0b7.tar.gz` & `tmp/scrapegraphai-0.9.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.9.0b7.tar", max compression
+gzip compressed data, was "scrapegraphai-0.9.0b8.tar", max compression
```

## Comparing `scrapegraphai-0.9.0b7.tar` & `scrapegraphai-0.9.0b8.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1065 2024-05-06 11:24:17.752334 scrapegraphai-0.9.0b7/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-06 11:24:17.752334 scrapegraphai-0.9.0b7/README.md
--rw-r--r--   0        0        0     1792 2024-05-06 11:24:36.024299 scrapegraphai-0.9.0b7/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      491 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    12862 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2440 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3359 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3738 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3628 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3569 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3513 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4297 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3502 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      369 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      479 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/claude.py
--rw-r--r--   0        0        0      606 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      835 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     8591 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3721 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     7038 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6462 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7038 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     7014 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     6670 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3537 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     3041 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/graph_iterator_node.py
--rw-r--r--   0        0        0     1980 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3902 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/merge_answers_node.py
--rw-r--r--   0        0        0     2709 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4495 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5664 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3948 2024-05-06 11:24:17.780334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6307 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2342 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     2140 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-06 11:24:17.784334 scrapegraphai-0.9.0b7/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-06 12:37:37.387034 scrapegraphai-0.9.0b8/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-06 12:37:37.391034 scrapegraphai-0.9.0b8/README.md
+-rw-r--r--   0        0        0     1792 2024-05-06 12:37:55.291453 scrapegraphai-0.9.0b8/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      491 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    12862 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2440 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3359 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3628 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3569 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3513 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4297 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3502 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     2181 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      369 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      479 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/claude.py
+-rw-r--r--   0        0        0      606 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      835 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     8591 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3721 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     7038 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6462 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     7038 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     7014 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     6670 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3537 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     3041 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/graph_iterator_node.py
+-rw-r--r--   0        0        0     1980 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3902 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/merge_answers_node.py
+-rw-r--r--   0        0        0     2709 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4495 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5664 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3948 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6307 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2342 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-06 12:37:37.419035 scrapegraphai-0.9.0b8/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     2140 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-06 12:37:37.423035 scrapegraphai-0.9.0b8/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b8/PKG-INFO
```

### Comparing `scrapegraphai-0.9.0b7/LICENSE` & `scrapegraphai-0.9.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/README.md` & `scrapegraphai-0.9.0b8/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/pyproject.toml` & `scrapegraphai-0.9.0b8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.9.0b7"
+version = "0.9.0b8"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.9.0b8/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.9.0b8/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.9.0b8/scrapegraphai/helpers/models_tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,20 +28,22 @@
         "gemini-pro": 128000,
         "models/embedding-001": 2048
     },
 
     "ollama": {
         "llama2": 4096,
         "llama3": 8192,
+        "llava": 4096,
+        "llava_next": 4096,
         "mistral": 8192,
         "codellama": 16000,
         "dolphin-mixtral": 32000,
         "mistral-openorca": 32000,
         "stablelm-zephyr": 8192,
-        "nomic-embed-text":8192
+        "nomic-embed-text": 8192
     },
     "groq": {
         "llama3-8b-8192": 8192,
         "llama3-70b-8192": 8192,
         "mixtral-8x7b-32768": 32768,
         "gemma-7b-it": 8192,
     },
@@ -66,9 +68,10 @@
         "mistral.mixtral-8x7b-instruct-v0:1": 32768,
         "mistral.mistral-large-2402-v1:0": 32768,
         "cohere.embed-english-v3": 512,
         "cohere.embed-multilingual-v3": 512
     },
     "mistral": {
         "mistralai/Mistral-7B-Instruct-v0.2": 32000
-    }
+    },
+    "hugging_face": {}
 }
```

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.9.0b8/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.9.0b8/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.9.0b8/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/models/gemini.py` & `scrapegraphai-0.9.0b8/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.9.0b8/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.9.0b8/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/graph_iterator_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/graph_iterator_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/merge_answers_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/merge_answers_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.9.0b8/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/remover.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.9.0b8/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b7/PKG-INFO` & `scrapegraphai-0.9.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.9.0b7
+Version: 0.9.0b8
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

