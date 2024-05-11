# Comparing `tmp/qtharmony-0.1.1.tar.gz` & `tmp/qtharmony-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.1.tar", max compression
+gzip compressed data, was "qtharmony-0.1.2.tar", max compression
```

## Comparing `qtharmony-0.1.1.tar` & `qtharmony-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.1/LICENSE
--rw-r--r--   0        0        0     1306 2024-05-11 05:39:27.964921 qtharmony-0.1.1/README.md
--rw-r--r--   0        0        0      609 2024-05-11 05:37:57.224772 qtharmony-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:29:31.059687 qtharmony-0.1.1/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-10 16:49:32.417643 qtharmony-0.1.1/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      552 2024-05-11 05:27:18.508019 qtharmony-0.1.1/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        0 2024-05-10 17:57:00.227375 qtharmony-0.1.1/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0    31042 2024-05-11 05:17:28.446106 qtharmony-0.1.1/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17484 2024-05-11 05:35:28.670029 qtharmony-0.1.1/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-10 17:57:00.227375 qtharmony-0.1.1/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      120 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      589 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       22 2024-05-10 17:57:00.227375 qtharmony-0.1.1/qtharmony/src/util/__init__.py
--rw-r--r--   0        0        0      125 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/src/util/config.py
--rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     1167 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0      809 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0      993 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      293 2024-05-10 18:26:23.539161 qtharmony-0.1.1/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      474 2024-05-10 18:26:23.539161 qtharmony-0.1.1/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     9395 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-11 05:27:18.644681 qtharmony-0.1.1/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-10 16:49:32.417643 qtharmony-0.1.1/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     1269 2024-05-11 05:36:37.654247 qtharmony-0.1.1/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0       58 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1306 2024-05-11 05:40:26.226219 qtharmony-0.1.2/README.md
+-rw-r--r--   0        0        0      609 2024-05-11 06:44:25.996882 qtharmony-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        0 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0    31042 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      120 2024-05-11 05:40:26.229552 qtharmony-0.1.2/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      922 2024-05-11 06:43:10.750191 qtharmony-0.1.2/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       22 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/src/util/__init__.py
+-rw-r--r--   0        0        0      125 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/src/util/config.py
+-rw-r--r--   0        0        0      269 2024-05-11 06:16:36.984815 qtharmony-0.1.2/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0      809 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0     1395 2024-05-11 06:43:59.931360 qtharmony-0.1.2/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0      278 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      521 2024-05-11 06:33:15.150636 qtharmony-0.1.2/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      293 2024-05-11 05:40:26.232885 qtharmony-0.1.2/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      474 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      153 2024-05-11 06:33:03.971169 qtharmony-0.1.2/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0       35 2024-05-11 06:40:07.225009 qtharmony-0.1.2/qtharmony/widgets/basic/styles/label.css
+-rw-r--r--   0        0        0      265 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     9395 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     1269 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0       58 2024-05-11 05:40:26.236219 qtharmony-0.1.2/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.2/PKG-INFO
```

### Comparing `qtharmony-0.1.1/LICENSE` & `qtharmony-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/README.md` & `qtharmony-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/pyproject.toml` & `qtharmony-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.1"
+version = "0.1.2"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.1/qtharmony/constructor/initialize.py` & `qtharmony-0.1.2/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.2/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/resources/ui/Logo.png` & `qtharmony-0.1.2/qtharmony/resources/ui/Logo.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.2/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/src/core/dialog.py` & `qtharmony-0.1.2/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/src/core/font.py` & `qtharmony-0.1.2/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/src/core/stylesheet.py` & `qtharmony-0.1.2/qtharmony/src/core/stylesheet.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,7 +17,20 @@
         if stylesheet is not None:
             return (
                 Loader.load_file(stylesheet_path) + "\n" 
                 + stylesheet.replace(name, obj_name)
             )
         else:
             return Loader.load_file(stylesheet_path)
+    
+    @staticmethod
+    def append_stylesheet(
+        default_stylesheet: str,
+        *additional: str,
+        name: str, obj_name: str
+    ) -> str:
+        result = default_stylesheet
+
+        for stylesheet in additional:
+            result += "\n" + stylesheet.replace(name, obj_name) + "\n"
+        
+        return result
```

### Comparing `qtharmony-0.1.1/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.2/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.2/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.2/qtharmony/widgets/basic/label.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PySide6.QtWidgets import QLabel
 
-from qtharmony.src.core import Font
+from qtharmony.src.core import Font, StyleSheetLoader
 
 from typing import Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from PySide6.QtWidgets import QWidget
 
 
@@ -21,13 +21,26 @@
             *,
             stylesheet: Optional[str] = None,
             parent: Optional["QWidget"] = None
     ) -> None:
         super().__init__(parent)
 
         self.setObjectName("label")
+        self.setStyleSheet(StyleSheetLoader.load_stylesheet(
+            __file__, "styles/label.css", 
+            name="Label", obj_name="QLabel#label",
+            stylesheet=stylesheet
+        ))
 
         self.setText(text)
-        self.setStyleSheet("QLabel#label {" f"color: {color}" + "}")
-        if stylesheet is not None: self.setStyleSheet(self.styleSheet() + "\n" + stylesheet.replace("Label", "QLabel#label"))
+        self.set_color(color)
+        
         self.setWordWrap(word_wrap)
         self.setFont(Font.get_system_font(font_family, font_size, bold, italic))
+    
+    def set_color(self, color: str) -> None:
+        self.__append_stylesheet("Label {" + f"color: {color}" + "}")
+    
+    def __append_stylesheet(self, stylesheet: str) -> None:
+        self.setStyleSheet(StyleSheetLoader.append_stylesheet(
+            self.styleSheet(), stylesheet, name="Label", obj_name="QLabel#label"
+        ))
```

### Comparing `qtharmony-0.1.1/qtharmony/widgets/basic/switchers.py` & `qtharmony-0.1.2/qtharmony/widgets/basic/switchers.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.1.2/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/qtharmony/windows/main_window.py` & `qtharmony-0.1.2/qtharmony/windows/main_window.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.1/PKG-INFO` & `qtharmony-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.1
+Version: 0.1.2
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

