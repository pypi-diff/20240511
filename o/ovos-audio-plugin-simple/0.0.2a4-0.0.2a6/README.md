# Comparing `tmp/ovos_audio_plugin_simple-0.0.2a4-py3-none-any.whl.zip` & `tmp/ovos_audio_plugin_simple-0.0.2a6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8712 bytes, number of entries: 8
--rw-r--r--  2.0 unx     7442 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple-0.0.2a4.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple-0.0.2a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple-0.0.2a4.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple-0.0.2a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       25 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple-0.0.2a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      780 b- defN 23-Sep-06 01:37 ovos_audio_plugin_simple-0.0.2a4.dist-info/RECORD
-8 files, 20431 bytes uncompressed, 7314 bytes compressed:  64.2%
+Zip file size: 9508 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    10568 b- defN 24-May-11 03:24 ovos_audio_plugin_simple/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-May-11 03:24 ovos_audio_plugin_simple/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 24-May-11 03:25 ovos_audio_plugin_simple-0.0.2a6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      341 b- defN 24-May-11 03:25 ovos_audio_plugin_simple-0.0.2a6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-11 03:25 ovos_audio_plugin_simple-0.0.2a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      186 b- defN 24-May-11 03:25 ovos_audio_plugin_simple-0.0.2a6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       25 b- defN 24-May-11 03:25 ovos_audio_plugin_simple-0.0.2a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      781 b- defN 24-May-11 03:25 ovos_audio_plugin_simple-0.0.2a6.dist-info/RECORD
+8 files, 23519 bytes uncompressed, 8110 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_audio_plugin_simple/__init__.py
 Comment: 
 
 Filename: ovos_audio_plugin_simple/version.py
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a4.dist-info/LICENSE
+Filename: ovos_audio_plugin_simple-0.0.2a6.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a4.dist-info/METADATA
+Filename: ovos_audio_plugin_simple-0.0.2a6.dist-info/METADATA
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a4.dist-info/WHEEL
+Filename: ovos_audio_plugin_simple-0.0.2a6.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a4.dist-info/entry_points.txt
+Filename: ovos_audio_plugin_simple-0.0.2a6.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a4.dist-info/top_level.txt
+Filename: ovos_audio_plugin_simple-0.0.2a6.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_audio_plugin_simple-0.0.2a4.dist-info/RECORD
+Filename: ovos_audio_plugin_simple-0.0.2a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_audio_plugin_simple/__init__.py

