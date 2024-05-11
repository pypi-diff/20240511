# Comparing `tmp/vr180_convert-0.2.0.tar.gz` & `tmp/vr180_convert-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vr180_convert-0.2.0.tar", max compression
+gzip compressed data, was "vr180_convert-0.2.1.tar", max compression
```

## Comparing `vr180_convert-0.2.0.tar` & `vr180_convert-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-04-30 08:11:19.111633 vr180_convert-0.2.0/LICENSE
--rw-r--r--   0        0        0     8872 2024-04-30 08:11:19.111633 vr180_convert-0.2.0/README.md
--rw-r--r--   0        0        0     3834 2024-04-30 08:11:19.931634 vr180_convert-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      707 2024-04-30 08:11:19.935634 vr180_convert-0.2.0/src/vr180_convert/__init__.py
--rw-r--r--   0        0        0      113 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/__main__.py
--rw-r--r--   0        0        0    12797 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/cli.py
--rw-r--r--   0        0        0        0 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/py.typed
--rw-r--r--   0        0        0    12090 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/remapper.py
--rw-r--r--   0        0        0     1889 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/testing.py
--rw-r--r--   0        0        0    18069 2024-04-30 08:11:19.127633 vr180_convert-0.2.0/src/vr180_convert/transformer.py
--rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 vr180_convert-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-11 03:21:10.758015 vr180_convert-0.2.1/LICENSE
+-rw-r--r--   0        0        0    10741 2024-05-11 03:21:10.758015 vr180_convert-0.2.1/README.md
+-rw-r--r--   0        0        0     3836 2024-05-11 03:21:11.642016 vr180_convert-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-05-11 03:21:11.642016 vr180_convert-0.2.1/src/vr180_convert/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/__main__.py
+-rw-r--r--   0        0        0    12817 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/cli.py
+-rw-r--r--   0        0        0        0 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/py.typed
+-rw-r--r--   0        0        0    12090 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/remapper.py
+-rw-r--r--   0        0        0     1889 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/testing.py
+-rw-r--r--   0        0        0    18069 2024-05-11 03:21:10.774015 vr180_convert-0.2.1/src/vr180_convert/transformer.py
+-rw-r--r--   0        0        0    12139 1970-01-01 00:00:00.000000 vr180_convert-0.2.1/PKG-INFO
```

### Comparing `vr180_convert-0.2.0/LICENSE` & `vr180_convert-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.0/README.md` & `vr180_convert-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 
 | left.jpg                       | right.jpg                       | Output                                               |
 | ------------------------------ | ------------------------------- | ---------------------------------------------------- |
 | ![left](docs/_static/test.jpg) | ![right](docs/_static/test.jpg) | ![output](docs/_static/test.lr.PolynomialScaler.jpg) |
 
 If left and right image paths are the same, the image is divided into two halves (left and right, SBS) and processed as if they were separate images.
 
