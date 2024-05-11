# Comparing `tmp/ptsqld-0.1.2.tar.gz` & `tmp/ptsqld-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsqld-0.1.2.tar", max compression
+gzip compressed data, was "ptsqld-0.1.3.tar", max compression
```

## Comparing `ptsqld-0.1.2.tar` & `ptsqld-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      810 2024-04-26 05:49:16.395339 ptsqld-0.1.2/README.md
--rw-r--r--   0        0        0     3934 2024-05-08 20:05:04.861387 ptsqld-0.1.2/ptsqld/__init__.py
--rw-r--r--   0        0        0     1462 2024-03-12 09:17:42.025413 ptsqld-0.1.2/ptsqld/__init__.py~
--rw-r--r--   0        0        0      487 2024-03-13 20:19:06.329725 ptsqld-0.1.2/ptsqld/__main__.py~
--rw-r--r--   0        0        0      515 2024-05-08 19:46:15.927359 ptsqld-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 ptsqld-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      810 2024-04-26 05:49:16.395339 ptsqld-0.1.3/README.md
+-rw-r--r--   0        0        0     7281 2024-05-11 19:44:00.963863 ptsqld-0.1.3/ptsqld/__init__.py
+-rw-r--r--   0        0        0     1462 2024-03-12 09:17:42.025413 ptsqld-0.1.3/ptsqld/__init__.py~
+-rw-r--r--   0        0        0      487 2024-03-13 20:19:06.329725 ptsqld-0.1.3/ptsqld/__main__.py~
+-rw-r--r--   0        0        0      488 2024-05-11 19:47:19.018537 ptsqld-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 ptsqld-0.1.3/PKG-INFO
```

### Comparing `ptsqld-0.1.2/README.md` & `ptsqld-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ptsqld-0.1.2/ptsqld/__init__.py~` & `ptsqld-0.1.3/ptsqld/__init__.py~`

 * *Files identical despite different names*

### Comparing `ptsqld-0.1.2/PKG-INFO` & `ptsqld-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ptsqld
-Version: 0.1.2
+Version: 0.1.3
 Summary: An SQL Database which shall avoid any further PTSD associated to other SQL Database setup (understand flexible, simple)
 Author: Charles Bajeux
 Author-email: charles.bajeux@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: echovault (>=0.2.3,<0.3.0)
-Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: sqletic (>=0.1.4,<0.2.0)
 Description-Content-Type: text/markdown
 
 # ptsqld
 
 You suffered torment setting up SQL Database... You fear the day you will have to setup storage connect it to an engine ... maintain it...
 Fear no more... It is now as easy as setting up a git repository... No daemon server required everything is now decentralized ... distributes...
```

