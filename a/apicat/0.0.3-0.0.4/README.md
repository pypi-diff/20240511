# Comparing `tmp/apicat-0.0.3.tar.gz` & `tmp/apicat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicat-0.0.3.tar", max compression
+gzip compressed data, was "apicat-0.0.4.tar", max compression
```

## Comparing `apicat-0.0.3.tar` & `apicat-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      924 2024-05-11 11:35:35.261902 apicat-0.0.3/apicat/__init__.py
--rw-r--r--   0        0        0      585 2024-05-11 10:50:01.154407 apicat-0.0.3/apicat/config.py
--rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.3/apicat/core.py
--rw-r--r--   0        0        0      413 2024-05-11 11:46:26.266138 apicat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.3/README.md
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 apicat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      924 2024-05-11 12:53:55.687247 apicat-0.0.4/apicat/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-11 12:54:32.274728 apicat-0.0.4/apicat/config.py
+-rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.4/apicat/core.py
+-rw-r--r--   0        0        0      413 2024-05-11 12:53:20.588642 apicat-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.4/README.md
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 apicat-0.0.4/PKG-INFO
```

### Comparing `apicat-0.0.3/apicat/__init__.py` & `apicat-0.0.4/apicat/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 def docs():
     plugin_docs = {}
     for blueprint_name in app.blueprints:
         if blueprint_name.startswith('plugin'):
             blueprint = app.blueprints[blueprint_name]
             plugin_docs[blueprint_name] = blueprint.get('docs', '')
     
-    combined_html = ''
+    combined_html = '<h1>欢迎使用 ApiCat 🎉</h1>'
     for plugin_name, docs_content in plugin_docs.items():
-        combined_html += f'<h1>欢迎使用 ApiCat 🎉</h1><div>{plugin_name}\n{docs_content}</div>'
+        combined_html += f'<div>{plugin_name}\n{docs_content}</div>'
     return render_template_string(combined_html)
 
 def start(plugin_list: list):
     log.info("欢迎使用 ApiCat🎉")
     log.info("开发团队: 星海码队")
     log.info("项目地址: https://github.com/xinghai-osc/apicat")
     core.register_plugins(plugin_list,app)
```

### Comparing `apicat-0.0.3/apicat/core.py` & `apicat-0.0.4/apicat/core.py`

 * *Files identical despite different names*

### Comparing `apicat-0.0.3/PKG-INFO` & `apicat-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apicat
-Version: 0.0.3
+Version: 0.0.4
 Summary: ApiCat 是一个API框架，它能帮助站长快速部署各种API。
 Author: Yeying-Xingchen
 Author-email: yeyingxingchen@yeah.net
 Requires-Python: >=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flask (>=2.3.2)
```

