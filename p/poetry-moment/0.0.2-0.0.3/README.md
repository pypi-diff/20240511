# Comparing `tmp/poetry_moment-0.0.2.tar.gz` & `tmp/poetry_moment-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_moment-0.0.2.tar", max compression
+gzip compressed data, was "poetry_moment-0.0.3.tar", max compression
```

## Comparing `poetry_moment-0.0.2.tar` & `poetry_moment-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1425 2024-05-11 11:32:56.509771 poetry_moment-0.0.2/poetry_moment/__init__.py
--rw-r--r--   0        0        0     2115 2024-05-11 11:32:30.632663 poetry_moment-0.0.2/poetry_moment/core.py
--rw-r--r--   0        0        0      352 2024-05-11 11:34:01.187034 poetry_moment-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.2/README.md
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 poetry_moment-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1425 2024-05-11 11:32:56.509771 poetry_moment-0.0.3/poetry_moment/__init__.py
+-rw-r--r--   0        0        0     2115 2024-05-11 11:32:30.632663 poetry_moment-0.0.3/poetry_moment/core.py
+-rw-r--r--   0        0        0      354 2024-05-11 11:45:57.285583 poetry_moment-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.3/README.md
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 poetry_moment-0.0.3/PKG-INFO
```

### Comparing `poetry_moment-0.0.2/poetry_moment/__init__.py` & `poetry_moment-0.0.3/poetry_moment/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_moment-0.0.2/poetry_moment/core.py` & `poetry_moment-0.0.3/poetry_moment/core.py`

 * *Files identical despite different names*

