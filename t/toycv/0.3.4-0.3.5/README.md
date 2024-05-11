# Comparing `tmp/toycv-0.3.4.tar.gz` & `tmp/toycv-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toycv-0.3.4.tar", last modified: Sat May 11 09:52:22 2024, max compression
+gzip compressed data, was "toycv-0.3.5.tar", last modified: Sat May 11 10:07:56 2024, max compression
```

## Comparing `toycv-0.3.4.tar` & `toycv-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.418763 toycv-0.3.4/
--rw-r--r--   0 xiangyang   (501) staff       (20)     1067 2024-03-16 04:38:20.000000 toycv-0.3.4/LICENSE
--rw-r--r--   0 xiangyang   (501) staff       (20)      214 2024-03-14 15:54:16.000000 toycv-0.3.4/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-11 09:52:22.418638 toycv-0.3.4/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)       84 2024-03-16 04:38:20.000000 toycv-0.3.4/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-11 09:52:22.000000 toycv-0.3.4/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2024-05-11 09:52:22.418807 toycv-0.3.4/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1958 2024-05-11 09:52:02.000000 toycv-0.3.4/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.416786 toycv-0.3.4/toycv/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 06:11:05.000000 toycv-0.3.4/toycv/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     8409 2024-05-06 06:23:06.000000 toycv-0.3.4/toycv/common.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.417869 toycv-0.3.4/toycv/file/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 20:37:55.000000 toycv-0.3.4/toycv/file/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)    14431 2024-05-11 09:11:37.000000 toycv-0.3.4/toycv/file/image.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1873 2024-04-09 03:48:43.000000 toycv-0.3.4/toycv/file/path.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      300 2024-04-26 09:56:43.000000 toycv-0.3.4/toycv/metrics.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.418369 toycv-0.3.4/toycv/pytorch/
--rw-r--r--   0 xiangyang   (501) staff       (20)      933 2024-03-17 20:12:36.000000 toycv-0.3.4/toycv/pytorch/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      737 2024-05-08 21:32:59.000000 toycv-0.3.4/toycv/pytorch/datasets.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2805 2024-05-11 01:21:47.000000 toycv-0.3.4/toycv/pytorch/transform.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      502 2024-04-26 08:43:20.000000 toycv-0.3.4/toycv/string.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.418486 toycv-0.3.4/toycv/visualization/
--rw-r--r--   0 xiangyang   (501) staff       (20)     7887 2024-05-09 04:12:49.000000 toycv-0.3.4/toycv/visualization/__init__.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.417486 toycv-0.3.4/toycv.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      439 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        6 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 10:07:56.694739 toycv-0.3.5/
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1067 2024-03-16 04:38:20.000000 toycv-0.3.5/LICENSE
+-rw-r--r--   0 xiangyang   (501) staff       (20)      214 2024-03-14 15:54:16.000000 toycv-0.3.5/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-11 10:07:56.694568 toycv-0.3.5/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)       84 2024-03-16 04:38:20.000000 toycv-0.3.5/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-11 10:07:56.000000 toycv-0.3.5/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2024-05-11 10:07:56.694803 toycv-0.3.5/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1958 2024-05-11 10:07:41.000000 toycv-0.3.5/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 10:07:56.692407 toycv-0.3.5/toycv/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 06:11:05.000000 toycv-0.3.5/toycv/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     8409 2024-05-06 06:23:06.000000 toycv-0.3.5/toycv/common.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 10:07:56.693516 toycv-0.3.5/toycv/file/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 20:37:55.000000 toycv-0.3.5/toycv/file/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)    14431 2024-05-11 09:11:37.000000 toycv-0.3.5/toycv/file/image.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1873 2024-04-09 03:48:43.000000 toycv-0.3.5/toycv/file/path.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      300 2024-04-26 09:56:43.000000 toycv-0.3.5/toycv/metrics.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 10:07:56.694119 toycv-0.3.5/toycv/pytorch/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      933 2024-03-17 20:12:36.000000 toycv-0.3.5/toycv/pytorch/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      845 2024-05-11 10:02:00.000000 toycv-0.3.5/toycv/pytorch/datasets.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2805 2024-05-11 01:21:47.000000 toycv-0.3.5/toycv/pytorch/transform.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      502 2024-04-26 08:43:20.000000 toycv-0.3.5/toycv/string.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 10:07:56.694286 toycv-0.3.5/toycv/visualization/
+-rw-r--r--   0 xiangyang   (501) staff       (20)     7887 2024-05-09 04:12:49.000000 toycv-0.3.5/toycv/visualization/__init__.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 10:07:56.693087 toycv-0.3.5/toycv.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-11 10:07:56.000000 toycv-0.3.5/toycv.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      439 2024-05-11 10:07:56.000000 toycv-0.3.5/toycv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2024-05-11 10:07:56.000000 toycv-0.3.5/toycv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-11 10:07:56.000000 toycv-0.3.5/toycv.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        6 2024-05-11 10:07:56.000000 toycv-0.3.5/toycv.egg-info/top_level.txt
```

### Comparing `toycv-0.3.4/LICENSE` & `toycv-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/PKG-INFO` & `toycv-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toycv
-Version: 0.3.4
+Version: 0.3.5
 Summary: A simple and flexible tool for building and training neural network models.
 Home-page: https://github.com/coderelease
 Author: Yang Xiang
 Author-email: btk@qq.com
 License: MIT
 Keywords: toycv
 Classifier: Intended Audience :: Developers
