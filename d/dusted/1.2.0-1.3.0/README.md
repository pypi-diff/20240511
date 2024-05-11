# Comparing `tmp/dusted-1.2.0.tar.gz` & `tmp/dusted-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dusted-1.2.0.tar", last modified: Sat Oct 30 11:06:34 2021, max compression
+gzip compressed data, was "dusted-1.3.0.tar", last modified: Fri May 10 23:40:31 2024, max compression
```

## Comparing `dusted-1.2.0.tar` & `dusted-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-10-30 11:06:34.994817 dusted-1.2.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     1068 2021-03-20 16:31:13.000000 dusted-1.2.0/LICENSE.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      936 2021-10-30 11:06:34.994817 dusted-1.2.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      542 2021-03-23 13:12:46.000000 dusted-1.2.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-10-30 11:06:34.991484 dusted-1.2.0/dusted/
--rw-r--r--   0 alex      (1000) alex      (1000)      494 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/__main__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      236 2021-03-20 16:30:35.000000 dusted-1.2.0/dusted/broadcaster.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4146 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/commands.py
--rw-r--r--   0 alex      (1000) alex      (1000)      777 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/config.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2695 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/cursor.py
--rw-r--r--   0 alex      (1000) alex      (1000)      902 2021-03-20 16:30:35.000000 dusted-1.2.0/dusted/dialog.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-10-30 11:06:34.994817 dusted-1.2.0/dusted/dustforce/
--rw-r--r--   0 alex      (1000) alex      (1000)      370 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/dustforce/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)      431 2021-06-16 12:56:52.000000 dusted-1.2.0/dusted/dustforce/linux.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1199 2021-06-16 12:56:52.000000 dusted-1.2.0/dusted/dustforce/windows.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-10-30 11:06:34.994817 dusted-1.2.0/dusted/geom/
--rw-r--r--   0 alex      (1000) alex      (1000)       88 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/geom/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)       34 2021-03-20 16:30:35.000000 dusted-1.2.0/dusted/geom/lines.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2413 2021-06-15 14:13:04.000000 dusted-1.2.0/dusted/geom/tiles.py
--rw-r--r--   0 alex      (1000) alex      (1000)     8465 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/gui.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4586 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/inputs.py
--rw-r--r--   0 alex      (1000) alex      (1000)    15306 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/inputs_view.py
--rw-r--r--   0 alex      (1000) alex      (1000)      326 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/level.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4627 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/level_view.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1709 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/undo_stack.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1880 2021-10-30 10:47:32.000000 dusted-1.2.0/dusted/utils.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-10-30 11:06:34.994817 dusted-1.2.0/dusted.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)      936 2021-10-30 11:06:34.000000 dusted-1.2.0/dusted.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      680 2021-10-30 11:06:34.000000 dusted-1.2.0/dusted.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2021-10-30 11:06:34.000000 dusted-1.2.0/dusted.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       45 2021-10-30 11:06:34.000000 dusted-1.2.0/dusted.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       47 2021-10-30 11:06:34.000000 dusted-1.2.0/dusted.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        7 2021-10-30 11:06:34.000000 dusted-1.2.0/dusted.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2021-03-23 13:47:20.000000 dusted-1.2.0/dusted.egg-info/zip-safe
--rw-r--r--   0 alex      (1000) alex      (1000)       90 2021-03-20 16:31:13.000000 dusted-1.2.0/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)      662 2021-10-30 11:06:34.994817 dusted-1.2.0/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2021-10-30 11:06:34.994817 dusted-1.2.0/test/
--rw-r--r--   0 alex      (1000) alex      (1000)     3460 2021-06-16 15:03:57.000000 dusted-1.2.0/test/test_cursor.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4330 2021-06-16 14:59:58.000000 dusted-1.2.0/test/test_inputs.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-10 23:40:31.261537 dusted-1.3.0/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1068 2021-03-20 16:31:13.000000 dusted-1.3.0/LICENSE.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      991 2024-05-10 23:40:31.261537 dusted-1.3.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      542 2021-03-23 13:12:46.000000 dusted-1.3.0/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-10 23:40:31.164871 dusted-1.3.0/dusted/
+-rw-r--r--   0 alex      (1000) alex      (1000)      494 2021-10-30 10:47:32.000000 dusted-1.3.0/dusted/__main__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      236 2021-03-20 16:30:35.000000 dusted-1.3.0/dusted/broadcaster.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4146 2024-04-18 22:38:19.000000 dusted-1.3.0/dusted/commands.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1416 2024-05-09 20:10:45.000000 dusted-1.3.0/dusted/config.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2695 2021-10-30 10:47:32.000000 dusted-1.3.0/dusted/cursor.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      902 2021-03-20 16:30:35.000000 dusted-1.3.0/dusted/dialog.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-10 23:40:31.191537 dusted-1.3.0/dusted/dustforce/
+-rw-r--r--   0 alex      (1000) alex      (1000)      370 2021-10-30 10:47:32.000000 dusted-1.3.0/dusted/dustforce/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      431 2024-04-18 21:56:48.000000 dusted-1.3.0/dusted/dustforce/linux.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1231 2024-05-09 19:39:12.000000 dusted-1.3.0/dusted/dustforce/windows.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-10 23:40:31.218204 dusted-1.3.0/dusted/geom/
+-rw-r--r--   0 alex      (1000) alex      (1000)       88 2021-10-30 10:47:32.000000 dusted-1.3.0/dusted/geom/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       34 2021-03-20 16:30:35.000000 dusted-1.3.0/dusted/geom/lines.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2413 2021-06-15 14:13:04.000000 dusted-1.3.0/dusted/geom/tiles.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     8086 2024-05-09 21:21:40.000000 dusted-1.3.0/dusted/gui.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4650 2024-05-09 20:48:33.000000 dusted-1.3.0/dusted/inputs.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    15520 2024-04-18 22:40:31.000000 dusted-1.3.0/dusted/inputs_view.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      321 2024-05-09 21:12:35.000000 dusted-1.3.0/dusted/level.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4625 2024-04-18 21:55:51.000000 dusted-1.3.0/dusted/level_view.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1746 2024-05-09 21:17:52.000000 dusted-1.3.0/dusted/replay_metadata.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1709 2021-10-30 10:47:32.000000 dusted-1.3.0/dusted/undo_stack.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1912 2024-05-09 19:40:07.000000 dusted-1.3.0/dusted/utils.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-10 23:40:31.261537 dusted-1.3.0/dusted.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)      991 2024-05-10 23:40:30.000000 dusted-1.3.0/dusted.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      706 2024-05-10 23:40:30.000000 dusted-1.3.0/dusted.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2024-05-10 23:40:30.000000 dusted-1.3.0/dusted.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       44 2024-05-10 23:40:30.000000 dusted-1.3.0/dusted.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       47 2024-05-10 23:40:30.000000 dusted-1.3.0/dusted.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        7 2024-05-10 23:40:30.000000 dusted-1.3.0/dusted.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2021-03-23 13:47:20.000000 dusted-1.3.0/dusted.egg-info/zip-safe
+-rw-r--r--   0 alex      (1000) alex      (1000)       90 2021-03-20 16:31:13.000000 dusted-1.3.0/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)      647 2024-05-10 23:40:31.268204 dusted-1.3.0/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2024-05-10 23:40:31.238204 dusted-1.3.0/test/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3460 2024-04-18 21:53:22.000000 dusted-1.3.0/test/test_cursor.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4656 2024-04-18 21:53:48.000000 dusted-1.3.0/test/test_inputs.py
```

### Comparing `dusted-1.2.0/LICENSE.txt` & `dusted-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/PKG-INFO` & `dusted-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dusted
-Version: 1.2.0
+Version: 1.3.0
 Summary: Dustforce replay editor
 Home-page: https://github.com/AlexMorson/dusted
 Author: Alex Morson
 Author-email: alexmorson@btinternet.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: appdirs~=1.4.4