+## Advanced usage
+
 ### Automatic image search
 
 If one of left or right image path is a directory, the program will search for the closest image (in terms of creation time) in the other directory.
 
 ```shell
 v1c lr left.jpg right_dir
 v1c lr left_dir right.jpg
@@ -74,64 +76,71 @@
 It is recommended to synchronize the clocks of the cameras before shooting. However, it can be adjusted by specifying `-ac` option.
 
 ```shell
 v1c lr left.jpg right_dir -ac 1 # the clock of the right camera is 1 second faster / ahead
 v1c lr left_dir right.jpg -ac 1 # the clock of the right camera is 1 second faster / ahead
 ```
 
-### Custom conversion model
-
-You can also specify the conversion model by adding Python code directly to the `--transformer` option:
-
-```shell
-v1c lr left.jpg right.jpg ---transformer "EquirectangularEncoder() * Euclidean3DRotator(from_rotation_vector([0, np.pi / 4, 0])) * FisheyeDecoder("equidistant")"
-```
-
-If tuple, the first transformer is applied to the left image and the second transformer is applied to the right image. If a single transformer is given, it is applied to both images.
-
-Please refer to the [API documentation](https://vr180-convert.readthedocs.io/) for the available transformers and their parameters.
-For `from_rotation_vector`, please refer to the [numpy-quaternion documentation](https://quaternion.readthedocs.io/en/latest/Package%20API%3A/quaternion/#from_rotation_vector).
-
 ### Radius estimation
 
 The radius of the non-black area of the input image is assumed by counting black pixels by default, but it would be better to specify it manually to get stable results:
 
 ```shell
 v1c lr left.jpg right.jpg --radius 1000
 v1c lr left.jpg right.jpg --radius max # min(width, height) / 2
 ```
 
 ### Calibration
 
-Rotation matching using the least-squares method can be performed by clicking corresponding points that can be regarded as infinitely far away from the camera.
+[Rotation matching using the least-squares method](https://lisyarus.github.io/blog/posts/3d-shape-matching-with-quaternions.html) can be performed by clicking corresponding points that can be regarded as infinitely far away from the camera.
 
 ```shell
 v1c lr left.jpg right.jpg --automatch gui
 ```
 
 You can also specify the corresponding points manually:
 
 ```shell
 v1c lr left.jpg right.jpg --automatch "0,0;0,0;1,1;1,1" # left_x1,left_y1;right_x1,right_y1;...
 ```
 
+$$
+a_k, b_k \in \mathbb{R}^3,
+\min_{R \in SO(3)} \sum_k \|\|R a_k - b_k\|\|^2
+$$
+
+### Anaglyph
+
 `--merge` option (which exports as [anaglyph](https://en.wikipedia.org/wiki/Anaglyph_3D) image) can be used to check if the calibration is successful by checking if the infinitely far points are overlapped.
 
 ```shell
 v1c lr left.jpg right.jpg --automatch gui --merge
 ```
 
 ### Swap
 
-If the camera is mounted upside down, you can swap the left and right images for conversion:
+If the camera is mounted upside down, you can simply use the `--swap` option without changing the transformer or other parameters:
 
 ```shell
 v1c lr left.jpg right.jpg --swap
 ```
 
+### Custom conversion model
+
+You can also specify the conversion model by adding Python code directly to the `--transformer` option:
+
+```shell
+v1c lr left.jpg right.jpg --transformer 'EquirectangularEncoder() * Euclidean3DRotator(from_rotation_vector([0, np.pi / 4, 0])) * FisheyeDecoder("equidistant")'
+```
+
+If tuple, the first transformer is applied to the left image and the second transformer is applied to the right image. If a single transformer is given, it is applied to both images.
+
+Please refer to the [API documentation](https://vr180-convert.readthedocs.io/) for the available transformers and their parameters.
+For `from_rotation_vector`, please refer to the [numpy-quaternion documentation](https://quaternion.readthedocs.io/en/latest/Package%20API%3A/quaternion/#from_rotation_vector).
+
 ### Single image conversion
 
 To convert a single image, use `v1c s` instead.
 
 ### Help
 
 For more information, please refer to the help or API documentation:
@@ -155,19 +164,46 @@
     ) -> tuple[NDArray, NDArray]:
         return theta**0.98 + theta**1.01, roll
 
 transformer = EquirectangularEncoder() * MyTransformer() * FisheyeDecoder("equidistant")
 apply_lr(transformer, left_path="left.jpg", right_path="right.jpg", out_path="output.jpg")
 ```
 
