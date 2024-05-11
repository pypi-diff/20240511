# Comparing `tmp/dalpha-0.4.5rc1.tar.gz` & `tmp/dalpha-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.5rc1.tar", max compression
+gzip compressed data, was "dalpha-0.5.0rc0.tar", max compression
```

## Comparing `dalpha-0.4.5rc1.tar` & `dalpha-0.5.0rc0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.5rc1/README.md
--rw-r--r--   0        0        0     1862 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/__init__.py
--rw-r--r--   0        0        0    28968 2024-05-08 06:25:10.211719 dalpha-0.4.5rc1/dalpha/agent.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.4.5rc1/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/dto.py
--rw-r--r--   0        0        0      521 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/exception.py
--rw-r--r--   0        0        0     6098 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.5rc1/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.5rc1/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/logging/utils.py
--rw-r--r--   0        0        0     1702 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.4.5rc1/dalpha/redis_cls.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.5rc1/dalpha/signal_handler.py
--rw-r--r--   0        0        0      881 2024-05-08 06:25:10.211719 dalpha-0.4.5rc1/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.5rc1/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.0rc0/README.md
+-rw-r--r--   0        0        0     1949 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0     8158 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.0rc0/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.0rc0/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.0rc0/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.0rc0/dalpha/dto.py
+-rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/exception.py
+-rw-r--r--   0        0        0     6136 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.0rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.0rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.0rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.0rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.0rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.0rc0/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.0rc0/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.0rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.0rc0/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-10 10:54:52.516415 dalpha-0.5.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.0rc0/PKG-INFO
```

### Comparing `dalpha-0.4.5rc1/README.md` & `dalpha-0.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/__init__.py` & `dalpha-0.5.0rc0/dalpha/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,9 @@
 import requests, sys, os, pkg_resources
-
-from dalpha.signal_handler import get_shutdown_requested
-from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, get_context, Context
 from dalpha.logging import logger
-from dalpha.logging.events import Event
-
-from dalpha.dto import InferenceResult
-from dalpha.exception import BaseStatusCode
-
-from dalpha.agent import Agent
-from dalpha.cobra_cls import Cobra
-from dalpha.data_update_cls import DalphaDataUpdater
-from dalpha.inference_cls import DalphaAI
-from dalpha.redis_cls import DalphaRedis
-from dalpha.openai_cls import DalphaOpenAI
 
 
 def __load_config(file_path):
     if not os.path.isfile(file_path):
         logger.warning(f"{file_path} 파일을 찾을 수 없습니다.")
         return
     
@@ -46,7 +32,22 @@
     except Exception as e:
         logger.warning(f"dalpha sdk 버전 확인 중 오류가 발생했습니다:{e}")
 cfg_path = os.path.join(sys.path[0],'.dalphacfg')
 
 
 __load_config(cfg_path)
 check_package_version("dalpha")
+
+from dalpha.signal_handler import get_shutdown_requested
+from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, get_context, Context
+from dalpha.logging.events import Event
+
+from dalpha.dto import InferenceResult
+from dalpha.exception import BaseStatusCode, ExpectedError, WaitException
+
+from dalpha.agent import Agent
+from dalpha.cobra_cls import Cobra
+from dalpha.data_update_cls import DalphaDataUpdater
+from dalpha.inference_cls import DalphaAI
+from dalpha.redis_cls import DalphaRedis
+from dalpha.openai_cls import DalphaOpenAI
+from dalpha.backend_cli import BackendCli, internal_call
```

### Comparing `dalpha-0.4.5rc1/dalpha/cobra_cls.py` & `dalpha-0.5.0rc0/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/context.py` & `dalpha-0.5.0rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/data_update_cls.py` & `dalpha-0.5.0rc0/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/dto.py` & `dalpha-0.5.0rc0/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/inference_cls.py` & `dalpha-0.5.0rc0/dalpha/inference_cls.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                 eval_id=eval_id,
                 account_id=account_id,
                 debug=self.debug,
             )
             inference_end_time = time.time()
             logger.info(f"AI inference is done. Time taken: {inference_end_time - inference_start_time:.2f} sec")
         except ExpectedError as expected_error:
-            self.agent.validate_error(evaluate_id=eval_id, output=expected_error.error_json, mock=self.is_mock)
+            self.agent.validate_error(evaluate_id=eval_id, output=expected_error.error_json, mock=self.is_mock, error_code=expected_error.error_code)
             self.wait_flag = True
             return
         except Exception as unexpected_error:
             error_message = f"Unexpected error occurred while running ai : \033[31m{unexpected_error}\033[0m\n{traceback.format_exc()}\n"
             logger.error(error_message)
             error_json = {"reason": f"Unexpected error occurred while running ai: {unexpected_error}"}
             self.agent.validate_error(evaluate_id=eval_id, output=error_json, mock=self.is_mock)
```

### Comparing `dalpha-0.4.5rc1/dalpha/logging/__init__.py` & `dalpha-0.5.0rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/logging/log_formatter.py` & `dalpha-0.5.0rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/logging/utils.py` & `dalpha-0.5.0rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/openai_cls.py` & `dalpha-0.5.0rc0/dalpha/openai_cls.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,8 @@
                 "completion_tokens": ret.usage.completion_tokens,
                 "model": ret.model,
                 "prompt_tokens": ret.usage.prompt_tokens,
                 "total_tokens": ret.usage.total_tokens
             },
             data = {}
         )
-        return ret
+        return ret
```

### Comparing `dalpha-0.4.5rc1/dalpha/redis_cli.py` & `dalpha-0.5.0rc0/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/dalpha/redis_cls.py` & `dalpha-0.5.0rc0/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.5rc1/pyproject.toml` & `dalpha-0.5.0rc0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.5rc1"
+version = "0.5.0rc0"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.26.137"
 requests = "^2.30.0"
 build = "^0.10.0"
 sentry-sdk = "^1.30.0"
 python-json-logger = "^2.0.7"
 kafka-python = "^2.0.2"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.4.5rc1"
+version = "0.5.0rc0"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
+  { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dalpha-0.4.5rc1/PKG-INFO` & `dalpha-0.5.0rc0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.5rc1
+Version: 0.5.0rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.26.137,<2.0.0)
 Requires-Dist: build (>=0.10.0,<0.11.0)
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: python-json-logger (>=2.0.7,<3.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.30.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # internal-sdk
```