+Requires-Dist: dustmaker~=1.1.0
+Requires-Dist: requests~=2.22
 
 # Dusted
 
 An offline editor for Dustforce replays, largely based on dustkid.com's replay composer.
 
 ## Installation
 
@@ -35,9 +36,7 @@
 ```
 
 or, if the python scripts directory is on the PATH
 
 ```
 dusted
 ```
-
-
```

### Comparing `dusted-1.2.0/README.md` & `dusted-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/dusted/commands.py` & `dusted-1.3.0/dusted/commands.py`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/dusted/cursor.py` & `dusted-1.3.0/dusted/cursor.py`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/dusted/dialog.py` & `dusted-1.3.0/dusted/dialog.py`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/dusted/dustforce/windows.py` & `dusted-1.3.0/dusted/dustforce/windows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import queue
 import threading
 import time
 
-from dusted.config import config
+from dusted.config import config, ConfigOption
 
 watcher = None
 stdout = queue.Queue()
 
 
 class LogfileWatcher:
     def __init__(self, path):
@@ -35,13 +35,13 @@
                 self.file = None
                 time.sleep(1)
 
 
 def create_proc(uri):
     global watcher
     if watcher is None:
-        path = os.path.join(config.dustforce_path, "output.log")
+        path = os.path.join(config.get(ConfigOption.DUSTFORCE_PATH), "output.log")
         watcher = LogfileWatcher(path)
         logfile_thread = threading.Thread(target=watcher.start, daemon=True)
         logfile_thread.start()
 
     os.startfile(uri)
