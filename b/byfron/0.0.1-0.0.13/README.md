# Comparing `tmp/byfron-0.0.1.tar.gz` & `tmp/byfron-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byfron-0.0.1.tar", last modified: Sat May 11 00:09:11 2024, max compression
+gzip compressed data, was "byfron-0.0.13.tar", last modified: Sat May 11 00:12:51 2024, max compression
```

## Comparing `byfron-0.0.1.tar` & `byfron-0.0.13.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 valed     (1000) valed     (1000)        0 2024-05-11 00:09:11.259076 byfron-0.0.1/
--rwxrwxrwx   0 valed     (1000) valed     (1000)     1067 2024-05-10 17:45:06.000000 byfron-0.0.1/LICENSE
--rwxrwxrwx   0 valed     (1000) valed     (1000)      705 2024-05-11 00:09:11.256069 byfron-0.0.1/PKG-INFO
--rwxrwxrwx   0 valed     (1000) valed     (1000)      102 2024-05-10 17:45:06.000000 byfron-0.0.1/README.md
-drwxrwxrwx   0 valed     (1000) valed     (1000)        0 2024-05-11 00:09:11.170505 byfron-0.0.1/byfron.egg-info/
--rwxrwxrwx   0 valed     (1000) valed     (1000)      705 2024-05-11 00:09:10.000000 byfron-0.0.1/byfron.egg-info/PKG-INFO
--rwxrwxrwx   0 valed     (1000) valed     (1000)      239 2024-05-11 00:09:11.000000 byfron-0.0.1/byfron.egg-info/SOURCES.txt
--rwxrwxrwx   0 valed     (1000) valed     (1000)        1 2024-05-11 00:09:10.000000 byfron-0.0.1/byfron.egg-info/dependency_links.txt
--rwxrwxrwx   0 valed     (1000) valed     (1000)       32 2024-05-11 00:09:10.000000 byfron-0.0.1/byfron.egg-info/requires.txt
--rwxrwxrwx   0 valed     (1000) valed     (1000)       10 2024-05-11 00:09:10.000000 byfron-0.0.1/byfron.egg-info/top_level.txt
--rwxrwxrwx   0 valed     (1000) valed     (1000)       38 2024-05-11 00:09:11.260843 byfron-0.0.1/setup.cfg
--rwxrwxrwx   0 valed     (1000) valed     (1000)     1445 2024-05-10 17:45:06.000000 byfron-0.0.1/setup.py
-drwxrwxrwx   0 valed     (1000) valed     (1000)        0 2024-05-11 00:09:11.231945 byfron-0.0.1/vidstream/
--rwxrwxrwx   0 valed     (1000) valed     (1000)      269 2024-05-10 17:45:06.000000 byfron-0.0.1/vidstream/__init__.py
--rwxrwxrwx   0 valed     (1000) valed     (1000)     4203 2024-05-10 17:45:06.000000 byfron-0.0.1/vidstream/audio.py
--rwxrwxrwx   0 valed     (1000) valed     (1000)    14643 2024-05-10 17:45:06.000000 byfron-0.0.1/vidstream/streaming.py
+drwxrwxrwx   0 valed     (1000) valed     (1000)        0 2024-05-11 00:12:51.433350 byfron-0.0.13/
+-rwxrwxrwx   0 valed     (1000) valed     (1000)     1067 2024-05-10 17:45:06.000000 byfron-0.0.13/LICENSE
+-rwxrwxrwx   0 valed     (1000) valed     (1000)      723 2024-05-11 00:12:51.433350 byfron-0.0.13/PKG-INFO
+-rwxrwxrwx   0 valed     (1000) valed     (1000)      102 2024-05-10 17:45:06.000000 byfron-0.0.13/README.md
+drwxrwxrwx   0 valed     (1000) valed     (1000)        0 2024-05-11 00:12:51.349528 byfron-0.0.13/byfron.egg-info/
+-rwxrwxrwx   0 valed     (1000) valed     (1000)      723 2024-05-11 00:12:51.000000 byfron-0.0.13/byfron.egg-info/PKG-INFO
+-rwxrwxrwx   0 valed     (1000) valed     (1000)      239 2024-05-11 00:12:51.000000 byfron-0.0.13/byfron.egg-info/SOURCES.txt
+-rwxrwxrwx   0 valed     (1000) valed     (1000)        1 2024-05-11 00:12:51.000000 byfron-0.0.13/byfron.egg-info/dependency_links.txt
+-rwxrwxrwx   0 valed     (1000) valed     (1000)       32 2024-05-11 00:12:51.000000 byfron-0.0.13/byfron.egg-info/requires.txt
+-rwxrwxrwx   0 valed     (1000) valed     (1000)       10 2024-05-11 00:12:51.000000 byfron-0.0.13/byfron.egg-info/top_level.txt
+-rwxrwxrwx   0 valed     (1000) valed     (1000)       38 2024-05-11 00:12:51.433350 byfron-0.0.13/setup.cfg
+-rwxrwxrwx   0 valed     (1000) valed     (1000)     1140 2024-05-11 00:12:29.000000 byfron-0.0.13/setup.py
+drwxrwxrwx   0 valed     (1000) valed     (1000)        0 2024-05-11 00:12:51.409167 byfron-0.0.13/vidstream/
+-rwxrwxrwx   0 valed     (1000) valed     (1000)      269 2024-05-10 17:45:06.000000 byfron-0.0.13/vidstream/__init__.py
+-rwxrwxrwx   0 valed     (1000) valed     (1000)     4203 2024-05-10 17:45:06.000000 byfron-0.0.13/vidstream/audio.py
+-rwxrwxrwx   0 valed     (1000) valed     (1000)    14643 2024-05-10 17:45:06.000000 byfron-0.0.13/vidstream/streaming.py
```

### Comparing `byfron-0.0.1/LICENSE` & `byfron-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `byfron-0.0.1/PKG-INFO` & `byfron-0.0.13/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: byfron
-Version: 0.0.1
-Summary: Byfron Destroyer
+Version: 0.0.13
+Summary: Streaming video data via networks
 Home-page: UNKNOWN
 Author: munchdogs
 Author-email: <aledreamsaledreams2@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `byfron-0.0.1/byfron.egg-info/PKG-INFO` & `byfron-0.0.13/byfron.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: byfron
-Version: 0.0.1
-Summary: Byfron Destroyer
+Version: 0.0.13
+Summary: Streaming video data via networks
 Home-page: UNKNOWN
 Author: munchdogs
 Author-email: <aledreamsaledreams2@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `byfron-0.0.1/vidstream/audio.py` & `byfron-0.0.13/vidstream/audio.py`

 * *Files identical despite different names*

### Comparing `byfron-0.0.1/vidstream/streaming.py` & `byfron-0.0.13/vidstream/streaming.py`

 * *Files identical despite different names*

