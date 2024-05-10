# Comparing `tmp/api4all-0.3.1.tar.gz` & `tmp/api4all-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api4all-0.3.1.tar", last modified: Sun Mar 17 03:59:50 2024, max compression
+gzip compressed data, was "api4all-0.4.0.tar", last modified: Fri May 10 22:49:06 2024, max compression
```

## Comparing `api4all-0.3.1.tar` & `api4all-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.775973 api4all-0.3.1/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1073 2024-03-07 01:55:49.000000 api4all-0.3.1/LICENSE
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)    11382 2024-03-17 03:59:50.775428 api4all-0.3.1/PKG-INFO
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     9008 2024-03-17 03:59:22.000000 api4all-0.3.1/README.md
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.767484 api4all-0.3.1/api4all/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      111 2024-03-15 04:22:31.000000 api4all-0.3.1/api4all/__init__.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     4166 2024-03-15 04:41:57.000000 api4all-0.3.1/api4all/base.py
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.770470 api4all-0.3.1/api4all/data/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)       54 2024-03-15 03:36:25.000000 api4all-0.3.1/api4all/data/__init__.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)    12516 2024-03-17 02:56:36.000000 api4all-0.3.1/api4all/data/constant_data.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     3284 2024-03-15 03:46:13.000000 api4all-0.3.1/api4all/data/data.py
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.771563 api4all-0.3.1/api4all/engines/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)       86 2024-03-15 16:08:05.000000 api4all-0.3.1/api4all/engines/__init__.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)    33040 2024-03-17 00:38:53.000000 api4all-0.3.1/api4all/engines/engines.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      700 2024-03-15 03:34:56.000000 api4all-0.3.1/api4all/engines/factory.py
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.772249 api4all-0.3.1/api4all/examples/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     2321 2024-03-16 19:37:00.000000 api4all-0.3.1/api4all/examples/quick-start-with-env-file.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     2446 2024-03-16 19:41:31.000000 api4all-0.3.1/api4all/examples/quick-start.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1633 2024-03-15 21:10:44.000000 api4all-0.3.1/api4all/keys.py
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.772935 api4all-0.3.1/api4all/logger/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)       65 2024-03-15 03:37:16.000000 api4all-0.3.1/api4all/logger/__init__.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1689 2024-03-15 16:30:59.000000 api4all-0.3.1/api4all/logger/base_logger.py
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.774267 api4all-0.3.1/api4all/utils/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      104 2024-03-15 03:37:46.000000 api4all-0.3.1/api4all/utils/__init__.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      636 2024-03-13 03:44:52.000000 api4all-0.3.1/api4all/utils/configs.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      210 2024-03-13 02:52:39.000000 api4all-0.3.1/api4all/utils/models.py
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)        0 2024-03-15 03:32:15.000000 api4all-0.3.1/api4all/utils/utils.py
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.774880 api4all-0.3.1/api4all.egg-info/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)    11382 2024-03-17 03:59:50.000000 api4all-0.3.1/api4all.egg-info/PKG-INFO
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      660 2024-03-17 03:59:50.000000 api4all-0.3.1/api4all.egg-info/SOURCES.txt
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)        1 2024-03-17 03:59:50.000000 api4all-0.3.1/api4all.egg-info/dependency_links.txt
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      166 2024-03-17 03:59:50.000000 api4all-0.3.1/api4all.egg-info/requires.txt
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)        8 2024-03-17 03:59:50.000000 api4all-0.3.1/api4all.egg-info/top_level.txt
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1213 2024-03-17 03:41:57.000000 api4all-0.3.1/pyproject.toml
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)      182 2024-03-16 16:43:33.000000 api4all-0.3.1/requirements.txt
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)       38 2024-03-17 03:59:50.776077 api4all-0.3.1/setup.cfg
-drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:59:50.774531 api4all-0.3.1/tests/
--rw-r--r--   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:58:17.000000 api4all-0.3.1/tests/test.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.502591 api4all-0.4.0/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1073 2024-03-07 01:55:49.000000 api4all-0.4.0/LICENSE
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)    11767 2024-05-10 22:49:06.501916 api4all-0.4.0/PKG-INFO
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     9393 2024-05-10 22:47:34.000000 api4all-0.4.0/README.md
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.486982 api4all-0.4.0/api4all/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      111 2024-03-15 04:22:31.000000 api4all-0.4.0/api4all/__init__.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     4166 2024-03-15 04:41:57.000000 api4all-0.4.0/api4all/base.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.491195 api4all-0.4.0/api4all/data/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)       54 2024-03-15 03:36:25.000000 api4all-0.4.0/api4all/data/__init__.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)    15585 2024-05-10 22:43:29.000000 api4all-0.4.0/api4all/data/constant_data.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     3284 2024-03-15 03:46:13.000000 api4all-0.4.0/api4all/data/data.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.494424 api4all-0.4.0/api4all/engines/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)       86 2024-03-15 16:08:05.000000 api4all-0.4.0/api4all/engines/__init__.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)    33040 2024-03-17 00:38:53.000000 api4all-0.4.0/api4all/engines/engines.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      700 2024-03-15 03:34:56.000000 api4all-0.4.0/api4all/engines/factory.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.495911 api4all-0.4.0/api4all/examples/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     2321 2024-03-16 19:37:00.000000 api4all-0.4.0/api4all/examples/quick-start-with-env-file.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     2446 2024-03-16 19:41:31.000000 api4all-0.4.0/api4all/examples/quick-start.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1633 2024-03-15 21:10:44.000000 api4all-0.4.0/api4all/keys.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.497327 api4all-0.4.0/api4all/logger/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)       65 2024-03-15 03:37:16.000000 api4all-0.4.0/api4all/logger/__init__.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1689 2024-03-15 16:30:59.000000 api4all-0.4.0/api4all/logger/base_logger.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.500302 api4all-0.4.0/api4all/utils/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      104 2024-03-15 03:37:46.000000 api4all-0.4.0/api4all/utils/__init__.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      636 2024-03-13 03:44:52.000000 api4all-0.4.0/api4all/utils/configs.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      210 2024-03-13 02:52:39.000000 api4all-0.4.0/api4all/utils/models.py
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)        0 2024-03-15 03:32:15.000000 api4all-0.4.0/api4all/utils/utils.py
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.501186 api4all-0.4.0/api4all.egg-info/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)    11767 2024-05-10 22:49:06.000000 api4all-0.4.0/api4all.egg-info/PKG-INFO
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      660 2024-05-10 22:49:06.000000 api4all-0.4.0/api4all.egg-info/SOURCES.txt
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)        1 2024-05-10 22:49:06.000000 api4all-0.4.0/api4all.egg-info/dependency_links.txt
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      166 2024-05-10 22:49:06.000000 api4all-0.4.0/api4all.egg-info/requires.txt
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)        8 2024-05-10 22:49:06.000000 api4all-0.4.0/api4all.egg-info/top_level.txt
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)     1213 2024-05-10 22:48:36.000000 api4all-0.4.0/pyproject.toml
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)      182 2024-03-16 16:43:33.000000 api4all-0.4.0/requirements.txt
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)       38 2024-05-10 22:49:06.502703 api4all-0.4.0/setup.cfg
+drwxr-xr-x   0 hieunguyenminh   (501) staff       (20)        0 2024-05-10 22:49:06.500793 api4all-0.4.0/tests/
+-rw-r--r--   0 hieunguyenminh   (501) staff       (20)        0 2024-03-17 03:58:17.000000 api4all-0.4.0/tests/test.py
```

### Comparing `api4all-0.3.1/LICENSE` & `api4all-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/PKG-INFO` & `api4all-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api4all
-Version: 0.3.1
+Version: 0.4.0
 Summary: Easy-to-use LLM API from a state-of-the-art provider and comparison
 Author-email: Hieu Nguyen <hieung.tech@gmail.com>
 Maintainer-email: Hieu Nguyen <hieung.tech@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Hieu Minh Nguyen
         
