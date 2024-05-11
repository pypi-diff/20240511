# Comparing `tmp/jianyingdraft_py-1.0.3.tar.gz` & `tmp/jianyingdraft_py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianyingdraft_py-1.0.3.tar", max compression
+gzip compressed data, was "jianyingdraft_py-1.0.4.tar", max compression
```

## Comparing `jianyingdraft_py-1.0.3.tar` & `jianyingdraft_py-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.3/JianYingDraft/__init__.py
--rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-1.0.3/JianYingDraft/core/__init__.py
--rw-r--r--   0        0        0     9941 2024-04-09 10:35:35.917283 jianyingdraft_py-1.0.3/JianYingDraft/core/draft.py
--rw-r--r--   0        0        0     9058 2024-04-09 08:15:14.757157 jianyingdraft_py-1.0.3/JianYingDraft/core/media.py
--rw-r--r--   0        0        0     1995 2024-04-10 01:11:08.019622 jianyingdraft_py-1.0.3/JianYingDraft/core/mediaAudio.py
--rw-r--r--   0        0        0     1151 2024-04-10 03:23:50.885126 jianyingdraft_py-1.0.3/JianYingDraft/core/mediaEffect.py
--rw-r--r--   0        0        0     1230 2024-04-01 09:46:41.819510 jianyingdraft_py-1.0.3/JianYingDraft/core/mediaFactory.py
--rw-r--r--   0        0        0     1247 2024-04-10 01:09:28.398551 jianyingdraft_py-1.0.3/JianYingDraft/core/mediaImage.py
--rw-r--r--   0        0        0     1530 2024-04-09 07:37:42.070377 jianyingdraft_py-1.0.3/JianYingDraft/core/mediaText.py
--rw-r--r--   0        0        0     3982 2024-04-21 07:00:00.543052 jianyingdraft_py-1.0.3/JianYingDraft/core/mediaVideo.py
--rw-r--r--   0        0        0    13262 2024-04-21 00:54:40.541073 jianyingdraft_py-1.0.3/JianYingDraft/core/template.py
--rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-1.0.3/JianYingDraft/template/draft_content.json
--rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-1.0.3/JianYingDraft/template/draft_meta_info.json
--rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.3/JianYingDraft/utils/__init__.py
--rw-r--r--   0        0        0      731 2024-04-21 06:50:24.602526 jianyingdraft_py-1.0.3/JianYingDraft/utils/dataStruct.py
--rw-r--r--   0        0        0     5407 2024-04-21 04:53:08.962048 jianyingdraft_py-1.0.3/JianYingDraft/utils/innerBizTypes.py
--rw-r--r--   0        0        0     3698 2024-04-21 02:42:13.939891 jianyingdraft_py-1.0.3/JianYingDraft/utils/tools.py
--rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-1.0.3/LICENSE
--rw-r--r--   0        0        0      546 2024-04-21 07:04:20.566509 jianyingdraft_py-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1558 2024-04-08 21:29:46.189767 jianyingdraft_py-1.0.3/README.md
--rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 jianyingdraft_py-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.4/JianYingDraft/__init__.py
+-rw-r--r--   0        0        0      159 2024-03-24 09:09:33.984726 jianyingdraft_py-1.0.4/JianYingDraft/core/__init__.py
+-rw-r--r--   0        0        0     9944 2024-05-11 08:41:23.174958 jianyingdraft_py-1.0.4/JianYingDraft/core/draft.py
+-rw-r--r--   0        0        0     9457 2024-05-11 08:52:55.108755 jianyingdraft_py-1.0.4/JianYingDraft/core/media.py
+-rw-r--r--   0        0        0     1995 2024-04-10 01:11:08.019622 jianyingdraft_py-1.0.4/JianYingDraft/core/mediaAudio.py
+-rw-r--r--   0        0        0     1151 2024-04-10 03:23:50.885126 jianyingdraft_py-1.0.4/JianYingDraft/core/mediaEffect.py
+-rw-r--r--   0        0        0     1230 2024-04-01 09:46:41.819510 jianyingdraft_py-1.0.4/JianYingDraft/core/mediaFactory.py
+-rw-r--r--   0        0        0     1247 2024-04-10 01:09:28.398551 jianyingdraft_py-1.0.4/JianYingDraft/core/mediaImage.py
+-rw-r--r--   0        0        0     1530 2024-04-09 07:37:42.070377 jianyingdraft_py-1.0.4/JianYingDraft/core/mediaText.py
+-rw-r--r--   0        0        0     4115 2024-05-10 10:27:54.024110 jianyingdraft_py-1.0.4/JianYingDraft/core/mediaVideo.py
+-rw-r--r--   0        0        0    13262 2024-04-21 00:54:40.541073 jianyingdraft_py-1.0.4/JianYingDraft/core/template.py
+-rw-r--r--   0        0        0     3151 2024-03-24 09:08:48.975245 jianyingdraft_py-1.0.4/JianYingDraft/template/draft_content.json
+-rw-r--r--   0        0        0     1591 2024-03-24 09:08:52.740696 jianyingdraft_py-1.0.4/JianYingDraft/template/draft_meta_info.json
+-rw-r--r--   0        0        0      165 2024-03-24 09:08:29.415451 jianyingdraft_py-1.0.4/JianYingDraft/utils/__init__.py
+-rw-r--r--   0        0        0      871 2024-04-21 10:07:07.517328 jianyingdraft_py-1.0.4/JianYingDraft/utils/dataStruct.py
+-rw-r--r--   0        0        0     5407 2024-04-21 04:53:08.962048 jianyingdraft_py-1.0.4/JianYingDraft/utils/innerBizTypes.py
+-rw-r--r--   0        0        0     3698 2024-04-21 02:42:13.939891 jianyingdraft_py-1.0.4/JianYingDraft/utils/tools.py
+-rw-r--r--   0        0        0     1066 2024-03-24 09:07:42.089208 jianyingdraft_py-1.0.4/LICENSE
+-rw-r--r--   0        0        0      546 2024-05-11 08:57:13.554315 jianyingdraft_py-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1558 2024-04-08 21:29:46.189767 jianyingdraft_py-1.0.4/README.md
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 jianyingdraft_py-1.0.4/PKG-INFO
```

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/draft.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/draft.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,31 +58,31 @@
         self._materials_in_draft_meta_info: {} = self._draft_meta_info_data['draft_materials']  # 草稿元数据库的素材
         self._videos_material_in_draft_meta_info = self._materials_in_draft_meta_info[0]['value']
         self._audios_material_in_draft_meta_info = self._materials_in_draft_meta_info[6]['value']  # type为8的那条
 
         self._tracks_in_draft_content: [] = self._draft_content_data['tracks']  # 草稿内容库的轨道
         pass
 
-    def add_media(self, media_file_full_name: str, start=0, duration=0, index=0, **kwargs):
+    def add_media(self, media_file_full_name: str, start_at_track=0, duration=0, index=0, **kwargs):
         """
         添加媒体到草稿
         """
         _index = index
 
-        media = MediaFactory.create(media_file_full_name, start=start, duration=duration, **kwargs)
+        media = MediaFactory.create(media_file_full_name, duration=duration, **kwargs)
 
         if media is None:
             return
         pass
 
         # 将媒体信息添加到draft的素材库
         self.__add_media_to_content_materials(media)
 
         # 将媒体信息添加到draft的轨道库
-        self.__add_media_to_content_tracks(media, start=start)
+        self.__add_media_to_content_tracks(media, start=start_at_track)
 
         # 将媒体信息添加到draft的元数据库
         self.__add_media_to_meta_info(media)
         pass
 
     def add_effect(self, effect_name_or_resource_id: str | int, start=0, duration=0, index=0, **kwargs):
         """
@@ -128,15 +128,14 @@
         tools.write_json(draft_content_file_full_name, self._draft_content_data)
         tools.write_json(draft_meta_info_file_full_name, self._draft_meta_info_data)
 
     def __add_media_to_content_materials(self, media: Media):
         """
         添加媒体信息到素材内容库的素材部分：
         """
-
         for _key, _value in media.material_data_for_content.items():
             _key = str(_key)
 
             # 排除中转使用的临时信息
             if _key.startswith("X."):
                 continue
             pass
@@ -144,15 +143,14 @@
             self._materials_in_draft_content[_key].append(_value)
         pass
 
     def __add_media_to_content_tracks(self, media: Media, start=0):
         """
         添加媒体信息到素材内容库的轨道部分：
         """
-
         all_tracks = self._tracks_in_draft_content
         target_track = None
         for _track in all_tracks:
             if _track["type"] == media.category_type:
                 target_track = _track
                 break
             pass
@@ -166,16 +164,16 @@
 
         if not start:
             # 添加新片段之前轨道总时长
             start = self.__get_track_duration(media.category_type)
         pass
 
         # 设置新segment的在轨道上的开始时间
-        segment_source_timerange = media.segment_data_for_content["target_timerange"]
-        segment_source_timerange["start"] = start
+        segment_target_timerange = media.segment_data_for_content["target_timerange"]
+        segment_target_timerange["start"] = start
         target_track["segments"].append(media.segment_data_for_content)
 
     def __add_media_to_meta_info(self, media: Media):
         """
         添加媒体信息到元数据库：
         """
```

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/media.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,24 +173,29 @@
     pass
 
     def _set_segment_data_for_content(self):
         """
         设置草稿文件track中的segment部分
         """
         segment = template.get_segment()
