# Comparing `tmp/sphinxcontrib.asciinema-0.4.1.tar.gz` & `tmp/sphinxcontrib.asciinema-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib.asciinema-0.4.1.tar", last modified: Fri Mar  8 00:38:39 2024, max compression
+gzip compressed data, was "sphinxcontrib.asciinema-0.4.2.tar", last modified: Sat May 11 03:01:30 2024, max compression
```

## Comparing `sphinxcontrib.asciinema-0.4.1.tar` & `sphinxcontrib.asciinema-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/
--rw-r--r--   0 divisor   (1000) root         (0)     1066 2023-04-14 17:27:50.000000 sphinxcontrib.asciinema-0.4.1/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)       76 2021-03-25 09:15:31.000000 sphinxcontrib.asciinema-0.4.1/MANIFEST.in
--rw-r--r--   0 divisor   (1000) root         (0)     1776 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)     1253 2021-03-25 09:15:31.000000 sphinxcontrib.asciinema-0.4.1/README.md
--rw-r--r--   0 divisor   (1000) root         (0)       38 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1036 2024-03-08 00:37:39.000000 sphinxcontrib.asciinema-0.4.1/setup.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/
--rw-r--r--   0 divisor   (1000) root         (0)       56 2024-03-08 00:37:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/
--rw-r--r--   0 divisor   (1000) root         (0)      668 2024-03-08 00:37:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/__init__.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/_static/
--rw-r--r--   0 divisor   (1000) root         (0)    53739 2023-12-29 22:11:36.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.css
--rw-r--r--   0 divisor   (1000) root         (0)   158715 2023-12-29 22:11:36.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.js
--rw-r--r--   0 divisor   (1000) root         (0)     4514 2024-03-08 00:37:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/asciinema.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-03-08 00:38:39.204987 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)     1776 2024-03-08 00:38:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      544 2024-03-08 00:38:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2024-03-08 00:38:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)       14 2024-03-08 00:38:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/namespace_packages.txt
--rw-r--r--   0 divisor   (1000) root         (0)        7 2024-03-08 00:38:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       14 2024-03-08 00:38:39.000000 sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/top_level.txt
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-11 03:01:30.848366 sphinxcontrib.asciinema-0.4.2/
+-rw-r--r--   0 divisor   (1000) root         (0)     1066 2023-04-14 17:27:50.000000 sphinxcontrib.asciinema-0.4.2/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)       76 2021-03-25 09:15:31.000000 sphinxcontrib.asciinema-0.4.2/MANIFEST.in
+-rw-r--r--   0 divisor   (1000) root         (0)     1776 2024-05-11 03:01:30.848366 sphinxcontrib.asciinema-0.4.2/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)     1253 2021-03-25 09:15:31.000000 sphinxcontrib.asciinema-0.4.2/README.md
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2024-05-11 03:01:30.848366 sphinxcontrib.asciinema-0.4.2/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1036 2024-05-11 03:00:50.000000 sphinxcontrib.asciinema-0.4.2/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-11 03:01:30.844365 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/
+-rw-r--r--   0 divisor   (1000) root         (0)       56 2024-05-11 03:00:50.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-11 03:01:30.848366 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/
+-rw-r--r--   0 divisor   (1000) root         (0)      668 2024-05-11 03:00:50.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/__init__.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-11 03:01:30.848366 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/_static/
+-rw-r--r--   0 divisor   (1000) root         (0)    53739 2023-12-29 22:11:36.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.css
+-rw-r--r--   0 divisor   (1000) root         (0)   158715 2023-12-29 22:11:36.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.js
+-rw-r--r--   0 divisor   (1000) root         (0)     4758 2024-05-11 03:00:50.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/asciinema.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2024-05-11 03:01:30.848366 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)     1776 2024-05-11 03:01:30.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      544 2024-05-11 03:01:30.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2024-05-11 03:01:30.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       14 2024-05-11 03:01:30.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/namespace_packages.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        7 2024-05-11 03:01:30.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       14 2024-05-11 03:01:30.000000 sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/top_level.txt
```

### Comparing `sphinxcontrib.asciinema-0.4.1/LICENSE` & `sphinxcontrib.asciinema-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib.asciinema-0.4.1/PKG-INFO` & `sphinxcontrib.asciinema-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib.asciinema
-Version: 0.4.1
+Version: 0.4.2
 Summary: Embed asciinema casts in your Sphinx docs
 Home-page: https://github.com/divi255/sphinxcontrib.asciinema
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sphinxcontrib.asciinema-0.4.1/README.md` & `sphinxcontrib.asciinema-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib.asciinema-0.4.1/setup.py` & `sphinxcontrib.asciinema-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/__init__.py` & `sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __copyright__ = 'Copyright (C) 2023'
 __license__ = 'MIT'
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 def setup(app):
     from .asciinema import Asciinema, ASCIINemaDirective
     from .asciinema import copy_asset_files, _NODE_VISITORS
 
     app.add_config_value('sphinxcontrib_asciinema_defaults', {}, 'html')
