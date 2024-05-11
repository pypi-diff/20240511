# Comparing `tmp/eli_hello-0.0.1.tar.gz` & `tmp/eli_hello-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eli_hello-0.0.1.tar", max compression
+gzip compressed data, was "eli_hello-0.0.2.tar", max compression
```

## Comparing `eli_hello-0.0.1.tar` & `eli_hello-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-11 13:14:32.018540 eli_hello-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-11 13:14:32.018496 eli_hello-0.0.1/eli_hello/__init__.py
--rw-r--r--   0        0        0       96 2024-05-11 13:38:54.772831 eli_hello-0.0.1/eli_hello/app.py
--rw-r--r--   0        0        0      394 2024-05-11 14:19:29.432014 eli_hello-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 eli_hello-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-11 14:32:18.483924 eli_hello-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 13:14:32.018496 eli_hello-0.0.2/eli_hello/__init__.py
+-rw-r--r--   0        0        0       96 2024-05-11 13:38:54.772831 eli_hello-0.0.2/eli_hello/app.py
+-rw-r--r--   0        0        0      394 2024-05-11 14:32:34.313910 eli_hello-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 eli_hello-0.0.2/PKG-INFO
```

