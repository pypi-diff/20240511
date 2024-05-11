# Comparing `tmp/pluto_client-0.0.8.tar.gz` & `tmp/pluto_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluto_client-0.0.8.tar", max compression
+gzip compressed data, was "pluto_client-0.0.9.tar", max compression
```

## Comparing `pluto_client-0.0.8.tar` & `pluto_client-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.8/LICENSE
--rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.8/README.md
--rw-r--r--   0        0        0      593 2024-04-28 03:53:08.789970 pluto_client-0.0.8/pluto_client/__init__.py
--rw-r--r--   0        0        0     1690 2024-04-28 03:53:08.790970 pluto_client-0.0.8/pluto_client/bucket.py
--rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/__init__.py
--rw-r--r--   0        0        0      269 2024-04-28 03:53:08.790970 pluto_client-0.0.8/pluto_client/clients/aws/__init__.py
--rw-r--r--   0        0        0     1139 2024-04-28 03:53:08.791970 pluto_client-0.0.8/pluto_client/clients/aws/bucket_s3.py
--rw-r--r--   0        0        0     2830 2024-05-06 09:18:56.382401 pluto_client-0.0.8/pluto_client/clients/aws/function_lambda.py
--rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/aws/kvstore_dynamodb.py
--rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/aws/queue_sns.py
--rw-r--r--   0        0        0     1058 2024-04-28 03:53:08.792971 pluto_client-0.0.8/pluto_client/clients/aws/sagemaker.py
--rw-r--r--   0        0        0      575 2024-04-28 03:53:08.793970 pluto_client-0.0.8/pluto_client/clients/aws/utils.py
--rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/errors.py
--rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/shared/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/clients/shared/router.py
--rw-r--r--   0        0        0     1972 2024-05-06 09:18:21.896053 pluto_client-0.0.8/pluto_client/function.py
--rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/kvstore.py
--rw-r--r--   0        0        0     1889 2024-05-06 07:22:25.100312 pluto_client-0.0.8/pluto_client/queue.py
--rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/router.py
--rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.8/pluto_client/sagemaker.py
--rw-r--r--   0        0        0     1276 2024-04-28 03:53:08.793970 pluto_client-0.0.8/pluto_client/schedule.py
--rw-r--r--   0        0        0      796 2024-05-06 09:55:57.058392 pluto_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10139 2024-04-12 09:11:51.818491 pluto_client-0.0.9/LICENSE
+-rw-r--r--   0        0        0      241 2024-04-12 09:11:51.818491 pluto_client-0.0.9/README.md
+-rw-r--r--   0        0        0      593 2024-04-28 03:53:08.789970 pluto_client-0.0.9/pluto_client/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-28 03:53:08.790970 pluto_client-0.0.9/pluto_client/bucket.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/clients/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-28 03:53:08.790970 pluto_client-0.0.9/pluto_client/clients/aws/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-28 03:53:08.791970 pluto_client-0.0.9/pluto_client/clients/aws/bucket_s3.py
+-rw-r--r--   0        0        0     2830 2024-05-09 07:08:51.033004 pluto_client-0.0.9/pluto_client/clients/aws/function_lambda.py
+-rw-r--r--   0        0        0     1018 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/clients/aws/kvstore_dynamodb.py
+-rw-r--r--   0        0        0     1198 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/clients/aws/queue_sns.py
+-rw-r--r--   0        0        0     1058 2024-04-28 03:53:08.792971 pluto_client-0.0.9/pluto_client/clients/aws/sagemaker.py
+-rw-r--r--   0        0        0      575 2024-04-28 03:53:08.793970 pluto_client-0.0.9/pluto_client/clients/aws/utils.py
+-rw-r--r--   0        0        0      187 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/clients/errors.py
+-rw-r--r--   0        0        0       33 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/clients/shared/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/clients/shared/router.py
+-rw-r--r--   0        0        0     2043 2024-05-09 11:56:29.370189 pluto_client-0.0.9/pluto_client/function.py
+-rw-r--r--   0        0        0     1703 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/kvstore.py
+-rw-r--r--   0        0        0     1889 2024-05-06 07:22:25.100312 pluto_client-0.0.9/pluto_client/queue.py
+-rw-r--r--   0        0        0     2059 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/router.py
+-rw-r--r--   0        0        0     3610 2024-04-12 09:11:51.818491 pluto_client-0.0.9/pluto_client/sagemaker.py
+-rw-r--r--   0        0        0     1276 2024-04-28 03:53:08.793970 pluto_client-0.0.9/pluto_client/schedule.py
+-rw-r--r--   0        0        0      796 2024-05-09 12:01:36.231451 pluto_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.9/PKG-INFO
```

### Comparing `pluto_client-0.0.8/LICENSE` & `pluto_client-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/__init__.py` & `pluto_client-0.0.9/pluto_client/__init__.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/bucket.py` & `pluto_client-0.0.9/pluto_client/bucket.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/clients/aws/bucket_s3.py` & `pluto_client-0.0.9/pluto_client/clients/aws/bucket_s3.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/clients/aws/function_lambda.py` & `pluto_client-0.0.9/pluto_client/clients/aws/function_lambda.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/clients/aws/kvstore_dynamodb.py` & `pluto_client-0.0.9/pluto_client/clients/aws/kvstore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/clients/aws/queue_sns.py` & `pluto_client-0.0.9/pluto_client/clients/aws/queue_sns.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/clients/aws/sagemaker.py` & `pluto_client-0.0.9/pluto_client/clients/aws/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/clients/aws/utils.py` & `pluto_client-0.0.9/pluto_client/clients/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/function.py` & `pluto_client-0.0.9/pluto_client/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     body: Any
 
 
 @dataclass
 class FunctionOptions:
     memory: int | None = 128  # The memory size in MB, default is 128.
     envs: Dict[str, Any] | None = None
+    raw: bool = False  # This option only works for the AWS currently.
 
 
 class IFunctionClientApi(Generic[FnHandler], IResourceClientApi):
     def invoke(self, *args, **kwargs) -> Any:
         raise NotImplementedError
```

### Comparing `pluto_client-0.0.8/pluto_client/kvstore.py` & `pluto_client-0.0.9/pluto_client/kvstore.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/queue.py` & `pluto_client-0.0.9/pluto_client/queue.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/router.py` & `pluto_client-0.0.9/pluto_client/router.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/sagemaker.py` & `pluto_client-0.0.9/pluto_client/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pluto_client/schedule.py` & `pluto_client-0.0.9/pluto_client/schedule.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.8/pyproject.toml` & `pluto_client-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pluto-client"
-version = "0.0.8"
+version = "0.0.9"
 description = "The Client Library for Pluto Programming Language."
 authors = ["Jade Zheng <zheng.shoujian@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     'Development Status :: 1 - Planning',
     'Environment :: Console',
```

### Comparing `pluto_client-0.0.8/PKG-INFO` & `pluto_client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluto-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Client Library for Pluto Programming Language.
 License: Apache-2.0
 Author: Jade Zheng
 Author-email: zheng.shoujian@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

