# Comparing `tmp/poetry_moment-0.0.3.tar.gz` & `tmp/poetry_moment-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_moment-0.0.3.tar", max compression
+gzip compressed data, was "poetry_moment-0.0.4.tar", max compression
```

## Comparing `poetry_moment-0.0.3.tar` & `poetry_moment-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1425 2024-05-11 11:32:56.509771 poetry_moment-0.0.3/poetry_moment/__init__.py
--rw-r--r--   0        0        0     2115 2024-05-11 11:32:30.632663 poetry_moment-0.0.3/poetry_moment/core.py
--rw-r--r--   0        0        0      354 2024-05-11 11:45:57.285583 poetry_moment-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.3/README.md
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 poetry_moment-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1383 2024-05-11 12:52:21.979244 poetry_moment-0.0.4/poetry_moment/__init__.py
+-rw-r--r--   0        0        0     2127 2024-05-11 12:26:28.391307 poetry_moment-0.0.4/poetry_moment/core.py
+-rw-r--r--   0        0        0      354 2024-05-11 12:52:55.829127 poetry_moment-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.4/README.md
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 poetry_moment-0.0.4/PKG-INFO
```

### Comparing `poetry_moment-0.0.3/poetry_moment/__init__.py` & `poetry_moment-0.0.4/poetry_moment/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from flask import Blueprint, render_template_string, request, jsonify
 from . import core
 import xhlog as log
 
 # 定义蓝图
-poetry_moment_blueprint = Blueprint('poetry_moment', __name__, url_prefix='/poetry-moment')
+blueprint = Blueprint('poetry_moment', __name__, url_prefix='/poetry-moment')
 
 # 插件的文档内容
-poetry_moment_blueprint.docs = """
+blueprint.docs = """
 <h2>诗歌时刻</h2>
 <p>让诗意，流露此刻。诗歌时刻是一款开源的API软件。他能帮助开发者简单快速的在网站/应用中嵌入诗歌。</p>
 """
 
-main = poetry_moment_blueprint
+main = blueprint
 
 @main.route('/')
 def index():
     return "欢迎使用诗歌时刻！"
 
 @main.route('/get/<poetry_type>')
 def get_poetry(poetry_type):
```

### Comparing `poetry_moment-0.0.3/poetry_moment/core.py` & `poetry_moment-0.0.4/poetry_moment/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from apicat import config
 import os
 import json
 import random
 import time
 
 plugin_name = 'poetry_moment'
-directory = config.get_plugin_cfg(plugin_name)
+directory = config.get_plugin_cfg(plugin_name,"directory")
 
 def get():
     # 获取该目录下所有文件的列表
     json_files = [file for file in os.listdir(directory) if file.endswith('.json')]
     # 随机选择一个语录文件
     discourse_file = random.choice(json_files)
     # 打开并读取所选文件的内容，将其解析为JSON对象
```

### Comparing `poetry_moment-0.0.3/PKG-INFO` & `poetry_moment-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-moment
-Version: 0.0.3
+Version: 0.0.4
 Summary: [诗歌时刻]让诗意，流露此刻。
 Author: Yeying-Xingchen
 Author-email: yeyingxingchen@yeah.net
 Requires-Python: >=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: apicat (>=0.0.2)
```

