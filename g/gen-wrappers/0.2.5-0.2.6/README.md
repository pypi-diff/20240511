# Comparing `tmp/gen_wrappers-0.2.5.tar.gz` & `tmp/gen_wrappers-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.2.5.tar", last modified: Fri May 10 20:36:52 2024, max compression
+gzip compressed data, was "gen_wrappers-0.2.6.tar", last modified: Fri May 10 20:51:41 2024, max compression
```

## Comparing `gen_wrappers-0.2.5.tar` & `gen_wrappers-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.283790 gen_wrappers-0.2.5/
--rw-rw-rw-   0        0        0      847 2024-05-10 20:36:52.281798 gen_wrappers-0.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.176976 gen_wrappers-0.2.5/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.5/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.187686 gen_wrappers-0.2.5/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.5/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     6713 2024-05-03 20:01:50.000000 gen_wrappers-0.2.5/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.5/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.5/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.201222 gen_wrappers-0.2.5/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.5/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.5/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.5/creator/base/base_request.py
--rw-rw-rw-   0        0        0     3028 2024-05-03 21:08:54.000000 gen_wrappers-0.2.5/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.5/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.210170 gen_wrappers-0.2.5/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.5/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9509 2024-05-10 20:31:50.000000 gen_wrappers-0.2.5/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     9370 2024-05-10 20:36:48.000000 gen_wrappers-0.2.5/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.5/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.220150 gen_wrappers-0.2.5/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.5/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.5/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.5/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.5/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-10 20:36:52.277780 gen_wrappers-0.2.5/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      847 2024-05-10 20:36:52.000000 gen_wrappers-0.2.5/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-10 20:36:52.000000 gen_wrappers-0.2.5/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 20:36:52.000000 gen_wrappers-0.2.5/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-10 20:36:52.000000 gen_wrappers-0.2.5/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 20:36:52.000000 gen_wrappers-0.2.5/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 20:36:52.284792 gen_wrappers-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1035 2024-05-10 20:36:48.000000 gen_wrappers-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.895217 gen_wrappers-0.2.6/
+-rw-rw-rw-   0        0        0      847 2024-05-10 20:51:41.893225 gen_wrappers-0.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.811421 gen_wrappers-0.2.6/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.2.6/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.822840 gen_wrappers-0.2.6/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.2.6/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     6713 2024-05-03 20:01:50.000000 gen_wrappers-0.2.6/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     6018 2024-05-03 19:52:10.000000 gen_wrappers-0.2.6/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.2.6/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.836260 gen_wrappers-0.2.6/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.2.6/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1584 2024-05-09 21:53:52.000000 gen_wrappers-0.2.6/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.2.6/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     3028 2024-05-03 21:08:54.000000 gen_wrappers-0.2.6/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.2.6/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.846273 gen_wrappers-0.2.6/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.2.6/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9534 2024-05-10 20:51:21.000000 gen_wrappers-0.2.6/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     9370 2024-05-10 20:36:48.000000 gen_wrappers-0.2.6/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.2.6/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.856852 gen_wrappers-0.2.6/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.2.6/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6344 2024-05-03 18:21:55.000000 gen_wrappers-0.2.6/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3973 2024-05-03 18:13:30.000000 gen_wrappers-0.2.6/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.2.6/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-10 20:51:41.891216 gen_wrappers-0.2.6/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-10 20:51:41.000000 gen_wrappers-0.2.6/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 20:51:41.895217 gen_wrappers-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2024-05-10 20:51:31.000000 gen_wrappers-0.2.6/setup.py
```

### Comparing `gen_wrappers-0.2.5/PKG-INFO` & `gen_wrappers-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.2.5
+Version: 0.2.6
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.5/creator/auto/creator_auto.py` & `gen_wrappers-0.2.6/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/auto/request_auto.py` & `gen_wrappers-0.2.6/creator/auto/request_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/auto/response_auto.py` & `gen_wrappers-0.2.6/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/base/base_app.py` & `gen_wrappers-0.2.6/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/base/base_request.py` & `gen_wrappers-0.2.6/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/base/base_response.py` & `gen_wrappers-0.2.6/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.2.6/creator/cmfy/creator_cmfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 data_type=ResponseDataType.IMAGE,
                 total_count=len(data)
             )
             logger.info(f"Success, returning response with {len(data)} images")
             return ResponseCmfy.success(response_data)
         return ResponseCmfy.error("Error creating prompt")
 
-    async def create_async(self, params: CmfyWorkflow) -> ResponseCmfy:
+    async def create_async(self, params: Union[CmfyWorkflow, CmfyWorkflowFcus]) -> ResponseCmfy:
         cmfy_port = os.environ.get("PORT_CMFY", 8889)
         url = f"http://localhost:{cmfy_port}/prompt"
         workflow = json.loads(params.workflow_json)
         self._check_loaded_model(workflow)
         logger.debug(f"CMFY data: {workflow}")
         # Send a POST to cmfy_url with the workflow json
         # The response will be JSON string with the below format
```

### Comparing `gen_wrappers-0.2.5/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.2.6/creator/cmfy/request_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.2.6/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.2.6/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.2.6/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.2.6/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.2.5
+Version: 0.2.6
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.2.5/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.2.6/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.2.5/setup.py` & `gen_wrappers-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.2.5',
+    version='0.2.6',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

