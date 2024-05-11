# Comparing `tmp/qtharmony-0.1.4.tar.gz` & `tmp/qtharmony-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.4.tar", max compression
+gzip compressed data, was "qtharmony-0.1.5.tar", max compression
```

## Comparing `qtharmony-0.1.4.tar` & `qtharmony-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.4/LICENSE
--rw-r--r--   0        0        0     1306 2024-05-11 05:40:26.226219 qtharmony-0.1.4/README.md
--rw-r--r--   0        0        0      609 2024-05-11 07:53:55.653155 qtharmony-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      552 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        0 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.4/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      965 2024-05-11 06:53:13.297360 qtharmony-0.1.4/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       22 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/util/__init__.py
--rw-r--r--   0        0        0      125 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/src/util/config.py
--rw-r--r--   0        0        0      296 2024-05-11 07:40:36.584284 qtharmony-0.1.4/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     1143 2024-05-11 07:40:36.584284 qtharmony-0.1.4/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2556 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2406 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3383 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2403 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1518 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3737 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1876 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.4/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0      278 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      521 2024-05-11 06:45:00.352043 qtharmony-0.1.4/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      293 2024-05-11 05:40:26.232885 qtharmony-0.1.4/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      474 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.4/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.4/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0      265 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0      210 2024-05-11 07:40:36.584284 qtharmony-0.1.4/qtharmony/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     1269 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0       58 2024-05-11 05:40:26.236219 qtharmony-0.1.4/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1306 2024-05-11 05:40:26.226219 qtharmony-0.1.5/README.md
+-rw-r--r--   0        0        0      609 2024-05-11 08:07:49.278048 qtharmony-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:00:19.969973 qtharmony-0.1.5/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-11 08:01:55.762526 qtharmony-0.1.5/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.5/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      965 2024-05-11 06:53:13.297360 qtharmony-0.1.5/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0      296 2024-05-11 07:40:36.584284 qtharmony-0.1.5/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2231 2024-05-11 08:06:40.834190 qtharmony-0.1.5/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2556 2024-05-11 08:05:32.046997 qtharmony-0.1.5/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2406 2024-05-11 07:50:41.511507 qtharmony-0.1.5/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3388 2024-05-11 08:02:40.433941 qtharmony-0.1.5/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2403 2024-05-11 07:50:41.511507 qtharmony-0.1.5/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1518 2024-05-11 07:50:41.511507 qtharmony-0.1.5/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.5/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3737 2024-05-11 07:50:41.511507 qtharmony-0.1.5/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1835 2024-05-11 08:03:28.768649 qtharmony-0.1.5/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.5/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0      278 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      521 2024-05-11 06:45:00.352043 qtharmony-0.1.5/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      293 2024-05-11 05:40:26.232885 qtharmony-0.1.5/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      474 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.5/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.5/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0      265 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0      210 2024-05-11 07:40:36.584284 qtharmony-0.1.5/qtharmony/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2604 2024-05-11 08:07:34.711980 qtharmony-0.1.5/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0       58 2024-05-11 05:40:26.236219 qtharmony-0.1.5/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.5/PKG-INFO
```

### Comparing `qtharmony-0.1.4/LICENSE` & `qtharmony-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/README.md` & `qtharmony-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/pyproject.toml` & `qtharmony-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.4"
+version = "0.1.5"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.4/qtharmony/constructor/initialize.py` & `qtharmony-0.1.5/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.5/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/resources/ui/Logo.png` & `qtharmony-0.1.5/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.5/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/src/core/dialog.py` & `qtharmony-0.1.5/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/src/core/font.py` & `qtharmony-0.1.5/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/src/core/stylesheet.py` & `qtharmony-0.1.5/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/groups.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-from PySide6.QtWidgets import QPushButton
-from PySide6.QtCore import QSize
+from typing import Optional, TYPE_CHECKING
 
-from qtharmony.src.core import StyleSheetLoader
+from PySide6.QtWidgets import (
+    QGroupBox, QButtonGroup
+)
 
