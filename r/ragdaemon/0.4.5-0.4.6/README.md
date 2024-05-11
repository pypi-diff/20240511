# Comparing `tmp/ragdaemon-0.4.5.tar.gz` & `tmp/ragdaemon-0.4.6.tar.gz`

## Comparing `ragdaemon-0.4.5.tar` & `ragdaemon-0.4.6.tar`

### file list

```diff
@@ -1,70 +1,78 @@
--rw-r--r--   0        0        0   669446 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/app.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/context.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/graph.py
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/utils.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/clusterer_binary.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/conftest.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/app.py
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/context.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8471 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6675 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    11629 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/conftest.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    14226 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.6/PKG-INFO
```

### Comparing `ragdaemon-0.4.5/tutorial.ipynb` & `ragdaemon-0.4.6/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/.github/workflows/run-tests.yml` & `ragdaemon-0.4.6/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/app.py` & `ragdaemon-0.4.6/ragdaemon/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,20 @@
 refresh = args.refresh
 verbose = True  # Always verbose in server mode
 code_extensions = None if args.code_extensions is None else set(args.code_extensions)
 diff = args.diff
 annotators = {
     "hierarchy": {},
     "chunker_llm": {"chunk_extensions": code_extensions},
+    "call_graph": {"call_extensions": code_extensions},
+    "summarizer": {},
     # "summarizer": {},
     # "clusterer_binary": {},
-    # "call_graph": {"call_extensions": code_extensions},
-    "diff": {"diff": diff},
-    "layout_hierarchy": {},
+    # "diff": {"diff": diff},
+    # "layout_hierarchy": {},
 }
 daemon = Daemon(Path.cwd(), annotators=annotators, verbose=verbose)
 
 
 # Start/run daemon in the background
 @asynccontextmanager
 async def lifespan(app: FastAPI):
```

### Comparing `ragdaemon-0.4.5/ragdaemon/context.py` & `ragdaemon-0.4.6/ragdaemon/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import re
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 from dict2xml import dict2xml
 from ragdaemon.annotators.diff import parse_diff_id
 from ragdaemon.database import Database
@@ -20,15 +21,18 @@
         content: NestedStrDict,
         tags: list[str] = [],
     ):
         self.content = content
         self.tags = tags
 
     def render(self) -> str:
-        return dict2xml(self.content, indent="    ")
+        output = dict2xml(self.content, indent="    ")
+        if self.tags:
+            output += f" ({', '.join(self.tags)})"
+        return output
 
 
 def render_comments(comments: list[Comment]) -> str:
     return "\n".join(comment.render() for comment in comments)
 
 
 class ContextBuilder:
@@ -85,22 +89,31 @@
             "tags": set(),
             "document": document,
             "diffs": set(),
             "comments": dict[int, list[Comment]](),
         }
         self.context[path_str] = message
 
-    def add_id(self, node_id: str, tags: list[str] = []):
+    def add_id(
+        self, node_id: str, tags: list[str] = [], summary_field_id: Optional[str] = None
+    ):
         """Add the given id to the context."""
         if node_id not in self.graph.nodes:
             raise ValueError(f"Node {node_id} not found in graph.")
         ref = self.graph.nodes[node_id].get("ref")
         if not ref:
             raise ValueError(f"Node {node_id} has no ref.")
         self.add_ref(ref, tags)
+        if summary_field_id:
+            summary = self.graph.nodes[node_id].get(summary_field_id)
+            if summary:
+                path, lines = parse_path_ref(ref)
+                path_str = path.as_posix()
+                line = 0 if not lines else max(0, min(lines) - 1)
+                self.add_comment(path_str, summary, line, tags=["summary"])
 
     def add_ref(self, path_ref: str, tags: list[str] = []):
         """Manually include path_refs"""
         path, lines = parse_path_ref(path_ref)
         path_str = path.as_posix()
         if path_str not in self.context:
             self._add_path(path_str)
