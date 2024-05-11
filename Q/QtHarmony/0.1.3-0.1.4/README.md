# Comparing `tmp/qtharmony-0.1.3.tar.gz` & `tmp/qtharmony-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.3.tar", max compression
+gzip compressed data, was "qtharmony-0.1.4.tar", max compression
```

## Comparing `qtharmony-0.1.3.tar` & `qtharmony-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.3/LICENSE
--rw-r--r--   0        0        0     1306 2024-05-11 05:40:26.226219 qtharmony-0.1.3/README.md
--rw-r--r--   0        0        0      609 2024-05-11 07:39:53.936133 qtharmony-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      552 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        0 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.3/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      965 2024-05-11 06:53:13.297360 qtharmony-0.1.3/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       22 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/src/util/__init__.py
--rw-r--r--   0        0        0      125 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/src/util/config.py
--rw-r--r--   0        0        0      296 2024-05-11 07:38:57.408587 qtharmony-0.1.3/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     1143 2024-05-11 07:37:45.118396 qtharmony-0.1.3/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     1129 2024-05-11 07:35:34.954071 qtharmony-0.1.3/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     1436 2024-05-11 07:35:00.372249 qtharmony-0.1.3/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     2155 2024-05-11 07:37:33.075587 qtharmony-0.1.3/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     1413 2024-05-11 07:37:04.116848 qtharmony-0.1.3/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0      809 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     1395 2024-05-11 06:45:00.352043 qtharmony-0.1.3/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     2464 2024-05-11 07:33:53.978491 qtharmony-0.1.3/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0      943 2024-05-11 07:33:17.296767 qtharmony-0.1.3/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1306 2024-05-11 07:36:21.018726 qtharmony-0.1.3/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0      278 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      521 2024-05-11 06:45:00.352043 qtharmony-0.1.3/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      293 2024-05-11 05:40:26.232885 qtharmony-0.1.3/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      474 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.3/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.3/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0      265 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0      210 2024-05-11 07:38:47.092368 qtharmony-0.1.3/qtharmony/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     1269 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0       58 2024-05-11 05:40:26.236219 qtharmony-0.1.3/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1306 2024-05-11 05:40:26.226219 qtharmony-0.1.4/README.md
+-rw-r--r--   0        0        0      609 2024-05-11 07:53:55.653155 qtharmony-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        0 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      965 2024-05-11 06:53:13.297360 qtharmony-0.1.4/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       22 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/util/__init__.py
+-rw-r--r--   0        0        0      125 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/util/config.py
+-rw-r--r--   0        0        0      296 2024-05-11 07:40:36.584284 qtharmony-0.1.4/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-11 07:40:36.584284 qtharmony-0.1.4/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2556 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2406 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3383 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2403 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1518 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3737 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1876 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0      278 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      521 2024-05-11 06:45:00.352043 qtharmony-0.1.4/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      293 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      474 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.4/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.4/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0      265 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0      210 2024-05-11 07:40:36.584284 qtharmony-0.1.4/qtharmony/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     1269 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0       58 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.4/PKG-INFO
```

### Comparing `qtharmony-0.1.3/LICENSE` & `qtharmony-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/README.md` & `qtharmony-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/pyproject.toml` & `qtharmony-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.3"
+version = "0.1.4"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.3/qtharmony/constructor/initialize.py` & `qtharmony-0.1.4/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.4/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/resources/ui/Logo.png` & `qtharmony-0.1.4/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.4/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/src/core/dialog.py` & `qtharmony-0.1.4/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/src/core/font.py` & `qtharmony-0.1.4/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/src/core/stylesheet.py` & `qtharmony-0.1.4/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/digital_entry.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,30 +7,45 @@
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
     from PySide6.QtWidgets import QWidget
 
 
 class DigitalEntry(QSpinBox):
     """
-    Custom QSpinBox widget for entering digital values.
+    Custom QSpinBox widget for numerical input.
 
     Methods:
-    - __init__(__range: tuple[int, int], width: int = 30, height: int = 25, show_buttons: bool = False): None - Initializes the digital entry with a specified range, width, height, and button display.
+    - __init__(range: tuple[int, int] = (0, 100), size: tuple[int, int] = (40, 30),
+              font: Optional["QFont"] = None, include_buttons: bool = False,
+              *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the DigitalEntry widget with optional range, size, font, button inclusion, and stylesheet.
     """
 
     def __init__(
             self, 
             range: tuple[int, int] = (0, 100), 
             size: tuple[int, int] = (40, 30), 
             font: Optional["QFont"] = None, 
             include_buttons: bool = False,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
+        """
+        Initializes the DigitalEntry widget with optional range, size, font, button inclusion, and stylesheet.
+
+        Args:
+            range (tuple[int, int], optional): The range of values allowed in the spin box. Defaults to (0, 100).
+            size (tuple[int, int], optional): The size of the spin box widget (width, height). Defaults to (40, 30).
+            font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
+            include_buttons (bool, optional): Flag to include or exclude spin box buttons. Defaults to False.
+            stylesheet (Optional[str], optional): Custom stylesheet for the spin box widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the spin box. Defaults to None.
+        """
+
         super().__init__(parent)
 
         self.setFixedSize(QSize(*size))
         if not include_buttons: self.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         if font is not None: self.setFont(font)
 
         self.setObjectName("digital-entry")
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/entry.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/entry.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,30 +7,44 @@
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
     from PySide6.QtWidgets import QWidget
 
 
 class Entry(QLineEdit):
     """
-    Custom QLineEdit widget for text entry.
+    Custom QLineEdit widget for text input.
 
     Methods:
-    - __init__(__placed: str, placeholder: str = "", width: int = 200, height: int = 25): None - Initializes the text entry with default text and placeholder.
+    - __init__(placed: Optional[str] = None, placeholder: Optional[str] = None, size: tuple[int, int] = (200, 30),
+              font: Optional["QFont"] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the Entry widget with optional text, placeholder, size, font, and stylesheet.
     """
 
     def __init__(
             self, 
             placed: Optional[str] = None, 
             placeholder: Optional[str] = None,
             size: tuple[int, int] = (200, 30), 
             font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
+        """
+        Initializes the Entry widget with optional text, placeholder, size, font, and stylesheet.
+
+        Args:
+            placed (Optional[str], optional): The initial text to be displayed in the entry. Defaults to None.
+            placeholder (Optional[str], optional): The placeholder text to be displayed when the entry is empty. Defaults to None.
+            size (tuple[int, int], optional): The size of the entry widget (width, height). Defaults to (200, 30).
+            font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
+            stylesheet (Optional[str], optional): Custom stylesheet for the entry widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the entry. Defaults to None.
+        """
+
         super().__init__(parent)
 
         if placed is not None: self.setText(placed)
         if placeholder is not None: self.setPlaceholderText(placeholder)
         if font is not None: self.setFont(font)
 
         self.setFixedSize(QSize(*size))
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/groups.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,21 +9,38 @@
 import os.path
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
 class GroupBox(QGroupBox):
+    """
+    Custom QGroupBox widget for grouping widgets.
+
+    Methods:
+    - __init__(title: Optional[str] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the GroupBox widget with optional title and stylesheet.
+    """
+
     def __init__(
             self,
             title: Optional[str] = None,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
+        """
+        Initializes the GroupBox widget with optional title and stylesheet.
+
+        Args:
+            title (Optional[str], optional): The title of the group box. Defaults to None.
+            stylesheet (Optional[str], optional): Custom stylesheet for the group box widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
+        """
+
         super().__init__(parent)
 
         self.setObjectName("group-box")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/group_box.css", 
             name="GroupBox", obj_name="QGroupBox#group-box",
             stylesheet=stylesheet
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/widgets_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,52 @@
-from PySide6.QtWidgets import QLabel
+from typing import Optional, TYPE_CHECKING
 
-from qtharmony.src.core import Font, StyleSheetLoader
+from PySide6.QtWidgets import (
+    QListWidget, QListWidgetItem, QFrame,
+    QHBoxLayout, QLabel
+)
+from PySide6.QtCore import Qt
 
-from typing import Optional, TYPE_CHECKING
+from qtharmony.src.core import Loader
+
+import os.path
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
-class Label(QLabel):
+class WidgetsList(QFrame):
     def __init__(
             self, 
-            text: str,
-            font_family: str, 
-            font_size: int,
-            bold: bool = False,
-            italic: bool = False,
-            color: str = "#000000",
-            word_wrap: bool = False,
+            size: tuple[int, int] = (600, 400),
+            title: Optional[str] = None,
             *,
             stylesheet: Optional[str] = None,
-            parent: Optional["QWidget"] = None
+            parent: Optional["QWidget"] = None,
     ) -> None:
         super().__init__(parent)
 
-        self.setObjectName("label")
-        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/label.css", 
-            name="Label", obj_name="QLabel#label",
-            stylesheet=stylesheet
-        ))
-
-        self.setText(text)
-        self.set_color(color)
-        
-        self.setWordWrap(word_wrap)
-        self.setFont(Font.get_system_font(font_family, font_size, bold, italic))
-    
-    def set_color(self, color: str) -> None:
-        self.__append_stylesheet("Label {" + f"color: {color}" + "}")
-    
-    def __append_stylesheet(self, stylesheet: str) -> None:
-        self.setStyleSheet(StyleSheetLoader.append_stylesheet(
-            self.styleSheet(), stylesheet, name="Label", obj_name="QLabel#label"
-        ))
+        self.mainLayout = QHBoxLayout()
+        self.listWidget = QListWidget()
+
+        # self.setStyleSheet(Loader.load_file("modernqt/widgets/basic/styles/widgets_list.css"))
+        self.setObjectName("widgets-list")
+        self.setFocusPolicy(Qt.FocusPolicy.NoFocus)
+
+        stylesheet_path = os.path.join(os.path.dirname(__file__), "styles/widgets_list.css")
+
+        if stylesheet is not None:
+            self.setStyleSheet(
+                Loader.load_file(stylesheet_path) + "\n" 
+                + stylesheet.replace("WidgetsList", "QListWidget#widgets-list")
+            )
+        else:
+            self.setStyleSheet(Loader.load_file(stylesheet_path))
+
+        if stylesheet is not None:
+            self.setStyleSheet(self.styleSheet() + stylesheet)
+
+    def add_widget(self, widget) -> None:
+        item = QListWidgetItem()
+        item.setSizeHint(widget.sizeHint())
+        self.listWidget.addItem(item)
+        self.listWidget.setItemWidget(item, widget)
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/path_entry.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,35 +13,48 @@
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
 
 
 class PathEntry(QWidget):
     """
-    Custom QLineEdit widget for entering path to file and directories.
+    Custom QWidget combining a QLineEdit for path input and a button to specify the path.
 
     Methods:
-    - __init__(self, __placed: str, placeholder: str = "", width: int = 400, height: int = 25): None - Initializes the path entry with default text and placeholder.
-    - get_entry(self): Entry - returns the Entry widget.
-    - set_path(self, __path: str, only_existing: bool = True): None if only_existing is True and path is not exist this path won't be pasted.
-
-    Notes:
-    - This widget includes Entry and PushButton to specify the path to your file or directory
+    - __init__(placed: Optional[str] = None, placeholder: Optional[str] = None, size: tuple[int, int] = (200, 30),
+              font: Optional["QFont"] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the PathEntry widget with path input functionality.
+    - set_path(__path: Optional[str] = None, only_existing: bool = True) -> None
+              - Sets the path in the path entry widget.
+    - get_entry() -> Entry
+              - Returns the Entry widget used for path input.
     """
 
     def __init__(
             self, 
             placed: Optional[str] = None, 
             placeholder: Optional[str] = None,
             size: tuple[int, int] = (200, 30), 
             font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
+        """
+        Initializes the PathEntry widget with path input functionality.
+
+        Args:
+            placed (Optional[str], optional): The initial path text. Defaults to None.
+            placeholder (Optional[str], optional): The placeholder text for the path entry. Defaults to None.
+            size (tuple[int, int], optional): The size of the path entry widget (width, height). Defaults to (200, 30).
+            font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
+            stylesheet (Optional[str], optional): Custom stylesheet for the path entry widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the path entry. Defaults to None.
+        """        
+
         super().__init__(parent)
 
         self.setObjectName("path-entry")
         if font is not None: self.setFont(font)
 
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/path_entry.css", 
@@ -58,18 +71,33 @@
 
         self.mainLayout.addWidget(self.pathEntry)
         self.mainLayout.addWidget(self.specifyPathBtn)
         self.mainLayout.addItem(QSpacerItem(20, 20, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum))
         self.setLayout(self.mainLayout)
 
     def set_path(self, __path: Optional[str] = None, only_existing: bool = True) -> None:
+        """
+        Sets the path in the path entry widget.
+
+        Args:
+            __path (Optional[str], optional): The path to be set. Defaults to None.
+            only_existing (bool, optional): Flag to only set the path if it exists. Defaults to True.
+        """
+
         if __path is None: return
 
         if only_existing and os.path.exists(__path):
             self.pathEntry.setText(__path)
             return
 
         self.pathEntry.setText(__path)
 
     def get_entry(self) -> Entry:
+        """
+        Returns the Entry widget used for path input.
+
+        Returns:
+            Entry: The Entry widget for path input.
+        """
+
         return self.pathEntry
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.1.4/qtharmony/windows/main_window.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,41 @@
-from PySide6.QtWidgets import QRadioButton
-from PySide6.QtCore import QSize
+from PySide6.QtWidgets import QMainWindow, QWidget
+from PySide6.QtGui import QIcon
 
 from qtharmony.src.core import StyleSheetLoader
 from qtharmony.src.util import RESOURCES
 
-from typing import Optional, TYPE_CHECKING
-if TYPE_CHECKING:
-    from PySide6.QtWidgets import QWidget
+from typing import Optional
+import os.path
 
 
-class RadioButton(QRadioButton):
+class MainWindow(QMainWindow):
     def __init__(
-            self,
-            text: Optional[str] = None,
-            size: tuple[int, int] = (200, 30),
+            self, 
+            widget: Optional[QWidget] = None,
+            size: tuple[int, int] = (1000, 600),
+            title: Optional[str] = None,
+            is_resizable: bool = True,
             *,
             stylesheet: Optional[str] = None,
-            parent: Optional["QWidget"] = None
+            parent: Optional[QWidget] = None
     ) -> None:
         super().__init__(parent)
 
-        if text is not None: self.setText(text)
-        self.setFixedSize(QSize(*size))
-
-        self.setObjectName("radio-button")
+        if widget is not None: self.setCentralWidget(widget)
+        self.setWindowIcon(QIcon(f"{os.path.join(RESOURCES, 'ui/Icon.png')}"))
+        
+        self.setObjectName("main-window")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/radio_button.css", 
-            name="RadioButton", obj_name="QRadioButton#radio-button",
+            __file__, "styles/main_window.css", 
+            name="MainWindow", obj_name="QMainWindow#main-window",
             stylesheet=stylesheet
         ))
