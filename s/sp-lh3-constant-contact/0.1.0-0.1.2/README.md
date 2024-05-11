# Comparing `tmp/sp_lh3_constant_contact-0.1.0.tar.gz` & `tmp/sp_lh3_constant_contact-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sp_lh3_constant_contact-0.1.0.tar", max compression
+gzip compressed data, was "sp_lh3_constant_contact-0.1.2.tar", max compression
```

## Comparing `sp_lh3_constant_contact-0.1.0.tar` & `sp_lh3_constant_contact-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-05-08 01:23:12.490266 sp_lh3_constant_contact-0.1.0/README.md
--rw-r--r--   0        0        0      388 2024-05-08 08:25:09.052387 sp_lh3_constant_contact-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2990 2024-05-08 08:25:28.276005 sp_lh3_constant_contact-0.1.0/sp_lh3_constant_contact/__init__.py
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      895 2024-05-11 02:36:21.290691 sp_lh3_constant_contact-0.1.2/README.md
+-rw-r--r--   0        0        0      388 2024-05-11 02:31:02.777455 sp_lh3_constant_contact-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2990 2024-05-08 08:25:28.276005 sp_lh3_constant_contact-0.1.2/sp_lh3_constant_contact/__init__.py
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.2/PKG-INFO
```

### Comparing `sp_lh3_constant_contact-0.1.0/sp_lh3_constant_contact/__init__.py` & `sp_lh3_constant_contact-0.1.2/sp_lh3_constant_contact/__init__.py`

 * *Files identical despite different names*

