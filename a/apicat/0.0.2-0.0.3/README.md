# Comparing `tmp/apicat-0.0.2.tar.gz` & `tmp/apicat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicat-0.0.2.tar", max compression
+gzip compressed data, was "apicat-0.0.3.tar", max compression
```

## Comparing `apicat-0.0.2.tar` & `apicat-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      924 2024-05-11 11:35:35.261902 apicat-0.0.2/apicat/__init__.py
--rw-r--r--   0        0        0      585 2024-05-11 10:50:01.154407 apicat-0.0.2/apicat/config.py
--rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.2/apicat/core.py
--rw-r--r--   0        0        0      409 2024-05-11 10:47:12.418376 apicat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.2/README.md
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 apicat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      924 2024-05-11 11:35:35.261902 apicat-0.0.3/apicat/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-11 10:50:01.154407 apicat-0.0.3/apicat/config.py
+-rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.3/apicat/core.py
+-rw-r--r--   0        0        0      413 2024-05-11 11:46:26.266138 apicat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.3/README.md
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 apicat-0.0.3/PKG-INFO
```

### Comparing `apicat-0.0.2/apicat/__init__.py` & `apicat-0.0.3/apicat/__init__.py`

 * *Files identical despite different names*

### Comparing `apicat-0.0.2/apicat/config.py` & `apicat-0.0.3/apicat/config.py`

 * *Files identical despite different names*

### Comparing `apicat-0.0.2/apicat/core.py` & `apicat-0.0.3/apicat/core.py`

 * *Files identical despite different names*

### Comparing `apicat-0.0.2/PKG-INFO` & `apicat-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: apicat
-Version: 0.0.2
+Version: 0.0.3
 Summary: ApiCat 是一个API框架，它能帮助站长快速部署各种API。
 Author: Yeying-Xingchen
 Author-email: yeyingxingchen@yeah.net
-Requires-Python: >=3.13,<4.0
+Requires-Python: >=3.12
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: flask (>=2.3.2,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: xhlog (>=0.0.1,<0.0.2)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: flask (>=2.3.2)
+Requires-Dist: toml (>=0.10.2)
+Requires-Dist: xhlog (>=0.0.1)
 Description-Content-Type: text/markdown
 
 # ApiCat
 ![GitHub stars](https://img.shields.io/github/stars/xinghai-osc/apicat?style=social.svg?style=social&label=Star)  
 ## 简介
 ApiCat 是一个API框架，它能帮助站长快速部署各种API。
```