```

### Comparing `dusted-1.2.0/dusted/geom/tiles.py` & `dusted-1.3.0/dusted/geom/tiles.py`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/dusted/gui.py` & `dusted-1.3.0/dusted/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import tkinter as tk
 import tkinter.filedialog
 import tkinter.messagebox
 
 from dustmaker.replay import Replay, PlayerData, Character
 
 from dusted import dustforce, utils
-from dusted.config import config
+from dusted.config import config, ConfigOption
 from dusted.cursor import Cursor
-from dusted.dialog import Dialog, SimpleDialog
+from dusted.dialog import SimpleDialog
 from dusted.inputs import Inputs
 from dusted.inputs_view import InputsView
 from dusted.level import Level
 from dusted.level_view import LevelView
+from dusted.replay_metadata import ReplayMetadataDialog, ReplayMetadata
 from dusted.undo_stack import UndoStack
 
 LEVEL_PATTERN = r"START (.*)"
 COORD_PATTERN = r"(\d*) (-?\d*) (-?\d*)"
-CHARACTERS = ["dustman", "dustgirl", "dustkid", "dustworth"]
 
 log = logging.getLogger(__name__)
 
 
 class LoadReplayDialog(SimpleDialog):
     def __init__(self, app):
         super().__init__(app, "Replay id:", "Load")
@@ -32,82 +32,56 @@
 
     def ok(self, replay_id):
         replay = utils.load_replay_from_dustkid(replay_id)
         self.app.load_replay(replay)
         return True
 
 
-class NewReplayDialog(Dialog):
-    def __init__(self, app):
-        super().__init__(app)
-        self.app = app
-
-        character_label = tk.Label(self, text="Character:")
-        character_label.grid(row=0, column=0, sticky="e")
-        self.character_var = tk.StringVar(self)
-        character_choice = tk.OptionMenu(self, self.character_var, *CHARACTERS)
-        character_choice.grid(row=0, column=1, sticky="ew")
-
-        level_label = tk.Label(self, text="Level id:")
-        level_label.grid(row=1, column=0, sticky="e")
-        self.level_entry = tk.Entry(self)
-        self.level_entry.grid(row=1, column=1, sticky="ew")
-
-        button = tk.Button(self, text="Create", command=self.ok)
-        button.grid(row=2, columnspan=2)
-
-        self.character_var.set(CHARACTERS[app.character])
-
-    def ok(self):
-        level_id = self.level_entry.get()
-        character = Character(CHARACTERS.index(self.character_var.get()))
-        self.app.new_file(level_id, character)
-        self.destroy()
-
-
 class App(tk.Tk):
     def __init__(self):
         super().__init__()
 
         # Log exceptions
         self.report_callback_exception = lambda *args: log.error("", exc_info=args)
 
-        self.level = Level()
+        self.level = Level("downhill")
         self.character = Character.DUSTMAN
         self.inputs = Inputs()
         self.cursor = Cursor(self.inputs)
         self.undo_stack = UndoStack(self.inputs, self.cursor)
         self.undo_stack.subscribe(self.on_undo_stack_change)
 
         # Menu bar
         menu_bar = tk.Menu(self)
 
         file_menu = tk.Menu(menu_bar, tearoff=0)
         menu_bar.add_cascade(label="File", underline=0, menu=file_menu)
 
         new_file_menu = tk.Menu(file_menu, tearoff=0)
         file_menu.add_cascade(label="New", menu=new_file_menu)
-        new_file_menu.add_command(label="Empty replay", command=lambda: NewReplayDialog(self), accelerator="Ctrl+N")
-        new_file_menu.add_command(label="From replay id", command=lambda: LoadReplayDialog(self))
+        new_file_menu.add_command(label="Empty replay...", command=self.new_file, accelerator="Ctrl+N")
+        new_file_menu.add_command(label="From replay id...", command=lambda: LoadReplayDialog(self))
 
-        file_menu.add_command(label="Open", command=self.open_file, accelerator="Ctrl+O")
+        file_menu.add_command(label="Open...", command=self.open_file, accelerator="Ctrl+O")
         file_menu.add_command(label="Save", command=self.save_file, accelerator="Ctrl+S")
-        file_menu.add_command(label="Save As", command=lambda: self.save_file(True), accelerator="Ctrl+Shift+S")
+        file_menu.add_command(label="Save As...", command=lambda: self.save_file(True), accelerator="Ctrl+Shift+S")
 
         self.edit_menu = tk.Menu(menu_bar, tearoff=0)
         menu_bar.add_cascade(label="Edit", underline=0, menu=self.edit_menu)
 
         self.edit_menu.add_command(label="Undo", command=self.undo_stack.undo, state=tk.DISABLED, accelerator="Ctrl+Z")
         self.edit_menu.add_command(label="Redo", command=self.undo_stack.redo, state=tk.DISABLED,
                                    accelerator="Ctrl+Shift+Z")
+        self.edit_menu.add_separator()
+        self.edit_menu.add_command(label="Replay metadata...", command=self.edit_replay_metadata)
 
         settings_menu = tk.Menu(menu_bar, tearoff=0)
         menu_bar.add_cascade(label="Settings", underline=0, menu=settings_menu)
 
-        settings_menu.add_command(label="Set Dustforce directory", command=self.set_dustforce_directory)
+        settings_menu.add_command(label="Set Dustforce directory...", command=self.set_dustforce_directory)
 
         self.config(menu=menu_bar)
 
         # Widgets
         buttons = tk.Frame(self)
         button1 = tk.Button(buttons, text="Watch", command=self.watch)
         button2 = tk.Button(buttons, text="Load State and Watch", command=self.load_state_and_watch)
@@ -118,28 +92,28 @@
         button1.pack(side=tk.LEFT)
         button2.pack(side=tk.LEFT)
         buttons.pack(anchor=tk.W)
         canvas.pack(fill=tk.BOTH, expand=1)
         inputs.pack(fill=tk.X)
 
         # Hotkeys
-        self.bind("<Control-KeyPress-n>", lambda e: NewReplayDialog(self))
+        self.bind("<Control-KeyPress-n>", lambda e: self.new_file())
         self.bind("<Control-KeyPress-o>", lambda e: self.open_file())
         self.bind("<Control-KeyPress-s>", lambda e: self.save_file())
         self.bind("<Control-Shift-KeyPress-S>", lambda e: self.save_file(True))
         self.bind("<F5>", lambda e: self.watch())
         self.bind("<F6>", lambda e: self.load_state_and_watch())
 
         self.canvas = canvas
         self.file = None
         self.update_title()
         self.after_idle(self.handle_stdout)
 
         # Check if the Dustforce directory is valid
-        if not os.path.isdir(config.dustforce_path):
+        if not os.path.isdir(config.get(ConfigOption.DUSTFORCE_PATH)):
             tk.messagebox.showwarning(message="Could not find the Dustforce directory. Please update it in Settings.")
 
     def update_title(self):
         title = "Dusted"
         if self.file is not None:
             title += f" - {self.file}"
             if self.undo_stack.is_modified:
@@ -183,20 +157,31 @@
         )
 
         utils.write_replay_to_file(self.file, replay)
         self.undo_stack.set_unmodified()
 
         return True
 
-    def new_file(self, level_id: str, character: Character):
-        self.file = None
-        self.level.set(level_id)
-        self.character = character
-        self.inputs.reset()
-        self.undo_stack.clear()
+    def new_file(self):
+        def callback(metadata: ReplayMetadata):
+            self.file = None
+            self.level.set(metadata.level)
+            self.character = metadata.character
+            self.inputs.reset()
+            self.undo_stack.clear()
+
+        ReplayMetadataDialog(self, callback, creating=True)
+
+    def edit_replay_metadata(self):
+        def callback(metadata: ReplayMetadata):
+            self.level.set(metadata.level)
+            self.character = metadata.character
+
+        metadata = ReplayMetadata(self.character, self.level.get())
+        ReplayMetadataDialog(self, callback, defaults=metadata)
 
     def open_file(self):
         filepath = tk.filedialog.askopenfilename(
             defaultextension=".dfreplay",
             filetypes=[("replay files", "*.dfreplay")],
             title="Load replay"
         )
@@ -211,18 +196,18 @@
         self.inputs.set_intents(replay.players[0].intents)
 
         self.undo_stack.clear()
         if filepath is not None:
             self.undo_stack.set_unmodified()
 
     def set_dustforce_directory(self):
-        current_path = config.dustforce_path
+        current_path = config.get(ConfigOption.DUSTFORCE_PATH)
         new_path = tk.filedialog.askdirectory(initialdir=current_path)
         if new_path:
-            config.dustforce_path = new_path
+            config.set(ConfigOption.DUSTFORCE_PATH, new_path)
         config.write()
 
     def on_undo_stack_change(self):
         undo_state = tk.NORMAL if self.undo_stack.can_undo else tk.DISABLED
         redo_state = tk.NORMAL if self.undo_stack.can_redo else tk.DISABLED
 
         undo_label = "Undo " + self.undo_stack.undo_text()
```

