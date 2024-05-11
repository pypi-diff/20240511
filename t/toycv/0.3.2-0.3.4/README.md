# Comparing `tmp/toycv-0.3.2.tar.gz` & `tmp/toycv-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toycv-0.3.2.tar", last modified: Mon May  6 15:27:24 2024, max compression
+gzip compressed data, was "toycv-0.3.4.tar", last modified: Sat May 11 09:52:22 2024, max compression
```

## Comparing `toycv-0.3.2.tar` & `toycv-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.868742 toycv-0.3.2/
--rw-r--r--   0 xiangyang   (501) staff       (20)     1067 2024-03-16 04:38:20.000000 toycv-0.3.2/LICENSE
--rw-r--r--   0 xiangyang   (501) staff       (20)      214 2024-03-14 15:54:16.000000 toycv-0.3.2/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-06 15:27:24.868549 toycv-0.3.2/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)       84 2024-03-16 04:38:20.000000 toycv-0.3.2/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-06 15:27:22.000000 toycv-0.3.2/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2024-05-06 15:27:24.868795 toycv-0.3.2/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1958 2024-05-06 15:27:10.000000 toycv-0.3.2/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.866951 toycv-0.3.2/toycv/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 06:11:05.000000 toycv-0.3.2/toycv/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     8409 2024-05-06 06:23:06.000000 toycv-0.3.2/toycv/common.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.867736 toycv-0.3.2/toycv/file/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 20:37:55.000000 toycv-0.3.2/toycv/file/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)    12851 2024-05-06 06:24:19.000000 toycv-0.3.2/toycv/file/image.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1873 2024-04-09 03:48:43.000000 toycv-0.3.2/toycv/file/path.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      300 2024-04-26 09:56:43.000000 toycv-0.3.2/toycv/metrics.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.868171 toycv-0.3.2/toycv/pytorch/
--rw-r--r--   0 xiangyang   (501) staff       (20)      933 2024-03-17 20:12:36.000000 toycv-0.3.2/toycv/pytorch/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      417 2024-05-06 14:41:56.000000 toycv-0.3.2/toycv/pytorch/datasets.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2686 2024-05-06 14:44:19.000000 toycv-0.3.2/toycv/pytorch/transform.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      502 2024-04-26 08:43:20.000000 toycv-0.3.2/toycv/string.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.868315 toycv-0.3.2/toycv/visualization/
--rw-r--r--   0 xiangyang   (501) staff       (20)     7792 2024-05-06 07:31:32.000000 toycv-0.3.2/toycv/visualization/__init__.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-06 15:27:24.867446 toycv-0.3.2/toycv.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      439 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        6 2024-05-06 15:27:24.000000 toycv-0.3.2/toycv.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.418763 toycv-0.3.4/
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1067 2024-03-16 04:38:20.000000 toycv-0.3.4/LICENSE
+-rw-r--r--   0 xiangyang   (501) staff       (20)      214 2024-03-14 15:54:16.000000 toycv-0.3.4/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-11 09:52:22.418638 toycv-0.3.4/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)       84 2024-03-16 04:38:20.000000 toycv-0.3.4/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-11 09:52:22.000000 toycv-0.3.4/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2024-05-11 09:52:22.418807 toycv-0.3.4/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1958 2024-05-11 09:52:02.000000 toycv-0.3.4/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.416786 toycv-0.3.4/toycv/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 06:11:05.000000 toycv-0.3.4/toycv/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     8409 2024-05-06 06:23:06.000000 toycv-0.3.4/toycv/common.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.417869 toycv-0.3.4/toycv/file/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2024-03-17 20:37:55.000000 toycv-0.3.4/toycv/file/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)    14431 2024-05-11 09:11:37.000000 toycv-0.3.4/toycv/file/image.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1873 2024-04-09 03:48:43.000000 toycv-0.3.4/toycv/file/path.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      300 2024-04-26 09:56:43.000000 toycv-0.3.4/toycv/metrics.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.418369 toycv-0.3.4/toycv/pytorch/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      933 2024-03-17 20:12:36.000000 toycv-0.3.4/toycv/pytorch/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      737 2024-05-08 21:32:59.000000 toycv-0.3.4/toycv/pytorch/datasets.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2805 2024-05-11 01:21:47.000000 toycv-0.3.4/toycv/pytorch/transform.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      502 2024-04-26 08:43:20.000000 toycv-0.3.4/toycv/string.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.418486 toycv-0.3.4/toycv/visualization/
+-rw-r--r--   0 xiangyang   (501) staff       (20)     7887 2024-05-09 04:12:49.000000 toycv-0.3.4/toycv/visualization/__init__.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2024-05-11 09:52:22.417486 toycv-0.3.4/toycv.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      707 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      439 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)      123 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        6 2024-05-11 09:52:22.000000 toycv-0.3.4/toycv.egg-info/top_level.txt
```

### Comparing `toycv-0.3.2/LICENSE` & `toycv-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toycv-0.3.2/PKG-INFO` & `toycv-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toycv
-Version: 0.3.2
+Version: 0.3.4
 Summary: A simple and flexible tool for building and training neural network models.
 Home-page: https://github.com/coderelease
 Author: Yang Xiang
 Author-email: btk@qq.com
 License: MIT
 Keywords: toycv
 Classifier: Intended Audience :: Developers