@@ -183,15 +196,20 @@
             return
         self.context[path_str]["diffs"].remove(id)
         self.context[path_str]["tags"].remove("diff")
         if not self.context[path_str]["lines"] and not self.context[path_str]["diffs"]:
             del self.context[path_str]
         return id
 
-    def render(self, use_xml: bool = False, use_tags: bool = False) -> str:
+    def render(
+        self,
+        use_xml: bool = False,
+        use_tags: bool = False,
+        remove_whitespace: bool = False,
+    ) -> str:
         """Return a formatted context message for the given nodes."""
         output = ""
         for path_str, data in self.context.items():
             if output:
                 output += "\n"
 
             if use_tags and data["tags"]:
@@ -217,14 +235,20 @@
                     line_content = f"{line}:{file_lines[line]}"
                     if line in data["comments"]:
                         line_content += "\n" + render_comments(data["comments"][line])
                     output += line_content + "\n"
                     last_rendered = line
                 if last_rendered < len(file_lines) - 1:
                     output += "...\n"
+            if remove_whitespace:
+                # Remove empty ranges
+                output = re.sub(r"\.\.\.\n(\d+:\n)*(?=\.\.\.\n)", "", output)
+                # Remove last range if it's empty
+                output = re.sub(r"\.\.\.\n(\d+:\n)*$", "...\n", output)
+
             if data["diffs"]:
                 output += self.render_diffs(data["diffs"])
             if use_xml:
                 output += f"</{path_str}>\n"
         return output
 
     def render_diffs(self, ids: set[str]) -> str:
```

### Comparing `ragdaemon-0.4.5/ragdaemon/daemon.py` & `ragdaemon-0.4.6/ragdaemon/daemon.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import json
 import time
 from pathlib import Path
 from typing import Any, Iterable, Optional
 
 from networkx.readwrite import json_graph
 from spice import Spice
-from spice.spice import Model
+from spice.models import Model, TextModel
+from spice.spice import get_model_from_name
 
