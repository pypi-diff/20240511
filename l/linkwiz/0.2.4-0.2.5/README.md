# Comparing `tmp/linkwiz-0.2.4.tar.gz` & `tmp/linkwiz-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkwiz-0.2.4.tar", max compression
+gzip compressed data, was "linkwiz-0.2.5.tar", last modified: Sat May 11 04:09:05 2024, max compression
```

## Comparing `linkwiz-0.2.4.tar` & `linkwiz-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    18092 2024-04-10 02:50:31.877024 linkwiz-0.2.4/LICENSE
--rw-r--r--   0        0        0      997 2024-04-10 02:50:31.877024 linkwiz-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-04-10 02:50:31.877024 linkwiz-0.2.4/linkwiz/__init__.py
--rw-r--r--   0        0        0      585 2024-04-10 02:50:31.880357 linkwiz-0.2.4/linkwiz/__main__.py
--rw-r--r--   0        0        0     1812 2024-04-10 02:54:43.833742 linkwiz-0.2.4/linkwiz/browser.py
--rw-r--r--   0        0        0     2774 2024-04-10 02:50:31.880357 linkwiz-0.2.4/linkwiz/config.py
--rw-r--r--   0        0        0     1300 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/core.py
--rw-r--r--   0        0        0     4007 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/gui.py
--rw-r--r--   0        0        0     1259 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/install.py
--rw-r--r--   0        0        0     1360 2024-04-10 02:50:31.883690 linkwiz-0.2.4/linkwiz/launch.py
--rw-r--r--   0        0        0      853 2024-04-10 02:52:35.310383 linkwiz-0.2.4/linkwiz/match.py
--rw-r--r--   0        0        0      676 2024-04-12 09:07:34.567234 linkwiz-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 linkwiz-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    18092 2024-04-23 16:54:37.021744 linkwiz-0.2.5/LICENSE
+-rw-r--r--   0        0        0      997 2024-04-23 16:54:37.021744 linkwiz-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 16:54:37.021744 linkwiz-0.2.5/linkwiz/__init__.py
+-rw-r--r--   0        0        0      585 2024-04-23 16:54:37.021744 linkwiz-0.2.5/linkwiz/__main__.py
+-rw-r--r--   0        0        0     2236 2024-05-11 04:04:33.517315 linkwiz-0.2.5/linkwiz/browser.py
+-rw-r--r--   0        0        0     2774 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/config.py
+-rw-r--r--   0        0        0     1300 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/core.py
+-rw-r--r--   0        0        0     4007 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/gui.py
+-rw-r--r--   0        0        0     1494 2024-04-28 13:37:40.316740 linkwiz-0.2.5/linkwiz/install.py
+-rw-r--r--   0        0        0     1360 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/launch.py
+-rw-r--r--   0        0        0      853 2024-04-23 16:54:37.025077 linkwiz-0.2.5/linkwiz/match.py
+-rw-r--r--   0        0        0      788 2024-05-11 04:09:05.738196 linkwiz-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 linkwiz-0.2.5/PKG-INFO
```

### Comparing `linkwiz-0.2.4/LICENSE` & `linkwiz-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/README.md` & `linkwiz-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/linkwiz/__main__.py` & `linkwiz-0.2.5/linkwiz/__main__.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/linkwiz/browser.py` & `linkwiz-0.2.5/linkwiz/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 import logging
 from pathlib import Path
 import subprocess
 from typing import Dict, List
 from xdg import DesktopEntry
 from linkwiz.config import config
 
-APPNAME: str = "LinkWiz"
+SELF_DESKTOP: str = "linkwiz.desktop"
 HTTP_HANDLER: str = "x-scheme-handler/http"
 
 DESKTOP_PATHS = [
     Path("/usr/share/applications/"),
     Path.home() / ".local/share/applications/",
 ]
 
+MIMEINFO_PATHS = [
+    Path("/usr/share/applications/mimeinfo.cache"),
+    Path.home() / ".local/share/applications/mimeinfo.cache",
+]
+
 
 def get_browsers() -> Dict[str, Path]:
     """Get the name and exec path of browsers."""
     try:
         installed_browsers = []
         if config.main.get("auto_find_browsers", True):
-            output = subprocess.check_output(["gio", "mime", HTTP_HANDLER], text=True)
-            installed_browsers = (
-                output.split("Recommended applications:")[-1].strip().split("\n")
-            )
-            installed_browsers = [app.strip() for app in installed_browsers]
-
-            own_desktop = f"{APPNAME.lower()}.desktop"
+            installed_browsers = find_installed_browsers()
 