### Comparing `dusted-1.2.0/dusted/inputs.py` & `dusted-1.3.0/dusted/inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from typing import List, Dict
 
 from dustmaker.replay import IntentStream
 
 from dusted.broadcaster import Broadcaster
 
-INTENT_COUNT = 7
+INTENT_COUNT = 8
 
-DEFAULT_INPUTS = "1100000"
+DEFAULT_INPUTS = "11000000"
 VALID_INPUTS = [
     "012",
     "012",
     "012",
     "01",
     "01",
     "0123456789ab",
     "0123456789ab",
+    "012",
 ]
 INPUT_TO_TEXT = [
     lambda x: str(x + 1),
     lambda x: str(x + 1),
     lambda x: str(x),
     lambda x: str(x),
     lambda x: str(x),
     lambda x: hex(x)[2:],
     lambda x: hex(x)[2:],
+    lambda x: str(x),
 ]
 TEXT_TO_INPUT = [
     lambda x: int(x) - 1,
     lambda x: int(x) - 1,
     lambda x: int(x),
     lambda x: int(x),
     lambda x: int(x),
     lambda x: int(x, 16),
     lambda x: int(x, 16),
+    lambda x: int(x),
 ]
 
 
 class Inputs(Broadcaster):
     """Stores a rectangular grid of inputs."""
 
     def __init__(self, inputs=None):