+
+        self.resize(*size)
+        if title is not None: self.setWindowTitle(title)
+        else: self.setWindowTitle("QtHarmony")
+
+        if not is_resizable: self.setFixedSize(*size)
+    
+    def run(self) -> None:
+        self.show()
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.1.4/qtharmony/widgets/basic/splitter.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,21 +20,37 @@
     def __init__(
             self, 
             __orientation: str,
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
+        """
+        Initializes the Splitter instance with the specified orientation.
+
+        Args:
+            __orientation (str): The orientation of the splitter, either "horizontal" or "vertical".
+            stylesheet (Optional[str], optional): Custom stylesheet for the splitter. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the splitter. Defaults to None.
+        """
+
         if __orientation == "horizontal": super().__init__(Qt.Orientation.Horizontal, parent)
         elif __orientation == "vertical": super().__init__(Qt.Orientation.Vertical, parent)
 
         self.setObjectName("splitter")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/splitter.css", 
             name="Splitter", obj_name="QSplitter#splitter",
             stylesheet=stylesheet
         ))
 
     def addWidget(self, widget):
+        """
+        Adds a widget to the splitter and sets it as non-collapsible.
+
+        Args:
+            widget (QWidget): The widget to be added to the splitter.
+        """
+
         super().addWidget(widget)
         self.setCollapsible(self.indexOf(widget), False)
```

### Comparing `qtharmony-0.1.3/qtharmony/widgets/basic/styles/check_box.css` & `qtharmony-0.1.4/qtharmony/widgets/basic/styles/check_box.css`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.3/PKG-INFO` & `qtharmony-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.3
+Version: 0.1.4
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

