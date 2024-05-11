# Comparing `tmp/gh_copilot_chat-2024.5.11.441.tar.gz` & `tmp/gh_copilot_chat-2024.5.11.447.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gh_copilot_chat-2024.5.11.441.tar", max compression
+gzip compressed data, was "gh_copilot_chat-2024.5.11.447.tar", max compression
```

## Comparing `gh_copilot_chat-2024.5.11.441.tar` & `gh_copilot_chat-2024.5.11.447.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2531 2024-05-11 04:41:32.052729 gh_copilot_chat-2024.5.11.441/README.md
--rw-r--r--   0        0        0       67 2024-05-11 04:41:32.052729 gh_copilot_chat-2024.5.11.441/gh_copilot_chat/__init__.py
--rw-r--r--   0        0        0     2956 2024-05-11 04:41:32.052729 gh_copilot_chat-2024.5.11.441/gh_copilot_chat/copilot.py
--rw-r--r--   0        0        0      922 2024-05-11 04:41:32.052729 gh_copilot_chat-2024.5.11.441/gh_copilot_chat/main.py
--rw-r--r--   0        0        0      454 2024-05-11 04:41:32.136730 gh_copilot_chat-2024.5.11.441/pyproject.toml
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 gh_copilot_chat-2024.5.11.441/PKG-INFO
+-rw-r--r--   0        0        0     2531 2024-05-11 04:47:29.369390 gh_copilot_chat-2024.5.11.447/README.md
+-rw-r--r--   0        0        0       67 2024-05-11 04:47:29.369390 gh_copilot_chat-2024.5.11.447/gh_copilot_chat/__init__.py
+-rw-r--r--   0        0        0     2956 2024-05-11 04:47:29.369390 gh_copilot_chat-2024.5.11.447/gh_copilot_chat/copilot.py
+-rw-r--r--   0        0        0      922 2024-05-11 04:47:29.369390 gh_copilot_chat-2024.5.11.447/gh_copilot_chat/main.py
+-rw-r--r--   0        0        0      454 2024-05-11 04:47:29.453389 gh_copilot_chat-2024.5.11.447/pyproject.toml
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 gh_copilot_chat-2024.5.11.447/PKG-INFO
```

### Comparing `gh_copilot_chat-2024.5.11.441/README.md` & `gh_copilot_chat-2024.5.11.447/README.md`

 * *Files identical despite different names*

### Comparing `gh_copilot_chat-2024.5.11.441/gh_copilot_chat/copilot.py` & `gh_copilot_chat-2024.5.11.447/gh_copilot_chat/copilot.py`

 * *Files identical despite different names*

### Comparing `gh_copilot_chat-2024.5.11.441/gh_copilot_chat/main.py` & `gh_copilot_chat-2024.5.11.447/gh_copilot_chat/main.py`

 * *Files identical despite different names*

### Comparing `gh_copilot_chat-2024.5.11.441/PKG-INFO` & `gh_copilot_chat-2024.5.11.447/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gh_copilot_chat
-Version: 2024.5.11.441
+Version: 2024.5.11.447
 Summary: API Wrapper for GitHub Copilot Chat
 Author: Mohammed Rabil
 Author-email: rabil@email.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

