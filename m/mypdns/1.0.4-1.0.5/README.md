# Comparing `tmp/mypdns-1.0.4.tar.gz` & `tmp/mypdns-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypdns-1.0.4.tar", last modified: Sat May 11 01:03:08 2024, max compression
+gzip compressed data, was "mypdns-1.0.5.tar", last modified: Sat May 11 01:31:39 2024, max compression
```

## Comparing `mypdns-1.0.4.tar` & `mypdns-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:08.855315 mypdns-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-11 01:03:04.000000 mypdns-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 01:03:08.851315 mypdns-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-11 01:03:04.000000 mypdns-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:08.851315 mypdns-1.0.4/mypdns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:04.000000 mypdns-1.0.4/mypdns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:03:08.851315 mypdns-1.0.4/mypdns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 01:03:08.000000 mypdns-1.0.4/mypdns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:03:08.855315 mypdns-1.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2336 2024-05-11 01:03:04.000000 mypdns-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:31:39.138909 mypdns-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-11 01:31:34.000000 mypdns-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 01:31:39.138909 mypdns-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-11 01:31:34.000000 mypdns-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:31:39.134909 mypdns-1.0.5/mypdns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 01:31:34.000000 mypdns-1.0.5/mypdns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 01:31:39.138909 mypdns-1.0.5/mypdns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 01:31:39.000000 mypdns-1.0.5/mypdns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-11 01:31:39.000000 mypdns-1.0.5/mypdns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 01:31:39.000000 mypdns-1.0.5/mypdns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-11 01:31:39.000000 mypdns-1.0.5/mypdns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 01:31:39.138909 mypdns-1.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2336 2024-05-11 01:31:34.000000 mypdns-1.0.5/setup.py
```

### Comparing `mypdns-1.0.4/LICENSE` & `mypdns-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mypdns-1.0.4/PKG-INFO` & `mypdns-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypdns
-Version: 1.0.4
+Version: 1.0.5
 Summary: My Privacy DNS's Name space reservation
 Home-page: https://mypdns.org/
 Author: spirillen
 Author-email: pdns@protonmail.com
 License: UNKNOWN
 Project-URL: Tracker, https://github.com/mypdns/mypdns/issues
 Project-URL: Source, https://github.com/mypdns/mypdns
```

### Comparing `mypdns-1.0.4/README.md` & `mypdns-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mypdns-1.0.4/mypdns.egg-info/PKG-INFO` & `mypdns-1.0.5/mypdns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypdns
-Version: 1.0.4
+Version: 1.0.5
 Summary: My Privacy DNS's Name space reservation
 Home-page: https://mypdns.org/
 Author: spirillen
 Author-email: pdns@protonmail.com
 License: UNKNOWN
 Project-URL: Tracker, https://github.com/mypdns/mypdns/issues
 Project-URL: Source, https://github.com/mypdns/mypdns
```

### Comparing `mypdns-1.0.4/setup.py` & `mypdns-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     return open("README.md", encoding="utf-8").read()
 
 
 if __name__ == "__main__":
     # setuptools.
     setup(
         name="mypdns",
-        version="1.0.4",
+        version="1.0.5",
         author="spirillen",
         author_email="pdns@protonmail.com",
         description="My Privacy DNS's Name space reservation",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         url="https://mypdns.org/",
         project_urls={
```

