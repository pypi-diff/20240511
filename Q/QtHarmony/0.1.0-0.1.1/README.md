# Comparing `tmp/qtharmony-0.1.0.tar.gz` & `tmp/qtharmony-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtharmony-0.1.0.tar", max compression
+gzip compressed data, was "qtharmony-0.1.1.tar", max compression
```

## Comparing `qtharmony-0.1.0.tar` & `qtharmony-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.0/LICENSE
--rw-r--r--   0        0        0     1306 2024-05-11 05:31:03.186281 qtharmony-0.1.0/README.md
--rw-r--r--   0        0        0      609 2024-05-11 05:31:36.315068 qtharmony-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      327 2024-05-11 05:29:31.059687 qtharmony-0.1.0/qtharmony/__init__.py
--rw-r--r--   0        0        0       38 2024-05-10 16:49:32.417643 qtharmony-0.1.0/qtharmony/constructor/__init__.py
--rw-r--r--   0        0        0      552 2024-05-11 05:27:18.508019 qtharmony-0.1.0/qtharmony/constructor/initialize.py
--rw-r--r--   0        0        0        0 2024-05-10 17:57:00.227375 qtharmony-0.1.0/qtharmony/resources/__init__.py
--rw-r--r--   0        0        0    31042 2024-05-11 05:17:28.446106 qtharmony-0.1.0/qtharmony/resources/ui/Icon.png
--rw-r--r--   0        0        0    17003 2024-05-11 05:17:28.426107 qtharmony-0.1.0/qtharmony/resources/ui/Logo.png
--rw-r--r--   0        0        0     5387 2024-05-10 17:57:00.227375 qtharmony-0.1.0/qtharmony/resources/ui/angle-down.png
--rw-r--r--   0        0        0      120 2024-05-10 17:10:15.186165 qtharmony-0.1.0/qtharmony/src/core/__init__.py
--rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/src/core/dialog.py
--rw-r--r--   0        0        0      151 2024-05-10 17:10:15.186165 qtharmony-0.1.0/qtharmony/src/core/exceptions.py
--rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/src/core/font.py
--rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/src/core/load.py
--rw-r--r--   0        0        0      589 2024-05-10 17:10:15.186165 qtharmony-0.1.0/qtharmony/src/core/stylesheet.py
--rw-r--r--   0        0        0       22 2024-05-10 17:57:00.227375 qtharmony-0.1.0/qtharmony/src/util/__init__.py
--rw-r--r--   0        0        0      125 2024-05-11 05:27:18.558017 qtharmony-0.1.0/qtharmony/src/util/config.py
--rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/__init__.py
--rw-r--r--   0        0        0     1167 2024-05-11 05:27:18.558017 qtharmony-0.1.0/qtharmony/widgets/basic/button.py
--rw-r--r--   0        0        0      809 2024-05-11 05:27:18.558017 qtharmony-0.1.0/qtharmony/widgets/basic/groups.py
--rw-r--r--   0        0        0      993 2024-05-11 05:27:18.558017 qtharmony-0.1.0/qtharmony/widgets/basic/label.py
--rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/basic/styles/button.css
--rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/basic/styles/check_box.css
--rw-r--r--   0        0        0      293 2024-05-10 18:26:23.539161 qtharmony-0.1.0/qtharmony/widgets/basic/styles/digital_entry.css
--rw-r--r--   0        0        0      474 2024-05-10 18:26:23.539161 qtharmony-0.1.0/qtharmony/widgets/basic/styles/drop_down_menu.css
--rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/basic/styles/entry.css
--rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/basic/styles/group_box.css
--rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/basic/styles/radio_button.css
--rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 qtharmony-0.1.0/qtharmony/widgets/basic/styles/widgets_list.css
--rw-r--r--   0        0        0     9395 2024-05-11 05:27:18.558017 qtharmony-0.1.0/qtharmony/widgets/basic/switchers.py
--rw-r--r--   0        0        0     1578 2024-05-11 05:27:18.644681 qtharmony-0.1.0/qtharmony/widgets/basic/widgets_list.py
--rw-r--r--   0        0        0       36 2024-05-10 16:49:32.417643 qtharmony-0.1.0/qtharmony/windows/__init__.py
--rw-r--r--   0        0        0     1269 2024-05-11 05:27:18.644681 qtharmony-0.1.0/qtharmony/windows/main_window.py
--rw-r--r--   0        0        0       58 2024-05-10 17:10:15.186165 qtharmony-0.1.0/qtharmony/windows/styles/main_window.css
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-02 17:11:53.147941 qtharmony-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1306 2024-05-11 05:39:27.964921 qtharmony-0.1.1/README.md
+-rw-r--r--   0        0        0      609 2024-05-11 05:37:57.224772 qtharmony-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      327 2024-05-11 05:29:31.059687 qtharmony-0.1.1/qtharmony/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 16:49:32.417643 qtharmony-0.1.1/qtharmony/constructor/__init__.py
+-rw-r--r--   0        0        0      552 2024-05-11 05:27:18.508019 qtharmony-0.1.1/qtharmony/constructor/initialize.py
+-rw-r--r--   0        0        0        0 2024-05-10 17:57:00.227375 qtharmony-0.1.1/qtharmony/resources/__init__.py
+-rw-r--r--   0        0        0    31042 2024-05-11 05:17:28.446106 qtharmony-0.1.1/qtharmony/resources/ui/Icon.png
+-rw-r--r--   0        0        0    17484 2024-05-11 05:35:28.670029 qtharmony-0.1.1/qtharmony/resources/ui/Logo.png
+-rw-r--r--   0        0        0     5387 2024-05-10 17:57:00.227375 qtharmony-0.1.1/qtharmony/resources/ui/angle-down.png
+-rw-r--r--   0        0        0      120 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/src/core/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/src/core/dialog.py
+-rw-r--r--   0        0        0      151 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/src/core/exceptions.py
+-rw-r--r--   0        0        0     2506 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/src/core/font.py
+-rw-r--r--   0        0        0      324 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/src/core/load.py
+-rw-r--r--   0        0        0      589 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/src/core/stylesheet.py
+-rw-r--r--   0        0        0       22 2024-05-10 17:57:00.227375 qtharmony-0.1.1/qtharmony/src/util/__init__.py
+-rw-r--r--   0        0        0      125 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/src/util/config.py
+-rw-r--r--   0        0        0      238 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/button.py
+-rw-r--r--   0        0        0      809 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/groups.py
+-rw-r--r--   0        0        0      993 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/label.py
+-rw-r--r--   0        0        0      278 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/button.css
+-rw-r--r--   0        0        0      501 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/check_box.css
+-rw-r--r--   0        0        0      293 2024-05-10 18:26:23.539161 qtharmony-0.1.1/qtharmony/widgets/basic/styles/digital_entry.css
+-rw-r--r--   0        0        0      474 2024-05-10 18:26:23.539161 qtharmony-0.1.1/qtharmony/widgets/basic/styles/drop_down_menu.css
+-rw-r--r--   0        0        0      286 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/entry.css
+-rw-r--r--   0        0        0      134 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/group_box.css
+-rw-r--r--   0        0        0      265 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/radio_button.css
+-rw-r--r--   0        0        0      313 2024-05-10 14:59:21.961513 qtharmony-0.1.1/qtharmony/widgets/basic/styles/widgets_list.css
+-rw-r--r--   0        0        0     9395 2024-05-11 05:27:18.558017 qtharmony-0.1.1/qtharmony/widgets/basic/switchers.py
+-rw-r--r--   0        0        0     1578 2024-05-11 05:27:18.644681 qtharmony-0.1.1/qtharmony/widgets/basic/widgets_list.py
+-rw-r--r--   0        0        0       36 2024-05-10 16:49:32.417643 qtharmony-0.1.1/qtharmony/windows/__init__.py
+-rw-r--r--   0        0        0     1269 2024-05-11 05:36:37.654247 qtharmony-0.1.1/qtharmony/windows/main_window.py
+-rw-r--r--   0        0        0       58 2024-05-10 17:10:15.186165 qtharmony-0.1.1/qtharmony/windows/styles/main_window.css
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qtharmony-0.1.1/PKG-INFO
```

### Comparing `qtharmony-0.1.0/LICENSE` & `qtharmony-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/README.md` & `qtharmony-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-    <img src="Logo.png">
+    <img src="logo.png">
 </p>
 <h1></h1>
 
 <p align="center">
 
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/QtHarmony">
   <img src="https://img.shields.io/github/license/chebupelka8/QtHarmony">
