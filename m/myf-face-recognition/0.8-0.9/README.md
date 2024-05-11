# Comparing `tmp/myf_face_recognition-0.8.tar.gz` & `tmp/myf_face_recognition-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myf_face_recognition-0.8.tar", last modified: Tue Apr 30 17:51:14 2024, max compression
+gzip compressed data, was "myf_face_recognition-0.9.tar", last modified: Tue Apr 30 18:19:36 2024, max compression
```

## Comparing `myf_face_recognition-0.8.tar` & `myf_face_recognition-0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:51:13.995748 myf_face_recognition-0.8/
--rw-rw-rw-   0        0        0     1096 2024-03-24 20:45:15.000000 myf_face_recognition-0.8/LICENCE
--rw-rw-rw-   0        0        0      488 2024-04-30 17:51:13.988742 myf_face_recognition-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     8669 2024-04-30 17:11:50.000000 myf_face_recognition-0.8/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 17:51:13.658827 myf_face_recognition-0.8/myf_face_recognition/
--rw-rw-rw-   0        0        0        0 2024-03-25 05:22:33.000000 myf_face_recognition-0.8/myf_face_recognition/__init__.py
--rw-rw-rw-   0        0        0    11664 2024-04-30 17:50:05.000000 myf_face_recognition-0.8/myf_face_recognition/all.py
--rw-rw-rw-   0        0        0     3222 2024-03-25 09:28:35.000000 myf_face_recognition-0.8/myf_face_recognition/embeddings.py
--rw-rw-rw-   0        0        0     4107 2024-03-25 09:28:36.000000 myf_face_recognition-0.8/myf_face_recognition/images.py
--rw-rw-rw-   0        0        0     3841 2024-03-25 09:28:38.000000 myf_face_recognition-0.8/myf_face_recognition/simple_video.py
--rw-rw-rw-   0        0        0     4551 2024-04-30 17:50:08.000000 myf_face_recognition-0.8/myf_face_recognition/video.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:51:13.983743 myf_face_recognition-0.8/myf_face_recognition.egg-info/
--rw-rw-rw-   0        0        0      488 2024-04-30 17:51:08.000000 myf_face_recognition-0.8/myf_face_recognition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2024-04-30 17:51:08.000000 myf_face_recognition-0.8/myf_face_recognition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:51:08.000000 myf_face_recognition-0.8/myf_face_recognition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-04-30 17:51:08.000000 myf_face_recognition-0.8/myf_face_recognition.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       52 2024-04-30 17:51:08.000000 myf_face_recognition-0.8/myf_face_recognition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-04-30 17:51:08.000000 myf_face_recognition-0.8/myf_face_recognition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 17:51:13.997746 myf_face_recognition-0.8/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-04-30 17:48:57.000000 myf_face_recognition-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:19:35.710073 myf_face_recognition-0.9/
+-rw-rw-rw-   0        0        0     1096 2024-03-24 20:45:15.000000 myf_face_recognition-0.9/LICENCE
+-rw-rw-rw-   0        0        0      488 2024-04-30 18:19:35.704081 myf_face_recognition-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8669 2024-04-30 17:11:50.000000 myf_face_recognition-0.9/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 18:19:35.417832 myf_face_recognition-0.9/myf_face_recognition/
+-rw-rw-rw-   0        0        0        0 2024-03-25 05:22:33.000000 myf_face_recognition-0.9/myf_face_recognition/__init__.py
+-rw-rw-rw-   0        0        0    11672 2024-04-30 18:08:38.000000 myf_face_recognition-0.9/myf_face_recognition/all.py
+-rw-rw-rw-   0        0        0     3222 2024-03-25 09:28:35.000000 myf_face_recognition-0.9/myf_face_recognition/embeddings.py
+-rw-rw-rw-   0        0        0     4107 2024-03-25 09:28:36.000000 myf_face_recognition-0.9/myf_face_recognition/images.py
+-rw-rw-rw-   0        0        0     3841 2024-03-25 09:28:38.000000 myf_face_recognition-0.9/myf_face_recognition/simple_video.py
+-rw-rw-rw-   0        0        0     4559 2024-04-30 18:18:45.000000 myf_face_recognition-0.9/myf_face_recognition/video.py
+drwxrwxrwx   0        0        0        0 2024-04-30 18:19:35.698064 myf_face_recognition-0.9/myf_face_recognition.egg-info/
+-rw-rw-rw-   0        0        0      488 2024-04-30 18:19:31.000000 myf_face_recognition-0.9/myf_face_recognition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2024-04-30 18:19:31.000000 myf_face_recognition-0.9/myf_face_recognition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 18:19:31.000000 myf_face_recognition-0.9/myf_face_recognition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-04-30 18:19:31.000000 myf_face_recognition-0.9/myf_face_recognition.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2024-04-30 18:19:31.000000 myf_face_recognition-0.9/myf_face_recognition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-04-30 18:19:31.000000 myf_face_recognition-0.9/myf_face_recognition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 18:19:35.712065 myf_face_recognition-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-30 18:18:12.000000 myf_face_recognition-0.9/setup.py
```

### Comparing `myf_face_recognition-0.8/LICENCE` & `myf_face_recognition-0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.8/README.txt` & `myf_face_recognition-0.9/README.txt`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.8/myf_face_recognition/all.py` & `myf_face_recognition-0.9/myf_face_recognition/all.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 face_cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')
 
 # Get the directory path of the currently executing module
 current_dir = os.path.dirname(__file__)
 
 # Construct the path to the YOLO model file relative to the models directory
-model_path = os.path.join(current_dir, "models", "yolov8n-face.pt")
+default_model_path = os.path.join(current_dir, "models", "yolov8n-face.pt")
 
 
 # Initialize Yolo model
 yolo_model = None
 
 def load_yolo_model(model_path):
     print("Loading YOLO Model...")
```

### Comparing `myf_face_recognition-0.8/myf_face_recognition/embeddings.py` & `myf_face_recognition-0.9/myf_face_recognition/embeddings.py`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.8/myf_face_recognition/images.py` & `myf_face_recognition-0.9/myf_face_recognition/images.py`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.8/myf_face_recognition/simple_video.py` & `myf_face_recognition-0.9/myf_face_recognition/simple_video.py`

 * *Files identical despite different names*

### Comparing `myf_face_recognition-0.8/myf_face_recognition/video.py` & `myf_face_recognition-0.9/myf_face_recognition/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from ultralytics import YOLO
 
 # Get the directory path of the currently executing module
 current_dir = os.path.dirname(__file__)
 
 # Construct the path to the YOLO model file relative to the models directory
-model_path = os.path.join(current_dir, "models", "yolov8n-face.pt")
+default_model_path = os.path.join(current_dir, "models", "yolov8n-face.pt")
 
 # Initialize Yolo model
 yolo_model = None
 
 def load_yolo_model(model_path):
     print("Loading YOLO Model...")
     yolo_model = YOLO(model_path)
```

### Comparing `myf_face_recognition-0.8/setup.py` & `myf_face_recognition-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myf_face_recognition',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     package_data={'myf_face_recognition.models': ['yolov8n-face.pt']},
     install_requires=[
         'numpy',
         'keras-facenet',
         'opencv-python',
         'mtcnn',
```