-from ragdaemon.annotators import Annotator, annotators_map
+from ragdaemon.annotators import annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
+from ragdaemon.errors import RagdaemonError
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
+from ragdaemon.locate import locate
 from ragdaemon.utils import DEFAULT_COMPLETION_MODEL, mentat_dir_path
 
 
 def default_annotators():
     return {
         "hierarchy": {},
         "chunker_line": {"lines_per_chunk": 30},
@@ -175,7 +178,37 @@
             if (next_tokens - include_tokens) > auto_tokens:
                 if node["type"] == "diff":
                     context.remove_diff(node["id"])
                 else:
                     context.remove_ref(node["ref"])
                 break
         return context
+
+    async def locate(
+        self,
+        query: str,
+        instruction: Optional[str] = None,
+        revise: bool = True,
+        model: Model | TextModel | str = DEFAULT_COMPLETION_MODEL,
+    ) -> list[str]:
+        """Use summaries to scan the codebase and return relevant nodes."""
+        if "summarizer" not in self.pipeline:
+            raise RagdaemonError(f"Summarizer annotator required for locate.")
+        if instruction is None:
+            instruction = "Return items which are relevant to fulfilling the query."
+        if isinstance(model, str):
+            model = get_model_from_name(model)
+        if not isinstance(model, TextModel):
+            raise RagdaemonError(f"Invalid model: {model}")
+
+        edge_type = "hierarchy"
+        summary_field_id = "summary"
+        return await locate(
+            self.graph,
+            edge_type,
+            summary_field_id,
+            self.spice_client,
+            instruction,
+            query,
+            model,
+            revise=revise,
+        )
```

### Comparing `ragdaemon-0.4.5/ragdaemon/get_paths.py` & `ragdaemon-0.4.6/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/graph.py` & `ragdaemon-0.4.6/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/utils.py` & `ragdaemon-0.4.6/ragdaemon/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import hashlib
 import re
 import subprocess
 from base64 import b64encode
 from pathlib import Path
 
 from spice import Spice
-from spice.models import GPT_4_TURBO, UnknownModel
+from spice.models import GPT_4_TURBO, Model, UnknownModel
 from spice.spice import get_model_from_name
 
 from ragdaemon.errors import RagdaemonError
+from ragdaemon.get_paths import get_paths_for_directory
 
 mentat_dir_path = Path.home() / ".mentat"
 
 
 semaphore = asyncio.Semaphore(100)
 
 
@@ -97,14 +98,19 @@
             text = "\n".join(
                 [line for i, line in enumerate(diff.split("\n")) if i + 1 in lines]
             )
         else:
             text = diff
         ref = f"git diff{'' if diff_ref == 'DEFAULT' else f' {diff_ref}'}"
 
+    elif type == "directory":
+        path = cwd if ref == "ROOT" else cwd / ref
+        paths = sorted([p.as_posix() for p in get_paths_for_directory(path)])
+        text = "\n".join(paths)
+
     elif type in {"file", "chunk"}:
         path, lines = parse_path_ref(ref)
         if lines:
             text = ""
             with open(cwd / path, "r") as f:
                 file_lines = f.read().split("\n")
             if max(lines) > len(file_lines):
@@ -119,31 +125,38 @@
                 raise RagdaemonError(f"Not a text file: {path}")
     else:
         raise RagdaemonError(f"Invalid type: {type}")
 
     return f"{ref}\n{text}"
 
 
-def truncate(document, embedding_model: str | None) -> tuple[str, float]:
+def truncate(
+    document, model: str | Model | None = None, tokens: int | None = None
+) -> tuple[str, float]:
     """Return an embeddable document, and what fraction was removed."""
-    if embedding_model is None:
+    if model is None:
         return document, 0
-    spice_model = get_model_from_name(embedding_model)
-    if isinstance(spice_model, UnknownModel):
-        raise RagdaemonError(f"Unrecognized embedding model: {embedding_model}")
-    max_tokens = spice_model.context_length
-    if max_tokens is None:
+
+    if isinstance(model, str):
+        model = get_model_from_name(model)
+        if isinstance(model, UnknownModel):
+            raise RagdaemonError(f"Unrecognized model: {model}")
+    max_tokens = model.context_length
+    if tokens is not None:
+        max_tokens = tokens if max_tokens is None else min(max_tokens, tokens)
+    doc_tokens = Spice().count_tokens(document, model=model.name)
+    if max_tokens is None or doc_tokens <= max_tokens:
         return document, 0
-    tokens = Spice().count_tokens(document, model=spice_model.name)
-    original_tokens = tokens
-    while tokens > max_tokens:
-        truncate_ratio = (max_tokens / tokens) * 0.98  # Saw some errors with .99
+
+    original_tokens = doc_tokens
+    while doc_tokens > max_tokens:
+        truncate_ratio = (max_tokens / doc_tokens) * 0.98  # Saw some errors with .99
         document = document[: int(len(document) * truncate_ratio)]
-        tokens = Spice().count_tokens(document, model=spice_model.name)
-    truncate_ratio = 1 - tokens / original_tokens
+        doc_tokens = Spice().count_tokens(document, model=model.name)
+    truncate_ratio = 1 - doc_tokens / original_tokens
     if truncate_ratio > 0:
         label = "\n[TRUNCATED]"
         document = document[: -len(label)] + label
     return document, truncate_ratio
 
 
 def lines_set_to_ref(lines: set[int]) -> str:
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/__init__.py` & `ragdaemon-0.4.6/ragdaemon/annotators/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from ragdaemon.annotators.chunker import Chunker
 from ragdaemon.annotators.chunker_line import ChunkerLine
 from ragdaemon.annotators.chunker_llm import ChunkerLLM
 from ragdaemon.annotators.diff import Diff
 from ragdaemon.annotators.hierarchy import Hierarchy
 from ragdaemon.annotators.layout_hierarchy import LayoutHierarchy
 from ragdaemon.annotators.summarizer import Summarizer
-from ragdaemon.annotators.clusterer_binary import ClustererBinary
 
 annotators_map = {
     "call_graph": CallGraph,
     "chunker": Chunker,
     "chunker_line": ChunkerLine,
     "chunker_llm": ChunkerLLM,
-    "clusterer_binary": ClustererBinary,
     "diff": Diff,
     "hierarchy": Hierarchy,
     "layout_hierarchy": LayoutHierarchy,
     "summarizer": Summarizer,
 }
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.6/ragdaemon/annotators/base_annotator.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class Annotator:
     name: str = "base_annotator"
 
     def __init__(
         self,
         verbose: bool = False,
         spice_client: Optional[Spice] = None,
-        pipeline: Optional[list[Annotator]] = None,
+        pipeline: Optional[dict[str, Annotator]] = None,
     ):
         self.verbose = verbose
         self.spice_client = spice_client
         pass
 
     def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         raise NotImplementedError()
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.4.6/ragdaemon/annotators/call_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+from functools import partial
 import json
 from pathlib import Path
 from typing import Any, Optional
 
 from tqdm.asyncio import tqdm
 from spice import SpiceMessages
 from spice.models import TextModel
@@ -15,45 +16,35 @@
     DEFAULT_CODE_EXTENSIONS,
     DEFAULT_COMPLETION_MODEL,
     parse_path_ref,
     semaphore,
 )
 
 
