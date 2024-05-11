# Comparing `tmp/innertube-2.1.3.tar.gz` & `tmp/innertube-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innertube-2.1.3.tar", max compression
+gzip compressed data, was "innertube-2.1.9.tar", max compression
```

## Comparing `innertube-2.1.3.tar` & `innertube-2.1.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1067 2022-08-07 19:16:46.083277 innertube-2.1.3/LICENSE
--rw-r--r--   0        0        0     3507 2023-01-22 12:27:54.564314 innertube-2.1.3/README.md
--rw-r--r--   0        0        0      382 2022-08-07 19:16:46.083277 innertube-2.1.3/innertube/__init__.py
--rw-r--r--   0        0        0     2125 2022-08-08 12:36:32.175738 innertube-2.1.3/innertube/adaptor.py
--rw-r--r--   0        0        0     2737 2022-08-07 19:20:43.526183 innertube-2.1.3/innertube/api.py
--rw-r--r--   0        0        0     5316 2023-01-22 12:27:54.564314 innertube-2.1.3/innertube/clients.py
--rw-r--r--   0        0        0    13842 2022-08-07 19:19:24.620562 innertube-2.1.3/innertube/config.py
--rw-r--r--   0        0        0     2146 2023-01-22 12:27:54.564314 innertube-2.1.3/innertube/enums.py
--rw-r--r--   0        0        0      226 2022-08-07 19:16:46.083277 innertube-2.1.3/innertube/errors.py
--rw-r--r--   0        0        0     2649 2022-08-07 19:16:46.083277 innertube-2.1.3/innertube/models.py
--rw-r--r--   0        0        0      293 2022-08-07 19:16:46.083277 innertube-2.1.3/innertube/protocols.py
--rw-r--r--   0        0        0      123 2022-08-07 19:16:46.083277 innertube-2.1.3/innertube/utils.py
--rw-r--r--   0        0        0      895 2023-01-22 12:27:54.564314 innertube-2.1.3/pyproject.toml
--rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 innertube-2.1.3/setup.py
--rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 innertube-2.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-03-01 21:01:26.576305 innertube-2.1.9/LICENSE
+-rw-r--r--   0        0        0     3507 2023-03-01 21:01:26.576305 innertube-2.1.9/README.md
+-rw-r--r--   0        0        0      382 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/__init__.py
+-rw-r--r--   0        0        0     2125 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/adaptor.py
+-rw-r--r--   0        0        0     2737 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/api.py
+-rw-r--r--   0        0        0     5195 2023-07-30 12:39:12.304595 innertube-2.1.9/innertube/clients.py
+-rw-r--r--   0        0        0    13842 2023-07-30 12:39:12.304595 innertube-2.1.9/innertube/config.py
+-rw-r--r--   0        0        0     2146 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/enums.py
+-rw-r--r--   0        0        0      226 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/errors.py
+-rw-r--r--   0        0        0     2649 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/models.py
+-rw-r--r--   0        0        0      293 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/protocols.py
+-rw-r--r--   0        0        0      123 2023-03-01 21:01:26.576305 innertube-2.1.9/innertube/utils.py
+-rw-r--r--   0        0        0      895 2023-07-30 12:39:12.304595 innertube-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4370 1970-01-01 00:00:00.000000 innertube-2.1.9/PKG-INFO
```

### Comparing `innertube-2.1.3/LICENSE` & `innertube-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `innertube-2.1.3/README.md` & `innertube-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `innertube-2.1.3/innertube/adaptor.py` & `innertube-2.1.9/innertube/adaptor.py`

 * *Files identical despite different names*

### Comparing `innertube-2.1.3/innertube/api.py` & `innertube-2.1.9/innertube/api.py`

 * *Files identical despite different names*

### Comparing `innertube-2.1.3/innertube/clients.py` & `innertube-2.1.9/innertube/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,24 +102,19 @@
         browse_id: Optional[str] = None,
         *,
         params: Optional[str] = None,
         continuation: Optional[str] = None,
     ) -> dict:
         return self(
             Endpoint.BROWSE,
-            params=utils.filter(
-                dict(
-                    continuation=continuation,
-                    ctoken=continuation,
-                )
-            ),
             body=utils.filter(
                 dict(
                     browseId=browse_id,
                     params=params,
+                    continuation=continuation,
                 )
             ),
         )
 
     def search(
         self,
         query: Optional[str] = None,
@@ -155,15 +150,15 @@
         return self(
             Endpoint.NEXT,
             body=utils.filter(
                 dict(
                     params=params,
                     playlistId=playlist_id,
                     videoId=video_id,
-                    index=index,
+                    playlistIndex=index,
                     continuation=continuation,
                 )
             ),
         )
 
     def get_transcript(
         self,
```

### Comparing `innertube-2.1.3/innertube/config.py` & `innertube-2.1.9/innertube/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 config: Config = Config(
     base_url="https://youtubei.googleapis.com/youtubei/v1/",
     clients=[
         ClientContext(
             client_id=1,
             client_name="WEB",
-            client_version="2.20210223.09.00",
+            client_version="2.20230728.00.00",
             user_agent=USER_AGENT_WEB,
             referer=REFERER_YOUTUBE,
             api_key="AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8",
         ),
         ClientContext(
             client_id=2,
             client_name="MWEB",
@@ -282,15 +282,15 @@
             client_version="16.20",
             user_agent=USER_AGENT_IOS,
             api_key="AIzaSyDCU8hByM-4DrUqRUYnGn-3llEO78bcxq8",
         ),
         ClientContext(
             client_id=67,
             client_name="WEB_REMIX",
-            client_version="1.20220607.03.01",
+            client_version="1.20230724.00.00",
             user_agent=USER_AGENT_WEB,
             referer=REFERER_YOUTUBE_MUSIC,
             api_key="AIzaSyC9XL3ZjWddXya6X74dJoCTL-WEYFDNX30",
         ),
         ClientContext(
             client_id=68,
             client_name="IOS_UPTIME",
```

### Comparing `innertube-2.1.3/innertube/enums.py` & `innertube-2.1.9/innertube/enums.py`

 * *Files identical despite different names*

### Comparing `innertube-2.1.3/innertube/models.py` & `innertube-2.1.9/innertube/models.py`

 * *Files identical despite different names*

### Comparing `innertube-2.1.3/pyproject.toml` & `innertube-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "innertube"
-version = "2.1.3"
+version = "2.1.9"
 description = "Python Client for Google's Private InnerTube API. Works with Youtube, YouTube Music and more!"
 authors = ["Tom Bulled <26026015+tombulled@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/innertube/"
 repository = "https://github.com/tombulled/innertube"
 keywords = ["innertube", "youtube", "youtubei", "python", "api", "client"]
```

### Comparing `innertube-2.1.3/PKG-INFO` & `innertube-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: innertube
-Version: 2.1.3
+Version: 2.1.9
 Summary: Python Client for Google's Private InnerTube API. Works with Youtube, YouTube Music and more!
 Home-page: https://pypi.org/project/innertube/
 License: MIT
 Keywords: innertube,youtube,youtubei,python,api,client
 Author: Tom Bulled
 Author-email: 26026015+tombulled@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