@@ -51,15 +54,15 @@
     def __len__(self):
         """Return the number of frames that the inputs cover."""
         return self.length
 
     def set_intents(self, intents: Dict[IntentStream, List[int]]):
         inputs = []
         for intent, input_to_text in enumerate(INPUT_TO_TEXT):
-            inputs.append([input_to_text(x) for x in intents[IntentStream(intent)]])
+            inputs.append([input_to_text(x) for x in intents.get(IntentStream(intent), [])])
         self.set(inputs)
 
     def get_intents(self) -> Dict[IntentStream, List[int]]:
         intents = {}
         for intent, text_to_input in enumerate(TEXT_TO_INPUT):
             intents[IntentStream(intent)] = [text_to_input(c) for c in self.inputs[intent]]
         return intents
```

### Comparing `dusted-1.2.0/dusted/inputs_view.py` & `dusted-1.3.0/dusted/inputs_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,21 @@
     def clear_selection(self):
         self.undo_stack.execute(ClearInputsCommand(self.cursor.selection))
 
     def insert_frames(self, count):
         self.undo_stack.execute(InsertFramesCommand(self.cursor.selection_left, count))
 
     def delete_frames(self):
-        self.undo_stack.execute(DeleteFramesCommand(self.cursor.selection_left, self.cursor.selection_width))
+        # Protect against deleting the "frame-after-last"
+        width = self.cursor.selection_width
+        if self.cursor.selection_right == len(self.inputs):
+            width -= 1
+        if width == 0:
+            return
+        self.undo_stack.execute(DeleteFramesCommand(self.cursor.selection_left, width))
 
     def on_click(self, event, keep_selection=False):
         self.focus_set()
         col = (event.x_root - self.winfo_rootx()) // GRID_SIZE
         row = (event.y_root - self.winfo_rooty()) // GRID_SIZE - 2
         if 0 <= row < INTENT_COUNT and 0 <= col:
             self.cursor.set(row, col + self.current_col, keep_selection)
