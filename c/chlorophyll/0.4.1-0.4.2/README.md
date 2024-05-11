# Comparing `tmp/chlorophyll-0.4.1.tar.gz` & `tmp/chlorophyll-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chlorophyll-0.4.1.tar", last modified: Wed Jul 12 15:40:09 2023, max compression
+gzip compressed data, was "chlorophyll-0.4.2.tar", last modified: Sat May 11 14:21:41 2024, max compression
```

## Comparing `chlorophyll-0.4.1.tar` & `chlorophyll-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/chlorophyll/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/codeview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/chlorophyll/colorschemes/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-dark.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-light.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/dracula.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/mariana.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/colorschemes/monokai.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/chlorophyll/schemeparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/chlorophyll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 15:40:09.000000 chlorophyll-0.4.1/chlorophyll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:40:09.130279 chlorophyll-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-12 15:39:58.000000 chlorophyll-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:21:41.070162 chlorophyll-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-11 14:21:41.070162 chlorophyll-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:21:41.070162 chlorophyll-0.4.2/chlorophyll/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/codeview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:21:41.070162 chlorophyll-0.4.2/chlorophyll/colorschemes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/colorschemes/ayu-dark.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/colorschemes/ayu-light.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/colorschemes/dracula.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/colorschemes/mariana.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/colorschemes/monokai.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/chlorophyll/schemeparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 14:21:41.070162 chlorophyll-0.4.2/chlorophyll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-11 14:21:40.000000 chlorophyll-0.4.2/chlorophyll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-11 14:21:41.000000 chlorophyll-0.4.2/chlorophyll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 14:21:40.000000 chlorophyll-0.4.2/chlorophyll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 14:21:40.000000 chlorophyll-0.4.2/chlorophyll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 14:21:40.000000 chlorophyll-0.4.2/chlorophyll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 14:21:41.070162 chlorophyll-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-11 14:21:28.000000 chlorophyll-0.4.2/setup.py
```

### Comparing `chlorophyll-0.4.1/LICENSE` & `chlorophyll-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/PKG-INFO` & `chlorophyll-0.4.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.4.1
+Version: 0.4.2
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
-Home-page: https://gitlab.com/rdbende/chlorophyll
+Home-page: https://github.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,29 +26,40 @@
 
 > **Note**
 > This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it any more.
 
 ## Description
 Chlorophyll provides the `CodeView` widget for tkinter, which is a `Text` widget with syntax highlighting, line numbers, and works as a simple code editor. It is written in Python and uses the [`pygments`](https://pygments.org/) library for syntax highlighting and the [`TkLineNums`](https://www.github.com/Moosems/TkLineNums) module for line numbers.
 
-
 ## Installation
-
 `pip install chlorophyll`
 
+## Development install
+First, fork the repo, then run these commands in your terminal
+```console
+git clone https://github.com/your-username/chlorophyll
+cd chlorophyll
+python3 -m venv env
+source env/bin/activate
+pip install -e .
+```
+
 # Documentation
 
 ### `CodeView` Widget
-|Options      |Description                     |Input                                         |
-|-------------|--------------------------------|----------------------------------------------|
-|master       |The parent widget               |Tkinter widget                                |
-|lexer        |The Language lexer              |Pygments lexer                                |
-|color_scheme |A color scheme for the code     |Dict, string, or toml file                    |
-|tab_width    |The width of a tab (`\t`)       |Int                                           |
-|**kwargs      |Keyword arguments for the widget|Any keyword arguments given to a `Text` widget|
+|Options             |Description                     |Input                                         |
+|--------------------|--------------------------------|----------------------------------------------|
+|master              |The parent widget               |Tkinter widget                                |
+|lexer               |The Language lexer              |Pygments lexer                                |
+|color_scheme        |A color scheme for the code     |Dict, string, or toml file                    |
+|tab_width           |The width of a tab (`\t`)       |Int                                           |
+|autohide_scrollbar  |Auto hide scrollbars            |Bool                                          |
+|linenums_border     |Border width of the line numbers|Int                                           |
+|default_context_menu|Enable context menus in CodeView|Bool                                          |
+|**kwargs            |Keyword arguments for the widget|Any keyword arguments given to a `Text` widget|
 
 #### Basic Usage:
 ```python
 from tkinter import Tk
 
 import pygments.lexers
 from chlorophyll import CodeView
@@ -57,7 +68,8 @@
 
 codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
 codeview.pack(fill="both", expand=True)
 
 root.mainloop()
 ```
 
+
```

### Comparing `chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-dark.toml` & `chlorophyll-0.4.2/chlorophyll/colorschemes/ayu-dark.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/chlorophyll/colorschemes/ayu-light.toml` & `chlorophyll-0.4.2/chlorophyll/colorschemes/ayu-light.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/chlorophyll/colorschemes/dracula.toml` & `chlorophyll-0.4.2/chlorophyll/colorschemes/dracula.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/chlorophyll/colorschemes/mariana.toml` & `chlorophyll-0.4.2/chlorophyll/colorschemes/mariana.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/chlorophyll/colorschemes/monokai.toml` & `chlorophyll-0.4.2/chlorophyll/colorschemes/monokai.toml`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/chlorophyll/schemeparser.py` & `chlorophyll-0.4.2/chlorophyll/schemeparser.py`

 * *Files identical despite different names*

### Comparing `chlorophyll-0.4.1/chlorophyll.egg-info/PKG-INFO` & `chlorophyll-0.4.2/chlorophyll.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: chlorophyll
-Version: 0.4.1
+Version: 0.4.2
 Summary: A module that fills your code with color - syntax highlighted text box widget for Tkinter.
-Home-page: https://gitlab.com/rdbende/chlorophyll
+Home-page: https://github.com/rdbende/chlorophyll
 Author: rdbende
 Author-email: rdbende@gmail.com
 License: MIT license
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -26,29 +26,40 @@
 
 > **Note**
 > This module is the successor to [`tkcode`](https://github.com/rdbende/tkcode), as it is deprecated - please do not use it any more.
 
 ## Description
 Chlorophyll provides the `CodeView` widget for tkinter, which is a `Text` widget with syntax highlighting, line numbers, and works as a simple code editor. It is written in Python and uses the [`pygments`](https://pygments.org/) library for syntax highlighting and the [`TkLineNums`](https://www.github.com/Moosems/TkLineNums) module for line numbers.
 
-
 ## Installation
-
 `pip install chlorophyll`
 
+## Development install
+First, fork the repo, then run these commands in your terminal
+```console
+git clone https://github.com/your-username/chlorophyll
+cd chlorophyll
+python3 -m venv env
+source env/bin/activate
+pip install -e .
+```
+
 # Documentation
 
 ### `CodeView` Widget
-|Options      |Description                     |Input                                         |
-|-------------|--------------------------------|----------------------------------------------|
-|master       |The parent widget               |Tkinter widget                                |
-|lexer        |The Language lexer              |Pygments lexer                                |
-|color_scheme |A color scheme for the code     |Dict, string, or toml file                    |
-|tab_width    |The width of a tab (`\t`)       |Int                                           |
-|**kwargs      |Keyword arguments for the widget|Any keyword arguments given to a `Text` widget|
+|Options             |Description                     |Input                                         |
+|--------------------|--------------------------------|----------------------------------------------|
+|master              |The parent widget               |Tkinter widget                                |
+|lexer               |The Language lexer              |Pygments lexer                                |
+|color_scheme        |A color scheme for the code     |Dict, string, or toml file                    |
+|tab_width           |The width of a tab (`\t`)       |Int                                           |
+|autohide_scrollbar  |Auto hide scrollbars            |Bool                                          |
+|linenums_border     |Border width of the line numbers|Int                                           |
+|default_context_menu|Enable context menus in CodeView|Bool                                          |
+|**kwargs            |Keyword arguments for the widget|Any keyword arguments given to a `Text` widget|
 
 #### Basic Usage:
 ```python
 from tkinter import Tk
 
 import pygments.lexers
 from chlorophyll import CodeView
@@ -57,7 +68,8 @@
 
 codeview = CodeView(root, lexer=pygments.lexers.RustLexer, color_scheme="monokai")
 codeview.pack(fill="both", expand=True)
 
 root.mainloop()
 ```
 
+
```

### Comparing `chlorophyll-0.4.1/setup.py` & `chlorophyll-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 
 setup(
     name="chlorophyll",
-    version="0.4.1",
+    version="0.4.2",
     description="A module that fills your code with color - syntax highlighted text box widget for Tkinter.",
     author="rdbende",
     author_email="rdbende@gmail.com",
-    url="https://gitlab.com/rdbende/chlorophyll",
+    url="https://github.com/rdbende/chlorophyll",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["pygments", "toml", "tklinenums", "pyperclip"],
     python_requires=">=3.7",
     license="MIT license",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

