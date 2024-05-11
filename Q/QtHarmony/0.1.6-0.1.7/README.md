# Comparing `tmp/qtharmony-0.1.6.tar.gz` & `tmp/qtharmony-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.6.tar", max compression
+gzip compressed data, was "qtharmony-0.1.7.tar", max compression
```

## Comparing `qtharmony-0.1.6.tar` & `qtharmony-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.6/LICENSE
--rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.6/README.md
--rw-r--r--   0        0        0      609 2024-05-11 14:30:36.296317 qtharmony-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      552 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.6/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0     1545 2024-05-11 14:29:14.506368 qtharmony-0.1.6/qtharmony/resources/themes/dark-default.json
--rw-r--r--   0        0        0        0 2024-05-11 14:21:59.267556 qtharmony-0.1.6/qtharmony/resources/themes/light-default.json
--rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.6/qtharmony/src/config/__init__.py
--rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.6/qtharmony/src/config/config.py
--rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.6/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.6/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.6/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.6/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      876 2024-05-11 14:21:59.267556 qtharmony-0.1.6/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      965 2024-05-11 13:53:23.349703 qtharmony-0.1.6/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.6/qtharmony/src/core/theme/__init__.py
--rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.6/qtharmony/src/core/theme/theme_builder.py
--rw-r--r--   0        0        0     1914 2024-05-11 14:29:52.341470 qtharmony-0.1.6/qtharmony/src/core/theme/theme_manager.py
--rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.6/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     2318 2024-05-11 14:21:59.267556 qtharmony-0.1.6/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0     2556 2024-05-11 08:05:32.046997 qtharmony-0.1.6/qtharmony/widgets/basic/check_box.py
--rw-r--r--   0        0        0     2406 2024-05-11 07:50:41.511507 qtharmony-0.1.6/qtharmony/widgets/basic/digital_entry.py
--rw-r--r--   0        0        0     3478 2024-05-11 14:29:14.506368 qtharmony-0.1.6/qtharmony/widgets/basic/drop_down_menu.py
--rw-r--r--   0        0        0     2492 2024-05-11 14:29:14.506368 qtharmony-0.1.6/qtharmony/widgets/basic/entry.py
--rw-r--r--   0        0        0     1518 2024-05-11 07:50:41.511507 qtharmony-0.1.6/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.6/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0     3737 2024-05-11 07:50:41.511507 qtharmony-0.1.6/qtharmony/widgets/basic/path_entry.py
--rw-r--r--   0        0        0     1835 2024-05-11 08:08:22.630008 qtharmony-0.1.6/qtharmony/widgets/basic/radio_button.py
--rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.6/qtharmony/widgets/basic/splitter.py
--rw-r--r--   0        0        0       68 2024-05-11 14:29:14.506368 qtharmony-0.1.6/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      521 2024-05-11 06:45:00.352043 qtharmony-0.1.6/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      293 2024-05-11 05:40:26.232885 qtharmony-0.1.6/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.6/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.6/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.6/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.6/qtharmony/widgets/basic/styles/label.css
--rw-r--r--   0        0        0      265 2024-05-11 14:05:25.939050 qtharmony-0.1.6/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.6/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.6/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.6/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-11 14:29:14.509702 qtharmony-0.1.6/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.6/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1981 2024-05-11 08:16:36.349414 qtharmony-0.1.7/README.md
+-rw-r--r--   0        0        0      609 2024-05-11 14:57:35.851311 qtharmony-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        2 2024-05-11 08:08:22.630008 qtharmony-0.1.7/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0     2883 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/resources/themes/dark-default.json
+-rw-r--r--   0        0        0        0 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/resources/themes/light-default.json
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0       22 2024-05-11 08:08:22.630008 qtharmony-0.1.7/qtharmony/src/config/__init__.py
+-rw-r--r--   0        0        0      233 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/src/config/config.py
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.7/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.7/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.7/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.7/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      876 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      965 2024-05-11 13:53:23.349703 qtharmony-0.1.7/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       80 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/src/core/theme/__init__.py
+-rw-r--r--   0        0        0     1299 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/src/core/theme/theme_builder.py
+-rw-r--r--   0        0        0     1914 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/src/core/theme/theme_manager.py
+-rw-r--r--   0        0        0      433 2024-05-11 08:23:35.711704 qtharmony-0.1.7/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     2318 2024-05-11 14:21:59.267556 qtharmony-0.1.7/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0     2645 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/check_box.py
+-rw-r--r--   0        0        0     2495 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/digital_entry.py
+-rw-r--r--   0        0        0     3478 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/widgets/basic/drop_down_menu.py
+-rw-r--r--   0        0        0     2492 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/widgets/basic/entry.py
+-rw-r--r--   0        0        0     1518 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     3329 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0     3737 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/path_entry.py
+-rw-r--r--   0        0        0     1924 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/radio_button.py
+-rw-r--r--   0        0        0     1906 2024-05-11 07:50:41.511507 qtharmony-0.1.7/qtharmony/widgets/basic/splitter.py
+-rw-r--r--   0        0        0       68 2024-05-11 14:29:14.506368 qtharmony-0.1.7/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      115 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0       63 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      139 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0       56 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      153 2024-05-11 06:45:00.352043 qtharmony-0.1.7/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:45:00.352043 qtharmony-0.1.7/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0       67 2024-05-11 14:57:15.152216 qtharmony-0.1.7/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.7/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.7/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.7/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:29:14.509702 qtharmony-0.1.7/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 qtharmony-0.1.7/PKG-INFO
```

### Comparing `qtharmony-0.1.6/LICENSE` & `qtharmony-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/README.md` & `qtharmony-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/pyproject.toml` & `qtharmony-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.6"
+version = "0.1.7"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.6/qtharmony/constructor/initialize.py` & `qtharmony-0.1.7/qtharmony/constructor/initialize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from PySide6.QtWidgets import QApplication
 
 from typing import Optional
 from qtharmony.src.core.exceptions import NotInitializedError
