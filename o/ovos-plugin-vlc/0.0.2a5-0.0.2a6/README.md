# Comparing `tmp/ovos_plugin_vlc-0.0.2a5-py3-none-any.whl.zip` & `tmp/ovos_plugin_vlc-0.0.2a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7799 bytes, number of entries: 8
--rw-r--r--  2.0 unx     5704 b- defN 24-Apr-10 02:19 ovos_plugin_vlc/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 24-Apr-10 02:19 ovos_plugin_vlc/version.py
--rw-r--r--  2.0 unx    11349 b- defN 24-Apr-10 02:19 ovos_plugin_vlc-0.0.2a5.dist-info/LICENSE
--rw-r--r--  2.0 unx      387 b- defN 24-Apr-10 02:19 ovos_plugin_vlc-0.0.2a5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 02:19 ovos_plugin_vlc-0.0.2a5.dist-info/WHEEL
--rw-r--r--  2.0 unx      147 b- defN 24-Apr-10 02:19 ovos_plugin_vlc-0.0.2a5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-10 02:19 ovos_plugin_vlc-0.0.2a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      708 b- defN 24-Apr-10 02:19 ovos_plugin_vlc-0.0.2a5.dist-info/RECORD
-8 files, 18580 bytes uncompressed, 6545 bytes compressed:  64.8%
+Zip file size: 7846 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     5875 b- defN 24-May-11 03:25 ovos_plugin_vlc/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-11 03:25 ovos_plugin_vlc/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      348 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      147 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      708 b- defN 24-May-11 03:25 ovos_plugin_vlc-0.0.2a6.dist-info/RECORD
+8 files, 18712 bytes uncompressed, 6592 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_plugin_vlc/__init__.py
 Comment: 
 
 Filename: ovos_plugin_vlc/version.py
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a5.dist-info/LICENSE
+Filename: ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a5.dist-info/METADATA
+Filename: ovos_plugin_vlc-0.0.2a6.dist-info/METADATA
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a5.dist-info/WHEEL
+Filename: ovos_plugin_vlc-0.0.2a6.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a5.dist-info/entry_points.txt
+Filename: ovos_plugin_vlc-0.0.2a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a5.dist-info/top_level.txt
+Filename: ovos_plugin_vlc-0.0.2a6.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_plugin_vlc-0.0.2a5.dist-info/RECORD
+Filename: ovos_plugin_vlc-0.0.2a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_plugin_vlc/__init__.py

```diff
@@ -1,113 +1,117 @@
-from ovos_utils.log import LOG
-from ovos_bus_client.message import Message
-from ovos_plugin_common_play.ocp.base import OCPAudioPlayerBackend
-from ovos_plugin_common_play.ocp.status import TrackState, \
-    MediaState, PlayerState
-import vlc
 import time
+from typing import List
 
-
-VLCAudioPluginConfig = {
-    "vlc": {
-        "type": "ovos_vlc",
-        "active": True
-    }
-}
+import vlc
+from ovos_bus_client.message import Message
+from ovos_plugin_manager.templates.audio import AudioBackend
+from ovos_utils.log import LOG
 
 
-class OVOSVlcService(OCPAudioPlayerBackend):
+class OVOSVlcService(AudioBackend):
     def __init__(self, config, bus=None, name='ovos_vlc'):
         super(OVOSVlcService, self).__init__(config, bus)
         self.instance = vlc.Instance("--no-video")
 
         self.player = self.instance.media_player_new()
         self.vlc_events = self.player.event_manager()
 
         self.vlc_events.event_attach(vlc.EventType.MediaPlayerPlaying,
                                      self.track_start, 1)
         self.vlc_events.event_attach(vlc.EventType.MediaPlayerTimeChanged,
                                      self.update_playback_time, None)
         self.vlc_events.event_attach(vlc.EventType.MediaPlayerEndReached,
-                                          self.queue_ended, 0)
+                                     self.queue_ended, 0)
         self.vlc_events.event_attach(vlc.EventType.MediaPlayerEncounteredError,
                                      self.handle_vlc_error, None)
 
         self.config = config
         self.bus = bus
         self.name = name
         self.normal_volume = None
         self.low_volume = self.config.get('low_volume', 30)
         self._playback_time = 0
         self.player.audio_set_volume(100)
         self._last_sync = 0
 
+    ###################
     # vlc internals
-    @property
-    def playback_time(self):
-        """ in milliseconds """
-        return self._playback_time
-
     def handle_vlc_error(self, data, other):
         self.ocp_error()
 
     def update_playback_time(self, data, other):
         self._playback_time = data.u.new_time
         # this message is captured by ovos common play and used to sync the
         # seekbar
         if time.time() - self._last_sync > 2:
             # send event ~ every 2 s
             # the gui seems to lag a lot when sending messages too often,
             # gui expected to keep an internal fake progress bar and sync periodically
             self._last_sync = time.time()
-            self.bus.emit(Message("ovos.common_play.playback_time",
-                                  {"position": self._playback_time,
-                                   "length": self.get_track_length()}))
+            try:
+                self.ocp_sync_playback(self._playback_time)
+            except:  # too old OPM version
+                self.bus.emit(Message("ovos.common_play.playback_time",
+                                      {"position": self._playback_time,
+                                       "length": self.get_track_length()}))
 
     def track_start(self, data, other):
         LOG.debug('VLC playback start')
         if self._track_start_callback:
             self._track_start_callback(self.track_info().get('name', "track"))
 
     def queue_ended(self, data, other):
         LOG.debug('VLC playback ended')
         self._now_playing = None
         if self._track_start_callback:
             self._track_start_callback(None)
 
-    def supported_uris(self):
+    ############
+    # mandatory abstract methods
+    @property
+    def playback_time(self):
+        """ in milliseconds """
+        return self._playback_time
+
+    def supported_uris(self) -> List[str]:
+        """List of supported uri types.
+
+        Returns:
+            list: Supported uri's
+        """
         return ['file', 'http', 'https']
 
-    # audio service
     def play(self, repeat=False):
         """ Play playlist using vlc. """
         LOG.debug('VLCService Play')
-        self.ocp_start()  # emit ocp state events
         track = self.instance.media_new(self._now_playing)
         self.player.set_media(track)
         self.player.play()
 
     def stop(self):
         """ Stop vlc playback. """
         LOG.info('VLCService Stop')
         if self.player.is_playing():
             self.player.stop()
-            self.ocp_stop()  # emit ocp state events
             return True
         return False
 
     def pause(self):
         """ Pause vlc playback. """
         self.player.set_pause(1)
-        self.ocp_pause()  # emit ocp state events
 
     def resume(self):
         """ Resume paused playback. """
         self.player.set_pause(0)
-        self.ocp_resume()  # emit ocp state events
+
+    def lower_volume(self):
+        self.player.audio_set_volume(self.low_volume)
+
+    def restore_volume(self):
+        self.player.audio_set_volume(100)
 
     def track_info(self):
         """ Extract info of current track. """
         ret = {}
         t = self.player.get_media()
         if t:
             ret['album'] = t.get_meta(vlc.Meta.Album)
@@ -167,7 +171,15 @@
 def load_service(base_config, bus):
     backends = base_config.get('backends', [])
     services = [(b, backends[b]) for b in backends
                 if backends[b]['type'] in ["vlc", 'ovos_vlc'] and
                 backends[b].get('active', False)]
     instances = [OVOSVlcService(s[1], bus, s[0]) for s in services]
     return instances
+
+
+VLCAudioPluginConfig = {
+    "vlc": {
+        "type": "ovos_vlc",
+        "active": True
+    }
+}
```