-def is_calls_valid(calls: dict[str, list[dict[str, str | list[int]]]]) -> bool:
-    """Expected structure: {path/to/file:class.method: [1, 2, 3]}"""
-    for target, lines in calls.items():
-        if not target or not isinstance(target, str):
-            return False
-        if not lines or not isinstance(lines, list):
-            return False
-        if not all(isinstance(line, int) for line in lines):
-            return False
-    return True
-
-
 class CallGraph(Annotator):
     name = "call_graph"
     call_field_id = "calls"
 
     def __init__(
         self,
         *args,
         call_extensions: Optional[list[str]] = None,
         model: Optional[TextModel | str] = DEFAULT_COMPLETION_MODEL,
-        pipeline: list[Annotator] = [],
+        pipeline: dict[str, Annotator] = {},
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         if call_extensions is None:
             call_extensions = DEFAULT_CODE_EXTENSIONS
         self.call_extensions = call_extensions
         try:
             chunk_field_id = next(
-                getattr(a, "chunk_field_id") for a in pipeline if "chunker" in a.name
+                getattr(a, "chunk_field_id")
+                for a in pipeline.values()
+                if "chunker" in a.name
             )
         except (StopIteration, AttributeError):
             raise RagdaemonError(
                 "CallGraph annotator requires a 'chunker' annotator with chunk_field_id."
             )
         self.chunk_field_id = chunk_field_id
         self.model = model
@@ -83,54 +74,83 @@
                         if edge[-1].get("type") == "call"
                         if edge[0].startswith(node)
                     ]
                     if len(matching_edges) != len(lines):
                         return False
         return True
 
-    async def get_llm_response(self, document: str, graph: KnowledgeGraph) -> str:
+    async def get_llm_response(
+        self, document: str, graph: KnowledgeGraph
+    ) -> dict[str, list[int]]:
         if self.spice_client is None:
             raise RagdaemonError("Spice client is not initialized.")
 
         messages = SpiceMessages(self.spice_client)
         messages.add_system_prompt(name="call_graph.base")
         messages.add_user_prompt("call_graph.user", document=document)
 
