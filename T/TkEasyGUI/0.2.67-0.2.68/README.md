# Comparing `tmp/tkeasygui-0.2.67.tar.gz` & `tmp/tkeasygui-0.2.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.67.tar", last modified: Sat Apr 27 13:47:06 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.68.tar", last modified: Sat May 11 02:55:57 2024, max compression
```

## Comparing `tkeasygui-0.2.67.tar` & `tkeasygui-0.2.68.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-27 13:47:06.081625 tkeasygui-0.2.67/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.67/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-27 13:47:06.081276 tkeasygui-0.2.67/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     4343 2024-04-24 05:52:16.000000 tkeasygui-0.2.67/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-27 13:47:06.078857 tkeasygui-0.2.67/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.67/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    28011 2024-04-27 13:34:47.000000 tkeasygui-0.2.67/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.67/TkEasyGUI/locale_easy.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-27 13:29:24.000000 tkeasygui-0.2.67/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-27 13:47:04.000000 tkeasygui-0.2.67/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   124136 2024-04-27 13:31:46.000000 tkeasygui-0.2.67/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-27 13:47:06.080586 tkeasygui-0.2.67/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-27 13:47:06.000000 tkeasygui-0.2.67/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-27 13:34:59.000000 tkeasygui-0.2.67/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-27 13:47:06.081719 tkeasygui-0.2.67/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-11 02:55:57.946493 tkeasygui-0.2.68/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.68/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     7181 2024-05-11 02:55:57.946254 tkeasygui-0.2.68/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4777 2024-04-27 14:17:16.000000 tkeasygui-0.2.68/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-11 02:55:57.944342 tkeasygui-0.2.68/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.68/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    28011 2024-04-27 13:34:47.000000 tkeasygui-0.2.68/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.68/TkEasyGUI/locale_easy.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-27 13:29:24.000000 tkeasygui-0.2.68/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-05-11 02:55:56.000000 tkeasygui-0.2.68/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   124495 2024-05-11 02:49:19.000000 tkeasygui-0.2.68/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-05-11 02:55:57.945864 tkeasygui-0.2.68/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     7181 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-05-11 02:55:57.000000 tkeasygui-0.2.68/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-05-11 02:50:51.000000 tkeasygui-0.2.68/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-05-11 02:55:57.946550 tkeasygui-0.2.68/setup.cfg
```

### Comparing `tkeasygui-0.2.67/LICENSE` & `tkeasygui-0.2.68/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.67/PKG-INFO` & `tkeasygui-0.2.68/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.67
+Version: 0.2.68
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -107,20 +107,20 @@
 import TkEasyGUI as eg
 # define layout
 layout = [
     [eg.Text("Hello, World!")],
     [eg.Button("OK")]
 ]
 # create a window
-window = eg.Window("Hello App", layout)
-# event loop
-for event, values in window.event_iter():
-    if event == "OK":
-        eg.print("Thank you.")
-        break
+with eg.Window("Hello App", layout) as window:
+    # event loop
+    for event, values in window.event_iter():
+        if event == "OK":
+            eg.print("Thank you.")
+            break
 ```
 
 You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
 ```py
 import TkEasyGUI as eg
 
