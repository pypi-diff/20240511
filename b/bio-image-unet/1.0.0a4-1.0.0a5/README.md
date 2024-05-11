# Comparing `tmp/bio-image-unet-1.0.0a4.tar.gz` & `tmp/bio-image-unet-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-image-unet-1.0.0a4.tar", max compression
+gzip compressed data, was "bio-image-unet-1.0.0a5.tar", max compression
```

## Comparing `bio-image-unet-1.0.0a4.tar` & `bio-image-unet-1.0.0a5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1072 2022-06-27 10:34:59.772125 bio-image-unet-1.0.0a4/LICENSE
--rw-r--r--   0        0        0      544 2024-05-05 12:32:15.034287 bio-image-unet-1.0.0a4/README.md
--rw-r--r--   0        0        0     6148 2022-11-11 16:07:45.185829 bio-image-unet-1.0.0a4/biu/.DS_Store
--rw-r--r--   0        0        0        0 2024-04-12 12:06:47.828861 bio-image-unet-1.0.0a4/biu/__init__.py
--rw-r--r--   0        0        0       32 2022-06-27 10:34:59.772305 bio-image-unet-1.0.0a4/biu/progress/__init__.py
--rw-r--r--   0        0        0      196 2022-06-27 10:34:59.772393 bio-image-unet-1.0.0a4/biu/progress/note.txt
--rw-r--r--   0        0        0     5969 2022-11-10 16:09:23.098804 bio-image-unet-1.0.0a4/biu/progress/progressnotifier.py
--rw-r--r--   0        0        0     6148 2022-11-11 15:52:42.902284 bio-image-unet-1.0.0a4/biu/siam_unet/.DS_Store
--rw-r--r--   0        0        0      610 2024-04-12 12:06:47.829705 bio-image-unet-1.0.0a4/biu/siam_unet/__init__.py
--rw-r--r--   0        0        0    13741 2024-04-12 12:06:47.829913 bio-image-unet-1.0.0a4/biu/siam_unet/data.py
--rw-r--r--   0        0        0      156 2022-06-27 10:34:59.773322 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/__cpu_count__.py
--rw-r--r--   0        0        0      656 2022-06-27 10:34:59.773399 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/__md5sum__.py
--rw-r--r--   0        0        0     1318 2022-06-27 10:34:59.773503 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/average_tifs.py
--rw-r--r--   0        0        0     1745 2022-06-27 10:34:59.773598 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/create_pixel_value_histogram.py
--rw-r--r--   0        0        0      257 2022-06-27 10:34:59.773681 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/cuda_test.py
--rw-r--r--   0        0        0     1397 2022-06-27 10:34:59.773959 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/extract_frame_of_movie.py
--rw-r--r--   0        0        0     4669 2022-06-27 10:34:59.774141 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/find_frame_of_image.py
--rw-r--r--   0        0        0      699 2022-06-27 10:34:59.774260 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_plain_image.py
--rw-r--r--   0        0        0     5044 2022-09-14 12:28:05.579071 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py
--rw-r--r--   0        0        0     1442 2022-06-27 10:34:59.774530 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/low_mem_tif_utils.py
--rw-r--r--   0        0        0     1280 2022-06-27 10:34:59.774638 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/threshold_images.py
--rw-r--r--   0        0        0     3196 2022-06-27 10:34:59.774817 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/tif_to_mp4.py
--rw-r--r--   0        0        0     3914 2022-06-27 10:34:59.774949 bio-image-unet-1.0.0a4/biu/siam_unet/helpers/util.py
--rw-r--r--   0        0        0     3539 2024-05-10 17:20:33.893986 bio-image-unet-1.0.0a4/biu/siam_unet/losses.py
--rw-r--r--   0        0        0    11386 2024-05-10 17:20:33.894445 bio-image-unet-1.0.0a4/biu/siam_unet/predict.py
--rw-r--r--   0        0        0     5422 2024-05-05 12:32:15.035770 bio-image-unet-1.0.0a4/biu/siam_unet/siam_unet.py
--rw-r--r--   0        0        0     8216 2024-05-10 17:20:33.894666 bio-image-unet-1.0.0a4/biu/siam_unet/train.py
--rw-r--r--   0        0        0      329 2024-04-12 12:06:47.830762 bio-image-unet-1.0.0a4/biu/unet/__init__.py
--rw-r--r--   0        0        0     7148 2024-05-05 12:32:15.036490 bio-image-unet-1.0.0a4/biu/unet/attention_unet.py
--rw-r--r--   0        0        0     3456 2022-09-14 12:28:05.579805 bio-image-unet-1.0.0a4/biu/unet/baby_unet.py
--rw-r--r--   0        0        0    12210 2024-05-06 09:15:26.910839 bio-image-unet-1.0.0a4/biu/unet/data.py
--rw-r--r--   0        0        0     2868 2024-04-12 12:06:47.831488 bio-image-unet-1.0.0a4/biu/unet/losses.py
--rw-r--r--   0        0        0    10592 2024-05-10 17:20:33.894890 bio-image-unet-1.0.0a4/biu/unet/predict.py
--rw-r--r--   0        0        0     9362 2024-05-10 17:20:33.895131 bio-image-unet-1.0.0a4/biu/unet/train.py
--rw-r--r--   0        0        0     4298 2024-04-12 12:06:47.831999 bio-image-unet-1.0.0a4/biu/unet/unet.py
--rw-r--r--   0        0        0     4052 2024-05-06 09:15:26.911589 bio-image-unet-1.0.0a4/biu/unet/unet_v0.py
--rw-r--r--   0        0        0      291 2024-05-05 12:32:15.037423 bio-image-unet-1.0.0a4/biu/unet3d/__init__.py
--rw-r--r--   0        0        0    11989 2024-05-05 12:32:15.037643 bio-image-unet-1.0.0a4/biu/unet3d/data.py
--rw-r--r--   0        0        0     2868 2024-05-05 12:32:15.037758 bio-image-unet-1.0.0a4/biu/unet3d/losses.py
--rw-r--r--   0        0        0     8761 2024-05-10 17:20:33.895336 bio-image-unet-1.0.0a4/biu/unet3d/predict.py
--rw-r--r--   0        0        0     9874 2024-05-10 17:20:33.895529 bio-image-unet-1.0.0a4/biu/unet3d/train.py
--rw-r--r--   0        0        0     3956 2024-05-10 17:20:33.895730 bio-image-unet-1.0.0a4/biu/unet3d/unet3d.py
--rw-r--r--   0        0        0       21 2024-04-12 12:06:47.832254 bio-image-unet-1.0.0a4/biu/utils/__init__.py
--rw-r--r--   0        0        0     5039 2024-05-10 17:20:33.896485 bio-image-unet-1.0.0a4/biu/utils/test.py
--rw-r--r--   0        0        0     2264 2024-04-12 12:06:47.832460 bio-image-unet-1.0.0a4/biu/utils/utils.py
--rw-r--r--   0        0        0      636 2024-05-10 17:20:49.957960 bio-image-unet-1.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     1481 2024-05-10 17:20:55.743171 bio-image-unet-1.0.0a4/setup.py
--rw-r--r--   0        0        0     1414 2024-05-10 17:20:55.743409 bio-image-unet-1.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-27 10:34:59.772125 bio-image-unet-1.0.0a5/LICENSE
+-rw-r--r--   0        0        0      544 2024-05-05 12:32:15.034287 bio-image-unet-1.0.0a5/README.md
+-rw-r--r--   0        0        0     6148 2022-11-11 16:07:45.185829 bio-image-unet-1.0.0a5/biu/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-12 12:06:47.828861 bio-image-unet-1.0.0a5/biu/__init__.py
+-rw-r--r--   0        0        0       32 2022-06-27 10:34:59.772305 bio-image-unet-1.0.0a5/biu/progress/__init__.py
+-rw-r--r--   0        0        0      196 2022-06-27 10:34:59.772393 bio-image-unet-1.0.0a5/biu/progress/note.txt
+-rw-r--r--   0        0        0     5969 2022-11-10 16:09:23.098804 bio-image-unet-1.0.0a5/biu/progress/progressnotifier.py
+-rw-r--r--   0        0        0     6148 2022-11-11 15:52:42.902284 bio-image-unet-1.0.0a5/biu/siam_unet/.DS_Store
+-rw-r--r--   0        0        0      610 2024-04-12 12:06:47.829705 bio-image-unet-1.0.0a5/biu/siam_unet/__init__.py
+-rw-r--r--   0        0        0    13741 2024-04-12 12:06:47.829913 bio-image-unet-1.0.0a5/biu/siam_unet/data.py
+-rw-r--r--   0        0        0      156 2022-06-27 10:34:59.773322 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/__cpu_count__.py
+-rw-r--r--   0        0        0      656 2022-06-27 10:34:59.773399 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/__md5sum__.py
+-rw-r--r--   0        0        0     1318 2022-06-27 10:34:59.773503 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/average_tifs.py
+-rw-r--r--   0        0        0     1745 2022-06-27 10:34:59.773598 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/create_pixel_value_histogram.py
+-rw-r--r--   0        0        0      257 2022-06-27 10:34:59.773681 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/cuda_test.py
+-rw-r--r--   0        0        0     1397 2022-06-27 10:34:59.773959 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/extract_frame_of_movie.py
+-rw-r--r--   0        0        0     4669 2022-06-27 10:34:59.774141 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/find_frame_of_image.py
+-rw-r--r--   0        0        0      699 2022-06-27 10:34:59.774260 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/generate_plain_image.py
+-rw-r--r--   0        0        0     5044 2022-09-14 12:28:05.579071 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py
+-rw-r--r--   0        0        0     1442 2022-06-27 10:34:59.774530 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/low_mem_tif_utils.py
+-rw-r--r--   0        0        0     1280 2022-06-27 10:34:59.774638 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/threshold_images.py
+-rw-r--r--   0        0        0     3196 2022-06-27 10:34:59.774817 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/tif_to_mp4.py
+-rw-r--r--   0        0        0     3914 2022-06-27 10:34:59.774949 bio-image-unet-1.0.0a5/biu/siam_unet/helpers/util.py
+-rw-r--r--   0        0        0     3539 2024-05-10 17:20:33.893986 bio-image-unet-1.0.0a5/biu/siam_unet/losses.py
+-rw-r--r--   0        0        0    11386 2024-05-10 17:20:33.894445 bio-image-unet-1.0.0a5/biu/siam_unet/predict.py
+-rw-r--r--   0        0        0     5422 2024-05-05 12:32:15.035770 bio-image-unet-1.0.0a5/biu/siam_unet/siam_unet.py
+-rw-r--r--   0        0        0     8216 2024-05-10 17:20:33.894666 bio-image-unet-1.0.0a5/biu/siam_unet/train.py
+-rw-r--r--   0        0        0      329 2024-04-12 12:06:47.830762 bio-image-unet-1.0.0a5/biu/unet/__init__.py
+-rw-r--r--   0        0        0     7148 2024-05-05 12:32:15.036490 bio-image-unet-1.0.0a5/biu/unet/attention_unet.py
+-rw-r--r--   0        0        0     3456 2022-09-14 12:28:05.579805 bio-image-unet-1.0.0a5/biu/unet/baby_unet.py
+-rw-r--r--   0        0        0    12210 2024-05-06 09:15:26.910839 bio-image-unet-1.0.0a5/biu/unet/data.py
+-rw-r--r--   0        0        0     2868 2024-04-12 12:06:47.831488 bio-image-unet-1.0.0a5/biu/unet/losses.py
+-rw-r--r--   0        0        0    10592 2024-05-10 17:20:33.894890 bio-image-unet-1.0.0a5/biu/unet/predict.py
+-rw-r--r--   0        0        0     9362 2024-05-10 17:20:33.895131 bio-image-unet-1.0.0a5/biu/unet/train.py
+-rw-r--r--   0        0        0     4298 2024-04-12 12:06:47.831999 bio-image-unet-1.0.0a5/biu/unet/unet.py
+-rw-r--r--   0        0        0     4052 2024-05-06 09:15:26.911589 bio-image-unet-1.0.0a5/biu/unet/unet_v0.py
+-rw-r--r--   0        0        0      291 2024-05-05 12:32:15.037423 bio-image-unet-1.0.0a5/biu/unet3d/__init__.py
+-rw-r--r--   0        0        0    11989 2024-05-05 12:32:15.037643 bio-image-unet-1.0.0a5/biu/unet3d/data.py
+-rw-r--r--   0        0        0     2868 2024-05-05 12:32:15.037758 bio-image-unet-1.0.0a5/biu/unet3d/losses.py
+-rw-r--r--   0        0        0     8965 2024-05-11 15:34:16.672076 bio-image-unet-1.0.0a5/biu/unet3d/predict.py
+-rw-r--r--   0        0        0     9988 2024-05-11 15:34:16.672356 bio-image-unet-1.0.0a5/biu/unet3d/train.py
+-rw-r--r--   0        0        0     3956 2024-05-10 17:20:33.895730 bio-image-unet-1.0.0a5/biu/unet3d/unet3d.py
+-rw-r--r--   0        0        0       21 2024-04-12 12:06:47.832254 bio-image-unet-1.0.0a5/biu/utils/__init__.py
+-rw-r--r--   0        0        0     5039 2024-05-11 15:50:29.756224 bio-image-unet-1.0.0a5/biu/utils/test.py
+-rw-r--r--   0        0        0     2264 2024-04-12 12:06:47.832460 bio-image-unet-1.0.0a5/biu/utils/utils.py
+-rw-r--r--   0        0        0      636 2024-05-11 15:50:57.875970 bio-image-unet-1.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     1481 2024-05-11 15:51:03.251852 bio-image-unet-1.0.0a5/setup.py
+-rw-r--r--   0        0        0     1414 2024-05-11 15:51:03.252033 bio-image-unet-1.0.0a5/PKG-INFO
```

### Comparing `bio-image-unet-1.0.0a4/LICENSE` & `bio-image-unet-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/README.md` & `bio-image-unet-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/.DS_Store` & `bio-image-unet-1.0.0a5/biu/.DS_Store`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/progress/progressnotifier.py` & `bio-image-unet-1.0.0a5/biu/progress/progressnotifier.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/.DS_Store` & `bio-image-unet-1.0.0a5/biu/siam_unet/.DS_Store`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/__init__.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/__init__.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/data.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/data.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/__md5sum__.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/__md5sum__.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/average_tifs.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/average_tifs.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/create_pixel_value_histogram.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/create_pixel_value_histogram.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/extract_frame_of_movie.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/extract_frame_of_movie.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/find_frame_of_image.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/find_frame_of_image.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_plain_image.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/generate_plain_image.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/generate_siam_unet_input_imgs.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/low_mem_tif_utils.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/low_mem_tif_utils.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/threshold_images.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/threshold_images.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/tif_to_mp4.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/tif_to_mp4.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/helpers/util.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/helpers/util.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/losses.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/losses.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/predict.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/predict.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/siam_unet.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/siam_unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/siam_unet/train.py` & `bio-image-unet-1.0.0a5/biu/siam_unet/train.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/attention_unet.py` & `bio-image-unet-1.0.0a5/biu/unet/attention_unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/baby_unet.py` & `bio-image-unet-1.0.0a5/biu/unet/baby_unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/data.py` & `bio-image-unet-1.0.0a5/biu/unet/data.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/losses.py` & `bio-image-unet-1.0.0a5/biu/unet/losses.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/predict.py` & `bio-image-unet-1.0.0a5/biu/unet/predict.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/train.py` & `bio-image-unet-1.0.0a5/biu/unet/train.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/unet.py` & `bio-image-unet-1.0.0a5/biu/unet/unet.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet/unet_v0.py` & `bio-image-unet-1.0.0a5/biu/unet/unet_v0.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet3d/data.py` & `bio-image-unet-1.0.0a5/biu/unet3d/data.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet3d/losses.py` & `bio-image-unet-1.0.0a5/biu/unet3d/losses.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/unet3d/predict.py` & `bio-image-unet-1.0.0a5/biu/unet3d/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 from .unet3d import UNet3D
 from ..progress import ProgressNotifier
 from ..utils import save_as_tif, get_device
 
 
 class Predict:
