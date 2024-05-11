# Comparing `tmp/lmwrapper-0.9.2.0.tar.gz` & `tmp/lmwrapper-0.9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwrapper-0.9.2.0.tar", last modified: Sat May 11 02:05:12 2024, max compression
+gzip compressed data, was "lmwrapper-0.9.2.1.tar", last modified: Sat May 11 02:46:23 2024, max compression
```

## Comparing `lmwrapper-0.9.2.0.tar` & `lmwrapper-0.9.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:05:12.329509 lmwrapper-0.9.2.0/
--rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-11 02:05:12.329199 lmwrapper-0.9.2.0/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.9.2.0/README.md
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:05:12.320548 lmwrapper-0.9.2.0/lmwrapper/
--rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/_TokenStoppingCriteria.py
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     4461 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.0/lmwrapper/abstract_predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/env.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:05:12.323083 lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/
--rw-r--r--   0 dgros      (501) staff       (20)       90 2024-04-29 23:28:16.000000 lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/prediction.py
--rw-r--r--   0 dgros      (501) staff       (20)    41718 2024-05-11 01:30:32.000000 lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)      305 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/utilstorch.py
--rw-r--r--   0 dgros      (501) staff       (20)    27146 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/wrapper.py
--rw-r--r--   0 dgros      (501) staff       (20)     3920 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.0/lmwrapper/interals.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:05:12.323875 lmwrapper-0.9.2.0/lmwrapper/openai_wrapper/
--rw-r--r--   0 dgros      (501) staff       (20)       74 2024-05-01 22:58:02.000000 lmwrapper-0.9.2.0/lmwrapper/openai_wrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)    18567 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.0/lmwrapper/openai_wrapper/wrapper.py
--rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/runtime.py
--rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/secrets_manager.py
--rw-r--r--   0 dgros      (501) staff       (20)    16344 2024-05-11 01:22:44.000000 lmwrapper-0.9.2.0/lmwrapper/structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.9.2.0/lmwrapper/togethertoy.py
--rw-r--r--   0 dgros      (501) staff       (20)     2227 2024-04-06 06:54:30.000000 lmwrapper-0.9.2.0/lmwrapper/utils.py
--rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/lmwrapper/wrapping_config.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:05:12.327976 lmwrapper-0.9.2.0/lmwrapper.egg-info/
--rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-11 02:05:12.000000 lmwrapper-0.9.2.0/lmwrapper.egg-info/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     1044 2024-05-11 02:05:12.000000 lmwrapper-0.9.2.0/lmwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 dgros      (501) staff       (20)        1 2024-05-11 02:05:12.000000 lmwrapper-0.9.2.0/lmwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 dgros      (501) staff       (20)      402 2024-05-11 02:05:12.000000 lmwrapper-0.9.2.0/lmwrapper.egg-info/requires.txt
--rw-r--r--   0 dgros      (501) staff       (20)       10 2024-05-11 02:05:12.000000 lmwrapper-0.9.2.0/lmwrapper.egg-info/top_level.txt
--rw-r--r--   0 dgros      (501) staff       (20)     4823 2024-05-11 01:54:27.000000 lmwrapper-0.9.2.0/pyproject.toml
--rw-r--r--   0 dgros      (501) staff       (20)       38 2024-05-11 02:05:12.329616 lmwrapper-0.9.2.0/setup.cfg
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:05:12.327482 lmwrapper-0.9.2.0/test/
--rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.9.2.0/test/test_caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/test/test_docs.py
--rw-r--r--   0 dgros      (501) staff       (20)    31215 2024-05-02 00:01:14.000000 lmwrapper-0.9.2.0/test/test_huggingface.py
--rw-r--r--   0 dgros      (501) staff       (20)     6266 2024-05-11 01:59:20.000000 lmwrapper-0.9.2.0/test/test_huggingface_internals.py
--rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.9.2.0/test/test_huggingface_memory.py
--rw-r--r--   0 dgros      (501) staff       (20)    18789 2024-05-11 01:40:49.000000 lmwrapper-0.9.2.0/test/test_models_common.py
--rw-r--r--   0 dgros      (501) staff       (20)    10394 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.0/test/test_openai.py
--rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.0/test/test_prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.9.2.0/test/test_structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.9.2.0/test/test_util.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:46:23.845472 lmwrapper-0.9.2.1/
+-rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-11 02:46:23.845142 lmwrapper-0.9.2.1/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.9.2.1/README.md
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:46:23.836627 lmwrapper-0.9.2.1/lmwrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/_TokenStoppingCriteria.py
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4461 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.1/lmwrapper/abstract_predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/env.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:46:23.839335 lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)       90 2024-04-29 23:28:16.000000 lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/prediction.py
+-rw-r--r--   0 dgros      (501) staff       (20)    41718 2024-05-11 01:30:32.000000 lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)      305 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/utilstorch.py
+-rw-r--r--   0 dgros      (501) staff       (20)    27146 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3920 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.1/lmwrapper/interals.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:46:23.840213 lmwrapper-0.9.2.1/lmwrapper/openai_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)       74 2024-05-01 22:58:02.000000 lmwrapper-0.9.2.1/lmwrapper/openai_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18567 2024-04-29 22:31:00.000000 lmwrapper-0.9.2.1/lmwrapper/openai_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/runtime.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/secrets_manager.py
+-rw-r--r--   0 dgros      (501) staff       (20)    16344 2024-05-11 01:22:44.000000 lmwrapper-0.9.2.1/lmwrapper/structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.9.2.1/lmwrapper/togethertoy.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2227 2024-04-06 06:54:30.000000 lmwrapper-0.9.2.1/lmwrapper/utils.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/lmwrapper/wrapping_config.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:46:23.843794 lmwrapper-0.9.2.1/lmwrapper.egg-info/
+-rw-r--r--   0 dgros      (501) staff       (20)     6653 2024-05-11 02:46:23.000000 lmwrapper-0.9.2.1/lmwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     1044 2024-05-11 02:46:23.000000 lmwrapper-0.9.2.1/lmwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 dgros      (501) staff       (20)        1 2024-05-11 02:46:23.000000 lmwrapper-0.9.2.1/lmwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 dgros      (501) staff       (20)      402 2024-05-11 02:46:23.000000 lmwrapper-0.9.2.1/lmwrapper.egg-info/requires.txt
+-rw-r--r--   0 dgros      (501) staff       (20)       10 2024-05-11 02:46:23.000000 lmwrapper-0.9.2.1/lmwrapper.egg-info/top_level.txt
+-rw-r--r--   0 dgros      (501) staff       (20)     4823 2024-05-11 02:45:34.000000 lmwrapper-0.9.2.1/pyproject.toml
+-rw-r--r--   0 dgros      (501) staff       (20)       38 2024-05-11 02:46:23.845529 lmwrapper-0.9.2.1/setup.cfg
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-11 02:46:23.843286 lmwrapper-0.9.2.1/test/
+-rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.9.2.1/test/test_caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/test/test_docs.py
+-rw-r--r--   0 dgros      (501) staff       (20)    31215 2024-05-02 00:01:14.000000 lmwrapper-0.9.2.1/test/test_huggingface.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6266 2024-05-11 01:59:20.000000 lmwrapper-0.9.2.1/test/test_huggingface_internals.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.9.2.1/test/test_huggingface_memory.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18789 2024-05-11 01:40:49.000000 lmwrapper-0.9.2.1/test/test_models_common.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10394 2024-05-11 02:18:18.000000 lmwrapper-0.9.2.1/test/test_openai.py
+-rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.9.2.1/test/test_prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.9.2.1/test/test_structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.9.2.1/test/test_util.py
```

### Comparing `lmwrapper-0.9.2.0/PKG-INFO` & `lmwrapper-0.9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.9.2.0
+Version: 0.9.2.1
 Summary: Wrapper around language model APIs
 Author: David Gros, Claudio Spiess
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lmwrapper-0.9.2.0/README.md` & `lmwrapper-0.9.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/_TokenStoppingCriteria.py` & `lmwrapper-0.9.2.1/lmwrapper/_TokenStoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/abstract_predictor.py` & `lmwrapper-0.9.2.1/lmwrapper/abstract_predictor.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/caching.py` & `lmwrapper-0.9.2.1/lmwrapper/caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/prediction.py` & `lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/prediction.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/predictor.py` & `lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/predictor.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/huggingface_wrapper/wrapper.py` & `lmwrapper-0.9.2.1/lmwrapper/huggingface_wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/interals.py` & `lmwrapper-0.9.2.1/lmwrapper/interals.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/openai_wrapper/wrapper.py` & `lmwrapper-0.9.2.1/lmwrapper/openai_wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/prompt_trimming.py` & `lmwrapper-0.9.2.1/lmwrapper/prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/runtime.py` & `lmwrapper-0.9.2.1/lmwrapper/runtime.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/secrets_manager.py` & `lmwrapper-0.9.2.1/lmwrapper/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/structs.py` & `lmwrapper-0.9.2.1/lmwrapper/structs.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/togethertoy.py` & `lmwrapper-0.9.2.1/lmwrapper/togethertoy.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/utils.py` & `lmwrapper-0.9.2.1/lmwrapper/utils.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper/wrapping_config.py` & `lmwrapper-0.9.2.1/lmwrapper/wrapping_config.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/lmwrapper.egg-info/PKG-INFO` & `lmwrapper-0.9.2.1/lmwrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.9.2.0
+Version: 0.9.2.1
 Summary: Wrapper around language model APIs
 Author: David Gros, Claudio Spiess
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lmwrapper-0.9.2.0/lmwrapper.egg-info/SOURCES.txt` & `lmwrapper-0.9.2.1/lmwrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/pyproject.toml` & `lmwrapper-0.9.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["lmwrapper*"]
 
 [project]
 name = "lmwrapper"
