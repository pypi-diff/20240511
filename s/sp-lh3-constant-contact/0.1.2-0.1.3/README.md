# Comparing `tmp/sp_lh3_constant_contact-0.1.2.tar.gz` & `tmp/sp_lh3_constant_contact-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sp_lh3_constant_contact-0.1.2.tar", max compression
+gzip compressed data, was "sp_lh3_constant_contact-0.1.3.tar", max compression
```

## Comparing `sp_lh3_constant_contact-0.1.2.tar` & `sp_lh3_constant_contact-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      895 2024-05-11 02:36:21.290691 sp_lh3_constant_contact-0.1.2/README.md
--rw-r--r--   0        0        0      388 2024-05-11 02:31:02.777455 sp_lh3_constant_contact-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2990 2024-05-08 08:25:28.276005 sp_lh3_constant_contact-0.1.2/sp_lh3_constant_contact/__init__.py
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      895 2024-05-11 02:36:21.290691 sp_lh3_constant_contact-0.1.3/README.md
+-rw-r--r--   0        0        0      520 2024-05-11 02:44:12.549461 sp_lh3_constant_contact-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2990 2024-05-08 08:25:28.276005 sp_lh3_constant_contact-0.1.3/sp_lh3_constant_contact/__init__.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.3/PKG-INFO
```

### Comparing `sp_lh3_constant_contact-0.1.2/README.md` & `sp_lh3_constant_contact-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sp_lh3_constant_contact-0.1.2/sp_lh3_constant_contact/__init__.py` & `sp_lh3_constant_contact-0.1.3/sp_lh3_constant_contact/__init__.py`

 * *Files identical despite different names*

### Comparing `sp_lh3_constant_contact-0.1.2/PKG-INFO` & `sp_lh3_constant_contact-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: sp-lh3-constant-contact
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
+Home-page: https://github.com/guinslym/sp_lh3_constant_contact
 Author: Guinslym
 Author-email: guinslym@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: dateutils (>=0.6.12,<0.7.0)
 Requires-Dist: lh3api (>=0.2.0,<0.3.0)
+Project-URL: Repository, https://github.com/guinslym/sp_lh3_constant_contact
 Description-Content-Type: text/markdown
 
 [
 ![PyPI](https://img.shields.io/pypi/v/sp-lh3-constant-contact.svg)
 ![PyPI](https://img.shields.io/pypi/pyversions/sp-lh3-constant-contact.svg)
 ![PyPI](https://img.shields.io/github/license/guinslym/sp-lh3-constant-contact.svg)
 ](https://pypi.org/project/sp-lh3-constant-contact/)
```

