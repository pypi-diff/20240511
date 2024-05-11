# Comparing `tmp/cubetools-0.7.6.tar.gz` & `tmp/cubetools-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cubetools-0.7.6.tar", last modified: Tue Feb 20 01:39:58 2024, max compression
+gzip compressed data, was "dist/cubetools-0.7.7.tar", last modified: Sat May 11 03:51:09 2024, max compression
```

## Comparing `cubetools-0.7.6.tar` & `cubetools-0.7.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-02-20 01:39:58.000000 cubetools-0.7.6/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2464 2024-02-20 01:39:58.000000 cubetools-0.7.6/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)     1289 2024-01-16 04:10:16.000000 cubetools-0.7.6/README.md
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools/
--rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.7.6/cubetools/__init__.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     6906 2024-01-26 07:38:28.000000 cubetools-0.7.6/cubetools/download_model.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    14542 2024-02-20 01:34:08.000000 cubetools-0.7.6/cubetools/huggingface.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    10394 2024-02-20 01:34:08.000000 cubetools-0.7.6/cubetools/huggingface2.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.7.6/cubetools/image_tools.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.7.6/cubetools/mindspore_lite_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     9716 2024-02-20 01:39:02.000000 cubetools-0.7.6/cubetools/modelscope.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     6564 2024-02-20 01:39:02.000000 cubetools-0.7.6/cubetools/modelscope2.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.7.6/cubetools/onnx_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.7.6/cubetools/openvino_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.7.6/cubetools/paddle_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.7.6/cubetools/python_chat_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.7.6/cubetools/python_video_frontend.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2628 2023-07-12 07:01:07.000000 cubetools-0.7.6/cubetools/pytorch_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.7.6/cubetools/video_capture.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.7.6/cubetools/video_predict.py
--rw-rw-r--   0 hls       (1000) hls       (1000)     6213 2023-07-25 10:34:05.000000 cubetools-0.7.6/cubetools/video_predict2.py
-drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/
--rw-rw-r--   0 hls       (1000) hls       (1000)     2464 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/PKG-INFO
--rw-rw-r--   0 hls       (1000) hls       (1000)      693 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/SOURCES.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)        1 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/dependency_links.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)      749 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/entry_points.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       32 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/requires.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       10 2024-02-20 01:39:58.000000 cubetools-0.7.6/cubetools.egg-info/top_level.txt
--rw-rw-r--   0 hls       (1000) hls       (1000)       38 2024-02-20 01:39:58.000000 cubetools-0.7.6/setup.cfg
--rw-rw-r--   0 hls       (1000) hls       (1000)     3002 2024-02-20 01:39:56.000000 cubetools-0.7.6/setup.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-05-11 03:51:09.000000 cubetools-0.7.7/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2464 2024-05-11 03:51:09.000000 cubetools-0.7.7/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1289 2024-01-16 04:10:16.000000 cubetools-0.7.7/README.md
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-05-11 03:51:09.000000 cubetools-0.7.7/cubetools/
+-rw-rw-r--   0 hls       (1000) hls       (1000)        0 2022-11-15 06:16:42.000000 cubetools-0.7.7/cubetools/__init__.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     6906 2024-01-26 07:38:28.000000 cubetools-0.7.7/cubetools/download_model.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    14542 2024-02-20 01:43:35.000000 cubetools-0.7.7/cubetools/huggingface.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    10394 2024-02-20 01:43:35.000000 cubetools-0.7.7/cubetools/huggingface2.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9987 2023-05-15 01:24:04.000000 cubetools-0.7.7/cubetools/image_tools.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     1689 2023-04-03 13:20:28.000000 cubetools-0.7.7/cubetools/mindspore_lite_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     9716 2024-02-20 01:43:35.000000 cubetools-0.7.7/cubetools/modelscope.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     6564 2024-02-20 01:43:35.000000 cubetools-0.7.7/cubetools/modelscope2.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      607 2023-04-03 13:20:28.000000 cubetools-0.7.7/cubetools/onnx_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)      817 2023-04-06 07:12:09.000000 cubetools-0.7.7/cubetools/openvino_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3091 2023-04-03 13:20:28.000000 cubetools-0.7.7/cubetools/paddle_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2394 2023-05-23 12:05:30.000000 cubetools-0.7.7/cubetools/python_chat_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)    15694 2023-05-25 10:46:59.000000 cubetools-0.7.7/cubetools/python_video_frontend.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2628 2023-07-12 07:01:07.000000 cubetools-0.7.7/cubetools/pytorch_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2518 2023-03-08 07:16:48.000000 cubetools-0.7.7/cubetools/video_capture.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3799 2023-05-25 10:06:04.000000 cubetools-0.7.7/cubetools/video_predict.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     6213 2023-07-25 10:34:05.000000 cubetools-0.7.7/cubetools/video_predict2.py
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3287 2024-05-11 03:51:02.000000 cubetools-0.7.7/cubetools/yolo_process.py
+drwxrwxr-x   0 hls       (1000) hls       (1000)        0 2024-05-11 03:51:09.000000 cubetools-0.7.7/cubetools.egg-info/
+-rw-rw-r--   0 hls       (1000) hls       (1000)     2464 2024-05-11 03:51:08.000000 cubetools-0.7.7/cubetools.egg-info/PKG-INFO
+-rw-rw-r--   0 hls       (1000) hls       (1000)      719 2024-05-11 03:51:08.000000 cubetools-0.7.7/cubetools.egg-info/SOURCES.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)        1 2024-05-11 03:51:08.000000 cubetools-0.7.7/cubetools.egg-info/dependency_links.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)      749 2024-05-11 03:51:08.000000 cubetools-0.7.7/cubetools.egg-info/entry_points.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       32 2024-05-11 03:51:08.000000 cubetools-0.7.7/cubetools.egg-info/requires.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       10 2024-05-11 03:51:08.000000 cubetools-0.7.7/cubetools.egg-info/top_level.txt
+-rw-rw-r--   0 hls       (1000) hls       (1000)       38 2024-05-11 03:51:09.000000 cubetools-0.7.7/setup.cfg
+-rw-rw-r--   0 hls       (1000) hls       (1000)     3002 2024-05-11 03:51:02.000000 cubetools-0.7.7/setup.py
```

### Comparing `cubetools-0.7.6/PKG-INFO` & `cubetools-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.7.6
+Version: 0.7.7
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.7.6/README.md` & `cubetools-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/download_model.py` & `cubetools-0.7.7/cubetools/download_model.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/huggingface.py` & `cubetools-0.7.7/cubetools/huggingface.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/huggingface2.py` & `cubetools-0.7.7/cubetools/huggingface2.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/image_tools.py` & `cubetools-0.7.7/cubetools/image_tools.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/mindspore_lite_predict.py` & `cubetools-0.7.7/cubetools/mindspore_lite_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/modelscope.py` & `cubetools-0.7.7/cubetools/modelscope.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/modelscope2.py` & `cubetools-0.7.7/cubetools/modelscope2.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/onnx_predict.py` & `cubetools-0.7.7/cubetools/onnx_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/openvino_predict.py` & `cubetools-0.7.7/cubetools/openvino_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/paddle_predict.py` & `cubetools-0.7.7/cubetools/paddle_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/python_chat_frontend.py` & `cubetools-0.7.7/cubetools/python_chat_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/python_video_frontend.py` & `cubetools-0.7.7/cubetools/python_video_frontend.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/pytorch_predict.py` & `cubetools-0.7.7/cubetools/pytorch_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/video_capture.py` & `cubetools-0.7.7/cubetools/video_capture.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/video_predict.py` & `cubetools-0.7.7/cubetools/video_predict.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools/video_predict2.py` & `cubetools-0.7.7/cubetools/video_predict2.py`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/cubetools.egg-info/PKG-INFO` & `cubetools-0.7.7/cubetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubetools
-Version: 0.7.6
+Version: 0.7.7
 Summary: CubeAI模型开发常用工具集
 Home-page: https://openi.pcl.ac.cn/cubeai/cubetools
 Author: cubeai
 Author-email: cubeai@163.com
 License: Apache License 2.0
 Description: # CubeTools
```

### Comparing `cubetools-0.7.6/cubetools.egg-info/SOURCES.txt` & `cubetools-0.7.7/cubetools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 cubetools/paddle_predict.py
 cubetools/python_chat_frontend.py
 cubetools/python_video_frontend.py
 cubetools/pytorch_predict.py
 cubetools/video_capture.py
 cubetools/video_predict.py
 cubetools/video_predict2.py
+cubetools/yolo_process.py
 cubetools.egg-info/PKG-INFO
 cubetools.egg-info/SOURCES.txt
 cubetools.egg-info/dependency_links.txt
 cubetools.egg-info/entry_points.txt
 cubetools.egg-info/requires.txt
 cubetools.egg-info/top_level.txt
```

### Comparing `cubetools-0.7.6/cubetools.egg-info/entry_points.txt` & `cubetools-0.7.7/cubetools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cubetools-0.7.6/setup.py` & `cubetools-0.7.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(
     name='cubetools',
-    version='0.7.6',
+    version='0.7.7',
     author='cubeai',
     author_email='cubeai@163.com',
     description='CubeAI模型开发常用工具集',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     packages=find_packages(),
```

