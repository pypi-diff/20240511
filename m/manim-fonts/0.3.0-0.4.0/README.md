# Comparing `tmp/manim_fonts-0.3.0.tar.gz` & `tmp/manim_fonts-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manim_fonts-0.3.0.tar", max compression
+gzip compressed data, was "manim_fonts-0.4.0.tar", max compression
```

## Comparing `manim_fonts-0.3.0.tar` & `manim_fonts-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1518 2024-01-01 17:17:40.174874 manim_fonts-0.3.0/LICENSE
--rw-r--r--   0        0        0     1307 2024-01-01 17:17:40.174874 manim_fonts-0.3.0/README.md
--rw-r--r--   0        0        0      820 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       67 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/__init__.py
--rw-r--r--   0        0        0       58 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/_logging.py
--rw-r--r--   0        0        0      192 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/config.py
--rw-r--r--   0        0        0     1863 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/download.py
--rw-r--r--   0        0        0      756 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/register_font.py
--rw-r--r--   0        0        0      300 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/search.py
--rw-r--r--   0        0        0      923 2024-01-01 17:17:40.178874 manim_fonts-0.3.0/src/manim_fonts/utils.py
--rw-r--r--   0        0        0     2074 1970-01-01 00:00:00.000000 manim_fonts-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1518 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1307 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/README.md
+-rw-r--r--   0        0        0      807 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/src/manim_fonts/__init__.py
+-rw-r--r--   0        0        0       58 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/src/manim_fonts/_logging.py
+-rw-r--r--   0        0        0      197 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/src/manim_fonts/config.py
+-rw-r--r--   0        0        0     3395 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/src/manim_fonts/download.py
+-rw-r--r--   0        0        0      756 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/src/manim_fonts/register_font.py
+-rw-r--r--   0        0        0      929 2024-05-11 10:22:03.599486 manim_fonts-0.4.0/src/manim_fonts/utils.py
+-rw-r--r--   0        0        0     2079 1970-01-01 00:00:00.000000 manim_fonts-0.4.0/PKG-INFO
```

### Comparing `manim_fonts-0.3.0/LICENSE` & `manim_fonts-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manim_fonts-0.3.0/README.md` & `manim_fonts-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `manim_fonts-0.3.0/pyproject.toml` & `manim_fonts-0.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "manim-fonts"
-version = "0.3.0"
+version = "0.4.0"
 description = "Use Fonts from Internet With Manim."
 authors = ["Naveen M K <naveen@manim.community>"]
 license = "BSD-3-Clause"
 readme="README.md"
 repository="https://github.com/naveen521kk/manim-fonts"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 manim = ">=0.3.0"
 requests = ">=2.0.0"
-appdirs= ">=1"
+platformdirs = ">=4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2"
-black = "^22.10"
+pytest = "^8"
 
 [tool.poetry.plugins."manim.plugins"]
 "manim_fonts" = "manim_fonts"
 
 [tool.isort]
 # from https://black.readthedocs.io/en/stable/compatible_configs.html
 multi_line_output = 3
```

### Comparing `manim_fonts-0.3.0/src/manim_fonts/download.py` & `manim_fonts-0.4.0/src/manim_fonts/download.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import json
 import shutil
 import tempfile
 import time
-import zipfile
 from pathlib import Path
 
 import requests
 
 from ._logging import logger
 from .config import FONTS_DIR
 from .utils import (
-    gen_fonts_google_url,
+    gen_download_list_url,
     get_downloaded_fonts,
     str2hash,
     update_downloaded_fonts,
 )
 
 
 def download(url: str, local_filename: Path):
@@ -36,24 +36,69 @@
             logger.debug(e)
 
     else:
         raise requests.HTTPError("%s can't be downloaded" % url)
     return True
 
 
