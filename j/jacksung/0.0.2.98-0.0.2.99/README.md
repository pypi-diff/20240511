# Comparing `tmp/jacksung-0.0.2.98.tar.gz` & `tmp/jacksung-0.0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jacksung-0.0.2.98.tar", last modified: Tue Apr  2 12:31:54 2024, max compression
+gzip compressed data, was "jacksung-0.0.2.99.tar", last modified: Mon Apr  8 12:09:01 2024, max compression
```

## Comparing `jacksung-0.0.2.98.tar` & `jacksung-0.0.2.99.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:54.677676 jacksung-0.0.2.98/
--rw-rw-rw-   0        0        0    11558 2023-11-22 07:36:29.000000 jacksung-0.0.2.98/LICENSE
--rw-rw-rw-   0        0        0     5413 2024-04-02 12:31:54.676679 jacksung-0.0.2.98/PKG-INFO
--rw-rw-rw-   0        0        0     5255 2024-03-21 14:36:06.000000 jacksung-0.0.2.98/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:54.664454 jacksung-0.0.2.98/jacksung/
--rw-rw-rw-   0        0        0       24 2023-08-31 10:50:52.000000 jacksung-0.0.2.98/jacksung/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:54.676679 jacksung-0.0.2.98/jacksung/utils/
--rw-rw-rw-   0        0        0       17 2023-08-31 11:05:26.000000 jacksung-0.0.2.98/jacksung/utils/__init__.py
--rw-rw-rw-   0        0        0     1953 2024-04-02 09:10:13.000000 jacksung-0.0.2.98/jacksung/utils/base_db.py
--rw-rw-rw-   0        0        0     1869 2024-03-04 13:31:13.000000 jacksung-0.0.2.98/jacksung/utils/cache.py
--rw-rw-rw-   0        0        0     4744 2024-03-22 08:18:07.000000 jacksung-0.0.2.98/jacksung/utils/data_convert.py
--rw-rw-rw-   0        0        0     3982 2024-03-22 09:19:49.000000 jacksung-0.0.2.98/jacksung/utils/fastnumpy.py
--rw-rw-rw-   0        0        0      803 2023-09-01 08:33:07.000000 jacksung-0.0.2.98/jacksung/utils/hash.py
--rw-rw-rw-   0        0        0     3874 2024-04-02 12:31:48.000000 jacksung-0.0.2.98/jacksung/utils/image.py
--rw-rw-rw-   0        0        0     2705 2024-03-26 08:19:52.000000 jacksung-0.0.2.98/jacksung/utils/log.py
--rw-rw-rw-   0        0        0     5022 2023-12-19 05:11:54.000000 jacksung-0.0.2.98/jacksung/utils/login.py
--rw-rw-rw-   0        0        0     2253 2023-12-27 08:56:29.000000 jacksung-0.0.2.98/jacksung/utils/mean_std.py
--rw-rw-rw-   0        0        0     1836 2024-02-22 09:27:05.000000 jacksung-0.0.2.98/jacksung/utils/multi_task.py
--rw-rw-rw-   0        0        0     4371 2023-11-22 07:25:41.000000 jacksung-0.0.2.98/jacksung/utils/nvidia.py
--rw-rw-rw-   0        0        0     2200 2024-03-22 09:06:48.000000 jacksung-0.0.2.98/jacksung/utils/time.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:31:54.668540 jacksung-0.0.2.98/jacksung.egg-info/
--rw-rw-rw-   0        0        0     5413 2024-04-02 12:31:54.000000 jacksung-0.0.2.98/jacksung.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-04-02 12:31:54.000000 jacksung-0.0.2.98/jacksung.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:31:54.000000 jacksung-0.0.2.98/jacksung.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-02 12:31:54.000000 jacksung-0.0.2.98/jacksung.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       98 2024-04-02 12:31:54.000000 jacksung-0.0.2.98/jacksung.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 12:31:54.000000 jacksung-0.0.2.98/jacksung.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:31:54.677676 jacksung-0.0.2.98/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-04-02 12:31:48.000000 jacksung-0.0.2.98/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:09:01.649595 jacksung-0.0.2.99/
+-rw-rw-rw-   0        0        0    11558 2023-11-22 07:36:29.000000 jacksung-0.0.2.99/LICENSE
+-rw-rw-rw-   0        0        0     5413 2024-04-08 12:09:01.649595 jacksung-0.0.2.99/PKG-INFO
+-rw-rw-rw-   0        0        0     5255 2024-03-21 14:36:06.000000 jacksung-0.0.2.99/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 12:09:01.634904 jacksung-0.0.2.99/jacksung/
+-rw-rw-rw-   0        0        0       24 2023-08-31 10:50:52.000000 jacksung-0.0.2.99/jacksung/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:09:01.648598 jacksung-0.0.2.99/jacksung/utils/
+-rw-rw-rw-   0        0        0       17 2023-08-31 11:05:26.000000 jacksung-0.0.2.99/jacksung/utils/__init__.py
+-rw-rw-rw-   0        0        0     1953 2024-04-02 09:10:13.000000 jacksung-0.0.2.99/jacksung/utils/base_db.py
+-rw-rw-rw-   0        0        0     1869 2024-03-04 13:31:13.000000 jacksung-0.0.2.99/jacksung/utils/cache.py
+-rw-rw-rw-   0        0        0     4764 2024-04-08 12:08:19.000000 jacksung-0.0.2.99/jacksung/utils/data_convert.py
+-rw-rw-rw-   0        0        0     3982 2024-03-22 09:19:49.000000 jacksung-0.0.2.99/jacksung/utils/fastnumpy.py
+-rw-rw-rw-   0        0        0      803 2023-09-01 08:33:07.000000 jacksung-0.0.2.99/jacksung/utils/hash.py
+-rw-rw-rw-   0        0        0     3874 2024-04-02 12:31:48.000000 jacksung-0.0.2.99/jacksung/utils/image.py
+-rw-rw-rw-   0        0        0     2705 2024-03-26 08:19:52.000000 jacksung-0.0.2.99/jacksung/utils/log.py
+-rw-rw-rw-   0        0        0     5022 2023-12-19 05:11:54.000000 jacksung-0.0.2.99/jacksung/utils/login.py
+-rw-rw-rw-   0        0        0     2253 2023-12-27 08:56:29.000000 jacksung-0.0.2.99/jacksung/utils/mean_std.py
+-rw-rw-rw-   0        0        0     1836 2024-02-22 09:27:05.000000 jacksung-0.0.2.99/jacksung/utils/multi_task.py
+-rw-rw-rw-   0        0        0     4371 2023-11-22 07:25:41.000000 jacksung-0.0.2.99/jacksung/utils/nvidia.py
+-rw-rw-rw-   0        0        0     2200 2024-03-22 09:06:48.000000 jacksung-0.0.2.99/jacksung/utils/time.py
+drwxrwxrwx   0        0        0        0 2024-04-08 12:09:01.638866 jacksung-0.0.2.99/jacksung.egg-info/
+-rw-rw-rw-   0        0        0     5413 2024-04-08 12:09:01.000000 jacksung-0.0.2.99/jacksung.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-08 12:09:01.000000 jacksung-0.0.2.99/jacksung.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 12:09:01.000000 jacksung-0.0.2.99/jacksung.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-04-08 12:09:01.000000 jacksung-0.0.2.99/jacksung.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2024-04-08 12:09:01.000000 jacksung-0.0.2.99/jacksung.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-08 12:09:01.000000 jacksung-0.0.2.99/jacksung.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 12:09:01.649595 jacksung-0.0.2.99/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-04-08 12:08:28.000000 jacksung-0.0.2.99/setup.py
```

### Comparing `jacksung-0.0.2.98/LICENSE` & `jacksung-0.0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/PKG-INFO` & `jacksung-0.0.2.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacksung
-Version: 0.0.2.98
+Version: 0.0.2.99
 Author: Zijiang Song
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jacksung's utils
 Python version is required above 3.9.