```

### Comparing `toycv-0.3.4/setup.py` & `toycv-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='toycv',  # 包名
     python_requires='>=3.8.0',  # python环境
-    version='0.3.4',  # 包的版本
+    version='0.3.5',  # 包的版本
     description="A simple and flexible tool for building and training neural network models.",  # 包简介，显示在PyPI上
 
     long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
     long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
     # 作者相关信息
     author="Yang Xiang",
```

### Comparing `toycv-0.3.4/toycv/common.py` & `toycv-0.3.5/toycv/common.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/toycv/file/image.py` & `toycv-0.3.5/toycv/file/image.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/toycv/file/path.py` & `toycv-0.3.5/toycv/file/path.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/toycv/pytorch/__init__.py` & `toycv-0.3.5/toycv/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/toycv/pytorch/datasets.py` & `toycv-0.3.5/toycv/pytorch/datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from torch.utils.data import Dataset
 
 
 class SubDataset(Dataset):
     def __init__(self, original_dataset, available_index_list=None):
         self.original_dataset = original_dataset
-        self.available_index_list = available_index_list
+        self.available_index_list = [i for i in available_index_list if i < len(self.original_dataset)]
 
     def __len__(self):
         return len(self.available_index_list)
 
     def __getitem__(self, index):
         return self.original_dataset[self.available_index_list[index]]
 
@@ -18,8 +18,10 @@
         self.original_dataset = original_dataset
         self.limit = limit
 
     def __len__(self):
         return min(len(self.original_dataset), self.limit)
 
     def __getitem__(self, index):
+        if index >= self.limit:
+            raise IndexError
         return self.original_dataset[index]
```

### Comparing `toycv-0.3.4/toycv/pytorch/transform.py` & `toycv-0.3.5/toycv/pytorch/transform.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/toycv/visualization/__init__.py` & `toycv-0.3.5/toycv/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.4/toycv.egg-info/PKG-INFO` & `toycv-0.3.5/toycv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toycv
-Version: 0.3.4
+Version: 0.3.5
 Summary: A simple and flexible tool for building and training neural network models.
 Home-page: https://github.com/coderelease
 Author: Yang Xiang
 Author-email: btk@qq.com
 License: MIT
 Keywords: toycv
 Classifier: Intended Audience :: Developers
```