+def download_font_files(font_family: str, tmpdir: Path) -> None:
+    font_url = gen_download_list_url(font_family)
+    res = requests.get(font_url)
+    res.raise_for_status()
+
+    # find first { and string contents before it
+    contents = res.text
+    start = contents.find("{")
+    contents = contents[start:]
+
+    fonts = json.loads(contents)
+    file_refs = fonts.get("manifest", {}).get("fileRefs", None)
+
+    if not file_refs:
+        raise ValueError("No valid font files fount for font family %s" % font_family)
+
+    logger.info(
+        "Downloading font files for %s (number of font_file=%d)",
+        font_family,
+        len(file_refs),
+    )
+    for file in file_refs:
+        url = file.get("url")
+        filename = file.get("filename")
+        download_dest = tmpdir / filename
+
+        # if folder is not created, create it
+        download_dest.parent.mkdir(parents=True, exist_ok=True)
+        download_and_retry(url, tmpdir / filename)
+
+
 def download_fonts(font_family: str) -> Path:
-    font_url = gen_fonts_google_url(font_family)
     font_hash = str2hash(font_family)
     font_location = FONTS_DIR / font_hash
     font_location.mkdir(parents=True, exist_ok=True)
     if font_hash not in get_downloaded_fonts():
-        logger.info("Downloading %s from %s", font_family, font_url)
+        logger.info(
+            "Downloading %s font from google fonts to %s", font_family, font_location
+        )
         with tempfile.TemporaryDirectory(prefix="manim-fonts") as tmpdir:
-            tfile = Path(tmpdir) / "temp.zip"
-            download_and_retry(font_url, tfile)
-            with zipfile.ZipFile(tfile, "r") as zip:
-                zip.extractall(tmpdir)
+            try:
+                download_font_files(font_family, Path(tmpdir))
+            except requests.HTTPError as e:
+                error_message = (
+                    "Error while downloading font files for font family %s"
+                    % font_family
+                )
+                error_message += "\n" + repr(e)
+                error_message += (
+                    "\n" + "Please check if the font family is correct and try again."
+                )
+                error_message += (
+                    "\n" + "If the issue persists, please report it at"
+                    " https://github.com/naveen521kk/manim-fonts/issues"
+                )
+                logger.error(error_message)
+                raise Exception(error_message)
             for file in Path(tmpdir).glob("*.ttf"):
                 logger.info("Moving %s to %s", file, font_location)
                 shutil.copy(file, font_location)
         update_downloaded_fonts(font_hash, font_location)
     return font_location
```

### Comparing `manim_fonts-0.3.0/src/manim_fonts/register_font.py` & `manim_fonts-0.4.0/src/manim_fonts/register_font.py`

 * *Files identical despite different names*

### Comparing `manim_fonts-0.3.0/src/manim_fonts/utils.py` & `manim_fonts-0.4.0/src/manim_fonts/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 
 def str2hash(string: str) -> str:
     hash = hashlib.md5(string.encode())
     return hash.hexdigest()
 
 
-def gen_fonts_google_url(font_family: str) -> str:
-    return f"https://fonts.google.com/download?family={font_family}"
+def gen_download_list_url(font_family: str) -> str:
+    return f"https://fonts.google.com/download/list?family={font_family}"
 
 
 def get_downloaded_fonts() -> Dict[str, str]:
     font_file = FONTS_DIR / "fonts.json"
     if font_file.exists():
         with open(font_file) as f:
             return json.load(f)
```

### Comparing `manim_fonts-0.3.0/PKG-INFO` & `manim_fonts-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: manim-fonts
-Version: 0.3.0
+Version: 0.4.0
 Summary: Use Fonts from Internet With Manim.
 Home-page: https://github.com/naveen521kk/manim-fonts
 License: BSD-3-Clause
 Author: Naveen M K
 Author-email: naveen@manim.community
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: appdirs (>=1)
 Requires-Dist: manim (>=0.3.0)
+Requires-Dist: platformdirs (>=4)
 Requires-Dist: requests (>=2.0.0)
 Project-URL: Repository, https://github.com/naveen521kk/manim-fonts
 Description-Content-Type: text/markdown
 
 # Manim Fonts
 
 Get fonts on the fly from the internet which can be used with Manim.
```