-from typing import Optional, TYPE_CHECKING
+from qtharmony.src.core import Loader, StyleSheetLoader
+
+import os.path
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
-    from PySide6.QtGui import QFont
 
 
-class PushButton(QPushButton):
+class GroupBox(QGroupBox):
+    """
+    Custom QGroupBox widget for grouping widgets.
+
+    Methods:
+    - __init__(title: Optional[str] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the GroupBox widget with optional title and stylesheet.
+    """
+
     def __init__(
-            self, 
-            text: Optional[str] = None,
-            size: tuple[int, int] = (100, 25),
-            font: Optional["QFont"] = None, 
+            self,
+            title: Optional[str] = None,
             *,
             stylesheet: Optional[str] = None,
-            parent: Optional["QWidget"] = None, 
+            parent: Optional["QWidget"] = None
     ) -> None:
-        super().__init__(parent)
+        """
+        Initializes the GroupBox widget with optional title and stylesheet.
+
+        Args:
+            title (Optional[str], optional): The title of the group box. Defaults to None.
+            stylesheet (Optional[str], optional): Custom stylesheet for the group box widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
+        """
 
-        if font is not None: self.setFont(font)
+        super().__init__(parent)
 
+        self.setObjectName("group-box")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/button.css", 
-            name="PushButton", obj_name="QPushButton#button",
+            __file__, "styles/group_box.css", 
+            name="GroupBox", obj_name="QGroupBox#group-box",
             stylesheet=stylesheet
         ))
-        
-        self.setObjectName("button")
-        self.setMinimumSize(QSize(*size))
-
-        if text is not None:
-            self.setText(text)
-        
-        if stylesheet is not None:
-            self.setStyleSheet(self.styleSheet() + stylesheet)
+
+        if title is not None: self.setTitle(title)
```

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/check_box.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/digital_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os.path
 
 from PySide6.QtWidgets import QComboBox
 from PySide6.QtCore import Qt, QSize
 
 from qtharmony.src.core import StyleSheetLoader
-from qtharmony.src.util import RESOURCES
+from qtharmony.src.config import UI_RESOURCES
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
     from PySide6.QtWidgets import QWidget
 
 
@@ -67,15 +67,15 @@
     def __load_down_arrow_style(self) -> None:
         """
         Loads the custom style for the drop-down arrow in the DropDownMenu widget.
         """
 
         down_arrow = (
             "\nDropDownMenu::down-arrow {" 
-            + f"image: url({os.path.join(RESOURCES, 'ui/angle-down.png')})" 
+            + f"image: url({os.path.join(UI_RESOURCES, 'angle-down.png')})" 
             + "}"
         )
 
         self.setStyleSheet(StyleSheetLoader.append_stylesheet(
             self.styleSheet(), down_arrow, 
             name="DropDownMenu", obj_name="QComboBox#drop-down-menu"
         ))
```

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/entry.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/radio_button.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import Optional, TYPE_CHECKING
-
-from PySide6.QtWidgets import (
-    QGroupBox, QButtonGroup
-)
+from PySide6.QtWidgets import QRadioButton
+from PySide6.QtCore import QSize
 
-from qtharmony.src.core import Loader, StyleSheetLoader
-
-import os.path
+from qtharmony.src.core import StyleSheetLoader
 
