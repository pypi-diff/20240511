# Comparing `tmp/cheatshh-1.0.2.tar.gz` & `tmp/cheatshh-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cheatshh-1.0.2.tar", last modified: Thu May  9 10:24:34 2024, max compression
+gzip compressed data, was "cheatshh-1.0.3.tar", last modified: Sat May 11 12:19:37 2024, max compression
```

## Comparing `cheatshh-1.0.2.tar` & `cheatshh-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 10:24:34.912898 cheatshh-1.0.2/
--rw-r--r--   0 anirudhgupta   (501) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.2/LICENSE
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     1245 2024-05-09 10:24:34.912607 cheatshh-1.0.2/PKG-INFO
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     2548 2024-05-09 07:55:28.000000 cheatshh-1.0.2/README.md
-drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 10:24:34.911891 cheatshh-1.0.2/cheatshh.egg-info/
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     1245 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/PKG-INFO
--rw-r--r--   0 anirudhgupta   (501) staff       (20)      256 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/SOURCES.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)        1 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/dependency_links.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)       51 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/entry_points.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)       21 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/requires.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)        4 2024-05-09 10:24:34.000000 cheatshh-1.0.2/cheatshh.egg-info/top_level.txt
--rw-r--r--   0 anirudhgupta   (501) staff       (20)       38 2024-05-09 10:24:34.912948 cheatshh-1.0.2/setup.cfg
--rw-r--r--   0 anirudhgupta   (501) staff       (20)     2772 2024-05-09 10:24:06.000000 cheatshh-1.0.2/setup.py
-drwxr-xr-x   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 10:24:34.912133 cheatshh-1.0.2/src/
--rw-r--r--   0 anirudhgupta   (501) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.2/src/__init__.py
--rw-r--r--   0 anirudhgupta   (501) staff       (20)      222 2024-05-09 10:05:58.000000 cheatshh-1.0.2/src/run_cheatshh.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-11 12:19:37.889249 cheatshh-1.0.3/
+-rw-r--r--   0 root         (0) staff       (20)    11357 2024-05-09 07:38:12.000000 cheatshh-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     1340 2024-05-11 12:19:37.889013 cheatshh-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     4724 2024-05-11 12:12:30.000000 cheatshh-1.0.3/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-11 12:19:37.888333 cheatshh-1.0.3/cheatshh.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     1340 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      256 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       51 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)       21 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        4 2024-05-11 12:19:37.000000 cheatshh-1.0.3/cheatshh.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-05-11 12:19:37.889294 cheatshh-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     3115 2024-05-11 12:18:45.000000 cheatshh-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-05-11 12:19:37.888558 cheatshh-1.0.3/src/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-05-09 09:59:20.000000 cheatshh-1.0.3/src/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-05-10 19:10:43.000000 cheatshh-1.0.3/src/run_cheatshh.py
```

### Comparing `cheatshh-1.0.2/LICENSE` & `cheatshh-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cheatshh-1.0.2/PKG-INFO` & `cheatshh-1.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.2
+Version: 1.0.3
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -21,14 +21,17 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.2
+1.0.3
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
+## Bugs fixed in 1.0.3
+- Path configuration for Linux has been fixed.
+- docs has been updated.
```

### Comparing `cheatshh-1.0.2/cheatshh.egg-info/PKG-INFO` & `cheatshh-1.0.3/cheatshh.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cheatshh
-Version: 1.0.2
+Version: 1.0.3
 Author: Anirudh Gupta
 Keywords: cheatsheet, cheat, command-line, cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fuzzyfinder
 Requires-Dist: whiptail
 
@@ -21,14 +21,17 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.2
+1.0.3
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
+## Bugs fixed in 1.0.3
+- Path configuration for Linux has been fixed.
+- docs has been updated.
```

### Comparing `cheatshh-1.0.2/setup.py` & `cheatshh-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 import os
-import shutil, subprocess
-from setuptools import setup, find_packages
+import shutil
+import subprocess, gzip
+from setuptools import find_packages, setup
 from setuptools.command.install import install
 
