# Comparing `tmp/new_natnet_client-4.1.2b2.tar.gz` & `tmp/new_natnet_client-4.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.1.2b2.tar", max compression
+gzip compressed data, was "new_natnet_client-4.1.3b0.tar", max compression
```

## Comparing `new_natnet_client-4.1.2b2.tar` & `new_natnet_client-4.1.3b0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-03 00:35:37.958385 new_natnet_client-4.1.2b2/LICENSE
--rw-r--r--   0        0        0      632 2024-05-03 00:10:07.988386 new_natnet_client-4.1.2b2/README.md
--rw-r--r--   0        0        0    15156 2024-05-06 17:11:06.228822 new_natnet_client-4.1.2b2/new_natnet_client/Client.py
--rw-r--r--   0        0        0     8498 2024-05-06 18:27:28.019509 new_natnet_client-4.1.2b2/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    26325 2024-05-06 18:46:40.709526 new_natnet_client-4.1.2b2/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-03 00:03:07.918385 new_natnet_client-4.1.2b2/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      468 2024-05-06 18:47:13.599526 new_natnet_client-4.1.2b2/pyproject.toml
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 new_natnet_client-4.1.2b2/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/LICENSE
+-rw-r--r--   0        0        0     1582 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/README.md
+-rw-r--r--   0        0        0    15156 2024-05-11 19:16:24.793204 new_natnet_client-4.1.3b0/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     8498 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    26518 2024-05-11 20:41:40.316803 new_natnet_client-4.1.3b0/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.1.3b0/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      469 2024-05-11 20:39:29.717215 new_natnet_client-4.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 new_natnet_client-4.1.3b0/PKG-INFO
```

### Comparing `new_natnet_client-4.1.2b2/LICENSE` & `new_natnet_client-4.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b2/new_natnet_client/Client.py` & `new_natnet_client-4.1.3b0/new_natnet_client/Client.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b2/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.1.3b0/new_natnet_client/NatNetTypes.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.1.2b2/new_natnet_client/Unpackers.py` & `new_natnet_client-4.1.3b0/new_natnet_client/Unpackers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import new_natnet_client.NatNetTypes as NatNetTypes
 from dataclasses import asdict
 from typing import Tuple, Dict
 from collections import deque
 from struct import unpack
+from itertools import batched
 
 class DataUnpackerV3_0:
+  rigid_body_lenght:int = 38
+  marker_lenght:int = 26
   @classmethod
   def unpack_data_size(cls, data:bytes) -> Tuple[int, int]:
     return 0,0
 
   @classmethod
   def unpack_frame_prefix_data(cls, data:bytes) -> Tuple[NatNetTypes.Frame_prefix, int]:
     offset = 0
@@ -19,38 +22,39 @@
   def unpack_marker_set_data(cls, data:bytes) -> Tuple[NatNetTypes.Marker_set_data, int]:
     offset = 0
     template = {}
     template['num_marker_sets'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     markers = deque()
-    for i in range(template['num_marker_sets']):
+    for _ in range(template['num_marker_sets']):
       template_marker = {}
       name, _, _ = data[offset:].partition(b'\0')
       offset += len(name) + 1
       template_marker['name'] = str(name, encoding="utf-8")
       template_marker['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      positions = deque()
-      for j in range(template_marker['num_markers']):
-        positions.append(NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)]))
-      template_marker['positions'] = tuple(positions)
+      template_marker['positions'] = tuple(map(
+        lambda position_data: NatNetTypes.Position.unpack(bytes(position_data)),
+        batched(data[offset:offset:=offset+(12*template_marker['num_markers'])],12)
+      ))
       markers.append(NatNetTypes.Marker_data(**template_marker))
     template['marker_sets'] = tuple(markers)
     return NatNetTypes.Marker_set_data(**template), offset
 
   @classmethod
   def unpack_legacy_other_markers(cls, data:bytes) -> Tuple[NatNetTypes.Legacy_marker_set_data,int]:
     offset = 0
     template = {}
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    positions = deque()
-    for _ in range(template['num_markers']):
-      positions.append(NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)]))
+    positions = deque(map(
+      lambda position_data: NatNetTypes.Position.unpack(bytes(position_data)),
+      batched(data[offset:offset:=offset+(12*template['num_markers'])],12)
+    ))
     template['positions'] = tuple(positions)
     return NatNetTypes.Legacy_marker_set_data(**template), offset
 
   @classmethod
   def unpack_rigid_body(cls, data:bytes) -> Tuple[NatNetTypes.Rigid_body, int]:
     offset = 0
     template = {}
@@ -65,34 +69,30 @@
   @classmethod
   def unpack_rigid_body_data(cls, data:bytes) -> Tuple[NatNetTypes.Rigid_body_data, int]:
     offset = 0
     template = {}
     template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    rigid_bodies = deque()