```

### Comparing `sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.css` & `sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.js` & `sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/_static/asciinema-player_3.6.3.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib.asciinema-0.4.1/sphinxcontrib/asciinema/asciinema.py` & `sphinxcontrib.asciinema-0.4.2/sphinxcontrib/asciinema/asciinema.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,39 +25,43 @@
 def visit_html(self, node):
     rst_to_js_option_names: dict[str, str] = {
         "terminalfontsize": "terminalFontSize",
         "terminallineheigth": "terminalLineHeigth",
         "terminalfontfamily": "terminalFontFamily",
     }
 
+    options_raw = ['markers']
+
     gen = ((rst_option_name, js_option_name)
            for (rst_option_name,
                 js_option_name) in rst_to_js_option_names.items()
            if rst_option_name in node["options"])
     for rst_option_name, js_option_name in gen:
         node["options"][js_option_name] = node["options"].pop(rst_option_name)
 
     if node['type'] == 'local':
-        template = """<div id="asciicast-{src}"></div>
+        template = """<div id="asciicast-{id}"></div>
             <script>
                 AsciinemaPlayer.create(
                     "data:text/plain;base64,{src}",
-                    document.getElementById('asciicast-{src}'),
+                    document.getElementById('asciicast-{id}'),
                     {{{options} }});
             </script>"""
         option_template = '{}: "{}", '
+        option_template_raw = '{}: {}, '
     else:
         template = """<script async id="asciicast-{src}" {options}
                 src="https://asciinema.org/a/{src}.js"></script>"""
         option_template = 'data-{}="{}" '
-    src = node["content"]
+        option_template_raw = 'data-{}="{}" '
     options = ""
     for n, v in node["options"].items():
-        options += option_template.format(n, v)
-    tag = template.format(options=options, src=src)
+        options += option_template_raw.format(
+            n, v) if n in options_raw else option_template.format(n, v)
+    tag = template.format(options=options, src=node["content"], id=node["id"])
     self.body.append(tag)
 
 
 def visit_unsupported(self, node):
     logger.warning('asciinema: unsupported output format (node skipped)')
     raise nodes.SkipNode
 
@@ -100,17 +104,19 @@
         path = options.get('path', '')
         if path and not path.endswith('/'):
             path += '/'
         fname = arg if arg.startswith('./') else path + arg
         if self.is_file(fname):
             kw['content'] = self.to_b64(fname)
             kw['type'] = 'local'
+            kw['id'] = fname
             logger.debug('asciinema: added cast file %s' % fname)
         else:
             kw['content'] = arg
+            kw['id'] = arg
             kw['type'] = 'remote'
             logger.debug('asciinema: added cast id %s' % arg)
         if 'path' in kw['options']:
             del kw['options']['path']
         return [Asciinema(**kw)]
 
     def is_file(self, rel_file):
```

### Comparing `sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/PKG-INFO` & `sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib.asciinema
-Version: 0.4.1
+Version: 0.4.2
 Summary: Embed asciinema casts in your Sphinx docs
 Home-page: https://github.com/divi255/sphinxcontrib.asciinema
 License: MIT
 Platform: UNKNOWN
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sphinxcontrib.asciinema-0.4.1/sphinxcontrib.asciinema.egg-info/SOURCES.txt` & `sphinxcontrib.asciinema-0.4.2/sphinxcontrib.asciinema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