+from qtharmony.src.core.theme import ThemeManager
 
 
 class Initialization:
 
     application: Optional[QApplication] = None
 
     @classmethod
     def init(cls, argv: list[str]) -> None:
         cls.application = QApplication(argv)
     
     @classmethod
     def exec(cls) -> None:
         if cls.application is not None:
+            ThemeManager.update()
             cls.application.exec()
         
         else:
             raise NotInitializedError("Intialize application use: 'Initialization.init()'")
```

### Comparing `qtharmony-0.1.6/qtharmony/resources/themes/dark-default.json` & `qtharmony-0.1.7/qtharmony/resources/themes/dark-default.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'CheckBox'": "OrderedDict([('object-name', 'QCheckBox#check-box'), (':active', "*

 * *               "OrderedDict([('color', '#ffffff')])), ('::indicator', OrderedDict([('border', '1px "*

 * *               "solid #0166fc'), ('border-radius', '3px')])), ('::indicator:checked:enabled', "*

 * *               "OrderedDict([('background-color', '#0166fc')])), ('::indicator:checked:disabled', "*

 * *               "OrderedDict([('background-color', 'lightgray')])), (':disabled', "*

 * *               "OrderedDict([('color', 'gray')])) […]*

```diff
@@ -1,8 +1,45 @@
 {
+    "CheckBox": {
+        "::indicator": {
+            "border": "1px solid #0166fc",
+            "border-radius": "3px"
+        },
+        "::indicator:checked:disabled": {
+            "background-color": "lightgray"
+        },
+        "::indicator:checked:enabled": {
+            "background-color": "#0166fc"
+        },
+        "::indicator:disabled": {
+            "border-color": "gray"
+        },
+        ":active": {
+            "color": "#ffffff"
+        },
+        ":disabled": {
+            "color": "gray"
+        },
+        "object-name": "QCheckBox#check-box"
+    },
+    "DigitalEntry": {
+        ":active": {
+            "background-color": "#ffffff",
+            "border": "1px solid #adb5bd",
+            "border-radius": "6px",
+            "color": "#1A3B5D"
+        },
+        ":focus": {
+            "border-color": "#405cf5"
+        },
+        ":hover": {
+            "border-color": "#6185DF"
+        },
+        "object-name": "QSpinBox#digital-entry"
+    },
     "DropDownMenu": {
         " QAbstractItemView": {
             "background-color": "#ffffff"
         },
         "::drop-down": {
             "border": "none"
         },
@@ -53,9 +90,22 @@
         ":hover": {
             "background-color": "#3045B8"
         },
         ":pressed": {
             "background-color": "#283A9A"
         },
         "object-name": "QPushButton#button"
+    },
+    "RadioButton": {
+        "::indicator": {
+            "border": "1px solid #0166fc",
+            "border-radius": "7px"
+        },
+        "::indicator:checked": {
+            "background-color": "#0166fc"
+        },
+        ":active": {
+            "color": "#ffffff"
+        },
+        "object-name": "QRadioButton#radio-button"
     }
 }
```

### Comparing `qtharmony-0.1.6/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.7/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/resources/ui/Logo.png` & `qtharmony-0.1.7/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.7/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/src/core/dialog.py` & `qtharmony-0.1.7/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/src/core/font.py` & `qtharmony-0.1.7/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/src/core/load.py` & `qtharmony-0.1.7/qtharmony/src/core/load.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/src/core/stylesheet.py` & `qtharmony-0.1.7/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/src/core/theme/theme_builder.py` & `qtharmony-0.1.7/qtharmony/src/core/theme/theme_builder.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/src/core/theme/theme_manager.py` & `qtharmony-0.1.7/qtharmony/src/core/theme/theme_manager.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/check_box.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/check_box.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from PySide6.QtWidgets import QCheckBox
 from PySide6.QtCore import QSize
 
 from qtharmony.src.core import StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
 class CheckBox(QCheckBox):
@@ -40,14 +41,15 @@
             is_checked (bool, optional): Flag to set the initial checked state of the checkbox. Defaults to False.
             is_disabled (bool, optional): Flag to set the initial disabled state of the checkbox. Defaults to False.
             stylesheet (Optional[str], optional): Custom stylesheet for the checkbox widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the checkbox. Defaults to None.
         """
 
         super().__init__(parent)
+        ThemeManager.add_widgets(self)
 
         self.setFixedSize(QSize(*size))
         self.setChecked(is_checked)
         self.setCheckable(is_checkable)
         self.setDisabled(is_disabled)
 
         self.setObjectName("check-box")
```

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/digital_entry.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/digital_entry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from PySide6.QtWidgets import QSpinBox
 from PySide6.QtCore import QSize
 
 from qtharmony.src.core import StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtGui import QFont
     from PySide6.QtWidgets import QWidget
 
 
@@ -39,14 +40,15 @@
             font (Optional["QFont"], optional): The font to be used for text input. Defaults to None.
             include_buttons (bool, optional): Flag to include or exclude spin box buttons. Defaults to False.
             stylesheet (Optional[str], optional): Custom stylesheet for the spin box widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the spin box. Defaults to None.
         """
 
         super().__init__(parent)
+        ThemeManager.add_widgets(self)
 
         self.setFixedSize(QSize(*size))
         if not include_buttons: self.setButtonSymbols(QSpinBox.ButtonSymbols.NoButtons)
         if font is not None: self.setFont(font)
 
         self.setObjectName("digital-entry")
         self.setRange(*range)
```

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/drop_down_menu.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/drop_down_menu.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/entry.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/path_entry.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/path_entry.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/radio_button.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/radio_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from PySide6.QtWidgets import QRadioButton
 from PySide6.QtCore import QSize
 
 from qtharmony.src.core import StyleSheetLoader
+from qtharmony.src.core.theme import ThemeManager
 
 from typing import Optional, TYPE_CHECKING
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
 class RadioButton(QRadioButton):
@@ -33,14 +34,15 @@
             text (Optional[str], optional): The text displayed next to the radio button. Defaults to None.
             size (tuple[int, int], optional): The size of the radio button widget (width, height). Defaults to (200, 30).
             stylesheet (Optional[str], optional): Custom stylesheet for the radio button widget. Defaults to None.
             parent (Optional["QWidget"], optional): Parent widget of the radio button. Defaults to None.
         """ 
 
         super().__init__(parent)
+        ThemeManager.add_widgets(self)
 
         if text is not None: self.setText(text)
         self.setFixedSize(QSize(*size))
 
         self.setObjectName("radio-button")
         self.setStyleSheet(StyleSheetLoader.load_stylesheet(
             __file__, "styles/radio_button.css",
```

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/splitter.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/splitter.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.1.7/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/qtharmony/windows/main_window.py` & `qtharmony-0.1.7/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.6/PKG-INFO` & `qtharmony-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.6
+Version: 0.1.7
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