-## How to edit images
+## Tips
+
+### How to determine which image is left or right
+
+<!--
+- In the left image, the subject faces more to the right.
+- In the right image, the subject faces more to the left.
+- In other words, in a SBS image, the subject is oriented toward the center.
+
+In anaglyph images,
+
+- The left eye is covered with a red film, so the portion for the left eye is shown in blue.
+- The right eye is covered with a blue film, so the portion for the right eye is shown in red.
+| Film Color          | <span style="color:red">Red</span>   | <span style="color:blue">Blue</span> |
+| Anaglyph Color      | <span style="color:blue">Blue</span> | <span style="color:red">Red</span>   |
+-->
+
+|                     | Left                        | Right                       |
+| ------------------- | --------------------------- | --------------------------- |
+| Subject Orientation | Right                       | Left                        |
+| Film Color          | ${\color{red}\text{Red}}$   | ${\color{blue}\text{Blue}}$ |
+| Anaglyph Color      | ${\color{blue}\text{Blue}}$ | ${\color{red}\text{Red}}$   |
+
+- In a SBS image, the subject is oriented toward the center.
+
+### How to edit images
+
+This program cannot read RAW files. To deal with white-outs, etc., it is required to process each image with a program such as Photoshop, Lightroom, [RawTherapee](https://rawtherapee.com/downloads/), [Darktable](https://www.darktable.org/install/), etc.
 
-This program cannot read RAW files. To deal with white-outs, etc., it is recommended to process the image in Photoshop or other software first.
+However, this is so exhaustive, so it is recommended to take the images with jpeg format, being careful not to overexpose the images, and convert them with this program, then use Lightroom, [RawTherapee](https://rawtherapee.com/downloads/), [Darktable](https://www.darktable.org/install/) or other software to adjust colors and exposure, etc.
 
-### Example of processing in Photoshop
+#### Example of processing in Photoshop (Exquisite editing)
 
 1. Open one of the images just for specifying the canvas size.
 2. Add each image as Smart Objects (`LRaw`, `RRaw`) and make **minimal** corrections to match the exposure using `Camera Raw Filter`.
 3. Make each Smart Object into Smart Objects (`L`, `R`) again and do any image-dependent processing, such as removing the background.
 4. Make both images into a single Smart Object (`P`) and process them as a whole.
 5. Delete the background image created in step 1.
 6. Export as a PNG file.
```

### Comparing `vr180_convert-0.2.0/pyproject.toml` & `vr180_convert-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vr180-convert"
-version = "0.2.0"
+version = "0.2.1"
 description = "Simple VR180 image converter"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/vr180-convert"
 documentation = "https://vr180-convert.readthedocs.io"
 classifiers = [
@@ -34,15 +34,15 @@
 attrs = "^23.2.0"
 scikit-learn = "^1.4.2"
 numpy-quaternion = "^2023.0.3"
 strenum = "^0.4.15"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
-pytest-cov = "^3.0"
+pytest-cov = "^5.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = { version = ">=0.16", python = ">=3.11"}
 sphinx = { version = ">=4.0", python = ">=3.11"}
```

### Comparing `vr180_convert-0.2.0/src/vr180_convert/__init__.py` & `vr180_convert-0.2.1/src/vr180_convert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 from .remapper import apply, apply_lr, get_map
 from .transformer import (
     DenormalizeTransformer,
     EquirectangularEncoder,
     Euclidean3DRotator,
     Euclidean3DTransformer,
     FisheyeDecoder,
```

### Comparing `vr180_convert-0.2.0/src/vr180_convert/cli.py` & `vr180_convert-0.2.1/src/vr180_convert/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,18 +111,18 @@
     size: Annotated[
         str, typer.Option(help="Output image size, defaults to 4096x4096")
     ] = "4096x4096",
     interpolation: Annotated[
         _InterpolationFlags,
         typer.Option(help="Interpolation method, defaults to lanczos4"),
     ] = _InterpolationFlags.INTER_LANCZOS4,  # type: ignore
-    boarder_mode: Annotated[
+    border_mode: Annotated[
         _BorderTypes, typer.Option(help="Border mode, defaults to constant")
     ] = _BorderTypes.BORDER_CONSTANT,  # type: ignore
-    boarder_value: int = 0,
+    border_value: int = 0,
     radius: Annotated[
         str, typer.Option(help="Radius of the fisheye image, defaults to 'auto'")
     ] = "auto",
     merge: Annotated[bool, typer.Option(help="Export as an anaglyph")] = False,
     autosearch_timestamp_calib_r_earlier_l: Annotated[
         float,
         typer.Option(
@@ -261,30 +261,30 @@
             transformer_until_encoder
             * Euclidean3DRotator(q)
             * transformer_after_encoder,
             transformer_,
         )
         LOG.info(f"Automatched transformer: {transformer_}")
 
-    if swap:
-        if isinstance(transformer_, tuple):
-            transformer_ = transformer_[1], transformer_[0]
+    # if swap:
+    #     if isinstance(transformer_, tuple) and automatch == "":
+    #         transformer_ = transformer_[1], transformer_[0]
 
     # apply transformer
     name_unique_content = (
         (
             "-"
             + sha256(
                 "".join(
                     [
                         transformer,
                         size,
                         interpolation,
-                        boarder_mode,
-                        str(boarder_value),
+                        border_mode,
+                        str(border_value),
                         radius,
                         str(merge),
                         str(autosearch_timestamp_calib_r_earlier_l),
                         str(swap),
                     ]
                 ).encode("utf-8")
             ).hexdigest()[:8]
@@ -304,16 +304,16 @@
             Path(left_path).parent / filename_default
             if out_path == Path("")
             else out_path / filename_default if out_path.is_dir() else out_path
         ),
         radius=float(radius) if radius not in ["auto", "max"] else radius,  # type: ignore
         size_output=tuple(map(int, size.split("x"))),  # type: ignore
         interpolation=getattr(cv, interpolation.upper()),
-        boarder_mode=getattr(cv, boarder_mode.upper()),
-        boarder_value=boarder_value,
+        boarder_mode=getattr(cv, border_mode.upper()),
+        boarder_value=border_value,
         merge=merge,
     )
 
 
 @app.command()
 def s(
     in_paths: Annotated[list[Path], typer.Argument(help="Image paths")],
```

### Comparing `vr180_convert-0.2.0/src/vr180_convert/remapper.py` & `vr180_convert-0.2.1/src/vr180_convert/remapper.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.0/src/vr180_convert/testing.py` & `vr180_convert-0.2.1/src/vr180_convert/testing.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.0/src/vr180_convert/transformer.py` & `vr180_convert-0.2.1/src/vr180_convert/transformer.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.0/PKG-INFO` & `vr180_convert-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vr180-convert
-Version: 0.2.0
+Version: 0.2.1
 Summary: Simple VR180 image converter
 Home-page: https://github.com/34j/vr180-convert
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -91,14 +91,16 @@
 
 | left.jpg                       | right.jpg                       | Output                                               |
 | ------------------------------ | ------------------------------- | ---------------------------------------------------- |
 | ![left](docs/_static/test.jpg) | ![right](docs/_static/test.jpg) | ![output](docs/_static/test.lr.PolynomialScaler.jpg) |
 
 If left and right image paths are the same, the image is divided into two halves (left and right, SBS) and processed as if they were separate images.
 
+## Advanced usage
+
 ### Automatic image search
 
 If one of left or right image path is a directory, the program will search for the closest image (in terms of creation time) in the other directory.
 
 ```shell
 v1c lr left.jpg right_dir
 v1c lr left_dir right.jpg
@@ -107,64 +109,71 @@
 It is recommended to synchronize the clocks of the cameras before shooting. However, it can be adjusted by specifying `-ac` option.
 
 ```shell
 v1c lr left.jpg right_dir -ac 1 # the clock of the right camera is 1 second faster / ahead
 v1c lr left_dir right.jpg -ac 1 # the clock of the right camera is 1 second faster / ahead
 ```
 
-### Custom conversion model
-
-You can also specify the conversion model by adding Python code directly to the `--transformer` option:
-
-```shell
-v1c lr left.jpg right.jpg ---transformer "EquirectangularEncoder() * Euclidean3DRotator(from_rotation_vector([0, np.pi / 4, 0])) * FisheyeDecoder("equidistant")"
-```
-
-If tuple, the first transformer is applied to the left image and the second transformer is applied to the right image. If a single transformer is given, it is applied to both images.
-
-Please refer to the [API documentation](https://vr180-convert.readthedocs.io/) for the available transformers and their parameters.
-For `from_rotation_vector`, please refer to the [numpy-quaternion documentation](https://quaternion.readthedocs.io/en/latest/Package%20API%3A/quaternion/#from_rotation_vector).
-
 ### Radius estimation
 
 The radius of the non-black area of the input image is assumed by counting black pixels by default, but it would be better to specify it manually to get stable results:
 
 ```shell
 v1c lr left.jpg right.jpg --radius 1000
 v1c lr left.jpg right.jpg --radius max # min(width, height) / 2
 ```
 
 ### Calibration
 
-Rotation matching using the least-squares method can be performed by clicking corresponding points that can be regarded as infinitely far away from the camera.
+[Rotation matching using the least-squares method](https://lisyarus.github.io/blog/posts/3d-shape-matching-with-quaternions.html) can be performed by clicking corresponding points that can be regarded as infinitely far away from the camera.
 
 ```shell
 v1c lr left.jpg right.jpg --automatch gui
 ```
 
 You can also specify the corresponding points manually:
 
 ```shell
 v1c lr left.jpg right.jpg --automatch "0,0;0,0;1,1;1,1" # left_x1,left_y1;right_x1,right_y1;...
 ```
 
+$$
+a_k, b_k \in \mathbb{R}^3,
+\min_{R \in SO(3)} \sum_k \|\|R a_k - b_k\|\|^2
+$$
+
+### Anaglyph
+
 `--merge` option (which exports as [anaglyph](https://en.wikipedia.org/wiki/Anaglyph_3D) image) can be used to check if the calibration is successful by checking if the infinitely far points are overlapped.
 
 ```shell
 v1c lr left.jpg right.jpg --automatch gui --merge
 ```
 
 ### Swap
 
-If the camera is mounted upside down, you can swap the left and right images for conversion:
+If the camera is mounted upside down, you can simply use the `--swap` option without changing the transformer or other parameters:
 
 ```shell
 v1c lr left.jpg right.jpg --swap
 ```
 
+### Custom conversion model
+
+You can also specify the conversion model by adding Python code directly to the `--transformer` option:
+
+```shell
+v1c lr left.jpg right.jpg --transformer 'EquirectangularEncoder() * Euclidean3DRotator(from_rotation_vector([0, np.pi / 4, 0])) * FisheyeDecoder("equidistant")'
+```
+
+If tuple, the first transformer is applied to the left image and the second transformer is applied to the right image. If a single transformer is given, it is applied to both images.
+
+Please refer to the [API documentation](https://vr180-convert.readthedocs.io/) for the available transformers and their parameters.
+For `from_rotation_vector`, please refer to the [numpy-quaternion documentation](https://quaternion.readthedocs.io/en/latest/Package%20API%3A/quaternion/#from_rotation_vector).
+
 ### Single image conversion
 
 To convert a single image, use `v1c s` instead.
 
 ### Help
 
 For more information, please refer to the help or API documentation:
@@ -188,19 +197,46 @@
     ) -> tuple[NDArray, NDArray]:
         return theta**0.98 + theta**1.01, roll
 
 transformer = EquirectangularEncoder() * MyTransformer() * FisheyeDecoder("equidistant")
 apply_lr(transformer, left_path="left.jpg", right_path="right.jpg", out_path="output.jpg")
 ```
 
-## How to edit images
+## Tips
+
+### How to determine which image is left or right
+
+<!--
+- In the left image, the subject faces more to the right.
+- In the right image, the subject faces more to the left.
+- In other words, in a SBS image, the subject is oriented toward the center.
+
+In anaglyph images,
+
+- The left eye is covered with a red film, so the portion for the left eye is shown in blue.
+- The right eye is covered with a blue film, so the portion for the right eye is shown in red.
+| Film Color          | <span style="color:red">Red</span>   | <span style="color:blue">Blue</span> |
+| Anaglyph Color      | <span style="color:blue">Blue</span> | <span style="color:red">Red</span>   |
+-->
+
+|                     | Left                        | Right                       |
+| ------------------- | --------------------------- | --------------------------- |
+| Subject Orientation | Right                       | Left                        |
+| Film Color          | ${\color{red}\text{Red}}$   | ${\color{blue}\text{Blue}}$ |
+| Anaglyph Color      | ${\color{blue}\text{Blue}}$ | ${\color{red}\text{Red}}$   |
+
+- In a SBS image, the subject is oriented toward the center.
+
+### How to edit images
+
+This program cannot read RAW files. To deal with white-outs, etc., it is required to process each image with a program such as Photoshop, Lightroom, [RawTherapee](https://rawtherapee.com/downloads/), [Darktable](https://www.darktable.org/install/), etc.
 
-This program cannot read RAW files. To deal with white-outs, etc., it is recommended to process the image in Photoshop or other software first.
+However, this is so exhaustive, so it is recommended to take the images with jpeg format, being careful not to overexpose the images, and convert them with this program, then use Lightroom, [RawTherapee](https://rawtherapee.com/downloads/), [Darktable](https://www.darktable.org/install/) or other software to adjust colors and exposure, etc.
 
-### Example of processing in Photoshop
+#### Example of processing in Photoshop (Exquisite editing)
 
 1. Open one of the images just for specifying the canvas size.
 2. Add each image as Smart Objects (`LRaw`, `RRaw`) and make **minimal** corrections to match the exposure using `Camera Raw Filter`.
 3. Make each Smart Object into Smart Objects (`L`, `R`) again and do any image-dependent processing, such as removing the background.
 4. Make both images into a single Smart Object (`P`) and process them as a whole.
 5. Delete the background image created in step 1.
 6. Export as a PNG file.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vr180-convert Version: 0.2.0 Summary: Simple VR180
+Metadata-Version: 2.1 Name: vr180-convert Version: 0.2.1 Summary: Simple VR180
 image converter Home-page: https://github.com/34j/vr180-convert License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
@@ -27,64 +27,79 @@
 the following command to convert 2 fisheye images to a SBS equirectangular
 VR180 image: ```shell v1c lr left.jpg right.jpg ``` | left.jpg | right.jpg |
 Output | | ------------------------------ | ------------------------------- | -
 --------------------------------------------------- | | ![left](docs/_static/
 test.jpg) | ![right](docs/_static/test.jpg) | ![output](docs/_static/
 test.lr.PolynomialScaler.jpg) | If left and right image paths are the same, the
 image is divided into two halves (left and right, SBS) and processed as if they
-were separate images. ### Automatic image search If one of left or right image
-path is a directory, the program will search for the closest image (in terms of
-creation time) in the other directory. ```shell v1c lr left.jpg right_dir v1c
-lr left_dir right.jpg ``` It is recommended to synchronize the clocks of the
-cameras before shooting. However, it can be adjusted by specifying `-ac`
-option. ```shell v1c lr left.jpg right_dir -ac 1 # the clock of the right
-camera is 1 second faster / ahead v1c lr left_dir right.jpg -ac 1 # the clock
-of the right camera is 1 second faster / ahead ``` ### Custom conversion model
-You can also specify the conversion model by adding Python code directly to the
-`--transformer` option: ```shell v1c lr left.jpg right.jpg ---transformer
-"EquirectangularEncoder() * Euclidean3DRotator(from_rotation_vector([0, np.pi /
-4, 0])) * FisheyeDecoder("equidistant")" ``` If tuple, the first transformer is
+were separate images. ## Advanced usage ### Automatic image search If one of
+left or right image path is a directory, the program will search for the
+closest image (in terms of creation time) in the other directory. ```shell v1c
+lr left.jpg right_dir v1c lr left_dir right.jpg ``` It is recommended to
+synchronize the clocks of the cameras before shooting. However, it can be
+adjusted by specifying `-ac` option. ```shell v1c lr left.jpg right_dir -ac 1 #
+the clock of the right camera is 1 second faster / ahead v1c lr left_dir
+right.jpg -ac 1 # the clock of the right camera is 1 second faster / ahead ```
+### Radius estimation The radius of the non-black area of the input image is
+assumed by counting black pixels by default, but it would be better to specify
+it manually to get stable results: ```shell v1c lr left.jpg right.jpg --radius
+1000 v1c lr left.jpg right.jpg --radius max # min(width, height) / 2 ``` ###
+Calibration [Rotation matching using the least-squares method](https://
+lisyarus.github.io/blog/posts/3d-shape-matching-with-quaternions.html) can be
+performed by clicking corresponding points that can be regarded as infinitely
+far away from the camera. ```shell v1c lr left.jpg right.jpg --automatch gui
+``` You can also specify the corresponding points manually: ```shell v1c lr
+left.jpg right.jpg --automatch "0,0;0,0;1,1;1,1" #
+left_x1,left_y1;right_x1,right_y1;... ``` $$ a_k, b_k \in \mathbb{R}^3, \min_{R
+\in SO(3)} \sum_k \|\|R a_k - b_k\|\|^2 $$ ### Anaglyph `--merge` option (which
+exports as [anaglyph](https://en.wikipedia.org/wiki/Anaglyph_3D) image) can be
+used to check if the calibration is successful by checking if the infinitely
+far points are overlapped. ```shell v1c lr left.jpg right.jpg --automatch gui -
+-merge ``` ### Swap If the camera is mounted upside down, you can simply use
+the `--swap` option without changing the transformer or other parameters:
+```shell v1c lr left.jpg right.jpg --swap ``` ### Custom conversion model You
+can also specify the conversion model by adding Python code directly to the `--
+transformer` option: ```shell v1c lr left.jpg right.jpg --transformer
+'EquirectangularEncoder() * Euclidean3DRotator(from_rotation_vector([0, np.pi /
+4, 0])) * FisheyeDecoder("equidistant")' ``` If tuple, the first transformer is
 applied to the left image and the second transformer is applied to the right
 image. If a single transformer is given, it is applied to both images. Please
 refer to the [API documentation](https://vr180-convert.readthedocs.io/) for the
 available transformers and their parameters. For `from_rotation_vector`, please
 refer to the [numpy-quaternion documentation](https://
 quaternion.readthedocs.io/en/latest/Package%20API%3A/quaternion/
-#from_rotation_vector). ### Radius estimation The radius of the non-black area
-of the input image is assumed by counting black pixels by default, but it would
-be better to specify it manually to get stable results: ```shell v1c lr
-left.jpg right.jpg --radius 1000 v1c lr left.jpg right.jpg --radius max # min
-(width, height) / 2 ``` ### Calibration Rotation matching using the least-
-squares method can be performed by clicking corresponding points that can be
-regarded as infinitely far away from the camera. ```shell v1c lr left.jpg
-right.jpg --automatch gui ``` You can also specify the corresponding points
-manually: ```shell v1c lr left.jpg right.jpg --automatch "0,0;0,0;1,1;1,1" #
-left_x1,left_y1;right_x1,right_y1;... ``` `--merge` option (which exports as
-[anaglyph](https://en.wikipedia.org/wiki/Anaglyph_3D) image) can be used to
-check if the calibration is successful by checking if the infinitely far points
-are overlapped. ```shell v1c lr left.jpg right.jpg --automatch gui --merge ```
-### Swap If the camera is mounted upside down, you can swap the left and right
-images for conversion: ```shell v1c lr left.jpg right.jpg --swap ``` ### Single
-image conversion To convert a single image, use `v1c s` instead. ### Help For
-more information, please refer to the help or API documentation: ```shell v1c -
--help ``` ## Usage as a library For more complex transformations, it is
-recommended to create your own `Transformer`. Note that the transformation is
-applied in inverse order (new[(x, y)] = old[transform(x, y)], e.g. to decode
-[orthographic](https://en.wikipedia.org/wiki/Fisheye_lens#Mapping_function)
-fisheye images, `transform_polar` should be `arcsin(theta)`, not `sin(theta)`.)
-```python from vr180_convert import PolarRollTransformer, apply_lr class
-MyTransformer(PolarRollTransformer): def transform_polar( self, theta: NDArray,
-roll: NDArray, **kwargs: Any ) -> tuple[NDArray, NDArray]: return theta**0.98 +
-theta**1.01, roll transformer = EquirectangularEncoder() * MyTransformer() *
-FisheyeDecoder("equidistant") apply_lr(transformer, left_path="left.jpg",
-right_path="right.jpg", out_path="output.jpg") ``` ## How to edit images This
-program cannot read RAW files. To deal with white-outs, etc., it is recommended
-to process the image in Photoshop or other software first. ### Example of
-processing in Photoshop 1. Open one of the images just for specifying the
-canvas size. 2. Add each image as Smart Objects (`LRaw`, `RRaw`) and make
+#from_rotation_vector). ### Single image conversion To convert a single image,
+use `v1c s` instead. ### Help For more information, please refer to the help or
+API documentation: ```shell v1c --help ``` ## Usage as a library For more
+complex transformations, it is recommended to create your own `Transformer`.
+Note that the transformation is applied in inverse order (new[(x, y)] = old
+[transform(x, y)], e.g. to decode [orthographic](https://en.wikipedia.org/wiki/
+Fisheye_lens#Mapping_function) fisheye images, `transform_polar` should be
+`arcsin(theta)`, not `sin(theta)`.) ```python from vr180_convert import
+PolarRollTransformer, apply_lr class MyTransformer(PolarRollTransformer): def
+transform_polar( self, theta: NDArray, roll: NDArray, **kwargs: Any ) -> tuple
+[NDArray, NDArray]: return theta**0.98 + theta**1.01, roll transformer =
+EquirectangularEncoder() * MyTransformer() * FisheyeDecoder("equidistant")
+apply_lr(transformer, left_path="left.jpg", right_path="right.jpg",
+out_path="output.jpg") ``` ## Tips ### How to determine which image is left or
+right | | Left | Right | | ------------------- | --------------------------- |
+--------------------------- | | Subject Orientation | Right | Left | | Film
+Color | ${\color{red}\text{Red}}$ | ${\color{blue}\text{Blue}}$ | | Anaglyph
+Color | ${\color{blue}\text{Blue}}$ | ${\color{red}\text{Red}}$ | - In a SBS
+image, the subject is oriented toward the center. ### How to edit images This
+program cannot read RAW files. To deal with white-outs, etc., it is required to
+process each image with a program such as Photoshop, Lightroom, [RawTherapee]
+(https://rawtherapee.com/downloads/), [Darktable](https://www.darktable.org/
+install/), etc. However, this is so exhaustive, so it is recommended to take
+the images with jpeg format, being careful not to overexpose the images, and
+convert them with this program, then use Lightroom, [RawTherapee](https://
+rawtherapee.com/downloads/), [Darktable](https://www.darktable.org/install/) or
+other software to adjust colors and exposure, etc. #### Example of processing
+in Photoshop (Exquisite editing) 1. Open one of the images just for specifying
+the canvas size. 2. Add each image as Smart Objects (`LRaw`, `RRaw`) and make
 **minimal** corrections to match the exposure using `Camera Raw Filter`. 3.
 Make each Smart Object into Smart Objects (`L`, `R`) again and do any image-
 dependent processing, such as removing the background. 4. Make both images into
 a single Smart Object (`P`) and process them as a whole. 5. Delete the
 background image created in step 1. 6. Export as a PNG file. 7. Hide the other
 Smart Object (`L` or `R`) (created in step 3) in the Smart Object `P` (created
 in step 4) and save the Smart Object `P`, then export as a PNG file. ##
```

