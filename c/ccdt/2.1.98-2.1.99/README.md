# Comparing `tmp/ccdt-2.1.98.tar.gz` & `tmp/ccdt-2.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccdt-2.1.98.tar", last modified: Sat Apr 20 07:38:36 2024, max compression
+gzip compressed data, was "ccdt-2.1.99.tar", last modified: Sat Apr 20 08:59:27 2024, max compression
```

## Comparing `ccdt-2.1.98.tar` & `ccdt-2.1.99.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.330175 ccdt-2.1.98/
--rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.98/LICENSE
--rw-rw-rw-   0        0        0     4806 2024-04-20 07:38:36.329177 ccdt-2.1.98/PKG-INFO
--rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.98/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.302264 ccdt-2.1.98/ccdt/
--rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.98/ccdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.310228 ccdt-2.1.98/ccdt/dataset/
--rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.98/ccdt/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.312223 ccdt-2.1.98/ccdt/dataset/base_coco/
--rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.98/ccdt/dataset/base_coco/__init__.py
--rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.98/ccdt/dataset/base_coco/base_coco.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.315214 ccdt-2.1.98/ccdt/dataset/base_labelme/
--rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.98/ccdt/dataset/base_labelme/__init__.py
--rw-rw-rw-   0        0        0    15439 2024-04-17 03:45:32.000000 ccdt-2.1.98/ccdt/dataset/base_labelme/async_io_task.py
--rw-rw-rw-   0        0        0   116306 2024-04-17 03:29:29.000000 ccdt-2.1.98/ccdt/dataset/base_labelme/base_labelme.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.320201 ccdt-2.1.98/ccdt/dataset/base_voc/
--rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.98/ccdt/dataset/base_voc/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.98/ccdt/dataset/base_voc/base_sys.py
--rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.98/ccdt/dataset/base_voc/base_txt.py
--rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.98/ccdt/dataset/base_voc/base_voc.py
--rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.98/ccdt/dataset/base_voc/coco_to_labelme.py
--rw-rw-rw-   0        0        0    24566 2024-04-20 04:27:41.000000 ccdt-2.1.98/ccdt/dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.322196 ccdt-2.1.98/ccdt/dataset/utils/
--rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.98/ccdt/dataset/utils/__init__.py
--rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.98/ccdt/dataset/utils/encoder.py
--rw-rw-rw-   0        0        0    28644 2024-04-20 06:47:17.000000 ccdt-2.1.98/ccdt/dataset/utils/labelme_load.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.326186 ccdt-2.1.98/ccdt/video_tool/
--rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.98/ccdt/video_tool/__init__.py
--rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.98/ccdt/video_tool/intercept.py
--rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.98/ccdt/video_tool/split.py
--rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.98/ccdt/video_tool/video_main.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.328180 ccdt-2.1.98/ccdt.egg-info/
--rw-rw-rw-   0        0        0     4806 2024-04-20 07:38:36.000000 ccdt-2.1.98/ccdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-20 07:38:36.000000 ccdt-2.1.98/ccdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 07:38:36.000000 ccdt-2.1.98/ccdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2024-04-20 07:38:36.000000 ccdt-2.1.98/ccdt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2024-04-20 07:38:36.000000 ccdt-2.1.98/ccdt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-20 07:38:36.000000 ccdt-2.1.98/ccdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 07:38:36.330175 ccdt-2.1.98/setup.cfg
--rw-rw-rw-   0        0        0     2524 2024-04-20 07:38:09.000000 ccdt-2.1.98/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 07:38:36.327183 ccdt-2.1.98/test/
--rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.98/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.958733 ccdt-2.1.99/
+-rw-rw-rw-   0        0        0    35823 2023-05-23 02:06:29.000000 ccdt-2.1.99/LICENSE
+-rw-rw-rw-   0        0        0     4806 2024-04-20 08:59:27.957735 ccdt-2.1.99/PKG-INFO
+-rw-rw-rw-   0        0        0     3979 2023-06-26 09:05:42.000000 ccdt-2.1.99/README.md
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.923827 ccdt-2.1.99/ccdt/
+-rw-rw-rw-   0        0        0      150 2023-06-01 09:39:39.000000 ccdt-2.1.99/ccdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.931804 ccdt-2.1.99/ccdt/dataset/
+-rw-rw-rw-   0        0        0      248 2023-07-31 10:14:46.000000 ccdt-2.1.99/ccdt/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.934798 ccdt-2.1.99/ccdt/dataset/base_coco/
+-rw-rw-rw-   0        0        0      171 2023-05-17 01:51:28.000000 ccdt-2.1.99/ccdt/dataset/base_coco/__init__.py
+-rw-rw-rw-   0        0        0    34384 2024-03-09 03:14:32.000000 ccdt-2.1.99/ccdt/dataset/base_coco/base_coco.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.937788 ccdt-2.1.99/ccdt/dataset/base_labelme/
+-rw-rw-rw-   0        0        0      180 2023-05-17 01:47:52.000000 ccdt-2.1.99/ccdt/dataset/base_labelme/__init__.py
+-rw-rw-rw-   0        0        0    15439 2024-04-17 03:45:32.000000 ccdt-2.1.99/ccdt/dataset/base_labelme/async_io_task.py
+-rw-rw-rw-   0        0        0   116306 2024-04-17 03:29:29.000000 ccdt-2.1.99/ccdt/dataset/base_labelme/base_labelme.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.943773 ccdt-2.1.99/ccdt/dataset/base_voc/
+-rw-rw-rw-   0        0        0      326 2023-11-07 09:53:48.000000 ccdt-2.1.99/ccdt/dataset/base_voc/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-11-27 03:47:20.000000 ccdt-2.1.99/ccdt/dataset/base_voc/base_sys.py
+-rw-rw-rw-   0        0        0     3834 2023-10-14 07:34:34.000000 ccdt-2.1.99/ccdt/dataset/base_voc/base_txt.py
+-rw-rw-rw-   0        0        0     3430 2023-07-31 13:32:48.000000 ccdt-2.1.99/ccdt/dataset/base_voc/base_voc.py
+-rw-rw-rw-   0        0        0    14450 2024-04-08 09:36:39.000000 ccdt-2.1.99/ccdt/dataset/base_voc/coco_to_labelme.py
+-rw-rw-rw-   0        0        0    24566 2024-04-20 04:27:41.000000 ccdt-2.1.99/ccdt/dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.946764 ccdt-2.1.99/ccdt/dataset/utils/
+-rw-rw-rw-   0        0        0      221 2023-06-26 08:16:17.000000 ccdt-2.1.99/ccdt/dataset/utils/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-05-17 01:54:00.000000 ccdt-2.1.99/ccdt/dataset/utils/encoder.py
+-rw-rw-rw-   0        0        0    28721 2024-04-20 08:53:24.000000 ccdt-2.1.99/ccdt/dataset/utils/labelme_load.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.952777 ccdt-2.1.99/ccdt/video_tool/
+-rw-rw-rw-   0        0        0      172 2023-05-25 06:30:32.000000 ccdt-2.1.99/ccdt/video_tool/__init__.py
+-rw-rw-rw-   0        0        0     1726 2023-07-05 09:01:01.000000 ccdt-2.1.99/ccdt/video_tool/intercept.py
+-rw-rw-rw-   0        0        0     5367 2024-03-02 06:01:23.000000 ccdt-2.1.99/ccdt/video_tool/split.py
+-rw-rw-rw-   0        0        0     6301 2023-08-18 09:59:56.000000 ccdt-2.1.99/ccdt/video_tool/video_main.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.956738 ccdt-2.1.99/ccdt.egg-info/
+-rw-rw-rw-   0        0        0     4806 2024-04-20 08:59:27.000000 ccdt-2.1.99/ccdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-20 08:59:27.000000 ccdt-2.1.99/ccdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-20 08:59:27.000000 ccdt-2.1.99/ccdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-20 08:59:27.000000 ccdt-2.1.99/ccdt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-20 08:59:27.000000 ccdt-2.1.99/ccdt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-20 08:59:27.000000 ccdt-2.1.99/ccdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-20 08:59:27.958733 ccdt-2.1.99/setup.cfg
+-rw-rw-rw-   0        0        0     2524 2024-04-20 08:59:13.000000 ccdt-2.1.99/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-20 08:59:27.954745 ccdt-2.1.99/test/
+-rw-rw-rw-   0        0        0     8178 2023-06-09 06:33:20.000000 ccdt-2.1.99/test/test.py
```

### Comparing `ccdt-2.1.98/LICENSE` & `ccdt-2.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/PKG-INFO` & `ccdt-2.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.98
+Version: 2.1.99
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.98/README.md` & `ccdt-2.1.99/README.md`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_coco/base_coco.py` & `ccdt-2.1.99/ccdt/dataset/base_coco/base_coco.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_labelme/async_io_task.py` & `ccdt-2.1.99/ccdt/dataset/base_labelme/async_io_task.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_labelme/base_labelme.py` & `ccdt-2.1.99/ccdt/dataset/base_labelme/base_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_voc/base_sys.py` & `ccdt-2.1.99/ccdt/dataset/base_voc/base_sys.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_voc/base_txt.py` & `ccdt-2.1.99/ccdt/dataset/base_voc/base_txt.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_voc/base_voc.py` & `ccdt-2.1.99/ccdt/dataset/base_voc/base_voc.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/base_voc/coco_to_labelme.py` & `ccdt-2.1.99/ccdt/dataset/base_voc/coco_to_labelme.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/main.py` & `ccdt-2.1.99/ccdt/dataset/main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/utils/encoder.py` & `ccdt-2.1.99/ccdt/dataset/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/dataset/utils/labelme_load.py` & `ccdt-2.1.99/ccdt/dataset/utils/labelme_load.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,21 +389,21 @@
             for dirname in dirs:
                 original_dir = os.path.join(root, dirname)
                 pinyin_dirname = self.convert_chinese_to_pinyin(dirname)
                 new_dir = os.path.join(root, pinyin_dirname)
                 try:
                     os.rename(original_dir, new_dir)
                 except Exception as e:
-                    print(f"拷贝 {original_dir} 失败: {e}")
-            # 递归处理子目录
+                    print(f"重命名，存在相同名称的拼音 {original_dir} 失败: {e}")
+            # # 递归处理子目录
             for dirpath, dirnames, filenames in os.walk(self.type_args[0].get('input_dir')):
                 for subdir in dirnames:
                     self.convert_chinese_to_pinyin(os.path.join(dirpath, subdir))
                 # 重命名路径
-        print(f'重命名中文路径为英文开始')
+        print(f'注意不嵌套重命名自目录，嵌套几次目录就多执行几次指令')
 
     @staticmethod
     def convert_path_to_pinyin(path):
         """
         将给定路径中的汉字转换为拼音。
         path: 需要转换的路径。
         """
```

