# Comparing `tmp/webscout-1.4.5.tar.gz` & `tmp/webscout-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-1.4.5.tar", last modified: Fri May 10 04:43:15 2024, max compression
+gzip compressed data, was "webscout-1.4.6.tar", last modified: Fri May 10 15:14:11 2024, max compression
```

## Comparing `webscout-1.4.5.tar` & `webscout-1.4.6.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:15.902631 webscout-1.4.5/
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.667609 webscout-1.4.5/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.700147 webscout-1.4.5/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.801515 webscout-1.4.5/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:13.965411 webscout-1.4.5/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-1.4.5/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-1.4.5/LICENSE.md
--rw-rw-rw-   0        0        0    43415 2024-05-10 04:43:15.889556 webscout-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0    41114 2024-05-10 02:21:13.000000 webscout-1.4.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-10 04:43:15.903626 webscout-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     2800 2024-05-10 04:42:14.000000 webscout-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:15.716486 webscout-1.4.5/webscout/
--rw-rw-rw-   0        0        0   226145 2024-05-09 17:13:40.000000 webscout-1.4.5/webscout/AI.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33217 2024-05-09 17:15:58.000000 webscout-1.4.5/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/LLM.py
--rw-rw-rw-   0        0        0     1090 2024-05-09 17:15:47.000000 webscout-1.4.5/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/__main__.py
--rw-rw-rw-   0        0        0      971 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/cli.py
--rw-rw-rw-   0        0        0      378 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24489 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-1.4.5/webscout/utils.py
--rw-rw-rw-   0        0        0       25 2024-05-10 04:42:09.000000 webscout-1.4.5/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-1.4.5/webscout/voice.py
--rw-rw-rw-   0        0        0    82831 2024-05-09 17:15:32.000000 webscout-1.4.5/webscout/webai.py
--rw-rw-rw-   0        0        0     3393 2024-05-10 04:31:54.000000 webscout-1.4.5/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-1.4.5/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-10 04:43:15.882006 webscout-1.4.5/webscout.egg-info/
--rw-rw-rw-   0        0        0    43415 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2024-05-10 04:43:13.000000 webscout-1.4.5/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      379 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-10 04:43:12.000000 webscout-1.4.5/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.541437 webscout-1.4.6/
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.238857 webscout-1.4.6/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.254874 webscout-1.4.6/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.297797 webscout-1.4.6/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.344177 webscout-1.4.6/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-1.4.6/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-1.4.6/LICENSE.md
+-rw-rw-rw-   0        0        0    43356 2024-05-10 15:14:11.536437 webscout-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0    41114 2024-05-10 02:21:13.000000 webscout-1.4.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-10 15:14:11.544441 webscout-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     2741 2024-05-10 15:13:41.000000 webscout-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.485783 webscout-1.4.6/webscout/
+-rw-rw-rw-   0        0        0   226181 2024-05-10 14:33:23.000000 webscout-1.4.6/webscout/AI.py
+-rw-rw-rw-   0        0        0    17297 2024-05-10 14:45:32.000000 webscout-1.4.6/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33233 2024-05-10 14:47:44.000000 webscout-1.4.6/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/LLM.py
+-rw-rw-rw-   0        0        0     1104 2024-05-10 14:47:33.000000 webscout-1.4.6/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/__main__.py
+-rw-rw-rw-   0        0        0      711 2024-05-10 14:40:09.000000 webscout-1.4.6/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-1.4.6/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24489 2024-05-10 14:33:00.000000 webscout-1.4.6/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-1.4.6/webscout/utils.py
+-rw-rw-rw-   0        0        0       25 2024-05-10 04:42:09.000000 webscout-1.4.6/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-1.4.6/webscout/voice.py
+-rw-rw-rw-   0        0        0    83660 2024-05-10 14:56:15.000000 webscout-1.4.6/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-1.4.6/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-1.4.6/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-10 15:14:11.529066 webscout-1.4.6/webscout.egg-info/
+-rw-rw-rw-   0        0        0    43356 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1061 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      320 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-10 15:14:10.000000 webscout-1.4.6/webscout.egg-info/top_level.txt
```

### Comparing `webscout-1.4.5/DeepWEBS/documents/query_results_extractor.py` & `webscout-1.4.6/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-1.4.6/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/networks/filepath_converter.py` & `webscout-1.4.6/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/networks/google_searcher.py` & `webscout-1.4.6/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/networks/network_configs.py` & `webscout-1.4.6/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/networks/webpage_fetcher.py` & `webscout-1.4.6/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/utilsdw/enver.py` & `webscout-1.4.6/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/DeepWEBS/utilsdw/logger.py` & `webscout-1.4.6/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/LICENSE.md` & `webscout-1.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/PKG-INFO` & `webscout-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.5
+Version: 1.4.6
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -20,22 +20,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: docstring_inheritance
+Requires-Dist: click
+Requires-Dist: curl_cffi
+Requires-Dist: lxml
+Requires-Dist: nest-asyncio
+Requires-Dist: selenium
+Requires-Dist: tqdm
+Requires-Dist: webdriver-manager
 Requires-Dist: halo>=0.0.31
 Requires-Dist: g4f>=0.2.2.3
 Requires-Dist: rich
 Requires-Dist: python-dotenv
 Requires-Dist: Helpingai-T2
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.5 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.6 Summary: Search for
 anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -13,18 +13,17 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Description-Content-
 Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
+Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
+tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
 Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
 Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
```

### Comparing `webscout-1.4.5/README.md` & `webscout-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/setup.py` & `webscout-1.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="1.4.5", 
+    version="1.4.6", 
     description="Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
@@ -24,22 +24,22 @@
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Internet :: WWW/HTTP :: Indexing/Search',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     install_requires=[
-        "docstring_inheritance>=2.1.2",
-        "click>=8.1.7",
-        "curl_cffi>=0.6.0b7",
-        "lxml>=5.1.0",
-        "nest-asyncio>=1.6.0",
-        "selenium>=4.1.3",
-        "tqdm>=4.64.0",
-        "webdriver-manager>=3.5.4",
+        "docstring_inheritance",
+        "click",
+        "curl_cffi",
+        "lxml",
+        "nest-asyncio",
+        "selenium",
+        "tqdm",
+        "webdriver-manager",
         "halo>=0.0.31",
         "g4f>=0.2.2.3",
         "rich",
         "python-dotenv",
         "Helpingai-T2",
         "beautifulsoup4",
         "markdownify",
```

### Comparing `webscout-1.4.5/webscout/AI.py` & `webscout-1.4.6/webscout/AI.py`

 * *Files 0% similar despite different names*

```diff
@@ -3273,14 +3273,15 @@
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["content"]
 class AsyncOPENGPT(AsyncProvider):
     def __init__(
         self,
         is_conversation: bool = True,
         max_tokens: int = 600,
         timeout: int = 30,
         intro: str = None,
```

### Comparing `webscout-1.4.5/webscout/AIbase.py` & `webscout-1.4.6/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/AIutel.py` & `webscout-1.4.6/webscout/AIutel.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     "perplexity",
     "groq",
     "reka",
     "cohere",
     "yepchat",
     "you",
     "xjai",
-    "thinkany"
+    "thinkany",
+    "auto",
+
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
```

### Comparing `webscout-1.4.5/webscout/DWEBS.py` & `webscout-1.4.6/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/LLM.py` & `webscout-1.4.6/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/__init__.py` & `webscout-1.4.6/webscout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
 from .voice import play_audio
 
-
 __repo__ = "https://github.com/OE-LUCIFER/Webscout"
 
 webai = [
     "leo",
     "openai",
     "opengpt",
     "koboldai",
@@ -26,15 +25,17 @@
     "perplexity",
     "groq",
     "reka",
     "cohere",
     "yepchat",
     "you",
     "xjai",
-    "thinkany"
+    "thinkany",
+    "auto",
+
 ]
 
 gpt4free_providers = [
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
```

### Comparing `webscout-1.4.5/webscout/async_providers.py` & `webscout-1.4.6/webscout/async_providers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,21 @@
 from webscout.AI import AsyncOPENGPT
 from webscout.AI import AsyncOPENAI
 from webscout.AI import AsyncLLAMA2
 from webscout.AI import AsyncLEO
 from webscout.AI import AsyncKOBOLDAI
 from webscout.AI import AsyncGROQ
 from webscout.AI import AsyncBLACKBOXAI
-from webscout.AI import AsyncGPT4FREE
+from webscout.g4f import AsyncGPT4FREE
 
 mapper: dict[str, object] = {
     "phind": AsyncPhindSearch,
     "opengpt": AsyncOPENGPT,
     "koboldai": AsyncKOBOLDAI,
     "blackboxai": AsyncBLACKBOXAI,
     "gpt4free": AsyncGPT4FREE,
     "llama2": AsyncLLAMA2,
     "yepchat": AsyncYEPCHAT,
     "leo": AsyncLEO,
     "groq": AsyncGROQ,
     "openai": AsyncOPENAI,
 }
-
-tgpt_mapper: dict[str, object] = {
-    "phind": AsyncPhindSearch,
-    "opengpt": AsyncOPENGPT,
-    "koboldai": AsyncKOBOLDAI,
-    # "gpt4free": AsyncGPT4FREE,
-    "blackboxai": AsyncBLACKBOXAI,
-    "llama2": AsyncLLAMA2,
-    "yepchat": AsyncYEPCHAT,
-}
```

### Comparing `webscout-1.4.5/webscout/cli.py` & `webscout-1.4.6/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/g4f.py` & `webscout-1.4.6/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/models.py` & `webscout-1.4.6/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/tempid.py` & `webscout-1.4.6/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/transcriber.py` & `webscout-1.4.6/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/utils.py` & `webscout-1.4.6/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/voice.py` & `webscout-1.4.6/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout/webai.py` & `webscout-1.4.6/webscout/webai.py`

 * *Files 2% similar despite different names*

```diff
@@ -452,28 +452,42 @@
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
                 )
+            if provider == "auto":
+                from webscout.AIauto import AUTO
 
+                self.bot = AUTO(
+                    is_conversation=disable_conversation,
+                    max_tokens=max_tokens,
+                    timeout=timeout,
+                    intro=intro,
+                    filepath=filepath,
+                    update_file=update_file,
+                    proxies=proxies,
+                    history_offset=history_offset,
+                    act=awesome_prompt,
+                )
             elif provider == "opengpt":
                 from webscout.AI import OPENGPT
 
                 self.bot = OPENGPT(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
                     timeout=timeout,
                     intro=intro,
                     filepath=filepath,
                     update_file=update_file,
                     proxies=proxies,
                     history_offset=history_offset,
                     act=awesome_prompt,
+                    assistant_id="bca37014-6f97-4f2b-8928-81ea8d478d88"
                 )
             elif provider == "thinkany":
                 from webscout.AI import ThinkAnyAI
 
                 self.bot = ThinkAnyAI(
                     is_conversation=disable_conversation,
                     max_tokens=max_tokens,
@@ -721,43 +735,49 @@
         self.rawdog = rawdog
         self.read_aloud = False
         self.read_aloud_voice = "Brian"
         self.path_to_last_response_audio = None
         self.__init_time = time.time()
         self.__start_time = time.time()
         self.__end_time = time.time()
-
+        
+    @property
+    def get_provider(self):
+        if self.provider == "auto" and self.bot.provider_name is not None:
+            return self.bot.provider_name
+        else:
+            return self.provider
     @property
     def prompt(self):
         current_time = datetime.datetime.now().strftime("%H:%M:%S")
 
         def find_range(start, end, hms: bool = False):
             in_seconds = round(end - start, 1)
             return (
                 str(datetime.timedelta(seconds=in_seconds)).split(".")[0].zfill(8)
                 if hms
                 else in_seconds
             )
         if not self.disable_coloring:
             cmd_prompt = (
                 f"╭─[`{Fore.GREEN}{getpass.getuser().capitalize()}@webai]`"
-                f"(`{Fore.YELLOW}{self.provider})`"
+                f"(`{Fore.YELLOW}{self.get_provider})`"
                 f"~[`{Fore.LIGHTWHITE_EX}⏰{Fore.MAGENTA}{current_time}-`"
                 f"{Fore.LIGHTWHITE_EX}💻{Fore.BLUE}{find_range(self.__init_time, time.time(), True)}-`"
                 f"{Fore.LIGHTWHITE_EX}⚡️{Fore.RED}{find_range(self.__start_time, self.__end_time)}s]`"
                 f"\n╰─>"
             )
             whitelist = ["[", "]", "~", "-", "(", ")"]
             for character in whitelist:
                 cmd_prompt = cmd_prompt.replace(character + "`", Fore.RESET + character)
             return cmd_prompt
 
         else:
             return (
-                f"╭─[{getpass.getuser().capitalize()}@webscout]({self.provider})"
+                f"╭─[{getpass.getuser().capitalize()}@webscout]({self.get_provider})"
                 f"~[⏰{current_time}"
                 f"-💻{find_range(self.__init_time, time.time(), True)}"
                 f"-⚡️{find_range(self.__start_time, self.__end_time)}s]"
                 f"~[⏰{current_time}"
                 f"-💻{find_range(self.__init_time, time.time(), True)}"
                 f"-⚡️{find_range(self.__start_time, self.__end_time)}s]"
                 "\n╰─>"
@@ -1121,15 +1141,15 @@
                                 if self.prettify
                                 else response
                             )
                 else:
                     busy_bar.stop_spinning()
                     this.stream_output(
                         generated_response,
-                        title="AI Response",
+                        title="Webscout",
                         is_markdown=self.prettify,
                         style=Style(
                             color=self.color,
                         ),
                         code_theme=self.code_theme,
                         vertical_overflow=self.vertical_overflow,
                     )
```

### Comparing `webscout-1.4.5/webscout/webscout_search.py` & `webscout-1.4.6/webscout/webscout_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 import asyncio
 from concurrent.futures import Future
 from threading import Thread
 import sys
 from types import TracebackType
 from typing import Any, Awaitable, Dict, Optional, Type, Union
-if sys.platform == 'win32':
-    try:
-        asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-    except AttributeError:
-        # If WindowsSelectorEventLoopPolicy is not available, do nothing
-        pass
 from .webscout_search_async import AsyncWEBS
 
 
 class WEBS(AsyncWEBS):
     _loop: asyncio.AbstractEventLoop = asyncio.new_event_loop()
     Thread(target=_loop.run_forever, daemon=True).start()  # Start the event loop run in a separate thread.
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         proxy: Optional[str] = None,
         proxies: Union[Dict[str, str], str, None] = None,  # deprecated
         timeout: Optional[int] = 10,
     ) -> None:
-        """Initialize the DDGS object.
+        """Initialize the WEBS object.
 
         Args:
             headers (dict, optional): Dictionary of headers for the HTTP client. Defaults to None.
             proxy (str, optional): proxy for the HTTP client, supports http/https/socks5 protocols.
                 example: "http://user:pass@example.com:3128". Defaults to None.
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
@@ -77,8 +71,8 @@
     def suggestions(self, *args: Any, **kwargs: Any) -> Any:
         return self._run_async_in_thread(super().suggestions(*args, **kwargs))
 
     def maps(self, *args: Any, **kwargs: Any) -> Any:
         return self._run_async_in_thread(super().maps(*args, **kwargs))
 
     def translate(self, *args: Any, **kwargs: Any) -> Any:
-        return self._run_async_in_thread(super().translate(*args, **kwargs))
+        return self._run_async_in_thread(super().translate(*args, **kwargs))
```

### Comparing `webscout-1.4.5/webscout/webscout_search_async.py` & `webscout-1.4.6/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-1.4.5/webscout.egg-info/PKG-INFO` & `webscout-1.4.6/webscout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 1.4.5
+Version: 1.4.6
 Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -20,22 +20,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: docstring_inheritance>=2.1.2
-Requires-Dist: click>=8.1.7
-Requires-Dist: curl_cffi>=0.6.0b7
-Requires-Dist: lxml>=5.1.0
-Requires-Dist: nest-asyncio>=1.6.0
-Requires-Dist: selenium>=4.1.3
-Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4
+Requires-Dist: docstring_inheritance
+Requires-Dist: click
+Requires-Dist: curl_cffi
+Requires-Dist: lxml
+Requires-Dist: nest-asyncio
+Requires-Dist: selenium
+Requires-Dist: tqdm
+Requires-Dist: webdriver-manager
 Requires-Dist: halo>=0.0.31
 Requires-Dist: g4f>=0.2.2.3
 Requires-Dist: rich
 Requires-Dist: python-dotenv
 Requires-Dist: Helpingai-T2
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 1.4.5 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 1.4.6 Summary: Search for
 anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can
 transcribe yt videos, temporary email and phone number generation, have TTS
 support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
 email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
@@ -13,18 +13,17 @@
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Description-Content-
 Type: text/markdown License-File: LICENSE.md Requires-Dist:
-docstring_inheritance>=2.1.2 Requires-Dist: click>=8.1.7 Requires-Dist:
-curl_cffi>=0.6.0b7 Requires-Dist: lxml>=5.1.0 Requires-Dist: nest-
-asyncio>=1.6.0 Requires-Dist: selenium>=4.1.3 Requires-Dist: tqdm>=4.64.0
-Requires-Dist: webdriver-manager>=3.5.4 Requires-Dist: halo>=0.0.31 Requires-
+docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
+Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
+tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
 Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
 Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
 Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
 Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist: pytest>=7.4.2; extra
```

### Comparing `webscout-1.4.5/webscout.egg-info/SOURCES.txt` & `webscout-1.4.6/webscout.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 DeepWEBS/networks/google_searcher.py
 DeepWEBS/networks/network_configs.py
 DeepWEBS/networks/webpage_fetcher.py
 DeepWEBS/utilsdw/__init__.py
 DeepWEBS/utilsdw/enver.py
 DeepWEBS/utilsdw/logger.py
 webscout/AI.py
+webscout/AIauto.py
 webscout/AIbase.py
 webscout/AIutel.py
 webscout/DWEBS.py
 webscout/LLM.py
 webscout/__init__.py
 webscout/__main__.py
 webscout/async_providers.py
```

