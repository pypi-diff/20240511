# Comparing `tmp/ytmusic_deleter-2.3.0.tar.gz` & `tmp/ytmusic_deleter-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.3.0.tar", last modified: Tue May  7 02:32:09 2024, max compression
+gzip compressed data, was "ytmusic_deleter-2.3.1.tar", last modified: Sat May 11 20:58:23 2024, max compression
```

## Comparing `ytmusic_deleter-2.3.0.tar` & `ytmusic_deleter-2.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-05-07 02:31:49.361217 ytmusic_deleter-2.3.0/LICENSE
--rw-r--r--   0        0        0     1447 2024-05-07 02:32:09.001088 ytmusic_deleter-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5794 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1304 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/tests/resources/test.example.cfg
--rw-r--r--   0        0        0     4090 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     5475 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/README.md
--rw-r--r--   0        0        0       22 2024-05-07 02:32:09.001088 ytmusic_deleter-2.3.0/ytmusic_deleter/_version.py
--rw-r--r--   0        0        0     1142 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/auth.py
--rw-r--r--   0        0        0    20465 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/cli.py
--rw-r--r--   0        0        0      168 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/constants.py
--rw-r--r--   0        0        0      319 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/progress.py
--rw-r--r--   0        0        0     9521 2024-05-07 02:31:49.365217 ytmusic_deleter-2.3.0/ytmusic_deleter/uploads.py
--rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-11 20:58:07.178031 ytmusic_deleter-2.3.1/LICENSE
+-rw-r--r--   0        0        0     1447 2024-05-11 20:58:23.018068 ytmusic_deleter-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6578 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1304 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/tests/resources/test.example.cfg
+-rw-r--r--   0        0        0     4090 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     5475 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/ytmusic_deleter/README.md
+-rw-r--r--   0        0        0       22 2024-05-11 20:58:23.018068 ytmusic_deleter-2.3.1/ytmusic_deleter/_version.py
+-rw-r--r--   0        0        0     1142 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/ytmusic_deleter/auth.py
+-rw-r--r--   0        0        0    20465 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/ytmusic_deleter/cli.py
+-rw-r--r--   0        0        0      168 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/ytmusic_deleter/constants.py
+-rw-r--r--   0        0        0      319 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/ytmusic_deleter/progress.py
+-rw-r--r--   0        0        0     9521 2024-05-11 20:58:07.182031 ytmusic_deleter-2.3.1/ytmusic_deleter/uploads.py
+-rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.3.1/PKG-INFO
```

### Comparing `ytmusic_deleter-2.3.0/LICENSE` & `ytmusic_deleter-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/pyproject.toml` & `ytmusic_deleter-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "click>=8.1.7",
     "enlighten>=1.12.4",
     "thefuzz>=0.22.1",
     "ytmusicapi>=1.7.0",
 ]
 requires-python = "<3.13,>=3.8.1"
 readme = "ytmusic_deleter/README.md"
-version = "2.3.0"
+version = "2.3.1"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.scripts]
 ytmusic-deleter = "ytmusic_deleter.cli:cli"
```

### Comparing `ytmusic_deleter-2.3.0/tests/conftest.py` & `ytmusic_deleter-2.3.1/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -92,29 +92,38 @@
 
 @pytest.fixture(name="upload_song")
 def fixture_upload_song(config, yt_browser: YTMusic) -> Dict | None:
     """
     Upload a song and wait for it to finish processing.
     Return the song object or None if it did not upload successfully.
     """
-    response = yt_browser.upload_song(get_resource(config["uploads"]["file"]))
-    if not isinstance(response, str) and response.status_code == 409:
-        # Song already uploaded
-        return True
+    upload_response = yt_browser.upload_song(get_resource(config["uploads"]["file"]))
+    if not isinstance(upload_response, str) and upload_response.status_code == 409:
+        # Song is already in uploads. Delete it and re-upload.
+        # Although this app is not responsible for verifying that upload works properly,
+        # we still want to verify that no errors happen if we try to delete a song right
+        # after it was uploaded, since this was an issue previously https://github.com/sigma67/ytmusicapi/issues/578.
+        songs = yt_browser.get_library_upload_songs()
+        delete_response = None
+        for song in songs:
+            if song.get("title") in config["uploads"]["file"]:
+                delete_response = yt_browser.delete_upload_entity(song["entityId"])
+        assert delete_response == "STATUS_SUCCEEDED"
+        # Need to wait for song to be fully deleted
+        time.sleep(10)
+        # Now re-upload
+        upload_response = yt_browser.upload_song(get_resource(config["uploads"]["file"]))
 
-    assert response == "STATUS_SUCCEEDED" or response.status_code == 200
+    assert upload_response == "STATUS_SUCCEEDED" or upload_response.status_code == 200
 
     # Wait for upload to finish processing
-    retries_remaining = 10
+    retries_remaining = 20
     while retries_remaining:
-        time.sleep(5)
-        try:
-            songs = yt_browser.get_library_upload_songs(limit=None)
-        except KeyError:
-            pass
+        time.sleep(2)
+        songs = yt_browser.get_library_upload_songs(limit=None)
         for song in songs:
             if song.get("title") in config["uploads"]["file"]:
                 return song
         retries_remaining -= 1
 
 
 @pytest.fixture(name="add_library_album")
```

### Comparing `ytmusic_deleter-2.3.0/tests/resources/test.example.cfg` & `ytmusic_deleter-2.3.1/tests/resources/test.example.cfg`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/tests/test_cli.py` & `ytmusic_deleter-2.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/ytmusic_deleter/README.md` & `ytmusic_deleter-2.3.1/ytmusic_deleter/README.md`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/ytmusic_deleter/auth.py` & `ytmusic_deleter-2.3.1/ytmusic_deleter/auth.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/ytmusic_deleter/cli.py` & `ytmusic_deleter-2.3.1/ytmusic_deleter/cli.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/ytmusic_deleter/uploads.py` & `ytmusic_deleter-2.3.1/ytmusic_deleter/uploads.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.0/PKG-INFO` & `ytmusic_deleter-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusic-deleter
-Version: 2.3.0
+Version: 2.3.1
 Summary: Easily delete your YouTube Music library
 Author-Email: apastel <alex.r.pastel@gmail.com>
 License: GPL-3.0
 Requires-Python: <3.13,>=3.8.1
 Requires-Dist: click>=8.1.7
 Requires-Dist: enlighten>=1.12.4
 Requires-Dist: thefuzz>=0.22.1
```