@@ -148,14 +148,21 @@
 
 ## Documents
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
+## Tutorial
+
+Sorry, we only provide Japanese tutorials at the moment.
+
+- [TkEasyGUI - Pythonで最も素早くデスクトップアプリを創るライブラリ](https://note.com/kujirahand/n/n33a2df3aa3e5)
+- [マイナビニュースPython連載116回目 - 金額合計ツールでExcel要らず - 合計/整形/コピーのツールを作ろう](https://news.mynavi.jp/techplus/article/zeropython-116/)
+
 ## About the relationship with PySimpleGUI
 
 - When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
 - The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
 - This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
 - We are not considering full compatibility with PySimpleGUI.
```

### Comparing `tkeasygui-0.2.67/README.md` & `tkeasygui-0.2.68/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 import TkEasyGUI as eg
 # define layout
 layout = [
     [eg.Text("Hello, World!")],
     [eg.Button("OK")]
 ]
 # create a window
-window = eg.Window("Hello App", layout)
-# event loop
-for event, values in window.event_iter():
-    if event == "OK":
-        eg.print("Thank you.")
-        break
+with eg.Window("Hello App", layout) as window:
+    # event loop
+    for event, values in window.event_iter():
+        if event == "OK":
+            eg.print("Thank you.")
+            break
 ```
 
 You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
 ```py
 import TkEasyGUI as eg
 
@@ -100,14 +100,21 @@
 
 ## Documents
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
+## Tutorial
+
+Sorry, we only provide Japanese tutorials at the moment.
+
+- [TkEasyGUI - Pythonで最も素早くデスクトップアプリを創るライブラリ](https://note.com/kujirahand/n/n33a2df3aa3e5)
+- [マイナビニュースPython連載116回目 - 金額合計ツールでExcel要らず - 合計/整形/コピーのツールを作ろう](https://news.mynavi.jp/techplus/article/zeropython-116/)
+
 ## About the relationship with PySimpleGUI
 
 - When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
 - The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
 - This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
 - We are not considering full compatibility with PySimpleGUI.
```

### Comparing `tkeasygui-0.2.67/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.68/TkEasyGUI/dialogs.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.67/TkEasyGUI/locale_easy.py` & `tkeasygui-0.2.68/TkEasyGUI/locale_easy.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.67/TkEasyGUI/utils.py` & `tkeasygui-0.2.68/TkEasyGUI/utils.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.67/TkEasyGUI/widgets.py` & `tkeasygui-0.2.68/TkEasyGUI/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     ) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = utils._get_active_window()
         if active_win is None:
             active_win = get_root_window()
+        self.title: str = title
         self.window: tk.Toplevel = tk.Toplevel(master=active_win)
         self.timeout: Union[int, None] = None
         self.timeout_key: str = WINDOW_TIMEOUT
         self.timeout_id: Union[str, None] = None
         self.events: Queue = Queue()
         self.key_elements: dict[str, Element] = {}
         self.last_values: dict[str, Any] = {}
@@ -156,15 +157,15 @@
             self.frame: tk.Frame = tk.Frame(self.canvas)
             self.canvas.create_window((0, 0), window=self.frame, anchor=tk.NW)
         else:
             self.frame: tk.Frame = tk.Frame(self.window)
             self.frame.pack(expand=True, fill="both", padx=padding_x, pady=padding_y)
         # self.frame.configure(style="TFrame")
         # set window properties
-        self.window.title(title)
+        self.set_title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         self.size: Union[tuple[int, int], None] = size
         if size is not None:
             self.set_size(size)
         self.window.resizable(resizable, resizable)
         # create widgets
         self._create_widget(self.frame, layout)
@@ -426,14 +427,20 @@
                 if win_x < 10 or win_y < 10:
                     win_x = 600 # TODO: 適当なサイズ
                     win_y = 400
             else:
                 win_x, win_y = self.size
             x = (cx - win_x // 2)
             y = (cy - win_y // 2)
+            # It will be out of range, so move it to the center.
+            if x < 0 or y < 0:
+                w, h = self.get_screen_size()
+                cx, cy = w // 2, h // 2
+                x = cx - win_x // 2
+                y = cy - win_y // 2
             self.move(x, y)
         except Exception as _:
             pass
     def get_size(self) -> tuple[int, int]:
         """Get the window size."""
         size = self.window.geometry().split("+")[0].split("x")
         return (int(size[0]), int(size[1]))
@@ -465,14 +472,15 @@
         # mainloop for hook
         key, values = (None, {}) # set default key and values
         # mainloop - read a event
         while True:
             # set timeout
             if self.timeout_id is not None:
                 self.window.after_cancel(self.timeout_id)
+            self.window.update_idletasks()
             self.timeout_id = self.window.after("idle", self._window_idle_handler)
             # -----------------------------------------------------
             # mainloop - should be called only once
             # -----------------------------------------------------
             root.mainloop()
             # -----------------------------------------------------
             # after mainloop, check events
@@ -536,14 +544,15 @@
         """Set the window size."""
         self.window.geometry(f"{size[0]}x{size[1]}")
         self.size = size
     
     def set_title(self, title: str) -> None:
         """Set the title of the window."""
         self.window.title(title)
+        self.title = title
 
     def minimize(self) -> None:
         """Minimize the window."""
         self.window.iconify()
         self.minimized = True
 
     def normal(self) -> None:
@@ -3025,15 +3034,15 @@
         self.file_types = file_types
         self.props["text"] = button_text
         self.enable_events = enable_events
         # force set params
         self.multiple_files = False
         self.save_as = True
 
-class FileSaveAs(FileBrowse):
+class FileSaveAs(FileSaveAsBrowse):
     """FileSaveAs element. (alias of FileSaveAsBrowse)"""
     pass
 
 class FolderBrowse(FileBrowse):
     """FolderBrowse element."""
     def __init__(
                 self,
```

### Comparing `tkeasygui-0.2.67/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.68/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.67
+Version: 0.2.68
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -107,20 +107,20 @@
 import TkEasyGUI as eg
 # define layout
 layout = [
     [eg.Text("Hello, World!")],
     [eg.Button("OK")]
 ]
 # create a window
-window = eg.Window("Hello App", layout)
-# event loop
-for event, values in window.event_iter():
-    if event == "OK":
-        eg.print("Thank you.")
-        break
+with eg.Window("Hello App", layout) as window:
+    # event loop
+    for event, values in window.event_iter():
+        if event == "OK":
+            eg.print("Thank you.")
+            break
 ```
 
 You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
 ```py
 import TkEasyGUI as eg
 
@@ -148,14 +148,21 @@
 
 ## Documents
 
 Below is a detailed list of classes and methods.
 
 - [docs](https://github.com/kujirahand/tkeasygui-python/tree/main/docs)
 
+## Tutorial
+
+Sorry, we only provide Japanese tutorials at the moment.
+
+- [TkEasyGUI - Pythonで最も素早くデスクトップアプリを創るライブラリ](https://note.com/kujirahand/n/n33a2df3aa3e5)
+- [マイナビニュースPython連載116回目 - 金額合計ツールでExcel要らず - 合計/整形/コピーのツールを作ろう](https://news.mynavi.jp/techplus/article/zeropython-116/)
+
 ## About the relationship with PySimpleGUI
 
 - When utilizing basic features, it is compatible with PySimpleGUI. You can write programs using the same event model as PySimpleGUI.
 - The names of basic GUI components are also kept the same. However, while some property names differ, many unique features have been implemented.
 - This project was developed with PySimpleGUI in mind, but has been implemented entirely from scratch. There are no licensing issues.
 - We are not considering full compatibility with PySimpleGUI.
```

### Comparing `tkeasygui-0.2.67/pyproject.toml` & `tkeasygui-0.2.68/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.67"
+version = "0.2.68"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

