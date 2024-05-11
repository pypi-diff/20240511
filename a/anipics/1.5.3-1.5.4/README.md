# Comparing `tmp/anipics-1.5.3.tar.gz` & `tmp/anipics-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipics-1.5.3.tar", max compression
+gzip compressed data, was "anipics-1.5.4.tar", max compression
```

## Comparing `anipics-1.5.3.tar` & `anipics-1.5.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0    34519 2024-01-20 19:04:25.749725 anipics-1.5.3/LICENSE
--rw-r--r--   0        0        0      728 2024-05-10 20:21:07.857078 anipics-1.5.3/README.md
--rw-r--r--   0        0        0      297 2024-05-07 15:43:31.902097 anipics-1.5.3/anipics/__init__.py
--rw-r--r--   0        0        0      179 2024-01-21 16:19:12.732175 anipics-1.5.3/anipics/models.py
--rw-r--r--   0        0        0      238 2024-01-21 16:19:12.734175 anipics-1.5.3/anipics/services/__init__.py
--rw-r--r--   0        0        0     1060 2024-05-06 18:31:41.106238 anipics-1.5.3/anipics/services/animepicsx.py
--rw-r--r--   0        0        0     2036 2024-05-06 18:31:41.143237 anipics-1.5.3/anipics/services/nekoslife.py
--rw-r--r--   0        0        0     3047 2024-05-06 18:31:41.194235 anipics-1.5.3/anipics/services/waifupics.py
--rw-r--r--   0        0        0      571 2024-05-07 15:43:22.793311 anipics-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 anipics-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0    34519 2024-01-20 19:04:25.749725 anipics-1.5.4/LICENSE
+-rw-r--r--   0        0        0      728 2024-05-10 20:21:07.857078 anipics-1.5.4/README.md
+-rw-r--r--   0        0        0      317 2024-05-11 17:25:04.444376 anipics-1.5.4/anipics/__init__.py
+-rw-r--r--   0        0        0      179 2024-01-21 16:19:12.732175 anipics-1.5.4/anipics/models.py
+-rw-r--r--   0        0        0      278 2024-05-11 17:29:16.114661 anipics-1.5.4/anipics/services/__init__.py
+-rw-r--r--   0        0        0     1060 2024-05-06 18:31:41.106238 anipics-1.5.4/anipics/services/animepicsx.py
+-rw-r--r--   0        0        0     2036 2024-05-06 18:31:41.143237 anipics-1.5.4/anipics/services/nekoslife.py
+-rw-r--r--   0        0        0     5613 2024-05-11 17:19:33.670831 anipics-1.5.4/anipics/services/purrbot.py
+-rw-r--r--   0        0        0     3047 2024-05-06 18:31:41.194235 anipics-1.5.4/anipics/services/waifupics.py
+-rw-r--r--   0        0        0      571 2024-05-11 17:24:58.713506 anipics-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 anipics-1.5.4/PKG-INFO
```

### Comparing `anipics-1.5.3/LICENSE` & `anipics-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anipics-1.5.3/README.md` & `anipics-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `anipics-1.5.3/anipics/services/animepicsx.py` & `anipics-1.5.4/anipics/services/animepicsx.py`

 * *Files identical despite different names*

### Comparing `anipics-1.5.3/anipics/services/nekoslife.py` & `anipics-1.5.4/anipics/services/nekoslife.py`

 * *Files identical despite different names*

### Comparing `anipics-1.5.3/anipics/services/waifupics.py` & `anipics-1.5.4/anipics/services/waifupics.py`

 * *Files identical despite different names*

### Comparing `anipics-1.5.3/pyproject.toml` & `anipics-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipics"
-version = "1.5.3"
+version = "1.5.4"
 description = "Simple module to get anime pictures"
 authors = ["Daniel <D4n13l3k00@yandex.ru>"]
 readme = "README.md"
 license = "AGPL-3.0"
 repository = "https://github.com/D4n13l3k00/anipics"
 
 [tool.poetry.dependencies]
```

### Comparing `anipics-1.5.3/PKG-INFO` & `anipics-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipics
-Version: 1.5.3
+Version: 1.5.4
 Summary: Simple module to get anime pictures
 Home-page: https://github.com/D4n13l3k00/anipics
 License: AGPL-3.0
 Author: Daniel
 Author-email: D4n13l3k00@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

