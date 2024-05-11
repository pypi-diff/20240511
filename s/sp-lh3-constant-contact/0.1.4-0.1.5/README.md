# Comparing `tmp/sp_lh3_constant_contact-0.1.4.tar.gz` & `tmp/sp_lh3_constant_contact-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sp_lh3_constant_contact-0.1.4.tar", max compression
+gzip compressed data, was "sp_lh3_constant_contact-0.1.5.tar", max compression
```

## Comparing `sp_lh3_constant_contact-0.1.4.tar` & `sp_lh3_constant_contact-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      895 2024-05-11 02:36:21.290691 sp_lh3_constant_contact-0.1.4/README.md
--rw-r--r--   0        0        0      520 2024-05-11 03:27:36.596150 sp_lh3_constant_contact-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3087 2024-05-11 03:27:20.026236 sp_lh3_constant_contact-0.1.4/sp_lh3_constant_contact/__init__.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      950 2024-05-11 03:36:53.906989 sp_lh3_constant_contact-0.1.5/README.md
+-rw-r--r--   0        0        0      647 2024-05-11 03:36:31.909266 sp_lh3_constant_contact-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3087 2024-05-11 03:27:20.026236 sp_lh3_constant_contact-0.1.5/sp_lh3_constant_contact/__init__.py
+-rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 sp_lh3_constant_contact-0.1.5/PKG-INFO
```

### Comparing `sp_lh3_constant_contact-0.1.4/README.md` & `sp_lh3_constant_contact-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![TravisCI](https://travis-ci.org/guinslym/sp-lh3-constant-contact.svg?branch=master)](https://travis-ci.org/guinslym/sp-lh3-constant-contact)
 
 <hr/>
 
 ## SP LibraryH3lp constant Contact
 
 <p>
-This script will assess a transcript to check if the operator has taken  see ```example.py```.
+This script will assess a transcript to check if the operator has taken more than 5 min to reply to any message from the patron see ```example.py```.
 </p>
 
 ## Installation & Usage
 
 **need credentials to connect to LibraryH3lp - see lh3api package on GitLab** 
 
 ```python
```

### Comparing `sp_lh3_constant_contact-0.1.4/pyproject.toml` & `sp_lh3_constant_contact-0.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "sp-lh3-constant-contact"
-version = "0.1.4"
-description = ""
+version = "0.1.5"
+description = "This script will assess a transcript to check if the operator has taken more than 5 min to reply to any message from the patron"
 authors = ["Guinslym <guinslym@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/guinslym/sp_lh3_constant_contact"
 homepage = "https://github.com/guinslym/sp_lh3_constant_contact"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `sp_lh3_constant_contact-0.1.4/sp_lh3_constant_contact/__init__.py` & `sp_lh3_constant_contact-0.1.5/sp_lh3_constant_contact/__init__.py`

 * *Files identical despite different names*

### Comparing `sp_lh3_constant_contact-0.1.4/PKG-INFO` & `sp_lh3_constant_contact-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sp-lh3-constant-contact
-Version: 0.1.4
-Summary: 
+Version: 0.1.5
+Summary: This script will assess a transcript to check if the operator has taken more than 5 min to reply to any message from the patron
 Home-page: https://github.com/guinslym/sp_lh3_constant_contact
 Author: Guinslym
 Author-email: guinslym@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -25,15 +25,15 @@
 [![TravisCI](https://travis-ci.org/guinslym/sp-lh3-constant-contact.svg?branch=master)](https://travis-ci.org/guinslym/sp-lh3-constant-contact)
 
 <hr/>
 
 ## SP LibraryH3lp constant Contact
 
 <p>
-This script will assess a transcript to check if the operator has taken  see ```example.py```.
+This script will assess a transcript to check if the operator has taken more than 5 min to reply to any message from the patron see ```example.py```.
 </p>
 
 ## Installation & Usage
 
 **need credentials to connect to LibraryH3lp - see lh3api package on GitLab** 
 
 ```python
```