@@ -351,15 +357,15 @@
         self.scrollbar.set(left, right)
 
 
 class InputsView(tk.Frame):
     def __init__(self, parent, inputs, cursor, undo_stack):
         super().__init__(parent)
 
-        for row, text in enumerate(["", "Frame", "X (L/R)", "Y (U/D)", "Jump", "Dash", "Fall", "Light", "Heavy"]):
+        for row, text in enumerate(["", "Frame", "X (L/R)", "Y (U/D)", "Jump", "Dash", "Fall", "Light", "Heavy", "Taunt"]):
             label = tk.Label(self, text=text, padx=5)
             label.grid(row=row, column=0, sticky="e")
 
         scrollbar = tk.Scrollbar(self, orient=tk.HORIZONTAL)
         grid = Grid(self, scrollbar, inputs, cursor, undo_stack)
         scrollbar.config(command=grid.on_scroll)
```

### Comparing `dusted-1.2.0/dusted/level_view.py` & `dusted-1.3.0/dusted/level_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,9 +128,9 @@
         for i, (x, y) in enumerate(self.coords):
             d = math.hypot(cx - x, cy - y)
             if d < dist:
                 dist = d
                 closest = i
 
         if closest is not None:
-            row, _ = self.cursor.position()
+            row, _ = self.cursor.position
             self.cursor.set(row, closest, keep_selection)
```

### Comparing `dusted-1.2.0/dusted/undo_stack.py` & `dusted-1.3.0/dusted/undo_stack.py`

 * *Files identical despite different names*

### Comparing `dusted-1.2.0/dusted/utils.py` & `dusted-1.3.0/dusted/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import requests
 from dustmaker.dfreader import DFReader
 from dustmaker.dfwriter import DFWriter
 from dustmaker.level import Level
 from dustmaker.replay import Replay
 
-from dusted.config import config
+from dusted.config import config, ConfigOption
 
 
 def load_replay_from_dustkid(replay_id: str) -> Replay:
     data = {"replay": replay_id}
     response = requests.post("https://dustkid.com/backend8/get_replay.php", data=data)
     if not response.ok:
         raise RuntimeError("Could not fetch replay from dustkid")
@@ -24,15 +24,15 @@
     if level is None:
         level = load_level_from_dustkid(level_id)
     return level
 
 
 def load_level_from_file(level_id: str) -> Level:
     for path in ("content/levels2", "content/levels3", "user/levels", "user/level_src"):
-        level_path = Path(config.dustforce_path) / path / level_id
+        level_path = Path(config.get(ConfigOption.DUSTFORCE_PATH)) / path / level_id
         try:
             with level_path.open("rb") as file:
                 return DFReader(file).read_level()
         except FileNotFoundError:
             pass
