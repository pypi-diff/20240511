# Comparing `tmp/sign_prosody_extraction-24.4.tar.gz` & `tmp/sign_prosody_extraction-24.5.tar.gz`

## Comparing `sign_prosody_extraction-24.4.tar` & `sign_prosody_extraction-24.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/.envrc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/.python-version
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/TODO.md
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/requirements-dev.lock
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/requirements.lock
--rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/img/dir_scale.png
--rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/img/dir_scale.svg
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/__init__.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/cli.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/plot.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/targets.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/typing.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/visualize.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/articulator/__init__.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/articulator/cotracker.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/src/sign_prosody_extraction/articulator/mediapipe.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/.gitignore
--rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/LICENSE
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/README.md
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/pyproject.toml
--rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.4/PKG-INFO
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/.envrc
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/.python-version
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/TODO.md
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/requirements-dev.lock
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/requirements.lock
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/__init__.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/cli.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/plot.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/targets.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/typing.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/visualize.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/articulator/__init__.py
+-rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/articulator/cotracker.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/articulator/mediapipe.py
+-rw-r--r--   0        0        0    12883 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/img/dir_scale.png
+-rw-r--r--   0        0        0    28352 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/src/sign_prosody_extraction/img/dir_scale.svg
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/.gitignore
+-rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/LICENSE
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/README.md
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/pyproject.toml
+-rw-r--r--   0        0        0     4635 2020-02-02 00:00:00.000000 sign_prosody_extraction-24.5/PKG-INFO
```

### Comparing `sign_prosody_extraction-24.4/requirements-dev.lock` & `sign_prosody_extraction-24.5/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/requirements.lock` & `sign_prosody_extraction-24.5/requirements.lock`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/img/dir_scale.png` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/img/dir_scale.png`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/img/dir_scale.svg` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/img/dir_scale.svg`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/__init__.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/cli.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     default=True,
     help="Use the original CoTracker algorithm for tracking.",
 )
 @click.option(
     "--mediapipe",
     "algorithm",
     flag_value="mediapipe",
-    help="Use the alternative MediaPipe algorithm for tracking.",
+    help="Use the alternative MediaPipe algorithm for tracking (pose_landmarker model needs to be available).",
 )
 @click.option(
     "--track-video/--no-track-video",
     default=False,
     help="Output a video with the extracted tracks overlaid. The filename will be the original filename with '_track' appended.",
 )
 @click.option(
```

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/plot.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .typing import ArticulatorArray
 
 # Colors for plotting direction
 colors = ["red", "green", "gold", "blue", "red"]  # H, X (right in the image), L, Y
 nodes = [0, 0.25, 0.5, 0.75, 1]
 cmap = LinearSegmentedColormap.from_list("custom", list(zip(nodes, colors)), N=256)
 
-scale_img = plt.imread(Path(__file__).parent.parent / "img/dir_scale.png")
+scale_img = plt.imread(Path(__file__).parent / "img/dir_scale.png")
 
 
 # Receive numpy array
 # long: make a wider plot
 # fps to write seconds value in axis
 # marks is a list of dicts with start, end and gloss to highlight parts
 # points is a list of points to demarkate
```

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/typing.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/typing.py`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/visualize.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/visualize.py`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/articulator/__init__.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/articulator/__init__.py`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/articulator/cotracker.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/articulator/cotracker.py`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/src/sign_prosody_extraction/articulator/mediapipe.py` & `sign_prosody_extraction-24.5/src/sign_prosody_extraction/articulator/mediapipe.py`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/LICENSE` & `sign_prosody_extraction-24.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/README.md` & `sign_prosody_extraction-24.5/README.md`

 * *Files identical despite different names*

### Comparing `sign_prosody_extraction-24.4/pyproject.toml` & `sign_prosody_extraction-24.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sign-prosody-extraction"
-version = "24.04"
+version = "24.05"
 description = """Code and command-line tool for "Automated Extraction of
 Prosodic Structure from Unannotated Sign Language Video" (Sevilla et al.,
 2024)."""
 authors = [
     { name = "Antonio F. G. Sevilla", email = "afgs@ucm.es" }
 ]
 dependencies = [
```

### Comparing `sign_prosody_extraction-24.4/PKG-INFO` & `sign_prosody_extraction-24.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sign-prosody-extraction
-Version: 24.4
+Version: 24.5
 Summary: Code and command-line tool for "Automated Extraction of Prosodic Structure from Unannotated Sign Language Video" (Sevilla et al., 2024).
 Author-email: "Antonio F. G. Sevilla" <afgs@ucm.es>
 License-File: LICENSE
 Requires-Python: ==3.10.*
 Requires-Dist: click>=8.1.7
 Requires-Dist: flow-vis>=0.1
 Requires-Dist: imageio[ffmpeg]>=2.34.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: sign-prosody-extraction Version: 24.4 Summary: Code
+Metadata-Version: 2.3 Name: sign-prosody-extraction Version: 24.5 Summary: Code
 and command-line tool for "Automated Extraction of Prosodic Structure from
 Unannotated Sign Language Video" (Sevilla et al., 2024). Author-email: "Antonio
 F. G. Sevilla"
 ucm.es> License-File: LICENSE Requires-Python: ==3.10.* Requires-Dist:
 click>=8.1.7 Requires-Dist: flow-vis>=0.1 Requires-Dist: imageio
 [ffmpeg]>=2.34.0 Requires-Dist: matplotlib>=3.8.4 Requires-Dist:
 mediapipe>=0.10.11 Requires-Dist: nptyping>=2.5.0 Requires-Dist: numpy>=1.26.4
```