```diff
@@ -1,21 +1,52 @@
 import mimetypes
 import re
 import signal
 import subprocess
+import time
 from distutils.spawn import find_executable
 from time import sleep
 
-from ovos_plugin_common_play.ocp.base import OCPAudioPlayerBackend
-from ovos_plugin_common_play.ocp.status import TrackState, MediaState, PlayerState
-from ovos_plugin_manager.templates.audio import AudioBackend
 from ovos_bus_client import Message
+from ovos_plugin_manager.templates.audio import AudioBackend
 from ovos_utils.log import LOG
 from requests import Session
 
+try:
+    from ovos_utils.ocp import MediaState
+except ImportError:
+    LOG.warning("Please update to ovos-utils~=0.1.")
+    from enum import IntEnum
+
+
+    class MediaState(IntEnum):
+        # https://doc.qt.io/qt-5/qmediaplayer.html#MediaStatus-enum
+        # The status of the media cannot be determined.
+        UNKNOWN = 0
+        # There is no current media. PlayerState == STOPPED
+        NO_MEDIA = 1
+        # The current media is being loaded. The player may be in any state.
+        LOADING_MEDIA = 2
+        # The current media has been loaded. PlayerState== STOPPED
+        LOADED_MEDIA = 3
+        # Playback of the current media has stalled due to
+        # insufficient buffering or some other temporary interruption.
+        # PlayerState != STOPPED
+        STALLED_MEDIA = 4
+        # The player is buffering data but has enough data buffered
+        # for playback to continue for the immediate future.
+        # PlayerState != STOPPED
+        BUFFERING_MEDIA = 5
+        # The player has fully buffered the current media. PlayerState != STOPPED
+        BUFFERED_MEDIA = 6
+        # Playback has reached the end of the current media. PlayerState == STOPPED
+        END_OF_MEDIA = 7
+        # The current media cannot be played. PlayerState == STOPPED
+        INVALID_MEDIA = 8
+
 
 def find_mime(path):
     mime = None
     if path.startswith('http'):
         response = Session().head(path, allow_redirects=True)
         if 200 <= response.status_code < 300:
             mime = response.headers['content-type']
@@ -42,42 +73,37 @@
         return subprocess.Popen(play_wav_cmd)
     except Exception as e:
         LOG.error(f"Failed to play: {play_wav_cmd}")
         LOG.debug(f"Error: {e}")
         return None
 
 
-SimpleAudioPluginConfig = {
-    "simple": {
-        "type": "ovos_simple",
-        "active": True
-    }
-}
-
-
-class OVOSSimpleService(OCPAudioPlayerBackend):
+class OVOSSimpleService(AudioBackend):
     sox_play = find_executable("play")
     pulse_play = find_executable("paplay")
     alsa_play = find_executable("aplay")
     mpg123_play = find_executable("mpg123")
 
     def __init__(self, config, bus=None, name='ovos_simple'):
         super(OVOSSimpleService, self).__init__(config, bus)
         self.name = name
 
         self.process = None
         self._stop_signal = False
         self._is_playing = False
+        self._time_accumulator = 0
+        self._start = 0
         self._paused = False
 
         self.supports_mime_hints = True
         mimetypes.init()
 
         self.bus.on('ovos.common_play.simple.play', self._play)
 
+    ###################
     # simple player internals
     def _get_track(self, track_data):
         if isinstance(track_data, list):
             track = track_data[0]
             mime = track_data[1]
             mime = mime.split('/')
         else:  # Assume string
@@ -151,81 +177,139 @@
         uri = track.replace('file://', '')
 
         try:
             self.process = play_audio(uri, player)
         except FileNotFoundError as e:
             LOG.error(f'Couldn\'t play audio, {e}')
             self.process = None
-            self.ocp_error()
         except Exception as e:
             LOG.exception(repr(e))
             self.process = None
-            self.ocp_error()
 
-        # Wait for completion or stop request
-        while (self._is_process_running() and not self._stop_signal):
-            sleep(0.25)
-
-        if self._stop_signal:
-            self._stop_running_process()
-            self._is_playing = False
-            self._paused = False
-            return
+        if self.process:
+            # Wait for completion or stop request
+            while (self._is_process_running() and not self._stop_signal):
+                sleep(0.25)
+
+            if self._stop_signal:
+                self._stop_running_process()
+                self._is_playing = False
+                self._paused = False
+                return
+            else:
+                self.process = None
         else:
-            self.process = None
+            try:
+                self.ocp_error()
+            except:  # too old OPM version
+                self.bus.emit(Message("ovos.common_play.media.state",
+                                      {"state": MediaState.INVALID_MEDIA}))
 
         self._track_start_callback(None)
         self._is_playing = False
         self._paused = False
-        self.ocp_stop()
 
-    # audio service
+    ############
+    # mandatory abstract methods
+
+    @property
+    def playback_time(self):
+        """ in milliseconds """
+        return max(self._start - time.time(), 0) + self._time_accumulator
+
     def supported_uris(self):
         uris = ['file', 'http']
         if self.sox_play:
             uris.append("https")
         return uris
 
     def play(self, repeat=False):
         """ Play playlist using simple. """
-        self.ocp_start()
+        self._start = time.time()
+        self._time_accumulator = 0
         self.bus.emit(Message('ovos.common_play.simple.play',
                               {'repeat': repeat}))
 
     def stop(self):
         """ Stop simple playback. """
         LOG.info('SimpleService Stop')
+        self._start = self._time_accumulator = 0
         if self._is_playing:
             self._stop_signal = True
             while self._is_playing:
                 sleep(0.1)
             self._stop_signal = False
-            self.ocp_stop()
             return True
         return False
 
     def pause(self):
         """ Pause simple playback. """
         if self.process and not self._paused:
+            if self._start:
+                self._time_accumulator += time.time() - self._start
+                self._start = 0
             # Suspend the playback process
             self.process.send_signal(signal.SIGSTOP)
             self._paused = True
-            self.ocp_pause()
 
     def resume(self):
         """ Resume paused playback. """
         if self.process and self._paused:
+            self._start = time.time()
             # Resume the playback process
             self.process.send_signal(signal.SIGCONT)
             self._paused = False
-            self.ocp_resume()
 
-    def track_info(self):
-        """ Extract info of current track. """
-        return {"track": self._now_playing}
+    def get_track_position(self):
+        """
+        get current position in milliseconds
+        """
+        return self.playback_time
+
+    ################
+    # missing features in simple audio plugin
+    def lower_volume(self):
+        LOG.error("simple audio player does not support lower_volume")
+
+    def restore_volume(self):
+        LOG.error("simple audio player does not support restore_volume")
+
+    def get_track_length(self):
+        """
+        getting the duration of the audio in milliseconds
+        """
+        LOG.error("simple audio player does not support get_track_length")
+        return self.playback_time
+
+    def set_track_position(self, milliseconds):
+        """
+        go to position in milliseconds
+
+          Args:
+                milliseconds (int): number of milliseconds of final position
+        """
+        LOG.error("simple audio player does not support set_track_position")
+
+    def seek_forward(self, seconds=1):
+        """
+        skip X seconds
+
+          Args:
+                seconds (int): number of seconds to seek, if negative rewind
+        """
+        LOG.error("simple audio player does not support seek_forward")
+
+    def seek_backward(self, seconds=1):
+        """
+        rewind X seconds
+
+          Args:
+                seconds (int): number of seconds to seek, if negative rewind
+        """
+        LOG.error("simple audio player does not support seek_backward")
 
 
 def load_service(base_config, bus):
     backends = base_config.get('backends', [])
     services = [(b, backends[b]) for b in backends
                 if backends[b]['type'] in ["simple", 'ovos_simple'] and
                 backends[b].get('active', False)]
@@ -235,7 +319,15 @@
                 OVOSSimpleService.alsa_play,
                 OVOSSimpleService.mpg123_play]):
         LOG.error("No basic playback functionality detected!!")
         return []
 
     instances = [OVOSSimpleService(s[1], bus, s[0]) for s in services]
     return instances
+
+
+SimpleAudioPluginConfig = {
+    "simple": {
+        "type": "ovos_simple",
+        "active": True
+    }
+}
```

## ovos_audio_plugin_simple/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 2
-VERSION_ALPHA = 4
+VERSION_ALPHA = 6
 # END_VERSION_BLOCK
```

## Comparing `ovos_audio_plugin_simple-0.0.2a4.dist-info/LICENSE` & `ovos_audio_plugin_simple-0.0.2a6.dist-info/LICENSE`

 * *Files identical despite different names*

