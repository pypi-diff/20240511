# Comparing `tmp/apicat-0.0.1.tar.gz` & `tmp/apicat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicat-0.0.1.tar", max compression
+gzip compressed data, was "apicat-0.0.2.tar", max compression
```

## Comparing `apicat-0.0.1.tar` & `apicat-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      673 2024-05-10 10:07:20.428315 apicat-0.0.1/apicat/__init__.py
--rw-r--r--   0        0        0      607 2024-05-10 10:05:09.238832 apicat-0.0.1/apicat/core.py
--rw-r--r--   0        0        0      287 2024-05-06 11:53:25.452935 apicat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.1/README.md
--rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 apicat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      924 2024-05-11 11:35:35.261902 apicat-0.0.2/apicat/__init__.py
+-rw-r--r--   0        0        0      585 2024-05-11 10:50:01.154407 apicat-0.0.2/apicat/config.py
+-rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.2/apicat/core.py
+-rw-r--r--   0        0        0      409 2024-05-11 10:47:12.418376 apicat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.2/README.md
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 apicat-0.0.2/PKG-INFO
```