## ovos_plugin_vlc/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 5
+VERSION_ALPHA = 6
 # END_VERSION_BLOCK
```

## Comparing `ovos_plugin_vlc-0.0.2a5.dist-info/LICENSE` & `ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_plugin_vlc-0.0.2a5.dist-info/RECORD` & `ovos_plugin_vlc-0.0.2a6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_plugin_vlc/__init__.py,sha256=AqZLllCWQIzcEiEDxSeFV2_x4cD5aSmwfXovpvVUT68,5704
-ovos_plugin_vlc/version.py,sha256=7I4_TLoM46vOezfC0pAzDfsFVAIOs1tEU_y-4SvIlcg,177
-ovos_plugin_vlc-0.0.2a5.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_plugin_vlc-0.0.2a5.dist-info/METADATA,sha256=3u6VTP3X4Qw6LjEdg0o-bxbPh7plk_CoQGvZUwSd2no,387
-ovos_plugin_vlc-0.0.2a5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ovos_plugin_vlc-0.0.2a5.dist-info/entry_points.txt,sha256=yyfZ-8jm_iKva1qJ1CfxkKRNgPnUeP6gveK1UiWx6eE,147
-ovos_plugin_vlc-0.0.2a5.dist-info/top_level.txt,sha256=Eh9jwKJdrdwsCh7iQkzQqn69pbD1-EkVK3Ud1mTDxxU,16
-ovos_plugin_vlc-0.0.2a5.dist-info/RECORD,,
+ovos_plugin_vlc/__init__.py,sha256=mvECoadIeiSEbhnvMbbuIB5k2O3ZrhXbPaY9KMAGssI,5875
+ovos_plugin_vlc/version.py,sha256=di5Z7K6nH7UaPd1uj2qxhcT0JK5MyN10xTqgznSb2b4,177
+ovos_plugin_vlc-0.0.2a6.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_plugin_vlc-0.0.2a6.dist-info/METADATA,sha256=ySqWC204tpwQy38AePv7SU_EhceQIXmJz1m_3devzj4,348
+ovos_plugin_vlc-0.0.2a6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ovos_plugin_vlc-0.0.2a6.dist-info/entry_points.txt,sha256=yyfZ-8jm_iKva1qJ1CfxkKRNgPnUeP6gveK1UiWx6eE,147
+ovos_plugin_vlc-0.0.2a6.dist-info/top_level.txt,sha256=Eh9jwKJdrdwsCh7iQkzQqn69pbD1-EkVK3Ud1mTDxxU,16
+ovos_plugin_vlc-0.0.2a6.dist-info/RECORD,,
```