-    for _ in range(template['num_rigid_bodies']):
-      rigid_body, tmp_offset = cls.unpack_rigid_body(data[offset:])
-      offset += tmp_offset
-      rigid_bodies.append(rigid_body)
-    template['rigid_bodies'] = tuple(rigid_bodies)
+    template['rigid_bodies'] = tuple(map(
+        lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data))[0],
+        batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*template['num_rigid_bodies']))], cls.rigid_body_lenght) 
+    ))
     return NatNetTypes.Rigid_body_data(**template), offset
   
   @classmethod
   def unpack_skeleton(cls, data:bytes) -> Tuple[NatNetTypes.Skeleton, int]:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    rigid_bodies = deque()
-    for _ in range(template['num_rigid_bodies']):
-      rigid_body, tmp_offset = cls.unpack_rigid_body(data[offset:])
-      offset += tmp_offset
-      rigid_bodies.append(rigid_body)
-    template['rigid_bodies'] = tuple(rigid_bodies)
+    template['rigid_bodies'] = tuple(map(
+        lambda rigid_body_data: cls.unpack_rigid_body(bytes(rigid_body_data))[0],
+        batched(data[offset:(offset:=offset+(cls.rigid_body_lenght*template['num_rigid_bodies']))], cls.rigid_body_lenght) 
+    ))
     return NatNetTypes.Skeleton(**template), offset
 
   @classmethod
   def unpack_skeleton_data(cls, data:bytes) -> Tuple[NatNetTypes.Skeleton_data, int]:
     offset = 0
     template = {}
     template['num_skeletons'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
@@ -126,80 +126,83 @@
   def decode_marker_id(cls, id:int) -> Tuple[int, int]:
     return (
       id >> 16,
       id & 0x0000ffff
     )
 
   @classmethod
+  def unpack_labeled_marker(cls, data:bytes) -> Tuple[NatNetTypes.Labeled_marker, int]:
+    offset = 0
+    template = {}
+    template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+    template['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
+    template['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
+    template['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
+    template['residual'] = unpack('<f', data[offset:(offset:=offset+4)])[0] * 1000.0
+    return NatNetTypes.Labeled_marker(**template), offset
+
+  @classmethod
   def unpack_labeled_marker_data(cls, data:bytes) -> Tuple[NatNetTypes.Labeled_marker_data, int]:
     offset = 0
     template = {}
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
-    markers = deque()
-    for _ in range(template['num_markers']):
-      template_marker = {}
-      template_marker['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      template_marker['pos'] = NatNetTypes.Position.unpack(data[offset:(offset:=offset+12)])
-      template_marker['size'] = unpack('<f', data[offset:(offset:=offset+4)])[0]
-      template_marker['param'] = unpack( 'h', data[offset:(offset:=offset+2)])[0]
-      template_marker['residual'] = unpack('<f', data[offset:(offset:=offset+4)])[0] * 1000.0
-      markers.append(NatNetTypes.Labeled_marker(**template_marker))
-    template['markers'] = tuple(markers)
+    template['markers'] = tuple(map(
+      lambda marker_data: cls.unpack_labeled_marker(bytes(marker_data))[0],
+      batched(data[offset:(offset:=offset+(cls.marker_lenght*template['num_markers']))],cls.marker_lenght)
+    ))
     return NatNetTypes.Labeled_marker_data(**template), offset
 
   @classmethod
+  def unpack_channels(cls, data:bytes, num_channels:int) -> Tuple[Tuple[NatNetTypes.Channel, ...],int]:
+    offset = 0
+    channels = deque()
+    for _ in range(num_channels):
+      template_channel = {}
+      template_channel['num_frames'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
+      template_channel['frames'] = tuple(map(
+        lambda frame_data: unpack('<f', frame_data)[0],
+        batched(data[offset:(offset:=offset+(4*template_channel['num_frames']))],4)
+      ))
+      channels.append(NatNetTypes.Channel(**template_channel))
+    return tuple(channels), offset
+
+  @classmethod
   def unpack_force_plate_data(cls, data:bytes) -> Tuple[NatNetTypes.Force_plate_data, int]:
     offset = 0
     template = {}
     template['num_force_plates'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     force_plates = deque()
-    for i in range(template['num_force_plates']):
+    for _ in range(template['num_force_plates']):
       template_force_plate = {}
       template_force_plate['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
       template_force_plate['num_channels'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      channels = deque()
-      for j in range(template_force_plate['num_channels']):
-        template_channel = {}
-        template_channel['num_frames'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-        frames = deque()
-        for k in range(template_channel['num_frames']):
-          frames.append(unpack('<f', data[offset:(offset:=offset+4)])[0])
-        template_channel['frames'] = tuple(frames)
-        channels.append(NatNetTypes.Channel(**template_channel))
-      template_force_plate['channels'] = tuple(channels)
+      template_force_plate['channels'], tmp_offset = cls.unpack_channels(data[offset:], template_force_plate['num_channels'])
+      offset += tmp_offset
       force_plates.append(NatNetTypes.Force_plate(**template_force_plate))
     template['force_plates'] = tuple(force_plates)
     return NatNetTypes.Force_plate_data(**template), offset
 
   @classmethod
   def unpack_device_data(cls, data:bytes) -> Tuple[NatNetTypes.Device_data, int]:
     offset = 0
     template = {}
     template['num_devices'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     _, tmp_offset = cls.unpack_data_size(data)
     offset += tmp_offset
     devices = deque()
-    for i in range(template['num_devices']):
+    for _ in range(template['num_devices']):
       template_device = {}
       template_device['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
       template_device['num_channels'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-      channels = deque()
-      for j in range(template_device['num_channels']):
-        template_channel = {}
-        template_channel['num_frames'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-        frames = deque()
-        for k in range(template_channel['num_frames']):
-          frames.append(unpack('<f', data[offset:(offset:=offset+4)])[0])
-        template_channel['frames'] = tuple(frames)
-        channels.append(NatNetTypes.Channel(**template_channel))
-      template_device['channels'] = tuple(channels)
+      template_device['channels'], tmp_offset = cls.unpack_channels(data[offset:], template_device['num_channels'])
+      offset += tmp_offset
       devices.append(NatNetTypes.Device(**template_device))
     template['devices'] = tuple(devices)
     return NatNetTypes.Device_data(**template), offset
 
   @classmethod
   def unpack_frame_suffix_data(cls, data:bytes) -> Tuple[NatNetTypes.Frame_suffix, int]:
     offset = 0
@@ -279,15 +282,15 @@
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     offset_pos = offset
     offset_id = offset_pos + (12*template['num_markers'])
     offset_name = offset_id + (4*template['num_markers'])
     template["name"] = ""
     markers = deque()
     for _ in range(template['num_markers']):
-      template['pos'] = data[offset_pos:(offset_pos:=offset_pos+12)]
+      template['pos'] = NatNetTypes.Position.unpack(data[offset_pos:(offset_pos:=offset_pos+12)])
       template['id'] = int.from_bytes(data[offset_Y:(offset_Y:=offset_Y+4)], byteorder='little', signed=True)
       markers.append(NatNetTypes.RB_marker(**template))
     template['markers'] = tuple(markers)
     return {template['id']:NatNetTypes.Rigid_body_description(**template)}, offset_name
 
   @classmethod
   def unpack_skeleton_description(cls, data:bytes) -> Tuple[Dict[int, NatNetTypes.Skeleton_description], int]:
@@ -412,14 +415,16 @@
       marker = list(d.values())[0]
       markers.append(marker)
       offset += offset_tmp
     template['markers'] = tuple(markers)
     return {template['id']:NatNetTypes.Asset_description(**template)}, offset
 
 class DataUnpackerV4_1(DataUnpackerV3_0):
+  asset_rigid_body_lenght:int = 38
+  asset_marker_lenght: int = 26
   @classmethod
   def unpack_data_size(cls, data: bytes) -> Tuple[int, int]:
     offset = 0
     size_in_bytes = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     return size_in_bytes, offset
 
   @classmethod
@@ -446,27 +451,23 @@
 
   @classmethod
   def unpack_asset(cls, data:bytes) -> Tuple[NatNetTypes.Asset, int]:
     offset = 0
     template = {}
     template['id'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
     template['num_rigid_bodies'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    rigid_bodies = deque()
-    for _ in range(template['num_rigid_bodies']):
-      rigid_body, tmp_offset = cls.unpack_asset_rigid_body(data[offset:])
-      offset += tmp_offset
-      rigid_bodies.append(rigid_body)
-    template['rigid_bodies'] = tuple(rigid_bodies)
+    template['rigid_bodies'] = tuple(map(
+      lambda rigid_body_data: cls.unpack_asset_rigid_body(bytes(rigid_body_data))[0],
+      batched(data[offset:(offset:=offset+(cls.asset_rigid_body_lenght*template['num_rigid_bodies']))], cls.asset_rigid_body_lenght)
+    ))
     template['num_markers'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
-    markers = deque()
-    for _ in range(template['num_markers']):
-      marker, tmp_offset = cls.unpack_asset_marker(data[offset:])
-      offset += tmp_offset
-      markers.append(marker)
-    template['markers'] = tuple(markers)
+    template['markers'] = tuple(map(
+      lambda marker_data: cls.unpack_asset_marker(bytes(marker_data))[0],
+      batched(data[offset:(offset:=offset+(cls.asset_marker_lenght*template['num_markers']))], cls.asset_marker_lenght)
+    ))
     return NatNetTypes.Asset(**template), offset
 
   @classmethod
   def unpack_asset_data(cls, data:bytes) -> Tuple[NatNetTypes.Asset_data, int]:
     offset = 0
     template = {}
     template['num_assets'] = int.from_bytes(data[offset:(offset:=offset+4)], byteorder='little', signed=True)
```