```

### Comparing `dusted-1.2.0/dusted.egg-info/PKG-INFO` & `dusted-1.3.0/dusted.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dusted
-Version: 1.2.0
+Version: 1.3.0
 Summary: Dustforce replay editor
 Home-page: https://github.com/AlexMorson/dusted
 Author: Alex Morson
 Author-email: alexmorson@btinternet.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: appdirs~=1.4.4
+Requires-Dist: dustmaker~=1.1.0
+Requires-Dist: requests~=2.22
 
 # Dusted
 
 An offline editor for Dustforce replays, largely based on dustkid.com's replay composer.
 
 ## Installation
 
@@ -35,9 +36,7 @@
 ```
 
 or, if the python scripts directory is on the PATH
 
 ```
 dusted
 ```
-
-
```

### Comparing `dusted-1.2.0/dusted.egg-info/SOURCES.txt` & `dusted-1.3.0/dusted.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 dusted/cursor.py
 dusted/dialog.py
 dusted/gui.py
 dusted/inputs.py
 dusted/inputs_view.py
 dusted/level.py
 dusted/level_view.py
+dusted/replay_metadata.py
 dusted/undo_stack.py
 dusted/utils.py
 dusted.egg-info/PKG-INFO
 dusted.egg-info/SOURCES.txt
 dusted.egg-info/dependency_links.txt
 dusted.egg-info/entry_points.txt
 dusted.egg-info/requires.txt
```

### Comparing `dusted-1.2.0/setup.cfg` & `dusted-1.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dusted
-version = 1.2.0
+version = 1.3.0
 url = https://github.com/AlexMorson/dusted
 author = Alex Morson
 author_email = alexmorson@btinternet.com
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 license_file = LICENSE.txt
@@ -18,15 +18,14 @@
 	appdirs ~= 1.4.4
 	dustmaker ~= 1.1.0
 	requests ~= 2.22
 packages = 
 	dusted
 	dusted.dustforce
 	dusted.geom
-	dusted.replay
 
 [options.entry_points]
 gui_scripts = 
 	dusted = dusted.__main__:main
 
 [egg_info]
 tag_build =
```

### Comparing `dusted-1.2.0/test/test_cursor.py` & `dusted-1.3.0/test/test_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def test_clamp_position(self):
         # Top
         self.cursor.set(-10, 2)
         self.assertEqual(self.cursor.selection, (0, 2, 0, 2))
 
         # Bottom
         self.cursor.set(10, 2)
-        self.assertEqual(self.cursor.selection, (6, 2, 6, 2))
+        self.assertEqual(self.cursor.selection, (7, 2, 7, 2))
 
         # Left
         self.cursor.set(2, -10)
         self.assertEqual(self.cursor.selection, (2, 0, 2, 0))
 
         # Right
         self.cursor.set(2, 100)
```

### Comparing `dusted-1.2.0/test/test_inputs.py` & `dusted-1.3.0/test/test_inputs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,111 +2,117 @@
 
 from dusted.inputs import Inputs
 
 
 class TestInputs(TestCase):
     def setUp(self):
         self.default = Inputs()
-        self.custom = Inputs(["".join(str((row + col) % 2) for col in range(100)) for row in range(7)])
+        self.custom = Inputs(["".join(str((row + col) % 2) for col in range(100)) for row in range(8)])
 
         self.callback = mock.Mock()
         self.default.subscribe(self.callback)
         self.custom.subscribe(self.callback)
 
     def test_length(self):
         self.assertEqual(len(self.default), 55)
         self.assertEqual(len(self.custom), 100)
 
     def test_get(self):
-        self.assertEqual(self.default.get(), [list(c * 55) for c in "1100000"])
+        self.assertEqual(self.default.get(), [list(c * 55) for c in "11000000"])
 
     def test_reset(self):
         self.custom.reset()
         self.callback.assert_called()
-        self.assertEqual(self.custom.get(), [list(c * 55) for c in "1100000"])
+        self.assertEqual(self.custom.get(), [list(c * 55) for c in "11000000"])
 
     def test_insert_frames(self):
         self.custom.insert_frames(1, 2)
         self.callback.assert_called()
 
         inputs = self.custom.get()
         self.assertEqual(inputs[0][:4], list("0111"))
         self.assertEqual(inputs[1][:4], list("1110"))
         self.assertEqual(inputs[2][:4], list("0001"))
         self.assertEqual(inputs[3][:4], list("1000"))
         self.assertEqual(inputs[4][:4], list("0001"))
         self.assertEqual(inputs[5][:4], list("1000"))
         self.assertEqual(inputs[6][:4], list("0001"))
