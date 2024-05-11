# Comparing `tmp/chrisbase-0.5.1.tar.gz` & `tmp/chrisbase-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrisbase-0.5.1.tar", last modified: Mon Mar 18 23:39:54 2024, max compression
+gzip compressed data, was "chrisbase-0.5.2.tar", last modified: Fri Apr 26 08:52:24 2024, max compression
```

## Comparing `chrisbase-0.5.1.tar` & `chrisbase-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-03-18 23:39:54.271437 chrisbase-0.5.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)     1066 2024-03-17 13:02:43.000000 chrisbase-0.5.1/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     1365 2024-03-18 23:39:54.271437 chrisbase-0.5.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      286 2024-03-17 13:02:43.000000 chrisbase-0.5.1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)       81 2024-03-17 13:02:43.000000 chrisbase-0.5.1/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)     1061 2024-03-18 23:39:54.271437 chrisbase-0.5.1/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-03-18 23:39:54.267437 chrisbase-0.5.1/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-03-18 23:39:54.271437 chrisbase-0.5.1/src/chrisbase/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      151 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/cli.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    24859 2024-03-17 15:27:19.000000 chrisbase-0.5.1/src/chrisbase/data.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    22302 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/io.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     2170 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/morp.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      505 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/net.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     1059 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/time.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     7235 2024-03-17 13:02:43.000000 chrisbase-0.5.1/src/chrisbase/util.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-03-18 23:39:54.271437 chrisbase-0.5.1/src/chrisbase.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     1365 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      474 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       48 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/entry_points.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)      198 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       10 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-03-18 23:39:54.000000 chrisbase-0.5.1/src/chrisbase.egg-info/zip-safe
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-26 08:52:24.615158 chrisbase-0.5.2/
+-rw-r--r--   0 chris      (501) staff       (20)     1066 2024-04-26 07:53:21.000000 chrisbase-0.5.2/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     1365 2024-04-26 08:52:24.615088 chrisbase-0.5.2/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      286 2024-04-26 07:53:21.000000 chrisbase-0.5.2/README.md
+-rw-r--r--   0 chris      (501) staff       (20)       81 2024-04-26 07:53:21.000000 chrisbase-0.5.2/pyproject.toml
+-rw-r--r--   0 chris      (501) staff       (20)     1061 2024-04-26 08:52:24.615479 chrisbase-0.5.2/setup.cfg
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-26 08:52:24.612408 chrisbase-0.5.2/src/
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-26 08:52:24.613821 chrisbase-0.5.2/src/chrisbase/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)      151 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/cli.py
+-rw-r--r--   0 chris      (501) staff       (20)    24859 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/data.py
+-rw-r--r--   0 chris      (501) staff       (20)    22401 2024-04-26 08:00:09.000000 chrisbase-0.5.2/src/chrisbase/io.py
+-rw-r--r--   0 chris      (501) staff       (20)     2170 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/morp.py
+-rw-r--r--   0 chris      (501) staff       (20)      505 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/net.py
+-rw-r--r--   0 chris      (501) staff       (20)     1059 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/time.py
+-rw-r--r--   0 chris      (501) staff       (20)     7235 2024-04-26 07:53:21.000000 chrisbase-0.5.2/src/chrisbase/util.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-26 08:52:24.614862 chrisbase-0.5.2/src/chrisbase.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     1365 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      474 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       48 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/entry_points.txt
+-rw-r--r--   0 chris      (501) staff       (20)      198 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       10 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-04-26 08:52:24.000000 chrisbase-0.5.2/src/chrisbase.egg-info/zip-safe
```

### Comparing `chrisbase-0.5.1/LICENSE` & `chrisbase-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chrisbase-0.5.1/PKG-INFO` & `chrisbase-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.5.1
+Version: 0.5.2
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `chrisbase-0.5.1/setup.cfg` & `chrisbase-0.5.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chrisbase
-version = 0.5.1
+version = 0.5.2
 author = Jihee Ryu
 author_email = chrisjihee@naver.com
 url = https://github.com/chrisjihee/chrisbase
 description = A base tool for python programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `chrisbase-0.5.1/src/chrisbase/data.py` & `chrisbase-0.5.2/src/chrisbase/data.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.5.1/src/chrisbase/io.py` & `chrisbase-0.5.2/src/chrisbase/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,19 @@
     for out in outs:
         if out and not out.closed:
             out.flush()
             if sec and sec > 0.001:
                 sleep(sec)
 
 
+def read_or(path):
+    path = Path(path)
+    return path.read_text() if path.is_file() else None
+
+
 def exists_or(path):
     path = Path(path)
     return path if path.exists() else None
 
 
 def first_path_or(path):
     try:
```

### Comparing `chrisbase-0.5.1/src/chrisbase/morp.py` & `chrisbase-0.5.2/src/chrisbase/morp.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.5.1/src/chrisbase/time.py` & `chrisbase-0.5.2/src/chrisbase/time.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.5.1/src/chrisbase/util.py` & `chrisbase-0.5.2/src/chrisbase/util.py`

 * *Files identical despite different names*

### Comparing `chrisbase-0.5.1/src/chrisbase.egg-info/PKG-INFO` & `chrisbase-0.5.2/src/chrisbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrisbase
-Version: 0.5.1
+Version: 0.5.2
 Summary: A base tool for python programming.
 Home-page: https://github.com/chrisjihee/chrisbase
 Author: Jihee Ryu
 Author-email: chrisjihee@naver.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

