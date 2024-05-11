# Comparing `tmp/soco-cli-0.4.8.tar.gz` & `tmp/soco-cli-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soco-cli-0.4.8.tar", last modified: Tue Aug  3 18:35:59 2021, max compression
+gzip compressed data, was "soco-cli-0.4.9.tar", last modified: Sat Aug  7 12:18:43 2021, max compression
```

## Comparing `soco-cli-0.4.8.tar` & `soco-cli-0.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2021-08-03 18:35:59.100247 soco-cli-0.4.8/
--rw-r--r--   0 pwt        (501) staff       (20)       25 2020-07-03 08:12:06.000000 soco-cli-0.4.8/MANIFEST.in
--rw-r--r--   0 pwt        (501) staff       (20)     4458 2021-08-03 18:35:59.100945 soco-cli-0.4.8/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)    74649 2021-08-03 18:35:09.000000 soco-cli-0.4.8/README.md
--rw-r--r--   0 pwt        (501) staff       (20)      106 2021-07-27 14:34:44.000000 soco-cli-0.4.8/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)       84 2021-08-03 18:35:59.120006 soco-cli-0.4.8/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)     1435 2021-07-07 10:52:06.000000 soco-cli-0.4.8/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2021-08-03 18:35:59.085537 soco-cli-0.4.8/soco_cli/
--rw-r--r--   0 pwt        (501) staff       (20)      494 2021-08-03 18:35:09.000000 soco-cli-0.4.8/soco_cli/__init__.py
--rw-r--r--   0 pwt        (501) staff       (20)      123 2021-02-05 13:36:30.000000 soco-cli-0.4.8/soco_cli/__main__.py
--rw-r--r--   0 pwt        (501) staff       (20)   108756 2021-08-03 18:35:09.000000 soco-cli-0.4.8/soco_cli/action_processor.py
--rw-r--r--   0 pwt        (501) staff       (20)     3691 2021-07-17 15:08:34.000000 soco-cli-0.4.8/soco_cli/aliases.py
--rw-r--r--   0 pwt        (501) staff       (20)     6283 2021-07-17 15:08:34.000000 soco-cli-0.4.8/soco_cli/api.py
--rw-r--r--   0 pwt        (501) staff       (20)     1442 2021-07-17 15:08:34.000000 soco-cli-0.4.8/soco_cli/check_for_update.py
--rw-r--r--   0 pwt        (501) staff       (20)     1800 2021-07-17 15:08:34.000000 soco-cli-0.4.8/soco_cli/cmd_parser.py
--rw-r--r--   0 pwt        (501) staff       (20)     4614 2021-07-17 15:08:34.000000 soco-cli-0.4.8/soco_cli/http_api.py
--rw-r--r--   0 pwt        (501) staff       (20)    30120 2021-08-03 18:35:09.000000 soco-cli-0.4.8/soco_cli/interactive.py
--rw-r--r--   0 pwt        (501) staff       (20)      812 2021-02-05 13:36:30.000000 soco-cli-0.4.8/soco_cli/keystroke_capture.py
--rw-r--r--   0 pwt        (501) staff       (20)     1737 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/m3u_parser.py
--rw-r--r--   0 pwt        (501) staff       (20)     2019 2021-02-05 13:36:30.000000 soco-cli-0.4.8/soco_cli/match_speaker_names.py
--rw-r--r--   0 pwt        (501) staff       (20)     9211 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/play_local_file.py
--rw-r--r--   0 pwt        (501) staff       (20)     5547 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/play_m3u_file.py
--rwxr--r--   0 pwt        (501) staff       (20)    17008 2021-07-30 15:54:05.000000 soco-cli-0.4.8/soco_cli/sonos.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2933 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/sonos_discover.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3818 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/speaker_info.py
--rw-r--r--   0 pwt        (501) staff       (20)    10146 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/speakers.py
--rw-r--r--   0 pwt        (501) staff       (20)     4921 2021-08-03 18:35:09.000000 soco-cli-0.4.8/soco_cli/track_follow.py
--rw-r--r--   0 pwt        (501) staff       (20)    23356 2021-08-03 18:35:09.000000 soco-cli-0.4.8/soco_cli/utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1411 2021-07-17 15:08:35.000000 soco-cli-0.4.8/soco_cli/wait_actions.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2021-08-03 18:35:59.098975 soco-cli-0.4.8/soco_cli.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     4458 2021-08-03 18:35:57.000000 soco-cli-0.4.8/soco_cli.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      753 2021-08-03 18:35:57.000000 soco-cli-0.4.8/soco_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2021-08-03 18:35:57.000000 soco-cli-0.4.8/soco_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      258 2021-08-03 18:35:57.000000 soco-cli-0.4.8/soco_cli.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       82 2021-08-03 18:35:57.000000 soco-cli-0.4.8/soco_cli.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)        9 2021-08-03 18:35:57.000000 soco-cli-0.4.8/soco_cli.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2021-08-07 12:18:43.694311 soco-cli-0.4.9/
+-rw-r--r--   0 pwt        (501) staff       (20)       25 2020-07-03 08:12:06.000000 soco-cli-0.4.9/MANIFEST.in
+-rw-r--r--   0 pwt        (501) staff       (20)     4458 2021-08-07 12:18:43.695783 soco-cli-0.4.9/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)    74649 2021-08-03 18:35:09.000000 soco-cli-0.4.9/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)      106 2021-07-27 14:34:44.000000 soco-cli-0.4.9/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       84 2021-08-07 12:18:43.702063 soco-cli-0.4.9/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)     1435 2021-07-07 10:52:06.000000 soco-cli-0.4.9/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2021-08-07 12:18:43.684962 soco-cli-0.4.9/soco_cli/
+-rw-r--r--   0 pwt        (501) staff       (20)      494 2021-08-07 12:18:00.000000 soco-cli-0.4.9/soco_cli/__init__.py
+-rw-r--r--   0 pwt        (501) staff       (20)      123 2021-02-05 13:36:30.000000 soco-cli-0.4.9/soco_cli/__main__.py
+-rw-r--r--   0 pwt        (501) staff       (20)   110013 2021-08-07 12:18:00.000000 soco-cli-0.4.9/soco_cli/action_processor.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3691 2021-07-17 15:08:34.000000 soco-cli-0.4.9/soco_cli/aliases.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6283 2021-07-17 15:08:34.000000 soco-cli-0.4.9/soco_cli/api.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1442 2021-07-17 15:08:34.000000 soco-cli-0.4.9/soco_cli/check_for_update.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1800 2021-07-17 15:08:34.000000 soco-cli-0.4.9/soco_cli/cmd_parser.py
+-rw-r--r--   0 pwt        (501) staff       (20)     4614 2021-07-17 15:08:34.000000 soco-cli-0.4.9/soco_cli/http_api.py
+-rw-r--r--   0 pwt        (501) staff       (20)    30120 2021-08-03 18:35:09.000000 soco-cli-0.4.9/soco_cli/interactive.py
+-rw-r--r--   0 pwt        (501) staff       (20)      812 2021-02-05 13:36:30.000000 soco-cli-0.4.9/soco_cli/keystroke_capture.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1737 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/m3u_parser.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2019 2021-02-05 13:36:30.000000 soco-cli-0.4.9/soco_cli/match_speaker_names.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9211 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/play_local_file.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5547 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/play_m3u_file.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17008 2021-07-30 15:54:05.000000 soco-cli-0.4.9/soco_cli/sonos.py
+-rwxr--r--   0 pwt        (501) staff       (20)     2933 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/sonos_discover.py
+-rwxr--r--   0 pwt        (501) staff       (20)     3818 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/speaker_info.py
+-rw-r--r--   0 pwt        (501) staff       (20)    10146 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/speakers.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5469 2021-08-07 12:18:00.000000 soco-cli-0.4.9/soco_cli/track_follow.py
+-rw-r--r--   0 pwt        (501) staff       (20)    23356 2021-08-03 18:35:09.000000 soco-cli-0.4.9/soco_cli/utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1411 2021-07-17 15:08:35.000000 soco-cli-0.4.9/soco_cli/wait_actions.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2021-08-07 12:18:43.692417 soco-cli-0.4.9/soco_cli.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     4458 2021-08-07 12:18:40.000000 soco-cli-0.4.9/soco_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      753 2021-08-07 12:18:40.000000 soco-cli-0.4.9/soco_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2021-08-07 12:18:40.000000 soco-cli-0.4.9/soco_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      258 2021-08-07 12:18:40.000000 soco-cli-0.4.9/soco_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       82 2021-08-07 12:18:40.000000 soco-cli-0.4.9/soco_cli.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        9 2021-08-07 12:18:40.000000 soco-cli-0.4.9/soco_cli.egg-info/top_level.txt
```

### Comparing `soco-cli-0.4.8/PKG-INFO` & `soco-cli-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soco-cli
-Version: 0.4.8
+Version: 0.4.9
 Summary: Sonos command line control utility, based on SoCo
 Home-page: https://github.com/avantrec/soco-cli
 Author: Avantrec Ltd
 Author-email: soco_cli@avantrec.com
 License: UNKNOWN
 Description: 
         [![Buy Me A Coffee](https://github.com/avantrec/soco-cli/raw/next_version/assets/bmc-button.png)](https://www.buymeacoffee.com/avantrec)
```

### Comparing `soco-cli-0.4.8/README.md` & `soco-cli-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/setup.py` & `soco-cli-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/action_processor.py` & `soco-cli-0.4.9/soco_cli/action_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,49 +366,62 @@
     logging.info("Current track info:\n{}".format(track_info))
 
     # Accumulate info elements to be printed
     elements = {"Channel": speaker.get_current_media_info()["channel"]}
 
     # Stream
     if track_info["duration"] == "0:00:00":
-        logging.info("Track is a stream")
+        logging.info("Track is a radio stream")
         for item in sorted(track_info):
             if item not in [
                 "metadata",
                 "album_art",
                 "duration",
                 "playlist_position",
                 "position",
                 "uri",
             ]:
                 elements[item.capitalize()] = track_info[item]
         try:
+            logging.info("Attempting to find 'Artist'")
             metadata = parse(track_info["metadata"])
             if elements["Artist"] == "":
                 elements["Artist"] = metadata["DIDL-Lite"]["item"]["dc:creator"]
         except:
-            pass
+            logging.info("Unable to find 'Artist'")
+        try:
+            logging.info("Attempting to find 'Radio Show' using events")
+            sub = speaker.avTransport.subscribe()
+            event = sub.events.get(timeout=0.5)
+            elements["Radio Show"] = event.variables[
+                "current_track_meta_data"
+            ].radio_show.rpartition(",")[0]
+            sub.unsubscribe()
+        except:
+            logging.info("Unable to find 'Radio Show'")
 
     # Podcast, Audio Book, or normal track
-    else:  # Track has duration
+    else:
+        logging.info("Track has a non-zero duration")
         metadata = parse(track_info["metadata"])
+        logging.info("Track metadata: {}".format(metadata))
 
         # Podcast
         if (
             metadata["DIDL-Lite"]["item"]["upnp:class"]
             == "object.item.audioItem.podcast"
         ):
             logging.info("Track is a podcast")
             try:
                 elements["Podcast"] = metadata["DIDL-Lite"]["item"]["r:podcast"]
                 elements["Release Date"] = metadata["DIDL-Lite"]["item"][
                     "r:releaseDate"
                 ][:10]
             except:
-                pass
+                logging.info("Failed to find 'Podcast' and/or 'Release Date'")
             for item in sorted(track_info):
                 if item not in ["metadata", "uri", "album_art", "album", "artist"]:
                     elements[item.capitalize()] = track_info[item]
 
         # Audio book
         elif (
             "object.item.audioItem.audioBook"
@@ -417,15 +430,15 @@
             logging.info("Track is an audio book")
             try:
                 elements["Book Title"] = elements.pop("Channel", "")
                 elements["Creator(s)"] = track_info["artist"]
                 elements["Narrator(s)"] = metadata["DIDL-Lite"]["item"]["r:narrator"]
                 elements["Chapter"] = metadata["DIDL-Lite"]["item"]["dc:title"]
             except:
-                pass
+                logging.info("Failed to find book details")
             for item in sorted(track_info):
                 if item not in [
                     "metadata",
                     "uri",
                     "album_art",
                     "album",
                     "artist",
@@ -445,16 +458,17 @@
     elements = {
         key: value
         for key, value in elements.items()
         if value != "" and value is not None
     }
 
     # Deduplicate 'Channel' and 'Title'
+    # Remove 'Title' if it contains no spaces (likely to be a URI or similar)
     try:
-        if elements["Channel"] == elements["Title"]:
+        if elements["Channel"] == elements["Title"] or not " " in elements["Title"]:
             elements.pop("Title", None)
     except KeyError:
         pass
 
     # Rename 'Playlist_position' and 'Position'
     try:
         elements["Playlist Position"] = elements["Playlist_position"]
@@ -2619,16 +2633,17 @@
         logging.info(
             "Subscribing to transport events from {}".format(speaker.player_name)
         )
     except Exception as e:
         error_report("Exception {}".format(e))
         return False
 
-    initial_playlist_number = None
     initial_title = None
+    initial_duration = None
+    initial_radio_show = None
 
     while True:
         try:
             event = sub.events.get(timeout=1.0)
             logging.info("Transport event received")
 
             # The code below didn't work; retain for possible future use
@@ -2645,43 +2660,49 @@
             #     return True
 
             if event.variables["transport_state"] not in ["PLAYING", "TRANSITIONING"]:
                 logging.info("Speaker is not playing")
                 event_unsubscribe(sub)
                 return True
 
-            if initial_playlist_number is None:
-                initial_playlist_number = event.variables["current_track"]
+            if initial_title is None:
+                track_info = speaker.get_current_track_info()
+                initial_title = track_info.pop("title", None)
+                initial_duration = track_info.pop("duration", None)
                 try:
-                    initial_title = speaker.get_current_track_info()["title"]
+                    initial_radio_show = event.variables["current_track_meta_data"].radio_show
                 except:
-                    initial_title = None
+                    pass
                 logging.info(
-                    "Initial title = '{}', initial playlist no. = {}".format(
-                        initial_title, initial_playlist_number
+                    "Initial title = '{}', initial duration = '{}', initial radio show = '{}'".format(
+                        initial_title, initial_duration, initial_radio_show
                     )
                 )
 
             else:
-                current_playlist_number = event.variables["current_track"]
+                track_info = speaker.get_current_track_info()
+                current_title = track_info.pop("title", None)
+                current_duration = track_info.pop("duration", None)
                 try:
-                    current_title = speaker.get_current_track_info()["title"]
+                    current_radio_show = event.variables["current_track_meta_data"].radio_show
                 except:
-                    current_title = None
+                    pass
                 logging.info(
-                    "Current title = '{}', current playlist no. = {}".format(
-                        current_title, current_playlist_number
+                    "Current title = '{}', current duration = '{}', current radio show = '{}'".format(
+                        current_title, current_duration, current_radio_show
                     )
                 )
-                # Check whether playlist number or track title have changed
+                # Check whether track title or duration have changed
                 if (
-                    current_playlist_number != initial_playlist_number
-                    or current_title != initial_title
+                    current_title != initial_title
+                    or current_duration != initial_duration
+                    or current_radio_show != initial_radio_show
                 ):
-                    logging.info("Track has changed")
+                    logging.info("Track/show has changed")
+                    logging.info("Unsubscribing from events")
                     event_unsubscribe(sub)
                     return True
 
         except Empty:
             pass
```

### Comparing `soco-cli-0.4.8/soco_cli/aliases.py` & `soco-cli-0.4.9/soco_cli/aliases.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/api.py` & `soco-cli-0.4.9/soco_cli/api.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/check_for_update.py` & `soco-cli-0.4.9/soco_cli/check_for_update.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/cmd_parser.py` & `soco-cli-0.4.9/soco_cli/cmd_parser.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/http_api.py` & `soco-cli-0.4.9/soco_cli/http_api.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/interactive.py` & `soco-cli-0.4.9/soco_cli/interactive.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/keystroke_capture.py` & `soco-cli-0.4.9/soco_cli/keystroke_capture.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/m3u_parser.py` & `soco-cli-0.4.9/soco_cli/m3u_parser.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/match_speaker_names.py` & `soco-cli-0.4.9/soco_cli/match_speaker_names.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/play_local_file.py` & `soco-cli-0.4.9/soco_cli/play_local_file.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/play_m3u_file.py` & `soco-cli-0.4.9/soco_cli/play_m3u_file.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/sonos.py` & `soco-cli-0.4.9/soco_cli/sonos.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/sonos_discover.py` & `soco-cli-0.4.9/soco_cli/sonos_discover.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/speaker_info.py` & `soco-cli-0.4.9/soco_cli/speaker_info.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/speakers.py` & `soco-cli-0.4.9/soco_cli/speakers.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/track_follow.py` & `soco-cli-0.4.9/soco_cli/track_follow.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,71 +65,82 @@
 
         # Print the track info
         exit_code, output, error_msg = run_command(
             speaker, "track", use_local_speaker_list=use_local_speaker_list
         )
         if exit_code == 0:
             # Manipulate output
-            output = output.split("\n ", 1)[1]
+            if "Using Line In" in output:
+                line_in = True
+                output = "   Playing from Line In\n"
+            else:
+                line_in = False
+                output = output.split("\n ", 1)[1]
             if not compact:
                 # Remove some of the line entries
                 output = re.sub(".*Playback.*\\n", "", output)
                 # output = re.sub(".*Elapsed.*\\n", "", output)
                 output = re.sub(".*URI.*\\n", "", output)
                 output = re.sub(".*Uri.*\\n", "", output)
                 # Prefix speaker name and timestamp
                 output = (
                     " [{}] Playing at ".format(speaker.player_name)
                     + timestamp()
                     + ":\n"
                     + output
                 )
             else:  # Compact (one line) output
-                # Ordering of keys determines output order
-                keys = [
-                    "Channel:",
-                    "Artist:",
-                    "Creator(s):",
-                    "Book Title:",
-                    "Chapter:",
-                    "Album:",
-                    "Podcast:",
-                    "Title:",
-                    "Release Date:",
-                    "Narrator(s):",
-                ]
-                elements = {}
-                for line in output.splitlines():
-                    for key in keys:
-                        if key in line:
-                            elements[key] = line.replace(key, "").lstrip()
-                output = "{:5d}: [{}] ".format(counter, timestamp(short=True))
+                if line_in:
+                    output = "{:5d}: [{}] Playing from Line In".format(
+                        counter, timestamp(short=True)
+                    )
+                else:
+                    # Ordering of keys determines output order
+                    keys = [
+                        "Channel:",
+                        "Radio Show:",
+                        "Artist:",
+                        "Creator(s):",
+                        "Book Title:",
+                        "Chapter:",
+                        "Album:",
+                        "Podcast:",
+                        "Title:",
+                        "Release Date:",
+                        "Narrator(s):",
+                    ]
+                    elements = {}
+                    for line in output.splitlines():
+                        for key in keys:
+                            if key in line:
+                                elements[key] = line.replace(key, "").lstrip()
+                    output = "{:5d}: [{}] ".format(counter, timestamp(short=True))
 
-                # Prune fields for audio books
-                if "Book Title:" in elements:
-                    elements.pop("Title:", None)
-                    elements.pop("Narrator(s):", None)
-                first = True
-                for key in keys:
-                    value = elements.pop(key, None)
-                    if value:
-                        if not first:
-                            output = output + "| "
-                        else:
-                            first = False
-                        output = output + key + " " + value + " "
+                    # Prune fields for audio books
+                    if "Book Title:" in elements:
+                        elements.pop("Title:", None)
+                        elements.pop("Narrator(s):", None)
+                    first = True
+                    for key in keys:
+                        value = elements.pop(key, None)
+                        if value:
+                            if not first:
+                                output = output + "| "
+                            else:
+                                first = False
+                            output = output + key + " " + value + " "
 
             print(output, flush=True)
         else:
             error_out = "{:5d}: [{}] {}".format(
                 counter, timestamp(short=True), error_msg
             )
             print(error_out, flush=True)
 
         logging.info("Waiting for end of track")
         run_command(
             speaker, "wait_end_track", use_local_speaker_list=use_local_speaker_list
         )
 
-        logging.info("Waiting 3s for playback to stabilise")
-        sleep(3.0)
+        logging.info("Waiting 1.5s for playback to stabilise")
+        sleep(1.5)
         counter += 1
```

### Comparing `soco-cli-0.4.8/soco_cli/utils.py` & `soco-cli-0.4.9/soco_cli/utils.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli/wait_actions.py` & `soco-cli-0.4.9/soco_cli/wait_actions.py`

 * *Files identical despite different names*

### Comparing `soco-cli-0.4.8/soco_cli.egg-info/PKG-INFO` & `soco-cli-0.4.9/soco_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soco-cli
-Version: 0.4.8
+Version: 0.4.9
 Summary: Sonos command line control utility, based on SoCo
 Home-page: https://github.com/avantrec/soco-cli
 Author: Avantrec Ltd
 Author-email: soco_cli@avantrec.com
 License: UNKNOWN
 Description: 
         [![Buy Me A Coffee](https://github.com/avantrec/soco-cli/raw/next_version/assets/bmc-button.png)](https://www.buymeacoffee.com/avantrec)
```

### Comparing `soco-cli-0.4.8/soco_cli.egg-info/SOURCES.txt` & `soco-cli-0.4.9/soco_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