+from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
-class GroupBox(QGroupBox):
+class RadioButton(QRadioButton):
     """
-    Custom QGroupBox widget for grouping widgets.
+    Custom QRadioButton widget for radio button functionality.
 
     Methods:
-    - __init__(title: Optional[str] = None, *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
-              - Initializes the GroupBox widget with optional title and stylesheet.
+    - __init__(text: Optional[str] = None, size: tuple[int, int] = (200, 30),
+              *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
+              - Initializes the RadioButton widget with optional text, size, and stylesheet.
     """
 
     def __init__(
             self,
-            title: Optional[str] = None,
+            text: Optional[str] = None,
+            size: tuple[int, int] = (200, 30),
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         """
-        Initializes the GroupBox widget with optional title and stylesheet.
+        Initializes the RadioButton widget with optional text, size, and stylesheet.
 
         Args:
-            title (Optional[str], optional): The title of the group box. Defaults to None.
-            stylesheet (Optional[str], optional): Custom stylesheet for the group box widget. Defaults to None.
-            parent (Optional["QWidget"], optional): Parent widget of the group box. Defaults to None.
-        """
+            text (Optional[str], optional): The text displayed next to the radio button. Defaults to None.
+            size (tuple[int, int], optional): The size of the radio button widget (width, height). Defaults to (200, 30).
+            stylesheet (Optional[str], optional): Custom stylesheet for the radio button widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
+        """ 
 
         super().__init__(parent)
 
-        self.setObjectName("group-box")
+        if text is not None: self.setText(text)
+        self.setFixedSize(QSize(*size))
+
+        self.setObjectName("radio-button")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/group_box.css", 
-            name="GroupBox", obj_name="QGroupBox#group-box",
+            __file__, "styles/radio_button.css", 
+            name="RadioButton", obj_name="QRadioButton#radio-button",
             stylesheet=stylesheet
         ))
-
-        if title is not None: self.setTitle(title)
```

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/path_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/button.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,63 @@
-from PySide6.QtWidgets import QRadioButton
+from PySide6.QtWidgets import QPushButton
 from PySide6.QtCore import QSize
 
 from qtharmony.src.core import StyleSheetLoader
-from qtharmony.src.util import RESOURCES
 
 from typing import Optional, TYPE_CHECKING
+
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
+    from PySide6.QtGui import QFont
 
 
-class RadioButton(QRadioButton):
+class PushButton(QPushButton):
     """
-    Custom QRadioButton widget for radio button functionality.
+    Custom QPushButton widget for push button functionality.
 
     Methods:
-    - __init__(text: Optional[str] = None, size: tuple[int, int] = (200, 30),
-              *, stylesheet: Optional[str] = None, parent: Optional["QWidget"] = None): None
-              - Initializes the RadioButton widget with optional text, size, and stylesheet.
+    - __init__(text: Optional[str] = None, size: tuple[int, int] = (100, 25), 
+              font: Optional["QFont"] = None, *, stylesheet: Optional[str] = None, 
+              parent: Optional["QWidget"] = None): None
+              - Initializes the PushButton widget with optional text, size, font, and stylesheet.
+
     """
 
     def __init__(
-            self,
+            self, 
             text: Optional[str] = None,
-            size: tuple[int, int] = (200, 30),
+            size: tuple[int, int] = (100, 25),
+            font: Optional["QFont"] = None, 
             *,
             stylesheet: Optional[str] = None,
-            parent: Optional["QWidget"] = None
+            parent: Optional["QWidget"] = None, 
     ) -> None:
         """
-        Initializes the RadioButton widget with optional text, size, and stylesheet.
+        Initializes the PushButton widget with optional text, size, font, and stylesheet.
 
         Args:
-            text (Optional[str], optional): The text displayed next to the radio button. Defaults to None.
-            size (tuple[int, int], optional): The size of the radio button widget (width, height). Defaults to (200, 30).
-            stylesheet (Optional[str], optional): Custom stylesheet for the radio button widget. Defaults to None.
-            parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
+            text (Optional[str], optional): The text displayed on the push button. Defaults to None.
+            size (tuple[int, int], optional): The size of the push button widget (width, height). Defaults to (100, 25).
+            font (Optional["QFont"], optional): The font used for the push button text. Defaults to None.
+            stylesheet (Optional[str], optional): Custom stylesheet for the push button widget. Defaults to None.
+            parent (Optional["QWidget"], optional): Parent widget of the push button. Defaults to None.
         """ 
 
+
         super().__init__(parent)
 
-        if text is not None: self.setText(text)
-        self.setFixedSize(QSize(*size))
+        if font is not None: self.setFont(font)
 
-        self.setObjectName("radio-button")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
-            __file__, "styles/radio_button.css", 
-            name="RadioButton", obj_name="QRadioButton#radio-button",
+            __file__, "styles/button.css", 
+            name="PushButton", obj_name="QPushButton#button",
             stylesheet=stylesheet
         ))
+        
+        self.setObjectName("button")
+        self.setMinimumSize(QSize(*size))
+
+        if text is not None:
+            self.setText(text)
+        
+        if stylesheet is not None:
+            self.setStyleSheet(self.styleSheet() + stylesheet)
```

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/styles/check_box.css` & `qtharmony-0.1.5/qtharmony/widgets/basic/styles/check_box.css`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.1.5/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.4/PKG-INFO` & `qtharmony-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.4
+Version: 0.1.5
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

