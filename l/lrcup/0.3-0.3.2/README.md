# Comparing `tmp/lrcup-0.3.tar.gz` & `tmp/lrcup-0.3.2.tar.gz`

## Comparing `lrcup-0.3.tar` & `lrcup-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 lrcup-0.3/lrcup/__init__.py
--rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 lrcup-0.3/lrcup/__main__.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 lrcup-0.3/lrcup/controller.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 lrcup-0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lrcup-0.3/LICENSE.txt
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 lrcup-0.3/README.md
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lrcup-0.3/pyproject.toml
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 lrcup-0.3/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 lrcup-0.3.2/lrcup/__init__.py
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 lrcup-0.3.2/lrcup/__main__.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 lrcup-0.3.2/lrcup/challenge.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 lrcup-0.3.2/lrcup/controller.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 lrcup-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 lrcup-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 lrcup-0.3.2/README.md
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 lrcup-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 lrcup-0.3.2/PKG-INFO
```

### Comparing `lrcup-0.3/lrcup/__main__.py` & `lrcup-0.3.2/lrcup/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 @lrcup.command(help = "Upload lyrics to LRCLIB from local file")
 @click.argument("filename")
 def upload(filename: str) -> None:
     def process_lyrics(lyrics: str) -> (str, str):
         if all([line.startswith("[") for line in lyrics.split("\n") if line.strip()]):
             print(t("LRC Status"), "\033[32msynced\033[0m", sep = "")
-            return None, lyrics
+            return "\n".join([line.split("]")[1].lstrip() for line in lyrics.split("\n") if line.strip()]), lyrics
 
         print(t("LRC Status"), "\033[31munsynced\033[0m", sep = "")
         return lyrics, None
 
     filename = Path(filename).resolve()
     if not filename.is_file():
         return click.secho("Specified filename does not exist.", fg = "red")
```

### Comparing `lrcup-0.3/lrcup/controller.py` & `lrcup-0.3.2/lrcup/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) 2024 iiPython
 
 # Modules
-import hashlib
 from typing import Any, List, Dict
 
 import requests
 
 from . import __version__
+from .challenge import solve
 
 # API Controller
 class LRCLib():
     def __init__(self, api_url: str = "https://lrclib.net/api/") -> None:
         self.api_url = api_url
         if not self.api_url.endswith("/"):
             self.api_url += "/"
@@ -112,23 +112,9 @@
                     return False
 
                 elif result[i] < target[i]:
                     break
 
             return True
 
-        def solve_challenge(prefix: str, target: str) -> int:
-            nonce, target = 0, bytes.fromhex(target)
-            while True:
-                if verify_nonce(
-                    hashlib.sha256(f"{prefix}{nonce}".encode()).digest(),
-                    target
-                ):
-                    break
-
-                else:
-                    nonce += 1
-
-            return nonce
-
-        nonce = solve_challenge(data["prefix"], data["target"])
+        nonce = solve(data["prefix"], data["target"])
         return f"{data['prefix']}:{nonce}"
```

### Comparing `lrcup-0.3/LICENSE.txt` & `lrcup-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lrcup-0.3/README.md` & `lrcup-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lrcup-0.3/pyproject.toml` & `lrcup-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lrcup-0.3/PKG-INFO` & `lrcup-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lrcup
-Version: 0.3
+Version: 0.3.2
 Summary: Python module and CLI for the LRCLIB API
 Project-URL: Homepage, https://github.com/iiPythonx/lrcup
 Project-URL: Issues, https://github.com/iiPythonx/lrcup/issues
 Author-email: iiPython <ben@iipython.dev>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