+        self.assertEqual(inputs[7][:4], list("1000"))
         self.assertEqual(len(inputs[0]), 102)
 
     def test_delete_frames(self):
         self.custom.delete_frames(1, 3)
         self.callback.assert_called()
 
         inputs = self.custom.get()
         self.assertEqual(inputs[0][:4], list("0010"))
         self.assertEqual(inputs[1][:4], list("1101"))
         self.assertEqual(inputs[2][:4], list("0010"))
         self.assertEqual(inputs[3][:4], list("1101"))
         self.assertEqual(inputs[4][:4], list("0010"))
         self.assertEqual(inputs[5][:4], list("1101"))
         self.assertEqual(inputs[6][:4], list("0010"))
+        self.assertEqual(inputs[7][:4], list("1101"))
         self.assertEqual(len(inputs[0]), 97)
 
     def test_write(self):
         self.custom.write((2, 1), [list("01"), list("10")])
         self.callback.assert_called()
 
         inputs = self.custom.get()
         self.assertEqual(inputs[0][:4], list("0101"))
         self.assertEqual(inputs[1][:4], list("1010"))
         self.assertEqual(inputs[2][:4], list("0011"))
         self.assertEqual(inputs[3][:4], list("1100"))
         self.assertEqual(inputs[4][:4], list("0101"))
         self.assertEqual(inputs[5][:4], list("1010"))
         self.assertEqual(inputs[6][:4], list("0101"))
+        self.assertEqual(inputs[7][:4], list("1010"))
 
     def test_invalid_write(self):
         self.custom.write((0, 1), [["3"], ["a"], ["3"], ["a"], ["z"], ["$"]])
         self.callback.assert_called()
 
         inputs = self.custom.get()
         self.assertEqual(inputs[0][:4], list("0101"))
         self.assertEqual(inputs[1][:4], list("1010"))
         self.assertEqual(inputs[2][:4], list("0101"))
         self.assertEqual(inputs[3][:4], list("1010"))
         self.assertEqual(inputs[4][:4], list("0101"))
         self.assertEqual(inputs[5][:4], list("1010"))
         self.assertEqual(inputs[6][:4], list("0101"))
+        self.assertEqual(inputs[7][:4], list("1010"))
 
     def test_fill(self):
         self.custom.fill((1, 1, 5, 2), "2")
         self.callback.assert_called()
 
         inputs = self.custom.get()
         self.assertEqual(inputs[0][:4], list("0101"))
         self.assertEqual(inputs[1][:4], list("1220"))
         self.assertEqual(inputs[2][:4], list("0221"))
         self.assertEqual(inputs[3][:4], list("1010"))
         self.assertEqual(inputs[4][:4], list("0101"))
         self.assertEqual(inputs[5][:4], list("1220"))
         self.assertEqual(inputs[6][:4], list("0101"))
+        self.assertEqual(inputs[7][:4], list("1010"))
 
     def test_clear(self):
         self.custom.clear((1, 1, 5, 2))
         self.callback.assert_called()
 
         inputs = self.custom.get()
         self.assertEqual(inputs[0][:4], list("0101"))
         self.assertEqual(inputs[1][:4], list("1110"))
         self.assertEqual(inputs[2][:4], list("0001"))
         self.assertEqual(inputs[3][:4], list("1000"))
         self.assertEqual(inputs[4][:4], list("0001"))
         self.assertEqual(inputs[5][:4], list("1000"))
         self.assertEqual(inputs[6][:4], list("0101"))
+        self.assertEqual(inputs[7][:4], list("1010"))
 
     def test_read(self):
         self.assertEqual(self.custom.read((1, 1, 3, 3)), [list("010"), list("101"), list("010")])
 
     def test_at(self):
         self.assertEqual(self.default.at(2, 1), "0")
         self.assertEqual(self.default.at(1, 2), "1")
```

