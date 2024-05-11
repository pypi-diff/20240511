# Comparing `tmp/poetry_moment-0.0.1.tar.gz` & `tmp/poetry_moment-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_moment-0.0.1.tar", max compression
+gzip compressed data, was "poetry_moment-0.0.2.tar", max compression
```

## Comparing `poetry_moment-0.0.1.tar` & `poetry_moment-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       27 2024-05-06 11:18:27.890911 poetry_moment-0.0.1/poetry_moment/__init__.py
--rw-r--r--   0        0        0      335 2024-05-06 11:13:16.460513 poetry_moment-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      183 2024-05-06 11:15:07.335256 poetry_moment-0.0.1/README.md
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 poetry_moment-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1425 2024-05-11 11:32:56.509771 poetry_moment-0.0.2/poetry_moment/__init__.py
+-rw-r--r--   0        0        0     2115 2024-05-11 11:32:30.632663 poetry_moment-0.0.2/poetry_moment/core.py
+-rw-r--r--   0        0        0      352 2024-05-11 11:34:01.187034 poetry_moment-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.2/README.md
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 poetry_moment-0.0.2/PKG-INFO
```