```

### Comparing `qtharmony-0.1.0/pyproject.toml` & `qtharmony-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "QtHarmony"
-version = "0.1.0"
+version = "0.1.1"
 description = "QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development."
 authors = ["chebupelka8 <stpzamyatin@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `qtharmony-0.1.0/qtharmony/constructor/initialize.py` & `qtharmony-0.1.1/qtharmony/constructor/initialize.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/resources/ui/Icon.png` & `qtharmony-0.1.1/qtharmony/resources/ui/Icon.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/resources/ui/angle-down.png` & `qtharmony-0.1.1/qtharmony/resources/ui/angle-down.png`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/src/core/dialog.py` & `qtharmony-0.1.1/qtharmony/src/core/dialog.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/src/core/font.py` & `qtharmony-0.1.1/qtharmony/src/core/font.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/src/core/stylesheet.py` & `qtharmony-0.1.1/qtharmony/src/core/stylesheet.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/widgets/basic/button.py` & `qtharmony-0.1.1/qtharmony/widgets/basic/button.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/widgets/basic/groups.py` & `qtharmony-0.1.1/qtharmony/widgets/basic/groups.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/widgets/basic/label.py` & `qtharmony-0.1.1/qtharmony/widgets/basic/label.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/widgets/basic/switchers.py` & `qtharmony-0.1.1/qtharmony/widgets/basic/switchers.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/widgets/basic/widgets_list.py` & `qtharmony-0.1.1/qtharmony/widgets/basic/widgets_list.py`

 * *Files identical despite different names*

### Comparing `qtharmony-0.1.0/qtharmony/windows/main_window.py` & `qtharmony-0.1.1/qtharmony/windows/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,13 +29,13 @@
             __file__, "styles/main_window.css", 
             name="MainWindow", obj_name="QMainWindow#main-window",
             stylesheet=stylesheet
         ))
 
         self.resize(*size)
         if title is not None: self.setWindowTitle(title)
-        else: self.setWindowTitle("ModernQQt")
+        else: self.setWindowTitle("QtHarmony")
 
         if not is_resizable: self.setFixedSize(*size)
     
     def run(self) -> None:
         self.show()
```

### Comparing `qtharmony-0.1.0/PKG-INFO` & `qtharmony-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: QtHarmony
-Version: 0.1.0
+Version: 0.1.1
 Summary: QtHarmony - is a Cutting-Edge GUI Library Built on PyQt6 QtHarmony is a intuitive graphical user interface (GUI) library designed to simplify the development of modern, visually stunning, and highly functional applications. Built on the robust foundation of PyQt6. Now QtHarmony is in development.
 License: MIT
 Author: chebupelka8
 Author-email: stpzamyatin@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pyside6 (>=6.7.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-    <img src="Logo.png">
+    <img src="logo.png">
 </p>
 <h1></h1>
 
 <p align="center">
 
   <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/QtHarmony">
   <img src="https://img.shields.io/github/license/chebupelka8/QtHarmony">
```

