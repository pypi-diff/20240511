# Comparing `tmp/bunkrruploader-0.10.4.tar.gz` & `tmp/bunkrruploader-0.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunkrruploader-0.10.4.tar", last modified: Sat May 11 01:17:18 2024, max compression
+gzip compressed data, was "bunkrruploader-0.10.5.tar", last modified: Sat May 11 01:31:40 2024, max compression
```

## Comparing `bunkrruploader-0.10.4.tar` & `bunkrruploader-0.10.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/
--rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-05-05 14:52:19.000000 bunkrruploader-0.10.4/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)     4747 2024-05-10 03:22:16.000000 bunkrruploader-0.10.4/README.md
--rw-r--r--   0 alex      (1000) alex      (1001)     1545 2024-05-11 01:16:52.000000 bunkrruploader-0.10.4/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/src/
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      507 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-11 01:17:18.000000 bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        0 2024-05-10 02:35:40.000000 bunkrruploader-0.10.4/src/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:17:18.839014 bunkrruploader-0.10.4/src/bunkrr_uploader/
--rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-05-10 02:38:32.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1001)    11984 2024-05-11 01:06:25.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/api.py
--rw-r--r--   0 alex      (1000) alex      (1001)     5755 2024-05-11 01:07:27.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/bunkrr_uploader.py
--rw-r--r--   0 alex      (1000) alex      (1001)     2176 2024-05-11 01:03:01.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/cli.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1557 2024-05-11 00:32:15.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/types.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1492 2024-05-10 03:02:29.000000 bunkrruploader-0.10.4/src/bunkrr_uploader/util.py
--rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-05-10 02:35:41.000000 bunkrruploader-0.10.4/src/bunkrr_uploader.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:31:40.453095 bunkrruploader-0.10.5/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-05-05 14:52:19.000000 bunkrruploader-0.10.5/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 01:31:40.453095 bunkrruploader-0.10.5/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)     4747 2024-05-10 03:22:16.000000 bunkrruploader-0.10.5/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)     1545 2024-05-11 01:31:28.000000 bunkrruploader-0.10.5/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-11 01:31:40.453095 bunkrruploader-0.10.5/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:31:40.449762 bunkrruploader-0.10.5/src/
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:31:40.453095 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 01:31:40.000000 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      507 2024-05-11 01:31:40.000000 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-11 01:31:40.000000 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-05-11 01:31:40.000000 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-05-11 01:31:40.000000 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-11 01:31:40.000000 bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        0 2024-05-10 02:35:40.000000 bunkrruploader-0.10.5/src/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 01:31:40.453095 bunkrruploader-0.10.5/src/bunkrr_uploader/
+-rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-05-10 02:38:32.000000 bunkrruploader-0.10.5/src/bunkrr_uploader/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    11984 2024-05-11 01:06:25.000000 bunkrruploader-0.10.5/src/bunkrr_uploader/api.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     5793 2024-05-11 01:30:44.000000 bunkrruploader-0.10.5/src/bunkrr_uploader/bunkrr_uploader.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     2176 2024-05-11 01:03:01.000000 bunkrruploader-0.10.5/src/bunkrr_uploader/cli.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1557 2024-05-11 00:32:15.000000 bunkrruploader-0.10.5/src/bunkrr_uploader/types.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1492 2024-05-10 03:02:29.000000 bunkrruploader-0.10.5/src/bunkrr_uploader/util.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-05-10 02:35:41.000000 bunkrruploader-0.10.5/src/bunkrr_uploader.py
```

### Comparing `bunkrruploader-0.10.4/LICENSE` & `bunkrruploader-0.10.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.4/PKG-INFO` & `bunkrruploader-0.10.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunkrrUploader
-Version: 0.10.4
+Version: 0.10.5
 Summary: Bunkrr uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/bunkrr-uploader
 Project-URL: Repository, https://github.com/alexmi256/bunkrr-uploader.git
 Keywords: bunkrr,upload,storage,parallel
```

### Comparing `bunkrruploader-0.10.4/README.md` & `bunkrruploader-0.10.5/README.md`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.4/pyproject.toml` & `bunkrruploader-0.10.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BunkrrUploader"
-version = "0.10.4"
+version = "0.10.5"
 description = "Bunkrr uploader supporting parallel uploads"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT License"}
 keywords = ["bunkrr", "upload", "storage", "parallel"]
 authors = [
     {name = "Alex Mi", email = "alexmi3.14@gmail.com"},
```

### Comparing `bunkrruploader-0.10.4/src/BunkrrUploader.egg-info/PKG-INFO` & `bunkrruploader-0.10.5/src/BunkrrUploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunkrrUploader
-Version: 0.10.4
+Version: 0.10.5
 Summary: Bunkrr uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/bunkrr-uploader
 Project-URL: Repository, https://github.com/alexmi256/bunkrr-uploader.git
 Keywords: bunkrr,upload,storage,parallel
```

### Comparing `bunkrruploader-0.10.4/src/bunkrr_uploader/api.py` & `bunkrruploader-0.10.5/src/bunkrr_uploader/api.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.4/src/bunkrr_uploader/bunkrr_uploader.py` & `bunkrruploader-0.10.5/src/bunkrr_uploader/bunkrr_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,19 +67,21 @@
     def prepare_file_for_upload(self, file: Path) -> List[Path]:
         file_size = os.stat(file).st_size
 
         # TODO: Truncate the file name if it is too long
         file_name = (file.name[:240] + "..") if len(file.name) > 240 else file.name
 
         if file.suffix in self.api.file_blacklist:
-            raise Exception(f"File {file} has blacklisted extension {file.suffix}")
+            logger.error(f"File {file} has blacklisted extension {file.suffix}")
+            return []
 
         if file_size > self.api.max_file_size:
             # TODO: Create temporary file archive
-            raise Exception(f"File {file} is bigger than max file size {self.api.max_file_size}")
+            logger.error(f"File {file} is bigger than max file size {self.api.max_file_size}")
+            return []
 
         return [file]
 
     async def upload_files(self, path: Path, folder: Optional[str] = None) -> None:
         if path.is_file():
             paths = [path]
         else:
```

### Comparing `bunkrruploader-0.10.4/src/bunkrr_uploader/cli.py` & `bunkrruploader-0.10.5/src/bunkrr_uploader/cli.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.4/src/bunkrr_uploader/types.py` & `bunkrruploader-0.10.5/src/bunkrr_uploader/types.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.4/src/bunkrr_uploader/util.py` & `bunkrruploader-0.10.5/src/bunkrr_uploader/util.py`

 * *Files identical despite different names*

