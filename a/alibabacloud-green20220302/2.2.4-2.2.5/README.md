# Comparing `tmp/alibabacloud_green20220302-2.2.4.tar.gz` & `tmp/alibabacloud_green20220302-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_green20220302-2.2.4.tar", last modified: Fri Apr 19 17:11:49 2024, max compression
+gzip compressed data, was "dist/alibabacloud_green20220302-2.2.5.tar", last modified: Sat May 11 06:09:58 2024, max compression
```

## Comparing `alibabacloud_green20220302-2.2.4.tar` & `alibabacloud_green20220302-2.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/
--rw-r--r--   0 root         (0) root         (0)     1291 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50071 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/client.py
--rw-r--r--   0 root         (0) root         (0)   121973 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-19 17:11:49.000000 alibabacloud_green20220302-2.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2024-04-19 17:11:48.000000 alibabacloud_green20220302-2.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63849 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/client.py
+-rw-r--r--   0 root         (0) root         (0)   124740 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-11 06:09:58.000000 alibabacloud_green20220302-2.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-05-11 06:09:57.000000 alibabacloud_green20220302-2.2.5/setup.py
```

### Comparing `alibabacloud_green20220302-2.2.4/ChangeLog.md` & `alibabacloud_green20220302-2.2.5/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-19 Version: 2.2.4
+- Update API ImageModeration: update response param.
+
+
 2024-04-11 Version: 2.2.3
 - Update API DescribeImageResultExt: update response param.
 
 
 2024-03-26 Version: 2.2.2
 - Update API VideoModeration: update response param.
 - Update API VideoModerationResult: update response param.
```

### Comparing `alibabacloud_green20220302-2.2.4/LICENSE` & `alibabacloud_green20220302-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.4/PKG-INFO` & `alibabacloud_green20220302-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_green20220302
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.4/README-CN.md` & `alibabacloud_green20220302-2.2.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.4/README.md` & `alibabacloud_green20220302-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_green20220302-2.2.4/alibabacloud_green20220302/models.py` & `alibabacloud_green20220302-2.2.5/alibabacloud_green20220302/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1713,14 +1713,94 @@
         if m.get('Service') is not None:
             self.service = m.get('Service')
         if m.get('ServiceParameters') is not None:
             self.service_parameters = m.get('ServiceParameters')
         return self
 
 
+class ImageModerationResponseBodyDataExtOcrResultLocation(TeaModel):
+    def __init__(
+        self,
+        h: int = None,
+        w: int = None,
+        x: int = None,
+        y: int = None,
+    ):
+        self.h = h
+        self.w = w
+        self.x = x
+        self.y = y
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.h is not None:
+            result['H'] = self.h
+        if self.w is not None:
+            result['W'] = self.w
+        if self.x is not None:
+            result['X'] = self.x
+        if self.y is not None:
+            result['Y'] = self.y
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('H') is not None:
+            self.h = m.get('H')
+        if m.get('W') is not None:
+            self.w = m.get('W')
+        if m.get('X') is not None:
+            self.x = m.get('X')
+        if m.get('Y') is not None:
+            self.y = m.get('Y')
+        return self
+
+
+class ImageModerationResponseBodyDataExtOcrResult(TeaModel):
+    def __init__(
+        self,
+        location: ImageModerationResponseBodyDataExtOcrResultLocation = None,
+        text: str = None,
+    ):
+        self.location = location
+        self.text = text
+
+    def validate(self):
+        if self.location:
+            self.location.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.location is not None:
+            result['Location'] = self.location.to_map()
+        if self.text is not None:
+            result['Text'] = self.text
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Location') is not None:
+            temp_model = ImageModerationResponseBodyDataExtOcrResultLocation()
+            self.location = temp_model.from_map(m['Location'])
+        if m.get('Text') is not None:
+            self.text = m.get('Text')
+        return self
+
+
 class ImageModerationResponseBodyDataExtRecognition(TeaModel):
     def __init__(
         self,
         classification: str = None,
         confidence: float = None,
     ):
         self.classification = classification
@@ -1749,38 +1829,53 @@
             self.confidence = m.get('Confidence')
         return self
 
 
 class ImageModerationResponseBodyDataExt(TeaModel):
     def __init__(
         self,
+        ocr_result: List[ImageModerationResponseBodyDataExtOcrResult] = None,
         recognition: List[ImageModerationResponseBodyDataExtRecognition] = None,
     ):
+        self.ocr_result = ocr_result
         self.recognition = recognition
 
     def validate(self):
+        if self.ocr_result:
+            for k in self.ocr_result:
+                if k:
+                    k.validate()
         if self.recognition:
             for k in self.recognition:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        result['OcrResult'] = []
+        if self.ocr_result is not None:
+            for k in self.ocr_result:
+                result['OcrResult'].append(k.to_map() if k else None)
         result['Recognition'] = []
         if self.recognition is not None:
             for k in self.recognition:
                 result['Recognition'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        self.ocr_result = []
+        if m.get('OcrResult') is not None:
+            for k in m.get('OcrResult'):
+                temp_model = ImageModerationResponseBodyDataExtOcrResult()
+                self.ocr_result.append(temp_model.from_map(k))
         self.recognition = []
         if m.get('Recognition') is not None:
             for k in m.get('Recognition'):
                 temp_model = ImageModerationResponseBodyDataExtRecognition()
                 self.recognition.append(temp_model.from_map(k))
         return self
```

### Comparing `alibabacloud_green20220302-2.2.4/alibabacloud_green20220302.egg-info/PKG-INFO` & `alibabacloud_green20220302-2.2.5/alibabacloud_green20220302.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-green20220302
-Version: 2.2.4
+Version: 2.2.5
 Summary: Alibaba Cloud Green (20220302) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_green20220302-2.2.4/setup.py` & `alibabacloud_green20220302-2.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_green20220302.
 
-Created on 19/04/2024
+Created on 11/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_green20220302"
 NAME = "alibabacloud_green20220302" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Green (20220302) SDK Library for Python"
```