+
 class CustomInstallCommand(install):
     def run(self):
         install.run(self)  # Run standard install logic
         post_install()
 
+
 def install_man_page():
-    source_path = os.path.join('docs', 'man', 'cheatshh.1')
-    dest_path = os.path.join('/usr/local/','share', 'man', 'man1', 'cheatshh.1')
-    os.makedirs(os.path.dirname(dest_path), exist_ok=True)
-    try:
-        shutil.copy(source_path, dest_path)
-    except PermissionError:
-        print("Permission denied. Please run this script as root for man pages.")
+    source_path = os.path.join("docs", "man", "cheatshh.1")
+    dest_path = os.path.join("/usr/local/", "share", "man", "man1", "cheatshh.1.gz")
+
+    # Compress the man page
+    with open(source_path, 'rb') as src, gzip.open(dest_path, 'wb') as dst:
+        shutil.copyfileobj(src, dst)
 
 
 def post_install():
     install_man_page()
+    
+    # Get the directory containing setup.py
+    setup_dir = os.path.dirname(os.path.abspath(__file__))
+    
     # Define the path to ~/.config/cheatshh
     config_dir = os.path.expanduser("~/.config/cheatshh")
-
     # Create ~/.config/cheatshh directory if it doesn't exist
     os.makedirs(config_dir, exist_ok=True)
-
+    
+    # Define files to copy with their respective paths
+    files_to_copy = [
+        ("cheats.sh", "cheats.sh"),
+        ("commands.json", "commands.json"),
+        ("groups.json", "groups.json"),
+        ("README.md", "README.md"),
+        ("requirements.txt", "requirements.txt")
+    ]
     # Copy files to ~/.config/cheatshh
-    files_to_copy = ["cheats.sh", "commands.json", "groups.json", "README.md", "requirements.txt"]
-    for file_name in files_to_copy:
-        with open(file_name, "rb") as src:
-            with open(os.path.join(config_dir, file_name), "wb") as dest:
-                dest.write(src.read())
+    for file_name, src_file in files_to_copy:
+        src_path = os.path.join(setup_dir, src_file)
+        dest_path = os.path.join(config_dir, file_name)
+        shutil.copy(src_path, dest_path)
+
 
 def run_cheatshh():
-    subprocess.run(['bash', '~/.config/cheatshh/cheats.sh'])
+    subprocess.run(["bash", "~/.config/cheatshh/cheats.sh"])
 
 
-setup(name="cheatshh", version="1.0.2", cmdclass={"install": CustomInstallCommand}, 
-    long_description="""
+setup(name="cheatshh", version="1.0.3", cmdclass={"install": CustomInstallCommand},
+      long_description="""
 # cheatshh
 
 Cheatshh is an interactive CLI meant for managing command line cheatshheets. Now you don't have to remember CLI commands and just refer your cheatshhet. You can group commands and view their TLDR and MAN pages along with a custom description for the command.
 
 # Features
 
 - Comprehensive cheatsheets for various command-line utilities and tools.
@@ -51,27 +64,29 @@
 - TLDR and MAN pages visible in the preview.
 - Easy to add, edit, delete commands and groups and playing around.
 - Press Enter on a command to copy it to clipboard and exit.
 
 Visit the Github Repository for more details: https://github.com/AnirudhG07/cheatshh
 
 # Version
-1.0.2
+1.0.3
 
 ## Note:
 - This package is best used in Unix based systems, like linux and MacOS. For Windows, see the github repository for more details.
 - The package is installed in ~/.config/cheatshh directory.
 
+## Bugs fixed in 1.0.3
+- Path configuration for Linux has been fixed.
+- docs has been updated.
 
 """,
     long_description_content_type="text/markdown",
     keywords=["cheatsheet, cheat, command-line, cli"],
     install_requires=["fuzzyfinder", "whiptail"],
     author="Anirudh Gupta",
     packages=find_packages(),
     entry_points={
-        'console_scripts': [
-            'cheatshh=src.run_cheatshh:main',
+        "console_scripts": [
+            "cheatshh=src.run_cheatshh:main",
         ],
     },
 )
-
```