```

### Comparing `toycv-0.3.2/setup.py` & `toycv-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='toycv',  # 包名
     python_requires='>=3.8.0',  # python环境
-    version='0.3.2',  # 包的版本
+    version='0.3.4',  # 包的版本
     description="A simple and flexible tool for building and training neural network models.",  # 包简介，显示在PyPI上
 
     long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
     long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
     # 作者相关信息
     author="Yang Xiang",
```

### Comparing `toycv-0.3.2/toycv/common.py` & `toycv-0.3.4/toycv/common.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.2/toycv/file/image.py` & `toycv-0.3.4/toycv/file/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -217,52 +217,58 @@
     """
     根据target_size，如果图像的比例和target_size不一致，则先按照target_size的比例切割图像，然后再进行缩放
     :param position:
     :param image: numpy.array, (h, w[, c])，输入图像。
     :param target_size: (h, w)，目标尺寸。
     :return: numpy.array, 缩放后的图像。
     """
+    ndim = image.ndim
     h, w = image.shape[:2]
     th, tw = target_size
 
     if h / w > th / tw:
         # 高度过长，需要先按照宽度切割
         new_h = int(w / tw * th)
         if position == "center":
             start = (h - new_h) // 2
-            image = image[start: start + new_h, :]
+            image = image[start: start + new_h, :, ...]
         elif position == "random":
             start = numpy.random.randint(0, h - new_h)
-            image = image[start: start + new_h, :]
+            image = image[start: start + new_h, :, ...]
         else:
             raise ValueError(f"Unknown position {position}.")
     else:
         # 宽度过长，需要先按照高度切割
         new_w = int(h / th * tw)
         if position == "center":
             start = (w - new_w) // 2
-            image = image[:, start: start + new_w]
+            image = image[:, start: start + new_w, ...]
         elif position == "random":
             start = numpy.random.randint(0, w - new_w)
-            image = image[:, start: start + new_w]
+            image = image[:, start: start + new_w, ...]
         else:
             raise ValueError(f"Unknown position {position}.")
 
     image = cv2.resize(image, (tw, th))
-    return image
+
+    if ndim == 3 and image.ndim == 2:
+        return image[..., numpy.newaxis]
+    else:
+        return image
 
 
 def keep_ratio_resize_video(video, target_size, position: Union[Literal["center", "random"],] = "center"):
     """
     根据target_size，如果视频的比例和target_size不一致，则先按照target_size的比例切割视频，然后再进行缩放
     :param position:
     :param video: numpy.array, (frames, h, w[, c])，输入视频。
     :param target_size: (h, w)，目标尺寸。
     :return: numpy.array, 缩放后的视频。
     """
+    ndim = video.ndim
     frames, h, w = video.shape[:3]
     th, tw = target_size
 
     if h / w > th / tw:
         # 高度过长，需要先按照宽度切割
         new_h = int(w / tw * th)
         if position == "center":
@@ -282,15 +288,21 @@
         elif position == "random":
             start = numpy.random.randint(0, w - new_w)
             video = video[:, :, start: start + new_w]
         else:
             raise ValueError(f"Unknown position {position}.")
 
     video = numpy.array([cv2.resize(frame, (tw, th)) for frame in video])
-    return video
+
+    if ndim == 3 and video.ndim == 2:
+        return video[..., numpy.newaxis]
+    elif ndim == 4 and video.ndim == 3:
+        return video[..., numpy.newaxis]
+    else:
+        return video
 
 
 def keep_ratio_resize(image_or_video, target_size, with_channel=True,
                       position: Union[Literal["center", "random"],] = "center"):
     """
     根据target_size，如果图像或视频的比例和target_size不一致，则先按照target_size的比例切割图像或视频，然后再进行缩放
     :param position: {"center", "random"}，默认为"center"，切割位置。
@@ -300,24 +312,29 @@
     :return: numpy.array, 缩放后的图像或视频。
     """
     if image_or_video.ndim == 2:
         return keep_ratio_resize_image(image_or_video, target_size, position)
     elif image_or_video.ndim == 3 and with_channel:
         return keep_ratio_resize_image(image_or_video, target_size, position)
     elif image_or_video.ndim == 3 and not with_channel:
-        return keep_ratio_resize_image(image_or_video, target_size, position)
+        return keep_ratio_resize_video(image_or_video, target_size, position)
     elif image_or_video.ndim == 4:
         return keep_ratio_resize_video(image_or_video, target_size, position)
     else:
         raise ValueError(f"image_or_video should be 3D or 4D. Got {image_or_video.ndim}D.")
 
 
