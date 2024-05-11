# Comparing `tmp/shroudstone-0.1.0a7.tar.gz` & `tmp/shroudstone-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroudstone-0.1.0a7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "shroudstone-0.1.0a8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `shroudstone-0.1.0a7.tar` & `shroudstone-0.1.0a8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       20 2024-02-24 10:29:15.326251 shroudstone-0.1.0a7/.gitignore
--rw-r--r--   0        0        0    32422 2024-02-24 10:29:15.326251 shroudstone-0.1.0a7/LICENSE
--rw-r--r--   0        0        0     2244 2024-02-24 12:28:47.704425 shroudstone-0.1.0a7/README.md
--rwxr-xr-x   0        0        0      297 2024-02-24 10:29:15.326251 shroudstone-0.1.0a7/codegen.sh
--rw-r--r--   0        0        0      723 2024-02-24 12:31:21.140159 shroudstone-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0       83 2024-02-24 12:31:31.702936 shroudstone-0.1.0a7/shroudstone/__init__.py
--rw-r--r--   0        0        0       28 2024-02-24 12:24:29.102030 shroudstone-0.1.0a7/shroudstone/__main__.py
--rw-r--r--   0        0        0     5886 2024-02-24 12:27:04.920294 shroudstone-0.1.0a7/shroudstone/cli.py
--rw-r--r--   0        0        0     1210 2024-02-24 12:12:08.196227 shroudstone-0.1.0a7/shroudstone/config.py
--rwxr-xr-x   0        0        0     9570 2024-02-24 12:25:57.857598 shroudstone-0.1.0a7/shroudstone/renamer.py
--rwxr-xr-x   0        0        0     2088 2024-02-24 10:29:15.330252 shroudstone-0.1.0a7/shroudstone/replay.py
--rw-r--r--   0        0        0     2121 2024-02-24 11:56:41.438150 shroudstone-0.1.0a7/shroudstone/stormgate_pb2.py
--rw-r--r--   0        0        0     1847 2024-02-24 11:56:41.442150 shroudstone-0.1.0a7/shroudstone/stormgate_pb2.pyi
--rwxr-xr-x   0        0        0      755 2024-02-24 10:29:15.334251 shroudstone-0.1.0a7/stormgate.proto
--rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 shroudstone-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0       20 2024-02-24 10:29:15.326251 shroudstone-0.1.0a8/.gitignore
+-rw-r--r--   0        0        0    32422 2024-02-24 10:29:15.326251 shroudstone-0.1.0a8/LICENSE
+-rw-r--r--   0        0        0     2365 2024-02-24 12:34:23.934514 shroudstone-0.1.0a8/README.md
+-rwxr-xr-x   0        0        0      297 2024-02-24 10:29:15.326251 shroudstone-0.1.0a8/codegen.sh
+-rw-r--r--   0        0        0      723 2024-02-24 12:31:21.140159 shroudstone-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-02-24 13:15:37.006156 shroudstone-0.1.0a8/shroudstone/__init__.py
+-rw-r--r--   0        0        0       28 2024-02-24 12:24:29.102030 shroudstone-0.1.0a8/shroudstone/__main__.py
+-rw-r--r--   0        0        0     6088 2024-02-24 13:14:37.800475 shroudstone-0.1.0a8/shroudstone/cli.py
+-rw-r--r--   0        0        0     1210 2024-02-24 12:12:08.196227 shroudstone-0.1.0a8/shroudstone/config.py
+-rwxr-xr-x   0        0        0     9570 2024-02-24 12:25:57.857598 shroudstone-0.1.0a8/shroudstone/renamer.py
+-rwxr-xr-x   0        0        0     2088 2024-02-24 10:29:15.330252 shroudstone-0.1.0a8/shroudstone/replay.py
+-rw-r--r--   0        0        0     2121 2024-02-24 11:56:41.438150 shroudstone-0.1.0a8/shroudstone/stormgate_pb2.py
+-rw-r--r--   0        0        0     1847 2024-02-24 11:56:41.442150 shroudstone-0.1.0a8/shroudstone/stormgate_pb2.pyi
+-rwxr-xr-x   0        0        0      755 2024-02-24 10:29:15.334251 shroudstone-0.1.0a8/stormgate.proto
+-rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 shroudstone-0.1.0a8/PKG-INFO
```

### Comparing `shroudstone-0.1.0a7/LICENSE` & `shroudstone-0.1.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/README.md` & `shroudstone-0.1.0a8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 Made possible by the great work of the [Stormgate
 World](https://www.stormgateworld.com/) team!
 
 ## Installation & Usage
 
 ### On Windows
 
-1. Install Python 3.11 from the Microsoft Store.
+1. Install Python 3.11 using
+   [the Microsoft Store](https://apps.microsoft.com/detail/9nrwmjp3717k) or the
+   [official installers](https://www.python.org/downloads/).
 2. Open Command Prompt and type `pip install shroudstone` to install shroudstone.
 3. You can now invoke `python -m shroudstone rename-replays` from the command
    line to rename your replays. To avoid having to do this every time, `python
    -m shroudstone create-rename-replays-shortcut` will create an icon on your
    desktop so it's just a double-click away :)
 
 You should also be able to get it working using a non-UWP python install, or
```

### Comparing `shroudstone-0.1.0a7/pyproject.toml` & `shroudstone-0.1.0a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/shroudstone/cli.py` & `shroudstone-0.1.0a8/shroudstone/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,19 +43,23 @@
         f"Wrote {i+1} replay messages in protoscope wire format to {output_directory}/."
     )
 
 
 @app.command()
 def edit_config():
     """Open the shroudstone configuration file in your default text editor."""
+    if not config_file.exists():
+        Config().save()
     if platform.system() == "Windows":
-        subprocess.run(["start", config_file])
+        # .resolve() is crucial when python is installed from the microsoft store
+        realpath = config_file.resolve()
+        subprocess.run(["cmd", "/c", f"start {realpath}"])
     else:
         editor = os.environ.get("VISUAL", os.environ.get("EDITOR", "nano"))
-        subprocess.run([editor, config_file])
+        subprocess.run([editor, config_file.resolve()])
 
 
 @app.command()
 def create_rename_replays_shortcut():
     """Create a desktop icon to launch the rename-replays script."""
     if platform.system() != "Windows":
         logger.error("This subcommand is only currently available on Windows.")
```

### Comparing `shroudstone-0.1.0a7/shroudstone/config.py` & `shroudstone-0.1.0a8/shroudstone/config.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/shroudstone/renamer.py` & `shroudstone-0.1.0a8/shroudstone/renamer.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/shroudstone/replay.py` & `shroudstone-0.1.0a8/shroudstone/replay.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/shroudstone/stormgate_pb2.py` & `shroudstone-0.1.0a8/shroudstone/stormgate_pb2.py`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/shroudstone/stormgate_pb2.pyi` & `shroudstone-0.1.0a8/shroudstone/stormgate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/stormgate.proto` & `shroudstone-0.1.0a8/stormgate.proto`

 * *Files identical despite different names*

### Comparing `shroudstone-0.1.0a7/PKG-INFO` & `shroudstone-0.1.0a8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroudstone
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: Python utilities for working with Stormgate replays
 Keywords: Stormgate
 Author-email: Anthony Carapetis <anthony.carapetis@gmail.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Games/Entertainment :: Real Time Strategy
@@ -36,15 +36,17 @@
 Made possible by the great work of the [Stormgate
 World](https://www.stormgateworld.com/) team!
 
 ## Installation & Usage
 
 ### On Windows
 
-1. Install Python 3.11 from the Microsoft Store.
+1. Install Python 3.11 using
+   [the Microsoft Store](https://apps.microsoft.com/detail/9nrwmjp3717k) or the
+   [official installers](https://www.python.org/downloads/).
 2. Open Command Prompt and type `pip install shroudstone` to install shroudstone.
 3. You can now invoke `python -m shroudstone rename-replays` from the command
    line to rename your replays. To avoid having to do this every time, `python
    -m shroudstone create-rename-replays-shortcut` will create an icon on your
    desktop so it's just a double-click away :)
 
 You should also be able to get it working using a non-UWP python install, or
```