```

### Comparing `jacksung-0.0.2.98/README.md` & `jacksung-0.0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/base_db.py` & `jacksung-0.0.2.99/jacksung/utils/base_db.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/cache.py` & `jacksung-0.0.2.99/jacksung/utils/cache.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/data_convert.py` & `jacksung-0.0.2.99/jacksung/utils/data_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         transform = from_origin(left, top, res1, res2)
         with rasterio.open(save_path, "w", driver="GTiff", width=w, height=h, count=1,
                            dtype=dtype if dtype else np_data.dtype, crs="EPSG:4326", transform=transform) as dst:
             dst.write(np_data, 1)
         print(f"GeoTIFF '{save_path}' generated with geographic coordinates.")
     else:
         # 将数据写入TIFF文件
-        with rasterio.open(save_path, "w", width=w, height=h, count=1, dtype=np_data.dtype) as dst:
+        with rasterio.open(save_path, "w", width=w, height=h, count=1, dtype=dtype if dtype else np_data.dtype) as dst:
             dst.write(np_data, 1)
         print(f"TIFF image saved as '{save_path}'")
 
 
 def np2tif(input_data, save_path='np2tif_dir', out_name='', left=None, top=None, x_res=None, y_res=None, dtype=None,
            dim_value=None, coord=None):
     if type(input_data) == str:
```

### Comparing `jacksung-0.0.2.98/jacksung/utils/fastnumpy.py` & `jacksung-0.0.2.99/jacksung/utils/fastnumpy.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/hash.py` & `jacksung-0.0.2.99/jacksung/utils/hash.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/image.py` & `jacksung-0.0.2.99/jacksung/utils/image.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/log.py` & `jacksung-0.0.2.99/jacksung/utils/log.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/login.py` & `jacksung-0.0.2.99/jacksung/utils/login.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/mean_std.py` & `jacksung-0.0.2.99/jacksung/utils/mean_std.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/multi_task.py` & `jacksung-0.0.2.99/jacksung/utils/multi_task.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/nvidia.py` & `jacksung-0.0.2.99/jacksung/utils/nvidia.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung/utils/time.py` & `jacksung-0.0.2.99/jacksung/utils/time.py`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/jacksung.egg-info/PKG-INFO` & `jacksung-0.0.2.99/jacksung.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jacksung
-Version: 0.0.2.98
+Version: 0.0.2.99
 Author: Zijiang Song
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Jacksung's utils
 Python version is required above 3.9.
```

### Comparing `jacksung-0.0.2.98/jacksung.egg-info/SOURCES.txt` & `jacksung-0.0.2.99/jacksung.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jacksung-0.0.2.98/setup.py` & `jacksung-0.0.2.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jacksung',
-    version='0.0.2.98',
+    version='0.0.2.99',
     author='Zijiang Song',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'tqdm',
         'requests',
```