+        def validate(response: str, max_line: int) -> bool:
+            """Expected structure: {path/to/file:class.method: [1, 2, 3]}"""
+            try:
+                calls = json.loads(response)
+            except json.JSONDecodeError:
+                return False
+            for target, lines in calls.items():
+                if not target or not isinstance(target, str):
+                    return False
+                if not lines or not isinstance(lines, list):
+                    return False
+                if not all(isinstance(line, int) for line in lines):
+                    return False
+                if any(line > max_line for line in lines):
+                    return False
+            return True
+
+        validator = partial(validate, max_line=len(document.split("\n")))
         async with semaphore:
-            response = await self.spice_client.get_response(
-                messages=messages,
-                model=self.model,
-                response_format={"type": "json_object"},
-            )
-        try:
-            calls = json.loads(response.text)
-        except json.JSONDecodeError:
-            raise RagdaemonError("Failed to parse JSON response.")
-        if not is_calls_valid(calls):
-            raise RagdaemonError(f"Model returned malformed calls: {calls}")
+            try:
+                response = await self.spice_client.get_response(
+                    messages=messages,
+                    model=self.model,
+                    response_format={"type": "json_object"},
+                    validator=validator,
+                    retries=2,
+                )
+            except ValueError:  # Raised after all retries fail
+                if self.verbose:
+                    file = document.split("\n")[0]
+                    print(
+                        f"Failed to generate call graph for {file} after 3 tries, Skipping."
+                    )
+                return {}
+
+        calls = json.loads(response.text)
 
         # Resolve library calls
         targets = set(calls.keys())
         unresolved = set()
+        """
+        TODO: Handle unresolved calls. Usually result from:
+        - Class inheritance. No method for resolving.
+        - Missing file extensions. Imports can be unclear which part is the file.
+        - Using '.' instead of '/' in the path definition. Again, imports.
+        """
         for target in targets:
             if target in graph:
                 continue
             candidates = [
                 node
                 for node, data in graph.nodes(data=True)
                 if data.get("type") == "chunk" and node.endswith(target)
             ]
             if len(candidates) != 1:
                 del calls[target]
                 unresolved.add(target)
             else:
                 calls[candidates[0]] = calls.pop(target)