-        self.segment_data_for_content = segment
 
         # # 将本片段应该表示的素材类型，临时记录在“X.xx”内
         # segment['X.material_type'] = self.material_type
 
+        speed = self.kwargs.get("speed", 1.0)
+        segment['speed'] = speed  # 速度
+        start_in_media = self.kwargs.get("start_in_media", 0)
+
         segment['material_id'] = self.id
         segment['extra_material_refs'] = self.material_data_for_content["X.extra_material_refs"]
 
-        segment['source_timerange'] = {"duration": self.duration, "start": 0}  # 使用原素材的开始位置和使用时长信息（素材自己的时间）
-        segment['target_timerange'] = {"duration": self.duration, "start": 0}  # 放入轨道上的开始位置和使用时长信息（轨道上的时间）
+        segment['source_timerange'] = {"duration": self.duration, "start": start_in_media}  # 使用原素材的开始位置和使用时长信息（素材自己的时间）
+        segment['target_timerange'] = {"duration": self.duration / speed, "start": 0}  # 放入轨道上的开始位置和使用时长信息（轨道上的时间）
+
+        self.segment_data_for_content = segment
 
     pass
 
     def __set_data_for_meta_info(self):
         """
         为稿文件draft_meta_info准备信息
         """
@@ -213,15 +218,18 @@
 
         if "width" in media_info:
             self.width = media_info['width']
             self.height = media_info['height']
         pass
 
         if "duration" in media_info:
-            self.duration = media_info['duration'] * 1000
+            _duration = media_info['duration'] * 1000
+            # 如果设置了截取时间start_in_media，那么duration需要减去start_in_media的时间
+            start_in_media = self.kwargs.get("start_in_media", 0)
+            self.duration = _duration - start_in_media
         pass
 
     def __set_type_info(self):
         _type = self.kwargs.get("media_type", "")
         if _type:
             self.media_type = _type
         pass
```

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/mediaAudio.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/mediaAudio.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/mediaEffect.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/mediaEffect.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/mediaFactory.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/mediaFactory.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/mediaImage.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/mediaImage.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/mediaText.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/mediaText.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/mediaVideo.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/mediaVideo.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,21 @@
         """
         设置草稿文件的content部分
         """
         speed_id = tools.generate_id()
         scm_id = tools.generate_id()
         canvas_id = tools.generate_id()
 
-        self.material_data_for_content["speeds"] = template.get_speed(speed_id)
         self.material_data_for_content["sound_channel_mappings"] = template.get_sound_channel_mapping(scm_id)
         self.material_data_for_content["canvases"] = template.get_canvas(canvas_id)
 
+        speed_data = template.get_speed(speed_id)
+        speed = self.kwargs.get("speed", 1.0)
+        speed_data["speed"] = speed
+        self.material_data_for_content["speeds"] = speed_data
         video_data = self.__generate_main_data()
 
         # 判定是否要对视频素材本身的背景音进行静音处理
         bgm_mute = self.kwargs.get("bgm_mute", False)
         if bgm_mute:
             video_data["extra_type_option"] = 1
         else:
@@ -59,15 +62,15 @@
         animation_datas: list[AnimationData] | None = self.kwargs.get("animation_datas", None)
         if animation_datas:
             animation_guid = tools.generate_id()
             material_animations = template.get_material_animation(animation_guid)
 
             for animation_data in animation_datas:
 
-                animation_start = 0
+                animation_start = animation_data.start
                 # 如果是入场动画，则动画的起始时间为0
                 if animation_data.animation_type == "in":
                     animation_start = 0
                 pass
 
                 # 如果是出场动画，则动画的起始时间为素材的持续时间向前推动画时长duration
                 if animation_data.animation_type == "out":
```

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/core/template.py` & `jianyingdraft_py-1.0.4/JianYingDraft/core/template.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/template/draft_content.json` & `jianyingdraft_py-1.0.4/JianYingDraft/template/draft_content.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/template/draft_meta_info.json` & `jianyingdraft_py-1.0.4/JianYingDraft/template/draft_meta_info.json`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/utils/dataStruct.py` & `jianyingdraft_py-1.0.4/JianYingDraft/utils/dataStruct.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,36 +13,44 @@
 
 
 @dataclass
 class ResourceData:
     """
     资源数据
     """
-    guid: str
-    name: str
-    resource_id: str
+    guid: str = ""
+    name: str = ""
+    resource_id: str = ""
 
 
 @dataclass
-class EffectData(ResourceData):
+class DurationResourceData(ResourceData):
+    """
+    延时资源数据
+    """
+    start: int = 0
+    duration: int = 0
+
+
+@dataclass
+class EffectData(DurationResourceData):
     """
     特效数据
     """
     pass
 
 
 @dataclass
-class TransitionData(ResourceData):
+class TransitionData(DurationResourceData):
     """
     转场数据
     """
-    duration: int
+    pass
 
 
 @dataclass
-class AnimationData(ResourceData):
+class AnimationData(DurationResourceData):
     """
     动画数据
     """
-    animation_type: AnimationTypes
-    start: int
-    duration: int
+    animation_type: AnimationTypes = "in"
+
```

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/utils/innerBizTypes.py` & `jianyingdraft_py-1.0.4/JianYingDraft/utils/innerBizTypes.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/JianYingDraft/utils/tools.py` & `jianyingdraft_py-1.0.4/JianYingDraft/utils/tools.py`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/LICENSE` & `jianyingdraft_py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/pyproject.toml` & `jianyingdraft_py-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "JianYingDraft.PY"
-version = "1.0.3"
+version = "1.0.4"
 description = "帮助剪映快速生成草稿的方案"
 authors = ["解大劦 <develope@163.com>"]
 readme = "README.md"
 packages = [{ include = "JianYingDraft" }]
 include = ["README.md", "LICENSE"]
 license = "MIT"
```

### Comparing `jianyingdraft_py-1.0.3/README.md` & `jianyingdraft_py-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jianyingdraft_py-1.0.3/PKG-INFO` & `jianyingdraft_py-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JianYingDraft.PY
-Version: 1.0.3
+Version: 1.0.4
 Summary: 帮助剪映快速生成草稿的方案
 License: MIT
 Author: 解大劦
 Author-email: develope@163.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

