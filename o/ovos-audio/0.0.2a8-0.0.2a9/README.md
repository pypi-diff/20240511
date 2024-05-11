# Comparing `tmp/ovos_audio-0.0.2a8-py3-none-any.whl.zip` & `tmp/ovos_audio-0.0.2a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,15 @@
-Zip file size: 5716 bytes, number of entries: 6
--rw-r--r--  2.0 unx    11423 b- defN 23-Apr-05 04:38 ovos_audio-0.0.2a8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      823 b- defN 23-Apr-05 04:38 ovos_audio-0.0.2a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 04:38 ovos_audio-0.0.2a8.dist-info/WHEEL
--rw-r--r--  2.0 unx       57 b- defN 23-Apr-05 04:38 ovos_audio-0.0.2a8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-05 04:38 ovos_audio-0.0.2a8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      513 b- defN 23-Apr-05 04:38 ovos_audio-0.0.2a8.dist-info/RECORD
-6 files, 12909 bytes uncompressed, 4774 bytes compressed:  63.0%
+Zip file size: 16720 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      545 b- defN 23-Apr-05 05:13 ovos_audio/__init__.py
+-rw-r--r--  2.0 unx     1496 b- defN 23-Apr-05 05:13 ovos_audio/__main__.py
+-rw-r--r--  2.0 unx    19015 b- defN 23-Apr-05 05:13 ovos_audio/audio.py
+-rw-r--r--  2.0 unx    15385 b- defN 23-Apr-05 05:13 ovos_audio/service.py
+-rw-r--r--  2.0 unx      267 b- defN 23-Apr-05 05:13 ovos_audio/tts.py
+-rw-r--r--  2.0 unx     1930 b- defN 23-Apr-05 05:13 ovos_audio/utils.py
+-rw-r--r--  2.0 unx      114 b- defN 23-Apr-05 05:13 ovos_audio/version.py
+-rw-r--r--  2.0 unx    11423 b- defN 23-Apr-05 05:13 ovos_audio-0.0.2a9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      823 b- defN 23-Apr-05 05:13 ovos_audio-0.0.2a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 05:13 ovos_audio-0.0.2a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       57 b- defN 23-Apr-05 05:13 ovos_audio-0.0.2a9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-05 05:13 ovos_audio-0.0.2a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1053 b- defN 23-Apr-05 05:13 ovos_audio-0.0.2a9.dist-info/RECORD
+13 files, 52211 bytes uncompressed, 14964 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -1,19 +1,40 @@
-Filename: ovos_audio-0.0.2a8.dist-info/LICENSE.md
+Filename: ovos_audio/__init__.py
 Comment: 
 
-Filename: ovos_audio-0.0.2a8.dist-info/METADATA
+Filename: ovos_audio/__main__.py
 Comment: 
 
-Filename: ovos_audio-0.0.2a8.dist-info/WHEEL
+Filename: ovos_audio/audio.py
 Comment: 
 
-Filename: ovos_audio-0.0.2a8.dist-info/entry_points.txt
+Filename: ovos_audio/service.py
 Comment: 
 
-Filename: ovos_audio-0.0.2a8.dist-info/top_level.txt
+Filename: ovos_audio/tts.py
 Comment: 
 
-Filename: ovos_audio-0.0.2a8.dist-info/RECORD
+Filename: ovos_audio/utils.py
+Comment: 
+
+Filename: ovos_audio/version.py
+Comment: 
+
+Filename: ovos_audio-0.0.2a9.dist-info/LICENSE.md
+Comment: 
+
+Filename: ovos_audio-0.0.2a9.dist-info/METADATA
+Comment: 
+
+Filename: ovos_audio-0.0.2a9.dist-info/WHEEL
+Comment: 
+
+Filename: ovos_audio-0.0.2a9.dist-info/entry_points.txt
+Comment: 
+
+Filename: ovos_audio-0.0.2a9.dist-info/top_level.txt
+Comment: 
+
+Filename: ovos_audio-0.0.2a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ovos_audio-0.0.2a8.dist-info/LICENSE.md` & `ovos_audio-0.0.2a9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `ovos_audio-0.0.2a8.dist-info/METADATA` & `ovos_audio-0.0.2a9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-audio
-Version: 0.0.2a8
+Version: 0.0.2a9
 Summary: ovos-core audio daemon client
 Home-page: https://github.com/OpenVoiceOS/ovos-audio
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

