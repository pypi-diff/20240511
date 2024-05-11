# Comparing `tmp/bunkrruploader-0.10.3.tar.gz` & `tmp/bunkrruploader-0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunkrruploader-0.10.3.tar", last modified: Sat May 11 00:59:07 2024, max compression
+gzip compressed data, was "bunkrruploader-0.10.4.tar", last modified: Sat May 11 01:17:18 2024, max compression
```

## Comparing `bunkrruploader-0.10.3.tar` & `bunkrruploader-0.10.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 00:59:07.567856 bunkrruploader-0.10.3/
--rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-05-05 14:52:19.000000 bunkrruploader-0.10.3/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 00:59:07.567856 bunkrruploader-0.10.3/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)     4747 2024-05-10 03:22:16.000000 bunkrruploader-0.10.3/README.md
--rw-r--r--   0 alex      (1000) alex      (1001)     1545 2024-05-10 02:52:52.000000 bunkrruploader-0.10.3/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-11 00:59:07.567856 bunkrruploader-0.10.3/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 00:59:07.567856 bunkrruploader-0.10.3/src/
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 00:59:07.567856 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 00:59:07.000000 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      507 2024-05-11 00:59:07.000000 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-11 00:59:07.000000 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-05-11 00:59:07.000000 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-05-11 00:59:07.000000 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-11 00:59:07.000000 bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        0 2024-05-10 02:35:40.000000 bunkrruploader-0.10.3/src/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 00:59:07.567856 bunkrruploader-0.10.3/src/bunkrr_uploader/
--rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-05-10 02:38:32.000000 bunkrruploader-0.10.3/src/bunkrr_uploader/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1001)    11958 2024-05-11 00:32:15.000000 bunkrruploader-0.10.3/src/bunkrr_uploader/api.py
--rw-r--r--   0 alex      (1000) alex      (1001)     5694 2024-05-11 00:40:45.000000 bunkrruploader-0.10.3/src/bunkrr_uploader/bunkrr_uploader.py
--rw-r--r--   0 alex      (1000) alex      (1001)     2034 2024-05-11 00:27:53.000000 bunkrruploader-0.10.3/src/bunkrr_uploader/cli.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1557 2024-05-11 00:32:15.000000 bunkrruploader-0.10.3/src/bunkrr_uploader/types.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1492 2024-05-10 03:02:29.000000 bunkrruploader-0.10.3/src/bunkrr_uploader/util.py
--rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-05-10 02:35:41.000000 bunkrruploader-0.10.3/src/bunkrr_uploader.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-05-05 14:52:19.000000 bunkrruploader-0.10.4/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)     4747 2024-05-10 03:22:16.000000 bunkrruploader-0.10.4/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)     1545 2024-05-11 01:16:52.000000 bunkrruploader-0.10.4/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/src/
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      507 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        0 2024-05-10 02:35:40.000000 bunkrruploader-0.10.4/src/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/src/bunkrr_uploader/
+-rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-05-10 02:38:32.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    11984 2024-05-11 01:06:25.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/api.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     5755 2024-05-11 01:07:27.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/bunkrr_uploader.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     2176 2024-05-11 01:03:01.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/cli.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1557 2024-05-11 00:32:15.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/types.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1492 2024-05-10 03:02:29.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/util.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-05-10 02:35:41.000000 bunkrruploader-0.10.4/src/bunkrr_uploader.py
```

### Comparing `bunkrruploader-0.10.3/LICENSE` & `bunkrruploader-0.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.3/PKG-INFO` & `bunkrruploader-0.10.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunkrrUploader
-Version: 0.10.3
+Version: 0.10.4
 Summary: Bunkrr uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/bunkrr-uploader
 Project-URL: Repository, https://github.com/alexmi256/bunkrr-uploader.git
 Keywords: bunkrr,upload,storage,parallel
```

### Comparing `bunkrruploader-0.10.3/README.md` & `bunkrruploader-0.10.4/README.md`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.3/pyproject.toml` & `bunkrruploader-0.10.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BunkrrUploader"
-version = "0.10.3"
+version = "0.10.4"
 description = "Bunkrr uploader supporting parallel uploads"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT License"}
 keywords = ["bunkrr", "upload", "storage", "parallel"]
 authors = [
     {name = "Alex Mi", email = "alexmi3.14@gmail.com"},
```

### Comparing `bunkrruploader-0.10.3/src/BunkrrUploader.egg-info/PKG-INFO` & `bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunkrrUploader
-Version: 0.10.3
+Version: 0.10.4
 Summary: Bunkrr uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/bunkrr-uploader
 Project-URL: Repository, https://github.com/alexmi256/bunkrr-uploader.git
 Keywords: bunkrr,upload,storage,parallel
```

### Comparing `bunkrruploader-0.10.3/src/bunkrr_uploader/api.py` & `bunkrruploader-0.10.4/src/bunkrr_uploader/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         }
         self.session = aiohttp.ClientSession("https://app.bunkrr.su", headers=self.session_headers)
 
         self.server_sessions = {}
         self.created_folders = {}
         self.sem = asyncio.Semaphore(max_connections)
         self.retries = retries
-        self.max_chunk_retries = retries
+        self.max_chunk_retries = options.get('chunk_retries') or 1
 
     async def get_check(self) -> CheckResponse:
         async with self.session.get("/api/check") as resp:
             response = await resp.json()
             return response
 
     async def get_node(self) -> NodeResponse:
```

### Comparing `bunkrruploader-0.10.3/src/bunkrr_uploader/bunkrr_uploader.py` & `bunkrruploader-0.10.4/src/bunkrr_uploader/bunkrr_uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pprint import pformat, pprint
 from typing import Any, List, Optional
 
 from .api import BunkrrAPI
 from .cli import cli
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(level=logging.DEBUG)
+logging.basicConfig(level=logging.WARNING)
 
 
 class BunkrrUploader:
     def __init__(
         self,
         token: str,
         max_connections: int = 1,
@@ -136,15 +136,18 @@
                 pprint(responses)
 
 
 async def async_main() -> None:
     args = cli()
     logger.debug(args)
 
-    options = {"save": args.save}
+    options = {
+        "save": args.save,
+        "chunk_retries": args.chunk_retries
+    }
 
     bunkrr_client = BunkrrUploader(args.token, max_connections=args.connections, retries=args.retries, options=options)
     try:
         await bunkrr_client.init()
         if args.dry_run:
             print("Dry run only, uploading skipped")
         else:
```

### Comparing `bunkrruploader-0.10.3/src/bunkrr_uploader/cli.py` & `bunkrruploader-0.10.4/src/bunkrr_uploader/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,12 +48,18 @@
         help="Whether to create and use a config file in $HOME/.config/gofile_upload/config.json",
     )
     parser.add_argument(
         "-r",
         "--retries",
         default=1,
         type=int,
-        help="How many times to retry a failed chunk, chunk completion, or upload",
+        help="How many times to retry a failed upload",
+    )
+    parser.add_argument(
+        "--chunk-retries",
+        default=1,
+        type=int,
+        help="How many times to retry a failed chunk or chunk completion",
     )
     args = parser.parse_args()
 
     return args
```

### Comparing `bunkrruploader-0.10.3/src/bunkrr_uploader/types.py` & `bunkrruploader-0.10.4/src/bunkrr_uploader/types.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.3/src/bunkrr_uploader/util.py` & `bunkrruploader-0.10.4/src/bunkrr_uploader/util.py`

 * *Files identical despite different names*