-    """Class for prediction of movies and images with U-Net"""
+    """Class for prediction of movies and images with 3D U-Net"""
 
     def __init__(self, vol, result_name, model_params, network=UNet3D, resize_dim=(512, 512),
                  invert=False, normalization_mode='single', clip_threshold=(0., 99.8), add_patch=0,
                  normalize_result=False, progress_bar=True, device: Union[torch.device, str] = 'auto',
                  progress_notifier: ProgressNotifier = ProgressNotifier.progress_notifier_tqdm()):
         """
-        Prediction of tif files with standard 2D U-Net
+        Prediction of tif files with 3D U-Net
 
         1) Loading file and preprocess (normalization)
         2) Resizing of images into patches with resize_dim
         3) Prediction with U-Net
         4) Stitching of predicted patches and averaging of overlapping regions
 
         Parameters
@@ -75,16 +75,19 @@
         vol = self.__reshape_data(vol)
         vol = self.__preprocess(vol)
         patches = self.__split(vol)
         del vol
 
         # load model and predict data
         self.model_params = torch.load(model_params, map_location=self.device)
+        if 'use_interpolation' not in self.model_params.keys():
+            self.model_params['use_interpolation'] = False
         self.model = network(n_filter=self.model_params['n_filter'], in_channels=self.model_params['in_channels'],
-                             out_channels=self.model_params['out_channels']).to(self.device)
+                             out_channels=self.model_params['out_channels'],
+                             use_interpolation=self.model_params['use_interpolation']).to(self.device)
         self.model.load_state_dict(self.model_params['state_dict'])
         self.model.eval()
         result_patches = self.__predict(patches, progress_notifier)
         del patches, self.model
 
         # stitch patches (mean of overlapped regions)
         vol_result = self.__stitch(result_patches)
```

### Comparing `bio-image-unet-1.0.0a4/biu/unet3d/train.py` & `bio-image-unet-1.0.0a5/biu/unet3d/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         self.save_iter = save_iter
         self.loss_function = loss_function
         self.loss_params = loss_params
         self.time_loss_weight = time_loss_weight
         self.n_filter = n_filter
         self.in_channels = in_channels
         self.out_channels = out_channels
+        self.use_interpolation = use_interpolation
         if channel_weights is None:
             self.channel_weights = torch.ones(out_channels)
         else:
             self.channel_weights = torch.tensor(channel_weights)
 
         # split training and validation data
         num_val = int(len(dataset) * val_split)
@@ -108,14 +109,15 @@
         self.save_name = save_name
         self.params = {'optimizer': self.optimizer.state_dict(),
                        'lr': self.lr,
                        'loss_function': self.loss_function,
                        'loss_params': self.loss_params,
                        'time_loss_weight': self.time_loss_weight,
                        'n_filter': self.n_filter,
+                       'use_interpolation': use_interpolation,
                        'dilation': dilation, 'batch_size': self.batch_size,
                        'augmentation': self.data.aug_factor,
                        'clip_threshold': self.data.clip_threshold,
                        'noise_amp': self.data.noise_amp,
                        'brightness_contrast': self.data.brightness_contrast,
                        'shiftscalerotate': self.data.shiftscalerotate,
                        'in_channels': in_channels, 'out_channels': out_channels}
```

### Comparing `bio-image-unet-1.0.0a4/biu/unet3d/unet3d.py` & `bio-image-unet-1.0.0a5/biu/unet3d/unet3d.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/utils/test.py` & `bio-image-unet-1.0.0a5/biu/utils/test.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/biu/utils/utils.py` & `bio-image-unet-1.0.0a5/biu/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bio-image-unet-1.0.0a4/pyproject.toml` & `bio-image-unet-1.0.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "bio-image-unet"
 packages = [
     { include = "biu" }
 ]
-version = "1.0.0-alpha.4"
+version = "1.0.0-alpha.5"
 description = "Implementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation"
 authors = ["Daniel Haertter", "Yuxi Long"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/danihae/bio-image-unet"
 
 [tool.poetry.dependencies]
```

### Comparing `bio-image-unet-1.0.0a4/setup.py` & `bio-image-unet-1.0.0a5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'scikit-image>0.18,<1.0',
  'tifffile',
  'torch>=2.0.0,<3.0.0',
  'tqdm>=4.61,<5.0']
 
 setup_kwargs = {
     'name': 'bio-image-unet',
-    'version': '1.0.0a4',
+    'version': '1.0.0a5',
     'description': 'Implementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation',
     'long_description': '# Bio Image U-Net\n\nImplementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation\n\n\n## Installation\n### PyPI\n``pip install bio-image-unet``\n### GitHub\n``pip install git+https://github.com/danihae/bio-image-unet``\n\n## Usage example\nImport package with ``import biu``\n\n[iPython Notebook for getting started with U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_unet.ipynb) \\\n[iPython Notebook for getting started with Siam U-Net](https://github.com/danihae/bio-image-unet/blob/master/using_siam_unet.ipynb)\n',
     'author': 'Daniel Haertter',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/danihae/bio-image-unet',
```

### Comparing `bio-image-unet-1.0.0a4/PKG-INFO` & `bio-image-unet-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-image-unet
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: Implementations of U-Net, Siam U-Net and 3D U-Net for biological image segmentation
 Home-page: https://github.com/danihae/bio-image-unet
 License: MIT
 Author: Daniel Haertter
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