-version = "0.9.2.0"
+version = "0.9.2.1"
 authors = [
     { name = "David Gros" },
     { name = "Claudio Spiess" },
 ]
 description = "Wrapper around language model APIs"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lmwrapper-0.9.2.0/test/test_caching.py` & `lmwrapper-0.9.2.1/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_docs.py` & `lmwrapper-0.9.2.1/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_huggingface.py` & `lmwrapper-0.9.2.1/test/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_huggingface_internals.py` & `lmwrapper-0.9.2.1/test/test_huggingface_internals.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_huggingface_memory.py` & `lmwrapper-0.9.2.1/test/test_huggingface_memory.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_models_common.py` & `lmwrapper-0.9.2.1/test/test_models_common.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_openai.py` & `lmwrapper-0.9.2.1/test/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,20 +174,20 @@
     assert out.completion_text.strip() == "5."
 
     # even at t=0, the logprobs have high variance
     # perhaps anti-reverse engineering measures?
 
     assert out.top_token_logprobs == [
         {
-            "5": pytest.approx(-0.00012689977, abs=2),
-            "The": pytest.approx(-9.452922, abs=2),
+            "5": pytest.approx(-0.00012689977, abs=4),
+            "The": pytest.approx(-9.452922, abs=4),
         },
         {
-            ".": pytest.approx(-4.2391708e-05, abs=2),
-            "<|end|>": pytest.approx(-10.109505, abs=2),
+            ".": pytest.approx(-4.2391708e-05, abs=4),
+            "<|end|>": pytest.approx(-10.109505, abs=4),
         },
     ]
 
 
 def test_ratelimit():
     try:
         OpenAIPredictor.configure_global_ratelimit(1, per_seconds=2)
```

### Comparing `lmwrapper-0.9.2.0/test/test_prompt_trimming.py` & `lmwrapper-0.9.2.1/test/test_prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.9.2.0/test/test_structs.py` & `lmwrapper-0.9.2.1/test/test_structs.py`

 * *Files identical despite different names*