-            if own_desktop in installed_browsers:
-                installed_browsers.remove(own_desktop)
+            if SELF_DESKTOP in installed_browsers:
+                installed_browsers.remove(SELF_DESKTOP)
 
         return get_browser_exec(installed_browsers)
     except subprocess.CalledProcessError:
         logging.error("Error getting installed browsers")
         exit(1)
 
 
+def find_installed_browsers() -> List[str]:
+    """Get the name of installed browsers."""
+    installed_browsers = set()
+    for path in MIMEINFO_PATHS:
+        if not path.exists():
+            continue
+        with open(path, "r") as f:
+            lines = f.readlines()
+            for line in lines:
+                if not line.startswith(HTTP_HANDLER):
+                    continue
+                browsers = line.split("=")[-1].strip().split(";")
+                installed_browsers.update(browsers)
+                break
+    return list(installed_browsers)
+
+
 def get_browser_exec(browsers_desktop: List[str]) -> Dict[str, Path]:
     """Get the exec path of installed browsers."""
     installed_browsers: Dict[str, Path] = {}
     for path in DESKTOP_PATHS:
         if not path.exists():
             continue
         for entry in path.glob("*.desktop"):
```

### Comparing `linkwiz-0.2.4/linkwiz/config.py` & `linkwiz-0.2.5/linkwiz/config.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/linkwiz/core.py` & `linkwiz-0.2.5/linkwiz/core.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/linkwiz/gui.py` & `linkwiz-0.2.5/linkwiz/gui.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/linkwiz/install.py` & `linkwiz-0.2.5/linkwiz/install.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,21 +20,27 @@
     desktop.set("Name", "Linkwiz")
     desktop.set("Type", "Application")
     desktop.set("MimeType", "x-scheme-handler/http;x-scheme-handler/https;")
     desktop.set("Categories", "Network;")
     desktop.set("NoDisplay", "true")
     desktop.set("Exec", script_path + " %u")
     desktop.write()
+    update_desktop_database()
 
 
 def set_default_app_for_mime_type(mime_type: str):
     cmd = ["xdg-mime", "default", DESKTOP_FILENAME, mime_type]
     mime_type_quoted = shlex.quote(mime_type)
-    subprocess.run(cmd + [mime_type_quoted], check=True)
+    subprocess.run(cmd + [mime_type_quoted], check=True).check_returncode()
 
 
 def uninstall():
     if DESKTOP_PATH.exists():
         DESKTOP_PATH.unlink()
+        update_desktop_database()
         print("Uninstalled")
     else:
         print("linkwiz is not installed.")
+
+
+def update_desktop_database():
+    subprocess.run(["update-desktop-database", Path(BaseDirectory.xdg_data_home) / "applications"]).check_returncode()
```

### Comparing `linkwiz-0.2.4/linkwiz/launch.py` & `linkwiz-0.2.5/linkwiz/launch.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/linkwiz/match.py` & `linkwiz-0.2.5/linkwiz/match.py`

 * *Files identical despite different names*

### Comparing `linkwiz-0.2.4/PKG-INFO` & `linkwiz-0.2.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: linkwiz
-Version: 0.2.4
+Version: 0.2.5
 Summary: LinkWiz is a Linux tool that lets users select their preferred browser for opening links.
-Home-page: https://github.com/icealtria/linkwiz
+Author-Email: Rin <icealtria+github@gmail.com>
 License: GPL-2.0-only
-Author: Rin
-Author-email: icealtria+github@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pyxdg (>=0.28,<0.29)
-Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
-Requires-Dist: unalix-rev (>=0.9.1,<0.10.0)
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Project-URL: Repository, https://github.com/icealtria/linkwiz
+Requires-Python: <4.0,>=3.11
+Requires-Dist: pyxdg<1.0,>=0.28
+Requires-Dist: tomli-w<2.0.0,>=1.0.0
+Requires-Dist: unalix-rev<1.0.0,>=0.9.1
 Description-Content-Type: text/markdown
 
 # LinkWiz
 
 LinkWiz is a Linux tool that lets users select their preferred browser for opening links.
 
 ![Screenshot](https://raw.githubusercontent.com/icealtria/linkwiz/assets/Screenshot.webp)
@@ -53,8 +48,7 @@
 [rules.hostname]
 "example.com" = "Brave Private"
 "github.com" = "Firefox Developer Edition"
 "google.com" = "Google Chrome"
 ```
 ## TODO
 - [ ] RIIR
-
```

