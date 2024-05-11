# Comparing `tmp/SQLibEngine-0.1.0.tar.gz` & `tmp/SQLibEngine-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLibEngine-0.1.0.tar", last modified: Fri May 10 14:50:54 2024, max compression
+gzip compressed data, was "SQLibEngine-0.1.1.tar", last modified: Fri May 10 15:11:20 2024, max compression
```

## Comparing `SQLibEngine-0.1.0.tar` & `SQLibEngine-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:54.396894 SQLibEngine-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-10 14:50:54.396894 SQLibEngine-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:54.392894 SQLibEngine-0.1.0/SQLib-Engine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:54.392894 SQLibEngine-0.1.0/SQLib-Engine/Database/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/Database/Connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/Database/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/Database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:54.396894 SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/SQLib-Engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:50:54.396894 SQLibEngine-0.1.0/SQLibEngine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-10 14:50:54.000000 SQLibEngine-0.1.0/SQLibEngine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-10 14:50:54.000000 SQLibEngine-0.1.0/SQLibEngine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:50:54.000000 SQLibEngine-0.1.0/SQLibEngine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 14:50:54.000000 SQLibEngine-0.1.0/SQLibEngine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:50:54.396894 SQLibEngine-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-10 14:50:50.000000 SQLibEngine-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.887151 SQLibEngine-0.1.1/SQLib-Engine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/SQLib-Engine/Database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/Database/Connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/Database/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/Database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/SQLib-Engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/SQLibEngine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 15:11:20.000000 SQLibEngine-0.1.1/SQLibEngine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:11:20.891151 SQLibEngine-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-10 15:11:13.000000 SQLibEngine-0.1.1/setup.py
```

### Comparing `SQLibEngine-0.1.0/LICENSE` & `SQLibEngine-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.0/SQLib-Engine/Database/Connection.py` & `SQLibEngine-0.1.1/SQLib-Engine/Database/Connection.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/operations.py` & `SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/operations.py`

 * *Files identical despite different names*

### Comparing `SQLibEngine-0.1.0/SQLib-Engine/SQLEngine/tables.py` & `SQLibEngine-0.1.1/SQLib-Engine/SQLEngine/tables.py`

 * *Files identical despite different names*