-        if unresolved and self.verbose:
-            path = document.split("\n")[0]
-            print(f"Unresolved calls in {path}: {unresolved}")
 
         return calls
 
     async def get_file_call_data(
         self,
         node: str,
         data: dict,
@@ -143,31 +163,30 @@
         record = db.get(data["checksum"])
         document = record["documents"][0]
 
         # Insert line numbers
         lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
-        if not file_lines or not any(line for line in file_lines):
-            return calls
-        file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
-        document = "\n".join([file] + file_lines)
-
-        for i in range(retries + 1, 0, -1):
-            try:
-                calls = await self.get_llm_response(document, graph)
-                break
-            except RagdaemonError as e:
-                if self.verbose:
-                    print(
-                        f"Error generating call graph for {node}:\n{e}\n"
-                        + f"{i-1} retries left."
-                        if i > 1
-                        else "Skipping."
-                    )
+        if any(line for line in file_lines):
+            file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
+            document = "\n".join([file] + file_lines)
+
+            for i in range(retries + 1, 0, -1):
+                try:
+                    calls = await self.get_llm_response(document, graph)
+                    break
+                except RagdaemonError as e:
+                    if self.verbose:
+                        print(
+                            f"Error generating call graph for {node}:\n{e}\n"
+                            + f"{i-1} retries left."
+                            if i > 1
+                            else "Skipping."
+                        )
 
         # Save to db and graph
         metadatas = record["metadatas"][0]
         metadatas[self.call_field_id] = json.dumps(calls)
         db.update(data["checksum"], metadatas=metadatas)
         data[self.call_field_id] = calls
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.6/ragdaemon/annotators/chunker.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,22 @@
         # Grab and validate chunks for given file
         chunks = data.get(self.chunk_field_id)
         if chunks is None:
             raise RagdaemonError(f"Node {file} missing {self.chunk_field_id}")
         if isinstance(chunks, str):
             chunks = json.loads(chunks)
             data[self.chunk_field_id] = chunks
+
+        add_to_db = {"ids": [], "documents": [], "metadatas": []}
+        if len(chunks) == 0:
+            return add_to_db
         base_id = f"{file}:BASE"
-        if len(chunks) > 0 and not any(chunk["id"] == base_id for chunk in chunks):
+        if not any(chunk["id"] == base_id for chunk in chunks):
             raise RagdaemonError(f"Node {file} missing base chunk")
         edges_to_add = {(file, base_id)}
-        add_to_db = {"ids": [], "documents": [], "metadatas": []}
         for chunk in chunks:
             # Locate or create record for chunk
             id, ref = chunk["id"], chunk["ref"]
             document = get_document(ref, Path(graph.graph["cwd"]))
             checksum = hash_str(document)
             records = db.get(checksum)["metadatas"]
             if not refresh and len(records) > 0:
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.6/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.6/ragdaemon/annotators/chunker_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,22 +139,24 @@
                 _chunks[id] = parent_lines
             return _chunks
 
         ids_longest_first = sorted(chunks, key=lambda x: len(x), reverse=True)
         for id in ids_longest_first:
             chunks = update_parent_nodes(id, chunks)
 
-        # Generate a 'BASE chunk' with all lines not already part of a chunk
-        base_chunk_lines = set(range(1, len(file_lines) + 1))
-        for lines in chunks.values():
-            base_chunk_lines -= lines
-        lines_ref = lines_set_to_ref(base_chunk_lines)
-        ref = f"{file}:{lines_ref}" if lines_ref else file
-        base_chunk = {"id": f"{file}:BASE", "ref": ref}
+        output = []
+        if chunks:
+            # Generate a 'BASE chunk' with all lines not already part of a chunk
+            base_chunk_lines = set(range(1, len(file_lines) + 1))
+            for lines in chunks.values():
+                base_chunk_lines -= lines
+            lines_ref = lines_set_to_ref(base_chunk_lines)
+            ref = f"{file}:{lines_ref}" if lines_ref else file
+            base_chunk = {"id": f"{file}:BASE", "ref": ref}
+            output.append(base_chunk)
 
         # Convert to refs and return
-        output = [base_chunk]
         for id, lines in chunks.items():
             lines_ref = lines_set_to_ref(lines)
             ref = f"{file}:{lines_ref}" if lines_ref else file
             output.append({"id": id, "ref": ref})
         return output
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.6/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.6/ragdaemon/annotators/hierarchy.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 def get_active_checksums(
     cwd: Path,
     db: Database,
     refresh: bool = False,
     verbose: bool = False,
     ignore_patterns: set[Path] = set(),
 ) -> dict[Path, str]:
+    # Get checksums for all active files
     checksums: dict[Path, str] = {}
     paths = get_paths_for_directory(cwd, exclude_patterns=ignore_patterns)
     add_to_db = {
         "ids": [],
         "documents": [],
         "metadatas": [],
     }
@@ -46,14 +47,53 @@
                 add_to_db["metadatas"].append(metadatas)
             checksums[path] = checksum
         except UnicodeDecodeError:  # Ignore non-text files
             pass
         except RagdaemonError as e:
             if verbose:
                 print(f"Error processing path {path}: {e}")
+
+    # Get checksums for all active directories
+    directories = set()
+    for path in paths:
+        for parent in path.parents:
+            if parent not in paths:
+                directories.add(parent)
+    for path in directories:
+        ref = path.as_posix()
+        document = get_document(ref, cwd, type="directory")
+
+        # The checksum for a directory is the hash of the checksums of its subpaths,
+        # which are listed in the document and were computed above.
+        subdir_checksums = ""
+        for subpath in document.split("\n")[1:]:
+            subpath = Path(ref) / subpath
+            if subpath in checksums:
+                subdir_checksums += checksums[subpath]
+            else:
+                raise RagdaemonError(f"Checksum not found for {subpath}")
+        checksum = hash_str(subdir_checksums)
+
+        existing_record = len(db.get(checksum)["ids"]) > 0
+        if refresh or not existing_record:
+            metadatas = {
+                "id": ref,
+                "type": "directory",
+                "ref": ref,
+                "checksum": checksum,
+                "active": False,
+            }
+            document, truncate_ratio = truncate(document, db.embedding_model)
+            if truncate_ratio > 0 and verbose:
+                print(f"Truncated {ref} by {truncate_ratio:.2%}")
+            add_to_db["ids"].append(checksum)
+            add_to_db["documents"].append(document)
+            add_to_db["metadatas"].append(metadatas)
+        checksums[path] = checksum
+
     if len(add_to_db["ids"]) > 0:
         add_to_db = remove_add_to_db_duplicates(**add_to_db)
         db.upsert(**add_to_db)
     return checksums
 
 
 def files_checksum(cwd: Path, ignore_patterns: set[Path] = set()) -> str:
@@ -96,32 +136,32 @@
 
         # Initialize an empty graph. We'll build it from scratch.
         graph = KnowledgeGraph()
         graph.graph["cwd"] = str(cwd)
         edges_to_add = set()
         for path, checksum in checksums.items():
             # add db reecord
-            id = path.as_posix()
+            id = path.as_posix() if len(path.parts) > 0 else "ROOT"
             results = db.get(checksum)
             data = results["metadatas"][0]
             graph.add_node(id, **data)
+            if id == "ROOT":
+                continue
 
             # add hierarchy edges
             def _link_to_cwd(_path: Path):
                 _parent = _path.parent.as_posix() if len(_path.parts) > 1 else "ROOT"
                 edges_to_add.add((_parent, _path.as_posix()))
                 if _parent != "ROOT":
                     _link_to_cwd(_path.parent)
 
             _link_to_cwd(path)
 
         # Add directory nodes with checksums
         for source, target in edges_to_add:
             for id in (source, target):
                 if id not in graph:
-                    # add directories to graph (to link hierarchy) but not db
-                    record = {"id": id, "type": "directory", "ref": id}
-                    graph.add_node(id, **record)
+                    raise RagdaemonError(f"Node {id} not found in graph")
             graph.add_edge(source, target, type="hierarchy")
 
         graph.graph["files_checksum"] = _files_checksum
         return graph
```

### Comparing `ragdaemon-0.4.5/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.6/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/database/__init__.py` & `ragdaemon-0.4.6/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.6/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/database/database.py` & `ragdaemon-0.4.6/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.6/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.4.6/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.6/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.6/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.6/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/static/js/main.js` & `ragdaemon-0.4.6/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.6/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.6/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.6/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/ragdaemon/templates/index.html` & `ragdaemon-0.4.6/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/conftest.py` & `ragdaemon-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/test_comments.py` & `ragdaemon-0.4.6/tests/test_comments.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,29 +35,29 @@
         {"author": "bot", "content": "hello", "replies": nested_comment},
         line=20,
     )
     context.add_comment("src/operations.py", "Comments can just be strings", line=12)
     actual = context.render()
     assert actual == dedent("""\
             src/operations.py
-            <comment>What is this file for?</comment>
+            <comment>What is this file for?</comment> (test-flag)
             1:import math
             2: #modified
             3: #modified
             4:def add(a, b): #modified
             5:    return a + b
             6:
             7:
             8:def subtract(a, b):
             9:return a - b #modified
             10:
             <comment>
                 <author>bot</author>
                 <content>test</content>
-            </comment>
+            </comment> (test-flag2)
             <comment>
                 <author>bot</author>
                 <content>Two comments on one line</content>
             </comment>
             11:
             12:def multiply(a, b):
             Comments can just be strings
@@ -92,15 +92,15 @@
             7:
             8:def subtract(a, b):
             9:return a - b #modified
             10:
             <comment>
                 <author>bot</author>
                 <content>test</content>
-            </comment>
+            </comment> (test-flag2)
             <comment>
                 <author>bot</author>
                 <content>Two comments on one line</content>
             </comment>
             11:
             12:def multiply(a, b):
             Comments can just be strings
```

### Comparing `ragdaemon-0.4.5/tests/test_context.py` & `ragdaemon-0.4.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/test_daemon.py` & `ragdaemon-0.4.6/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/test_get_paths.py` & `ragdaemon-0.4.6/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/test_sample.py` & `ragdaemon-0.4.6/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/annotators/test_chunker.py` & `ragdaemon-0.4.6/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.6/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/annotators/test_diff.py` & `ragdaemon-0.4.6/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.6/tests/annotators/test_hierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
     expected = {
         (node, data["checksum"])
         for node, data in hierarchy_graph.nodes(data=True)
         if data and "checksum" in data
     }
+    # Replace checksums "." with "ROOT"
+    checksums[Path("ROOT")] = checksums.pop(Path("."))
     actual = {(path.as_posix(), checksum) for path, checksum in checksums.items()}
     assert actual == expected, "Checksums are not equal"
 
 
 def test_hierarchy_is_complete(cwd, mock_db):
     empty_graph = KnowledgeGraph()
     empty_graph.graph["cwd"] = cwd.as_posix()
```

### Comparing `ragdaemon-0.4.5/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.6/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/data/chunker_graph.json` & `ragdaemon-0.4.6/tests/data/chunker_graph.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9955555555555555%*

 * *Differences: {"'nodes'": "{5: {'active': False, 'checksum': 'b97e74d824fca5e980257ed15bb800b3'}, 6: {'active': "*

 * *            "False, 'checksum': '6a31bb042874e065fea5bcbc36362d58'}}"}*

```diff
@@ -212,19 +212,23 @@
                 }
             ],
             "id": "src/interface.py",
             "ref": "src/interface.py",
             "type": "file"
         },
         {
+            "active": false,
+            "checksum": "b97e74d824fca5e980257ed15bb800b3",
             "id": "ROOT",
             "ref": "ROOT",
             "type": "directory"
         },
         {
+            "active": false,
+            "checksum": "6a31bb042874e065fea5bcbc36362d58",
             "id": "src",
             "ref": "src",
             "type": "directory"
         },
         {
             "active": false,
             "checksum": "771e07c404b686df1bcb59239a67d2e4",
```

### Comparing `ragdaemon-0.4.5/tests/data/context_message.txt` & `ragdaemon-0.4.6/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/data/diff_graph.json` & `ragdaemon-0.4.6/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.6/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.6/tests/data/hierarchy_graph.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'nodes'": "{6: {'active': False, 'checksum': 'b97e74d824fca5e980257ed15bb800b3'}, 7: {'active': "*

 * *            "False, 'checksum': '6a31bb042874e065fea5bcbc36362d58'}}"}*

```diff
@@ -89,18 +89,22 @@
             "active": false,
             "checksum": "39611184a249763e91b60432ae324486",
             "id": ".gitignore",
             "ref": ".gitignore",
             "type": "file"
         },
         {
+            "active": false,
+            "checksum": "b97e74d824fca5e980257ed15bb800b3",
             "id": "ROOT",
             "ref": "ROOT",
             "type": "directory"
         },
         {
+            "active": false,
+            "checksum": "6a31bb042874e065fea5bcbc36362d58",
             "id": "src",
             "ref": "src",
             "type": "directory"
         }
     ]
 }
```

### Comparing `ragdaemon-0.4.5/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.6/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/tests/sample/src/interface.py` & `ragdaemon-0.4.6/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/LICENSE` & `ragdaemon-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/README.md` & `ragdaemon-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.5/pyproject.toml` & `ragdaemon-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.5"
+version = "0.4.6"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.4.5/PKG-INFO` & `ragdaemon-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.5
+Version: 0.4.6
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