### Comparing `ccdt-2.1.98/ccdt/video_tool/intercept.py` & `ccdt-2.1.99/ccdt/video_tool/intercept.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/video_tool/split.py` & `ccdt-2.1.99/ccdt/video_tool/split.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt/video_tool/video_main.py` & `ccdt-2.1.99/ccdt/video_tool/video_main.py`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/ccdt.egg-info/PKG-INFO` & `ccdt-2.1.99/ccdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdt
-Version: 2.1.98
+Version: 2.1.99
 Summary: AI数据转换工具箱
 Home-page: https://github.com/chipeak/chipeak_cv_data_tool
 Author: zhanyong
 Author-email: zhan.yong@chipeak.com
 Project-URL: Bug Tracker, https://github.com/chipeak/chipeak_cv_data_tool/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `ccdt-2.1.98/ccdt.egg-info/SOURCES.txt` & `ccdt-2.1.99/ccdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccdt-2.1.98/setup.py` & `ccdt-2.1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ]
     return install_requires
 
 
 setup(
     # 取名不能够用_会自动变-   ccdt
     name='ccdt',
-    version='2.1.98',
+    version='2.1.99',
     packages=find_packages(exclude=['data']),
     install_requires=get_install_requires(),
     author='zhanyong',
     author_email='zhan.yong@chipeak.com',
     description='AI数据转换工具箱',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `ccdt-2.1.98/test/test.py` & `ccdt-2.1.99/test/test.py`

 * *Files identical despite different names*