-def to_grey(image_or_video: numpy.ndarray, with_channel=True):
+def pil_to_numpy(x):
+    return numpy.array(x)
+
+
+def to_grey(image_or_video: numpy.ndarray, with_channel=True, keep_dim=True):
     """
     Convert ndarray image or video to grey.
+    :param keep_dim: whether to keep the channel dimension.
     :param image_or_video:  numpy.ndarray, (h, w) or (h, w, c) or (frames, h, w, c).
     :param with_channel:  whether there is a channel dimension in the input.
     :return: numpy.ndarray, (h, w) or (h, w, 1) or (frames, h, w, 1).
     """
 
     if image_or_video.ndim == 2:
         # 已经是灰度图像
@@ -329,9 +346,47 @@
         result_image = image_or_video
     elif image_or_video.ndim == 4:
         result_image = numpy.mean(image_or_video, axis=-1)
     else:
         raise ValueError(
             f"image_or_video should be 2D (gray image), 3D (grey video or rgb image) or 4D (rgb video). "
             f"Got {image_or_video.ndim}D.")
+    if keep_dim:
+        return result_image[..., numpy.newaxis]
+    else:
+        return result_image
+
+
+def cv2_binary(image):
+    """
+    cv2二值化，对MNIST效果很好
+    :param image:
+    :return:
+    """
+    # img = cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)
+    # image = cv2.GaussianBlur(image, (5, 5), 0)
+    is_255 = numpy.max(image) > 1
+    is_float = image.dtype == numpy.float32 or image.dtype == numpy.float64
+    if not is_255:
+        image = (image * 255).astype(numpy.uint8)
+    if is_float:
+        image = image.astype(numpy.uint8)
+    # print(image.shape, image.dtype)
+    # 高斯模糊
+    image = cv2.GaussianBlur(image, (3, 3), 0)
+
+    # 直方图均衡化
+    equalized = cv2.equalizeHist(image)
+
+    # 全局 Otsu 二值化
+    _, global_otsu = cv2.threshold(equalized, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+
+    # 自适应阈值
+    adaptive_thresh = cv2.adaptiveThreshold(equalized, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 11, 2)
+
+    # 结合 Otsu 和自适应阈值的结果
+    combined = cv2.bitwise_and(global_otsu, adaptive_thresh)
+
+    if not is_255:
+        combined = combined / 255.0
 
-    return result_image[..., numpy.newaxis]
+    return combined
```

### Comparing `toycv-0.3.2/toycv/file/path.py` & `toycv-0.3.4/toycv/file/path.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.2/toycv/pytorch/__init__.py` & `toycv-0.3.4/toycv/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `toycv-0.3.2/toycv/pytorch/transform.py` & `toycv-0.3.4/toycv/pytorch/transform.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,17 @@
     If the input is 2D with shape (h, w), the output will be (h, w).
     If the input is 3D with shape (c, h, w), the output will be (h, w, c).
     If the input is 4D with shape (frames, c, h, w), the output will be (frames, h, w, c).
     :param with_channel: whether there is a channel dimension in the input.
     :param image_or_video_tensor: torch.Tensor with shape (c, h, w) or (frames, c, h, w).
     :return: numpy.ndarray with shape (h, w, c) or (frames, h, w, c).
     """
+    image_or_video_tensor = image_or_video_tensor.detach()
     if isinstance(image_or_video_tensor, Tensor):
+        image_or_video_tensor = image_or_video_tensor.cpu()
         if image_or_video_tensor.dim() == 2:
             return image_or_video_tensor.numpy()
         elif image_or_video_tensor.dim() == 3 and with_channel:
             return image_or_video_tensor.permute(1, 2, 0).numpy()
         elif image_or_video_tensor.dim() == 3 and not with_channel:
             return image_or_video_tensor.numpy()
         elif image_or_video_tensor.dim() == 4:
```

### Comparing `toycv-0.3.2/toycv/visualization/__init__.py` & `toycv-0.3.4/toycv/visualization/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,18 @@
     col_num = min(col_num, images_count)
 
     each_size = (each_size, each_size * 0.875) if isinstance(each_size, int) else each_size
 
     subtitles = [None] * images_count if subtitles is None else subtitles + [None] * (images_count - len(subtitles))
 
     row_num = (images_count + col_num - 1) // col_num
+    plt.subplots_adjust(top=0.85)  # 调整顶部间距
     fig, axs = plt.subplots(nrows=row_num, ncols=col_num, squeeze=False)
-    if title:
-        fig.suptitle(title)
+    if title is not None:
+        fig.suptitle(title, fontsize=each_size[0] * 4)
 
     fig.set_size_inches(each_size[0] * col_num, each_size[1] * row_num)
 
     for ax, image, subtitle in zip(axs.ravel(), images, subtitles):
         ax.set_title(subtitle, fontsize=each_size[0] * 3)
         ax.imshow(image, cmap='gray' if len(image.shape) == 2 else None)
         ax.axis('off')
```

### Comparing `toycv-0.3.2/toycv.egg-info/PKG-INFO` & `toycv-0.3.4/toycv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toycv
-Version: 0.3.2
+Version: 0.3.4
 Summary: A simple and flexible tool for building and training neural network models.
 Home-page: https://github.com/coderelease
 Author: Yang Xiang
 Author-email: btk@qq.com
 License: MIT
 Keywords: toycv
 Classifier: Intended Audience :: Developers
```