@@ -44,15 +44,15 @@
 Requires-Dist: mistralai==0.1.6
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: replicate==0.24.0
 Requires-Dist: together==0.2.11
 Requires-Dist: google-generativeai==0.4.1
 
 # api4all
-Easy-to-use LLM API from a state-of-the-art provider and comparison.
+Easy-to-use LLM API from state-of-the-art providers and comparison.
 
 ## Features
 - **Easy-to-use**: A simple and easy-to-use API for state-of-the-art language models from different providers but using in a same way.
 - **Comparison**: Compare the cost and performance of different providers and models. Let you choose the best provider and model for your use case.
 - **Log**: Log the response and cost of the request in a log file.
 - **Providers**: Support for all of providers both open-source and closed-source.
 - **Result**: See the actual time taken by the request, especially when you dont't trust the benchmark.
@@ -155,27 +155,27 @@
 |  [Anthropic](https://www.anthropic.com)    |     Free to try     | 5 Requests / Minute | ANTHROPIC_API_KEY | "anthropic"  |
 
 
 - **Free to try**: Free to try, no credit card required but limited to a certain number of tokens.
 - Rate limit is based on the free plan of the provider. The actual rate limit may be different based on the plan you choose.
 
 ### Open-source models
-  -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it |  Mistral-7B-Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct
-|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
-|  API string name          |     "mistralai/Mixtral-8x7B-Instruct-v0.1"    | "google/gemma-7b-it"    | "mistralai/Mistral-7B-Instruct-v0.1"  | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" |
-|  Context Length          |     32,768    | 8.192    |  4,096 | 4,096 | 32,768
-|  Developer          |     Mistral AI    | Google    |  Mistral AI | Meta
-|  **Cost (Input - Output / MTokens)**          |     -----    | ------    | ------ | -----
-|  [Groq](https://wow.groq.com)          |     $0-$0    | $0-$0    | &#x2715; | $0-$0 | &#x2715; | &#x2715;
-|  [Anyscale](https://www.anyscale.com)  |     $0.5-$0.5       | $0.15-$0.15       |  $0.05-$0.25 | $1.0-$1.0 | &#x2715; | $1.0-$1.0
-|  [Together AI](https://www.together.ai)|     $0.6-$0.6        | $0.2-$0.2        | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9
-|  [Replicate](https://replicate.com)    |     $0.3-$1       | &#x2715;       |  $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75
-|  [Fireworks](https://fireworks.ai)     |     $0.5-$0.5        | &#x2715;        |  $0.2-$0.2  | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
-|  [Deepinfra](https://deepinfra.com)    |     $0.27-$0.27    | $0.13-$0.13    |   $0.13-$0.13 | $0.7-$0.9 | &#x2715; | $0.7-$0.9
-|  [Lepton](https://www.lepton.ai)    |     $0.5-$0.5    | &#x2715;    |   &#x2715; | $0.8-$0.8 | &#x2715; | &#x2715; 
+  -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it |  Mistral-7B-Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct | LLaMA3-8b-Instruct | LLaMA3-80b
+|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
+|  API string name          |     "mistralai/Mixtral-8x7B-Instruct-v0.1"    | "google/gemma-7b-it"    | "mistralai/Mistral-7B-Instruct-v0.1"  | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" | "meta/Llama-3-8b-Instruct" | "meta/Llama-3-80b"
+|  Context Length          |     32,768    | 8.192    |  4,096 | 4,096 | 32,768 | 16,384 | 8,192 | 8,192
+|  Developer          |     Mistral AI    | Google    |  Mistral AI | Meta | Mistral AI | Meta | Meta | Meta
+|  **Cost (Input - Output / MTokens)**          |     -----    | ------    | ------ | ----- | ------ | ------ | ------ | ------ | ------ | ------ |
+|  [Groq](https://wow.groq.com)          |     $0-$0    | $0-$0    | &#x2715; | $0-$0 | &#x2715; | &#x2715; | $0-$0 | $0-$0
+|  [Anyscale](https://www.anyscale.com)  |     $0.5-$0.5       | $0.15-$0.15       |  $0.05-$0.25 | $1.0-$1.0 | &#x2715; | $1.0-$1.0 | $0.15-$0.15 | $1.0-$1.0
+|  [Together AI](https://www.together.ai)|     $0.6-$0.6        | $0.2-$0.2        | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
+|  [Replicate](https://replicate.com)    |     $0.3-$1       | &#x2715;       |  $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75 | $0.05-$0.25 | $0.65-$2.75
+|  [Fireworks](https://fireworks.ai)     |     $0.5-$0.5        | &#x2715;        |  $0.2-$0.2  | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
+|  [Deepinfra](https://deepinfra.com)    |     $0.27-$0.27    | $0.13-$0.13    |   $0.13-$0.13 | $0.7-$0.9 | &#x2715; | $0.7-$0.9 | $0.08-$0.08 | $0.59-$0.79
+|  [Lepton](https://www.lepton.ai)    |     $0.5-$0.5    | &#x2715;    |   &#x2715; | $0.8-$0.8 | &#x2715; | &#x2715; | $0.07-$0.07 | $0.8-$0.8
 
 ### Closed-source models
 #### 1. Mistral AI
 
 | Model | Input Pricing ($/1M Tokens) | Output Pricing ($/1M Tokens) | Context Length | API string name |
 |:------:|:------:|:------:|:------:|:------:|
 |  Mistral-7B-Instruct-v0.1          |     $0.25        | $0.25    |  8,192 | "mistral/open-mistral-7b" |
```

### Comparing `api4all-0.3.1/README.md` & `api4all-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # api4all
-Easy-to-use LLM API from a state-of-the-art provider and comparison.
+Easy-to-use LLM API from state-of-the-art providers and comparison.
 
 ## Features
 - **Easy-to-use**: A simple and easy-to-use API for state-of-the-art language models from different providers but using in a same way.
 - **Comparison**: Compare the cost and performance of different providers and models. Let you choose the best provider and model for your use case.
 - **Log**: Log the response and cost of the request in a log file.
 - **Providers**: Support for all of providers both open-source and closed-source.
 - **Result**: See the actual time taken by the request, especially when you dont't trust the benchmark.
@@ -106,27 +106,27 @@
 |  [Anthropic](https://www.anthropic.com)    |     Free to try     | 5 Requests / Minute | ANTHROPIC_API_KEY | "anthropic"  |
 
 
 - **Free to try**: Free to try, no credit card required but limited to a certain number of tokens.
 - Rate limit is based on the free plan of the provider. The actual rate limit may be different based on the plan you choose.
 
 ### Open-source models
-  -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it |  Mistral-7B-Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct
-|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
-|  API string name          |     "mistralai/Mixtral-8x7B-Instruct-v0.1"    | "google/gemma-7b-it"    | "mistralai/Mistral-7B-Instruct-v0.1"  | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" |
-|  Context Length          |     32,768    | 8.192    |  4,096 | 4,096 | 32,768
-|  Developer          |     Mistral AI    | Google    |  Mistral AI | Meta
-|  **Cost (Input - Output / MTokens)**          |     -----    | ------    | ------ | -----
-|  [Groq](https://wow.groq.com)          |     $0-$0    | $0-$0    | &#x2715; | $0-$0 | &#x2715; | &#x2715;
-|  [Anyscale](https://www.anyscale.com)  |     $0.5-$0.5       | $0.15-$0.15       |  $0.05-$0.25 | $1.0-$1.0 | &#x2715; | $1.0-$1.0
-|  [Together AI](https://www.together.ai)|     $0.6-$0.6        | $0.2-$0.2        | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9
-|  [Replicate](https://replicate.com)    |     $0.3-$1       | &#x2715;       |  $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75
-|  [Fireworks](https://fireworks.ai)     |     $0.5-$0.5        | &#x2715;        |  $0.2-$0.2  | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
-|  [Deepinfra](https://deepinfra.com)    |     $0.27-$0.27    | $0.13-$0.13    |   $0.13-$0.13 | $0.7-$0.9 | &#x2715; | $0.7-$0.9
-|  [Lepton](https://www.lepton.ai)    |     $0.5-$0.5    | &#x2715;    |   &#x2715; | $0.8-$0.8 | &#x2715; | &#x2715; 
+  -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it |  Mistral-7B-Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct | LLaMA3-8b-Instruct | LLaMA3-80b
+|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
+|  API string name          |     "mistralai/Mixtral-8x7B-Instruct-v0.1"    | "google/gemma-7b-it"    | "mistralai/Mistral-7B-Instruct-v0.1"  | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" | "meta/Llama-3-8b-Instruct" | "meta/Llama-3-80b"
+|  Context Length          |     32,768    | 8.192    |  4,096 | 4,096 | 32,768 | 16,384 | 8,192 | 8,192
+|  Developer          |     Mistral AI    | Google    |  Mistral AI | Meta | Mistral AI | Meta | Meta | Meta
+|  **Cost (Input - Output / MTokens)**          |     -----    | ------    | ------ | ----- | ------ | ------ | ------ | ------ | ------ | ------ |
+|  [Groq](https://wow.groq.com)          |     $0-$0    | $0-$0    | &#x2715; | $0-$0 | &#x2715; | &#x2715; | $0-$0 | $0-$0
+|  [Anyscale](https://www.anyscale.com)  |     $0.5-$0.5       | $0.15-$0.15       |  $0.05-$0.25 | $1.0-$1.0 | &#x2715; | $1.0-$1.0 | $0.15-$0.15 | $1.0-$1.0
+|  [Together AI](https://www.together.ai)|     $0.6-$0.6        | $0.2-$0.2        | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
+|  [Replicate](https://replicate.com)    |     $0.3-$1       | &#x2715;       |  $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75 | $0.05-$0.25 | $0.65-$2.75
+|  [Fireworks](https://fireworks.ai)     |     $0.5-$0.5        | &#x2715;        |  $0.2-$0.2  | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
+|  [Deepinfra](https://deepinfra.com)    |     $0.27-$0.27    | $0.13-$0.13    |   $0.13-$0.13 | $0.7-$0.9 | &#x2715; | $0.7-$0.9 | $0.08-$0.08 | $0.59-$0.79
+|  [Lepton](https://www.lepton.ai)    |     $0.5-$0.5    | &#x2715;    |   &#x2715; | $0.8-$0.8 | &#x2715; | &#x2715; | $0.07-$0.07 | $0.8-$0.8
 
 ### Closed-source models
 #### 1. Mistral AI
 
 | Model | Input Pricing ($/1M Tokens) | Output Pricing ($/1M Tokens) | Context Length | API string name |
 |:------:|:------:|:------:|:------:|:------:|
 |  Mistral-7B-Instruct-v0.1          |     $0.25        | $0.25    |  8,192 | "mistral/open-mistral-7b" |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# api4all Easy-to-use LLM API from a state-of-the-art provider and comparison.
+# api4all Easy-to-use LLM API from state-of-the-art providers and comparison.
 ## Features - **Easy-to-use**: A simple and easy-to-use API for state-of-the-
 art language models from different providers but using in a same way. -
 **Comparison**: Compare the cost and performance of different providers and
 models. Let you choose the best provider and model for your use case. -
 **Log**: Log the response and cost of the request in a log file. -
 **Providers**: Support for all of providers both open-source and closed-source.
 - **Result**: See the actual time taken by the request, especially when you
@@ -50,29 +50,34 @@
 Second | MISTRAL_API_KEY | "mistral" | | [Anthropic](https://www.anthropic.com)
 | Free to try | 5 Requests / Minute | ANTHROPIC_API_KEY | "anthropic" | -
 **Free to try**: Free to try, no credit card required but limited to a certain
 number of tokens. - Rate limit is based on the free plan of the provider. The
 actual rate limit may be different based on the plan you choose. ### Open-
 source models -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it | Mistral-7B-
 Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct
-|:------:|:------:|:------:|:------:|:------:|:------:|:------:| | API string
-name | "mistralai/Mixtral-8x7B-Instruct-v0.1" | "google/gemma-7b-it" |
-"mistralai/Mistral-7B-Instruct-v0.1" | "meta/Llama-2-70b-chat" | "mistralai/
-Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" | | Context Length |
-32,768 | 8.192 | 4,096 | 4,096 | 32,768 | Developer | Mistral AI | Google |
-Mistral AI | Meta | **Cost (Input - Output / MTokens)** | ----- | ------ | ----
--- | ----- | [Groq](https://wow.groq.com) | $0-$0 | $0-$0 | ✕ | $0-$0 | ✕ | ✕ |
-[Anyscale](https://www.anyscale.com) | $0.5-$0.5 | $0.15-$0.15 | $0.05-$0.25 |
-$1.0-$1.0 | ✕ | $1.0-$1.0 | [Together AI](https://www.together.ai)| $0.6-$0.6 |
-$0.2-$0.2 | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9 | [Replicate]
-(https://replicate.com) | $0.3-$1 | ✕ | $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 |
+| LLaMA3-8b-Instruct | LLaMA3-80b |:------:|:------:|:------:|:------:|:------:
+|:------:|:------:|:------:|:------:| | API string name | "mistralai/Mixtral-
+8x7B-Instruct-v0.1" | "google/gemma-7b-it" | "mistralai/Mistral-7B-Instruct-
+v0.1" | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/
+CodeLlama-2-70b-intruct" | "meta/Llama-3-8b-Instruct" | "meta/Llama-3-80b" |
+Context Length | 32,768 | 8.192 | 4,096 | 4,096 | 32,768 | 16,384 | 8,192 |
+8,192 | Developer | Mistral AI | Google | Mistral AI | Meta | Mistral AI | Meta
+| Meta | Meta | **Cost (Input - Output / MTokens)** | ----- | ------ | ------ |
+----- | ------ | ------ | ------ | ------ | ------ | ------ | | [Groq](https://
+wow.groq.com) | $0-$0 | $0-$0 | ✕ | $0-$0 | ✕ | ✕ | $0-$0 | $0-$0 | [Anyscale]
+(https://www.anyscale.com) | $0.5-$0.5 | $0.15-$0.15 | $0.05-$0.25 | $1.0-$1.0
+| ✕ | $1.0-$1.0 | $0.15-$0.15 | $1.0-$1.0 | [Together AI](https://
+www.together.ai)| $0.6-$0.6 | $0.2-$0.2 | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 |
+$0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | [Replicate](https://replicate.com) | $0.3-
+$1 | ✕ | $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75 | $0.05-$0.25 |
 $0.65-$2.75 | [Fireworks](https://fireworks.ai) | $0.5-$0.5 | ✕ | $0.2-$0.2 |
-$0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | [Deepinfra](https://deepinfra.com) | $0.27-
-$0.27 | $0.13-$0.13 | $0.13-$0.13 | $0.7-$0.9 | ✕ | $0.7-$0.9 | [Lepton](https:
-//www.lepton.ai) | $0.5-$0.5 | ✕ | ✕ | $0.8-$0.8 | ✕ | ✕ ### Closed-source
+$0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | [Deepinfra](https:/
+/deepinfra.com) | $0.27-$0.27 | $0.13-$0.13 | $0.13-$0.13 | $0.7-$0.9 | ✕ |
+$0.7-$0.9 | $0.08-$0.08 | $0.59-$0.79 | [Lepton](https://www.lepton.ai) | $0.5-
+$0.5 | ✕ | ✕ | $0.8-$0.8 | ✕ | ✕ | $0.07-$0.07 | $0.8-$0.8 ### Closed-source
 models #### 1. Mistral AI | Model | Input Pricing ($/1M Tokens) | Output
 Pricing ($/1M Tokens) | Context Length | API string name | |:------:|:------:|:
 ------:|:------:|:------:| | Mistral-7B-Instruct-v0.1 | $0.25 | $0.25 | 8,192 |
 "mistral/open-mistral-7b" | | Mixtral-8x7b-Instruct-v0.1 | $0.7 | $0.7 | 8,192
 | "mistral/open-mixtral-8x7b" | | Mixtral Small | $2 | $6 | ✕ | "mistral/
 mistral-small-latest" | | Mixtral Medium | $2.7 | $8.1 | ✕ | "mistral/mistral-
 medium-latest" | | Mixtral Large | $8 | $24 | ✕ | "mistral/mistral-large-
```

### Comparing `api4all-0.3.1/api4all/base.py` & `api4all-0.4.0/api4all/base.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/data/constant_data.py` & `api4all-0.4.0/api4all/data/constant_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -448,8 +448,116 @@
                     "input": 0.2,
                     "output": 0.2
                 }
             }
         },
         "context-length": 32768
     },
+    "meta/Llama-3-8b-Instruct": {
+        "provider": {
+            "anyscale": {
+                "name": "meta-llama/Meta-Llama-3-8B-Instruct",
+                "price": {
+                    "input": 0.15,
+                    "output": 0.15
+                }
+            },
+            "groq": {
+                "name": "llama3-8b-8192",
+                "price": {
+                    "input": 0,
+                    "output": 0
+                }
+            },
+            "together": {
+                "name": "meta-llama/Llama-3-8b-chat-hf",
+                "price": {
+                    "input": 0.2,
+                    "output": 0.2
+                }
+            },
+            "replicate": {
+                "name": "meta/meta-llama-3-8b",
+                "price": {
+                    "input": 0.05,
+                    "output": 0.25
+                }
+            },
+            "fireworks": {
+                "name": "llama-v3-8b-instruct",
+                "price": {
+                    "input": 0.2,
+                    "output": 0.2
+                }
+            },
+            "deepinfra": {
+                "name": "meta-llama/Meta-Llama-3-8B-Instruct",
+                "price": {
+                    "input": 0.08,
+                    "output": 0.08
+                }
+            },
+            "lepton": {
+                "name": "llama3-8b",
+                "price": {
+                    "input": 0.07,
+                    "output": 0.07
+                }
+            }
+        },
+        "context-length": 8192
+    },
+    "meta/Llama-3-80b": {
+        "provider": {
+            "anyscale": {
+                "name": "meta-llama/Meta-Llama-3-70B-Instruct",
+                "price": {
+                    "input": 1,
+                    "output": 1
+                }
+            },
+            "groq": {
+                "name": "llama3-70b-8192",
+                "price": {
+                    "input": 0,
+                    "output": 0
+                }
+            },
+            "together": {
+                "name": "meta-llama/Llama-3-70b-chat-hf",
+                "price": {
+                    "input": 0.9,
+                    "output": 0.9
+                }
+            },
+            "replicate": {
+                "name": "meta/meta-llama-3-70b",
+                "price": {
+                    "input": 0.65,
+                    "output": 2.75
+                }
+            },
+            "fireworks": {
+                "name": "llama-v3-70b-chat",
+                "price": {
+                    "input": 0.9,
+                    "output": 0.9
+                }
+            },
+            "deepinfra": {
+                "name": "meta-llama/Meta-Llama-3-70B-Instruct",
+                "price": {
+                    "input": 0.59,
+                    "output": 0.79
+                }
+            },
+            "lepton": {
+                "name": "llama3-70b",
+                "price": {
+                    "input": 0.8,
+                    "output": 0.8
+                }
+            }
+        },
+        "context-length": 8192
+    },
 }
```

### Comparing `api4all-0.3.1/api4all/data/data.py` & `api4all-0.4.0/api4all/data/data.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/engines/engines.py` & `api4all-0.4.0/api4all/engines/engines.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/engines/factory.py` & `api4all-0.4.0/api4all/engines/factory.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/examples/quick-start-with-env-file.py` & `api4all-0.4.0/api4all/examples/quick-start-with-env-file.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/examples/quick-start.py` & `api4all-0.4.0/api4all/examples/quick-start.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/keys.py` & `api4all-0.4.0/api4all/keys.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/logger/base_logger.py` & `api4all-0.4.0/api4all/logger/base_logger.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all/utils/configs.py` & `api4all-0.4.0/api4all/utils/configs.py`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/api4all.egg-info/PKG-INFO` & `api4all-0.4.0/api4all.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api4all
-Version: 0.3.1
+Version: 0.4.0
 Summary: Easy-to-use LLM API from a state-of-the-art provider and comparison
 Author-email: Hieu Nguyen <hieung.tech@gmail.com>
 Maintainer-email: Hieu Nguyen <hieung.tech@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Hieu Minh Nguyen
         
@@ -44,15 +44,15 @@
 Requires-Dist: mistralai==0.1.6
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: replicate==0.24.0
 Requires-Dist: together==0.2.11
 Requires-Dist: google-generativeai==0.4.1
 
 # api4all
-Easy-to-use LLM API from a state-of-the-art provider and comparison.
+Easy-to-use LLM API from state-of-the-art providers and comparison.
 
 ## Features
 - **Easy-to-use**: A simple and easy-to-use API for state-of-the-art language models from different providers but using in a same way.
 - **Comparison**: Compare the cost and performance of different providers and models. Let you choose the best provider and model for your use case.
 - **Log**: Log the response and cost of the request in a log file.
 - **Providers**: Support for all of providers both open-source and closed-source.
 - **Result**: See the actual time taken by the request, especially when you dont't trust the benchmark.
@@ -155,27 +155,27 @@
 |  [Anthropic](https://www.anthropic.com)    |     Free to try     | 5 Requests / Minute | ANTHROPIC_API_KEY | "anthropic"  |
 
 
 - **Free to try**: Free to try, no credit card required but limited to a certain number of tokens.
 - Rate limit is based on the free plan of the provider. The actual rate limit may be different based on the plan you choose.
 
 ### Open-source models
-  -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it |  Mistral-7B-Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct
-|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
-|  API string name          |     "mistralai/Mixtral-8x7B-Instruct-v0.1"    | "google/gemma-7b-it"    | "mistralai/Mistral-7B-Instruct-v0.1"  | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" |
-|  Context Length          |     32,768    | 8.192    |  4,096 | 4,096 | 32,768
-|  Developer          |     Mistral AI    | Google    |  Mistral AI | Meta
-|  **Cost (Input - Output / MTokens)**          |     -----    | ------    | ------ | -----
-|  [Groq](https://wow.groq.com)          |     $0-$0    | $0-$0    | &#x2715; | $0-$0 | &#x2715; | &#x2715;
-|  [Anyscale](https://www.anyscale.com)  |     $0.5-$0.5       | $0.15-$0.15       |  $0.05-$0.25 | $1.0-$1.0 | &#x2715; | $1.0-$1.0
-|  [Together AI](https://www.together.ai)|     $0.6-$0.6        | $0.2-$0.2        | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9
-|  [Replicate](https://replicate.com)    |     $0.3-$1       | &#x2715;       |  $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75
-|  [Fireworks](https://fireworks.ai)     |     $0.5-$0.5        | &#x2715;        |  $0.2-$0.2  | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
-|  [Deepinfra](https://deepinfra.com)    |     $0.27-$0.27    | $0.13-$0.13    |   $0.13-$0.13 | $0.7-$0.9 | &#x2715; | $0.7-$0.9
-|  [Lepton](https://www.lepton.ai)    |     $0.5-$0.5    | &#x2715;    |   &#x2715; | $0.8-$0.8 | &#x2715; | &#x2715; 
+  -- |Mixtral-8x7b-Instruct-v0.1 | Gemma 7B it |  Mistral-7B-Instruct-v0.1 | LLaMA2-70b | Mistral-7B-Instruct-v0.2 | CodeLlama-70b-Instruct | LLaMA3-8b-Instruct | LLaMA3-80b
+|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|:------:|
+|  API string name          |     "mistralai/Mixtral-8x7B-Instruct-v0.1"    | "google/gemma-7b-it"    | "mistralai/Mistral-7B-Instruct-v0.1"  | "meta/Llama-2-70b-chat" | "mistralai/Mistral-7B-Instruct-v0.2" | "meta/CodeLlama-2-70b-intruct" | "meta/Llama-3-8b-Instruct" | "meta/Llama-3-80b"
+|  Context Length          |     32,768    | 8.192    |  4,096 | 4,096 | 32,768 | 16,384 | 8,192 | 8,192
+|  Developer          |     Mistral AI    | Google    |  Mistral AI | Meta | Mistral AI | Meta | Meta | Meta
+|  **Cost (Input - Output / MTokens)**          |     -----    | ------    | ------ | ----- | ------ | ------ | ------ | ------ | ------ | ------ |
+|  [Groq](https://wow.groq.com)          |     $0-$0    | $0-$0    | &#x2715; | $0-$0 | &#x2715; | &#x2715; | $0-$0 | $0-$0
+|  [Anyscale](https://www.anyscale.com)  |     $0.5-$0.5       | $0.15-$0.15       |  $0.05-$0.25 | $1.0-$1.0 | &#x2715; | $1.0-$1.0 | $0.15-$0.15 | $1.0-$1.0
+|  [Together AI](https://www.together.ai)|     $0.6-$0.6        | $0.2-$0.2        | $0.2-$0.2 | $0.9-$0.9 | $0.05-$0.25 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
+|  [Replicate](https://replicate.com)    |     $0.3-$1       | &#x2715;       |  $0.05-$0.25 | $0.65-$2.75 | $0.2-$0.2 | $0.65-$2.75 | $0.05-$0.25 | $0.65-$2.75
+|  [Fireworks](https://fireworks.ai)     |     $0.5-$0.5        | &#x2715;        |  $0.2-$0.2  | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9 | $0.2-$0.2 | $0.9-$0.9
+|  [Deepinfra](https://deepinfra.com)    |     $0.27-$0.27    | $0.13-$0.13    |   $0.13-$0.13 | $0.7-$0.9 | &#x2715; | $0.7-$0.9 | $0.08-$0.08 | $0.59-$0.79
+|  [Lepton](https://www.lepton.ai)    |     $0.5-$0.5    | &#x2715;    |   &#x2715; | $0.8-$0.8 | &#x2715; | &#x2715; | $0.07-$0.07 | $0.8-$0.8
 
 ### Closed-source models
 #### 1. Mistral AI
 
 | Model | Input Pricing ($/1M Tokens) | Output Pricing ($/1M Tokens) | Context Length | API string name |
 |:------:|:------:|:------:|:------:|:------:|
 |  Mistral-7B-Instruct-v0.1          |     $0.25        | $0.25    |  8,192 | "mistral/open-mistral-7b" |
```

### Comparing `api4all-0.3.1/api4all.egg-info/SOURCES.txt` & `api4all-0.4.0/api4all.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `api4all-0.3.1/pyproject.toml` & `api4all-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "mistralai == 0.1.6",
     "python-dotenv == 1.0.1",
     "replicate == 0.24.0",
     "together == 0.2.11",
     "google-generativeai == 0.4.1",
 ]
 name = "api4all"
-version = "0.3.1"
+version = "0.4.0"
 requires-python = ">=3.8"
 authors = [
   {name = "Hieu Nguyen", email = "hieung.tech@gmail.com"}
 ]
 maintainers = [
   {name = "Hieu Nguyen", email = "hieung.tech@gmail.com"}
 ]
```

